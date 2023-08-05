# Comparing `tmp/c2y-0.1.2.tar.gz` & `tmp/c2y-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c2y-0.1.2.tar", max compression
+gzip compressed data, was "c2y-0.1.4.tar", max compression
```

## Comparing `c2y-0.1.2.tar` & `c2y-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2023-07-31 07:46:08.853000 c2y-0.1.2/LICENSE
--rw-r--r--   0        0        0      519 2023-08-04 15:13:42.677467 c2y-0.1.2/README.md
--rw-r--r--   0        0        0       45 2023-07-31 07:46:09.223000 c2y-0.1.2/c2y/__init__.py
--rw-r--r--   0        0        0      103 2023-07-31 07:46:09.233000 c2y-0.1.2/c2y/__main__.py
--rw-r--r--   0        0        0     9377 2023-07-31 12:10:58.309000 c2y-0.1.2/c2y/utils.py
--rw-r--r--   0        0        0      488 2023-08-04 15:21:09.041909 c2y-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 c2y-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-31 07:46:08.853843 c2y-0.1.4/LICENSE
+-rw-r--r--   0        0        0      519 2023-08-04 15:13:42.677000 c2y-0.1.4/README.md
+-rw-r--r--   0        0        0       45 2023-07-31 07:46:09.223861 c2y-0.1.4/c2y/__init__.py
+-rw-r--r--   0        0        0      591 2023-08-05 11:04:09.665353 c2y-0.1.4/c2y/__main__.py
+-rw-r--r--   0        0        0    10778 2023-08-05 10:31:24.884381 c2y-0.1.4/c2y/utils.py
+-rw-r--r--   0        0        0      540 2023-08-05 11:17:12.484018 c2y-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 c2y-0.1.4/PKG-INFO
```

### Comparing `c2y-0.1.2/LICENSE` & `c2y-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `c2y-0.1.2/README.md` & `c2y-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `c2y-0.1.2/c2y/utils.py` & `c2y-0.1.4/c2y/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,53 @@
 """
 utils.py
 """
 
+import io
 import os
 import shutil
 import tempfile
 import zipfile
+from contextlib import redirect_stderr, redirect_stdout
 from pathlib import Path
 from typing import Any, Optional
 
 import magic
 import oyaml as yaml
 from loguru import logger
 from pycocotools.coco import COCO
 
 COCO_ANN_DIR = "annotations"
 COCO_IMGS_DIR = "images"
 
 
+def capture_logger(func):
+    """
+    capture stdout and stderr to log
+    """
+
+    def wrapper(*args, **kwargs):
+        # Create file-like objects
+        stdout_stream = io.StringIO()
+        stderr_stream = io.StringIO()
+
+        # Redirect stdout and stderr
+        with redirect_stdout(stdout_stream), redirect_stderr(stderr_stream):
+            # Call the function
+            func(*args, **kwargs)
+
+        # Log output
+        if (_stdout := stdout_stream.getvalue()) != "":
+            logger.trace(f"{_stdout}")
+        if (_stderr := stderr_stream.getvalue()) != "":
+            logger.trace(f"{_stderr}")
+
+    return wrapper
+
+
 class Xcoco:
     """
     Xcoco
     """
 
     def __init__(
         self,
@@ -76,41 +102,45 @@
 
         def _imgs_name(files):
             _imgs = [f for f in files if f.startswith(COCO_IMGS_DIR)]
             if len(_imgs) > 0:
                 return _imgs
             return None
 
+        @capture_logger
+        def _load_coco(ann_path: str):
+            self._coco_ann_path = ann_path
+            logger.trace(f"Set COCO ann path:{self._coco_ann_path}")
+            self._coco = COCO(self._coco_ann_path)
+
         if (
             ann_path is not None
             and os.path.exists(ann_path)
             and os.path.isfile(ann_path)
         ):
             _mime = str(_mimetype(ann_path))
             if _mime == "application/zip":  # if zip
                 _temp_dir = tempfile.gettempdir()
                 with zipfile.ZipFile(ann_path, "r") as zip_ref:
                     _z_names = zip_ref.namelist()
                     if (_ann := _ann_name(_z_names)) is not None:
                         zip_ref.extract(
                             _ann, path=_temp_dir
                         )  # set coco annotations path
-                        self._coco_ann_path = os.path.join(_temp_dir, _ann)
-                        self._coco = COCO(self._coco_ann_path)
+                        _load_coco(os.path.join(_temp_dir, _ann))
                         if (self.coco_imgs_dir is None) and (
                             (_imgs := _imgs_name(_z_names)) is not None
                         ):  # set coco images directory
                             for f_name in _imgs:
                                 zip_ref.extract(f_name, _temp_dir)
                             self.coco_imgs_dir = os.path.join(
                                 _temp_dir, COCO_IMGS_DIR
                             )
             elif _mime == "application/json":  # if json
-                self._coco_ann_path = ann_path
-                self._coco = COCO(self._coco_ann_path)
+                _load_coco(ann_path)
 
     @property
     def coco_imgs_dir(self):
         """
         coco images directory path getter
         """
         return self._coco_imgs_dir
@@ -121,14 +151,15 @@
         coco_imgs_dir: Optional[str] = None,
     ):
         """
         set images directory path
         """
         if coco_imgs_dir is not None and os.path.isdir(coco_imgs_dir):
             self._coco_imgs_dir = coco_imgs_dir
