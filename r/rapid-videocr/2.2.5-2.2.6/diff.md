# Comparing `tmp/rapid_videocr-2.2.5-py3-none-any.whl.zip` & `tmp/rapid_videocr-2.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 18362 bytes, number of entries: 11
--rw-r--r--  2.0 unx      174 b- defN 23-Jul-22 04:40 rapid_videocr/__init__.py
--rw-r--r--  2.0 unx    10508 b- defN 23-Jul-22 04:40 rapid_videocr/main.py
--rw-r--r--  2.0 unx    13571 b- defN 23-Jul-22 04:40 rapid_videocr/rapid_videocr.py
--rw-r--r--  2.0 unx     5423 b- defN 23-Jul-22 04:40 rapid_videocr/utils.py
--rw-r--r--  2.0 unx     2996 b- defN 23-Jul-22 04:40 rapid_videocr/video_sub_finder.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-22 04:40 rapid_videocr-2.2.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     8165 b- defN 23-Jul-22 04:40 rapid_videocr-2.2.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-22 04:40 rapid_videocr-2.2.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 23-Jul-22 04:40 rapid_videocr-2.2.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 23-Jul-22 04:40 rapid_videocr-2.2.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      935 b- defN 23-Jul-22 04:40 rapid_videocr-2.2.5.dist-info/RECORD
-11 files, 53294 bytes uncompressed, 16772 bytes compressed:  68.5%
+Zip file size: 18580 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      174 b- defN 23-Aug-05 10:27 rapid_videocr/__init__.py
+-rw-r--r--  2.0 unx      811 b- defN 23-Aug-05 10:27 rapid_videocr/logger.py
+-rw-r--r--  2.0 unx    10389 b- defN 23-Aug-05 10:27 rapid_videocr/main.py
+-rw-r--r--  2.0 unx    13484 b- defN 23-Aug-05 10:27 rapid_videocr/rapid_videocr.py
+-rw-r--r--  2.0 unx     4526 b- defN 23-Aug-05 10:27 rapid_videocr/utils.py
+-rw-r--r--  2.0 unx     2996 b- defN 23-Aug-05 10:27 rapid_videocr/video_sub_finder.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Aug-05 10:27 rapid_videocr-2.2.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8163 b- defN 23-Aug-05 10:27 rapid_videocr-2.2.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-05 10:27 rapid_videocr-2.2.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 23-Aug-05 10:27 rapid_videocr-2.2.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-Aug-05 10:27 rapid_videocr-2.2.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1014 b- defN 23-Aug-05 10:27 rapid_videocr-2.2.6.dist-info/RECORD
+12 files, 53079 bytes uncompressed, 16868 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -1,34 +1,37 @@
 Filename: rapid_videocr/__init__.py
 Comment: 
 
+Filename: rapid_videocr/logger.py
+Comment: 
+
 Filename: rapid_videocr/main.py
 Comment: 
 
 Filename: rapid_videocr/rapid_videocr.py
 Comment: 
 
 Filename: rapid_videocr/utils.py
 Comment: 
 
 Filename: rapid_videocr/video_sub_finder.py
 Comment: 
 
-Filename: rapid_videocr-2.2.5.dist-info/LICENSE
+Filename: rapid_videocr-2.2.6.dist-info/LICENSE
 Comment: 
 
-Filename: rapid_videocr-2.2.5.dist-info/METADATA
+Filename: rapid_videocr-2.2.6.dist-info/METADATA
 Comment: 
 
-Filename: rapid_videocr-2.2.5.dist-info/WHEEL
+Filename: rapid_videocr-2.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: rapid_videocr-2.2.5.dist-info/entry_points.txt
+Filename: rapid_videocr-2.2.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapid_videocr-2.2.5.dist-info/top_level.txt
+Filename: rapid_videocr-2.2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: rapid_videocr-2.2.5.dist-info/RECORD
+Filename: rapid_videocr-2.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rapid_videocr/main.py

```diff
@@ -2,19 +2,21 @@
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
 import argparse
 from pathlib import Path
 from typing import Optional
 
 try:
+    from .logger import logger
     from .rapid_videocr import RapidVideOCR
-    from .utils import float_range, get_logger
+    from .utils import float_range
     from .video_sub_finder import VideoSubFinder
 except:
-    from utils import float_range, get_logger
+    from logger import logger
+    from utils import float_range
     from video_sub_finder import VideoSubFinder
 
     from rapid_videocr import RapidVideOCR
 
 
 class RapidVideoSubFinderOCR:
     def __init__(
@@ -68,54 +70,48 @@
         self.video_ocr = RapidVideOCR(
             is_concat_rec=is_concat_rec,
             concat_batch=concat_batch,
             out_format=out_format,
             is_print_console=print_console,
         )
         self.video_formats = [".mp4", ".avi", ".mov", ".mkv"]
-        self.logger = get_logger()
 
     def __call__(self, video_path: str, output_dir: str = "outputs"):
         if Path(video_path).is_dir():
             video_list = Path(video_path).rglob("*.*")
             video_list = [
                 v for v in video_list if v.suffix.lower() in self.video_formats
             ]
         else:
             video_list = [video_path]
 
-        self.logger.info(
+        logger.info(
             "Extracting subtitle images with VideoSubFinder (takes quite a long time) ..."
         )
         video_num = len(video_list)
         for i, one_video in enumerate(video_list):
-            self.logger.info(
-                "[%s/%s] Starting to extract %s key frame",
-                i + 1,
-                video_num,
-                one_video,
+            logger.info(
+                f"[{i+1}/{video_num}] Starting to extract {one_video} key frame",
             )
 
             save_name = Path(one_video).stem
             save_dir = Path(output_dir) / save_name
             save_vsf_dir = save_dir / "VSF_Results"
 
             try:
                 self.vsf(str(one_video), str(save_vsf_dir))
             except Exception as e:
-                self.logger.error("Extract %s error, %s, skip", one_video, e)
+                logger.error(f"Extract {one_video} error, {e}, skip")
                 continue
 
-            self.logger.info(
-                "[%s/%s] Starting to run %s ocr", i + 1, video_num, one_video
-            )
+            logger.info(f"[{i+1}/{video_num}] Starting to run {one_video} ocr")
 
             rgb_dir = Path(save_vsf_dir) / "RGBImages"
             if not list(rgb_dir.iterdir()):
-                self.logger.warning("Extracting frames from %s is 0, skip", one_video)
+                logger.warning(f"Extracting frames from {one_video} is 0, skip")
                 continue
             self.video_ocr(rgb_dir, save_dir, save_name=save_name)
 
 
 def main():
     parser = argparse.ArgumentParser()
```

## rapid_videocr/rapid_videocr.py

```diff
@@ -7,32 +7,21 @@
 
 import cv2
 import numpy as np
 from rapidocr_onnxruntime import RapidOCR
 from tqdm import tqdm
 
 try:
-    from .utils import (
-        CropByProject,
-        compute_poly_iou,
-        get_logger,
-        is_inclusive_each_other,
-        mkdir,
-    )
+    from .logger import logger
+    from .utils import CropByProject, compute_poly_iou, is_inclusive_each_other, mkdir
 except:
-    from utils import (
-        CropByProject,
-        compute_poly_iou,
-        get_logger,
-        is_inclusive_each_other,
-        mkdir,
-    )
+    from logger import logger
+    from utils import CropByProject, compute_poly_iou, is_inclusive_each_other, mkdir
 
 CUR_DIR = Path(__file__).resolve().parent
-logger = get_logger()
 
 
 class RapidVideOCR:
     def __init__(
         self,
         is_concat_rec: bool = False,
         concat_batch: int = 10,
@@ -184,15 +173,15 @@
         for i, frame_boxes in enumerate(img_coordinates):
             for idx, dt_box in enumerate(dt_boxes):
                 if idx in visited_idx:
                     continue
 
                 box_iou = compute_poly_iou(frame_boxes, dt_box)
                 if is_inclusive_each_other(frame_boxes, dt_box) or box_iou > 0.1:
-                    matched_path = img_paths[idx]
+                    matched_path = img_paths[i]
                     match_dict.setdefault(i, []).append(
                         [matched_path, dt_box, rec_res[idx]]
                     )
                     visited_idx.append(idx)
 
         for k, v in match_dict.items():
             cur_frame_idx = start_i + k
@@ -298,15 +287,15 @@
         elif self.out_format == "srt":
             self.save_file(srt_path, srt_result)
         elif self.out_format == "all":
             self.save_file(txt_path, txt_result)
             self.save_file(srt_path, srt_result)
         else:
             raise ValueError(f"The {self.out_format} dost not support.")
-        logger.info("[OCR] The result has been saved to %s directory.", save_dir)
+        logger.info(f"[OCR] The result has been saved to {save_dir} directory.")
 
     def print_console(self, txt_result: List) -> None:
         for v in txt_result:
             print(v.strip())
 
     @staticmethod
     def save_file(save_path: Union[str, Path], content: List, mode: str = "w") -> None:
@@ -315,15 +304,15 @@
 
         if not isinstance(content, list):
             content = [content]
 
         with open(save_path, mode, encoding="utf-8") as f:
             for value in content:
                 f.write(f"{value}\n")
-        logger.info("[OCR] The file has been saved in the %s", save_path)
+        logger.info(f"[OCR] The file has been saved in the {save_path}")
 
     @staticmethod
     def _compute_centroid(points: np.ndarray) -> List:
         """计算所给框的质心坐标
 
         :param points ([type]): (4, 2)
         :return: [description]
```