+            logger.trace(f"Set COCO images dir:{self._coco_imgs_dir}")
 
     @property
     def yolo_cfg_yaml_path(self):
         """
         yolo yaml config path getter
         """
         return self._yolo_cfg_yaml_path
@@ -143,14 +174,15 @@
         """
         if cfg_yaml_path is not None:
             self._yolo_cfg_yaml_path = cfg_yaml_path
         else:
             self._yolo_cfg_yaml_path = os.path.join(
                 self.output_dir, "yolo.yml"
             )
+        logger.trace(f"Set YOLO config yaml path:{self._yolo_cfg_yaml_path}")
 
     @property
     def output_dir(self):
         """
         output directory path getter
         """
         return self._output_dir
@@ -158,16 +190,18 @@
     @output_dir.setter
     def output_dir(self, output_dir: Optional[str] = None):
         """
         set output directory path
         """
         if output_dir is None:
             self._output_dir = "./"
+            logger.trace(f"Set Output dir:{self._output_dir}")
         elif os.path.isdir(output_dir):
             self._output_dir = output_dir
+            logger.trace(f"Set Output dir:{self._output_dir}")
         else:
             raise Exception(f"{output_dir}")
 
         self._yolo_labels_dir = os.path.join(self._output_dir, "labels")
         self._yolo_images_dir = os.path.join(self._output_dir, "images")
 
     @property
@@ -248,20 +282,22 @@
             fname = (
                 os.path.splitext(self._coco.imgs[img_id]["file_name"])[0]
                 + ".txt"
             )
             _txt = self._img_to_labels(img_id=img_id)
             if _txt == "":
                 continue
+            _f_label = os.path.join(self._yolo_labels_dir, fname)
             with open(
-                os.path.join(self._yolo_labels_dir, fname),
+                _f_label,
                 "w",
                 encoding="UTF-8",
             ) as f_handler:
                 f_handler.write(_txt)
+                logger.trace(f"Writle label file:{_f_label}")
 
     def write_images(self):
         """
         write images to yolo datasets
         """
         if self.coco_imgs_dir is None or not os.path.exists(
             self.coco_imgs_dir
@@ -273,25 +309,29 @@
             return
 
         for img_id in self._coco.getImgIds():
             source_path = os.path.join(
                 self._coco_imgs_dir, self._coco.imgs[img_id]["file_name"]
             )
             shutil.copy(source_path, self._yolo_images_dir)
+            logger.trace(f"Copy image file:{source_path}")
 
     def write_yaml(self):
         """
         write yaml file
         """
         if os.path.exists(self.yolo_cfg_yaml_path):
-            _in = input(
-                f"{self.yolo_cfg_yaml_path} exist.\nare you sure to overwrite? yes/(no)"
-            )
-            if _in.lower() != "y" and _in.lower() != "yes":  # input not yes
-                return
+            if self._force is not True:
+                _in = input(
+                    f"{self.yolo_cfg_yaml_path} exist.\nare you sure to overwrite? yes/(no)"
+                )
+                if (
+                    _in.lower() != "y" and _in.lower() != "yes"
+                ):  # input not yes
+                    return
 
             with open(
                 self.yolo_cfg_yaml_path, "r", encoding="UTF-8"
             ) as f_handler:
                 yaml_content_dict = yaml.load(
                     f_handler, Loader=yaml.FullLoader
                 )
@@ -306,14 +346,15 @@
         yaml_content_dict["names"] = {
             int(self._coco.cats[cid]["id"]) - 1: self._coco.cats[cid]["name"]
             for cid in self._coco.getCatIds()
         }
 
         with open(self.yolo_cfg_yaml_path, "w", encoding="UTF-8") as f_handler:
             yaml.dump(yaml_content_dict, f_handler)
+            logger.trace(f"Write yolo config file:{self.yolo_cfg_yaml_path}")
 
     def __call__(self) -> Any:
         if self.coco is None:
             logger.error("coco is None")
             return
 
         self.write_labels()
```

### Comparing `c2y-0.1.2/PKG-INFO` & `c2y-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c2y
-Version: 0.1.2
+Version: 0.1.4
 Summary: Convert coco datasets to yolo datasets
 Author: hobbymarks
 Author-email: ihobbymarks@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