## rapid_videocr/utils.py

```diff
@@ -1,19 +1,15 @@
 # -*- encoding: utf-8 -*-
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
 import argparse
-import functools
-import logging
-import sys
 from enum import Enum
 from pathlib import Path
 from typing import List, Union
 
-import colorlog
 import cv2
 import numpy as np
 import shapely
 from shapely.geometry import MultiPoint, Polygon
 
 logger_initialized = {}
 
@@ -79,43 +75,14 @@
         txt_path = str(txt_path)
 
     with open(txt_path, "r", encoding="utf-8") as f:
         data = list(map(lambda x: x.rstrip("\n"), f))
     return data
 
 
-@functools.lru_cache()
-def get_logger(name="rapid_videocr"):
-    logger = logging.getLogger(name)
-    if name in logger_initialized:
-        return logger
-
-    for logger_name in logger_initialized:
-        if name.startswith(logger_name):
-            return logger
-
-    fmt_string = "%(log_color)s[%(asctime)s] [%(name)s] %(levelname)s: %(message)s"
-    log_colors = {
-        "DEBUG": "white",
-        "INFO": "green",
-        "WARNING": "yellow",
-        "ERROR": "red",
-        "CRITICAL": "purple",
-    }
-    fmt = colorlog.ColoredFormatter(fmt_string, log_colors=log_colors)
-    stream_handler = logging.StreamHandler(stream=sys.stdout)
-    stream_handler.setFormatter(fmt)
-    logger.addHandler(stream_handler)
-
-    logger.setLevel(logging.INFO)
-    logger_initialized[name] = True
-    logger.propagate = False
-    return logger
-
-
 def compute_poly_iou(a: np.ndarray, b: np.ndarray) -> float:
     """计算两个多边形的IOU
 
     Args:
         poly1 (np.ndarray): (4, 2)
         poly2 (np.ndarray): (4, 2)
```

## Comparing `rapid_videocr-2.2.5.dist-info/LICENSE` & `rapid_videocr-2.2.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rapid_videocr-2.2.5.dist-info/METADATA` & `rapid_videocr-2.2.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapid-videocr
-Version: 2.2.5
+Version: 2.2.6
 Summary: Tool for extracting hard subtitles from videos.
 Home-page: https://github.com/SWHL/RapidVideOCR.git
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Keywords: rapidocr,videocr,subtitle
 Platform: Any
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: colorlog
+Requires-Dist: loguru
 Requires-Dist: rapidocr-onnxruntime (>=1.2.2)
 Requires-Dist: tqdm
 
 ## rapid_videocr Package
 <p align="left">
     <a href="https://colab.research.google.com/github/SWHL/RapidVideOCR/blob/75dae6e9804dec6e61bef98334601908dc9ec9fb/assets/RapidVideOCRDemo.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg"></a>
     <a href=""><img src="https://img.shields.io/badge/Python->=3.6,<3.12-aff.svg"></a>
```

### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: rapid-videocr Version: 2.2.5 Summary: Tool for
+Metadata-Version: 2.1 Name: rapid-videocr Version: 2.2.6 Summary: Tool for
 extracting hard subtitles from videos. Home-page: https://github.com/SWHL/
 RapidVideOCR.git Author: SWHL Author-email: liekkaskono@163.com License:
 Apache-2.0 Keywords: rapidocr,videocr,subtitle Platform: Any Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Python: >=3.6,<3.12 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: colorlog Requires-Dist: rapidocr-onnxruntime (>=1.2.2)
+LICENSE Requires-Dist: loguru Requires-Dist: rapidocr-onnxruntime (>=1.2.2)
 Requires-Dist: tqdm ## rapid_videocr Package
 [https://colab.research.google.com/assets/colab-badge.svg] [https://
 img.shields.io/badge/Python->=3.6,<3.12-aff.svg] [https://img.shields.io/badge/
 OS-Linux%2C%20Win%2C%20Mac-pink.svg] [https://img.shields.io/github/stars/SWHL/
 RapidVideOCR?color=ccf] [https://static.pepy.tech/personalized-badge/rapid-
 videocr?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads]
 [Documentation_Status] [SemVer2.0] [https://img.shields.io/badge/code%20style-
```

## Comparing `rapid_videocr-2.2.5.dist-info/RECORD` & `rapid_videocr-2.2.6.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 rapid_videocr/__init__.py,sha256=eODelyqvjJaceBues-U7fmLAE3JTDkVLUTbcsWivf_Q,174
-rapid_videocr/main.py,sha256=e8Zkkfil3HlXtVX9BxD2qQLh3iuE0_1G-7yNlXlf8_g,10508
-rapid_videocr/rapid_videocr.py,sha256=IL5wXVxPXdWOGmGEAGmCFv2KrtNGJTX6yQIwoRMOtOM,13571
-rapid_videocr/utils.py,sha256=tNYWmQGHVu_yjQisyPed9nVluYOvEiefz_HJ9kbxhso,5423
+rapid_videocr/logger.py,sha256=N3EqcXUElZo_Ta5fyueHRodIKe64PfDnFbqtz2IjfeU,811
+rapid_videocr/main.py,sha256=j0mPNWTh50thAPKxPPstTnxhWU54j221XI4LcGRz8tY,10389
+rapid_videocr/rapid_videocr.py,sha256=GTxPnDI5H6Bb6FxTUKGstKD_ZeKiQIvqfTkiY52R9GA,13484
+rapid_videocr/utils.py,sha256=aXQTl9EP1iKpifVUfMMOyCLsQ0nmfbEU-3rprPayYi4,4526
 rapid_videocr/video_sub_finder.py,sha256=FilAtJl0a2e81ZGDpPiL8n-JvYe3vRQrbw2rxLJyjIE,2996
-rapid_videocr-2.2.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-rapid_videocr-2.2.5.dist-info/METADATA,sha256=28C_pWNj0hqvlAp1oDqavWjveqWZx-FU2wNv2ScJssE,8165
-rapid_videocr-2.2.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-rapid_videocr-2.2.5.dist-info/entry_points.txt,sha256=-keKc5D46wZRqKWIPVZqb5paoQwqLf-OiXKtztK9VqA,59
-rapid_videocr-2.2.5.dist-info/top_level.txt,sha256=uPQbJQ346YJVTUi4CqGP2OZUrUSsUn57eiRiNtpe97E,14
-rapid_videocr-2.2.5.dist-info/RECORD,,
+rapid_videocr-2.2.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+rapid_videocr-2.2.6.dist-info/METADATA,sha256=qPPRQAyFPGX4P66vX-qmEF6MJ50r_tNB3qN3o7Ht26c,8163
+rapid_videocr-2.2.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+rapid_videocr-2.2.6.dist-info/entry_points.txt,sha256=-keKc5D46wZRqKWIPVZqb5paoQwqLf-OiXKtztK9VqA,59
+rapid_videocr-2.2.6.dist-info/top_level.txt,sha256=uPQbJQ346YJVTUi4CqGP2OZUrUSsUn57eiRiNtpe97E,14
+rapid_videocr-2.2.6.dist-info/RECORD,,
```

