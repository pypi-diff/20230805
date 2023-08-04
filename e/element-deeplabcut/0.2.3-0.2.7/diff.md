# Comparing `tmp/element-deeplabcut-0.2.3.tar.gz` & `tmp/element-deeplabcut-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "element-deeplabcut-0.2.3.tar", last modified: Wed Apr  5 22:31:28 2023, max compression
+gzip compressed data, was "element-deeplabcut-0.2.7.tar", last modified: Fri Aug  4 22:22:20 2023, max compression
```

## Comparing `element-deeplabcut-0.2.3.tar` & `element-deeplabcut-0.2.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:31:28.388653 element-deeplabcut-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-05 22:31:25.000000 element-deeplabcut-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-05 22:31:28.388653 element-deeplabcut-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-05 22:31:25.000000 element-deeplabcut-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:31:28.388653 element-deeplabcut-0.2.3/element_deeplabcut/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 22:31:25.000000 element-deeplabcut-0.2.3/element_deeplabcut/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:31:28.388653 element-deeplabcut-0.2.3/element_deeplabcut/export/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-05 22:31:25.000000 element-deeplabcut-0.2.3/element_deeplabcut/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-05 22:31:25.000000 element-deeplabcut-0.2.3/element_deeplabcut/export/nwb.py
--rw-r--r--   0 runner    (1001) docker     (123)    31536 2023-04-05 22:31:25.000000 element-deeplabcut-0.2.3/element_deeplabcut/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:31:28.388653 element-deeplabcut-0.2.3/element_deeplabcut/readers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 22:31:25.000000 element-deeplabcut-0.2.3/element_deeplabcut/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-04-05 22:31:25.000000 element-deeplabcut-0.2.3/element_deeplabcut/readers/dlc_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    12019 2023-04-05 22:31:25.000000 element-deeplabcut-0.2.3/element_deeplabcut/train.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-05 22:31:25.000000 element-deeplabcut-0.2.3/element_deeplabcut/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:31:28.388653 element-deeplabcut-0.2.3/element_deeplabcut.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-05 22:31:28.000000 element-deeplabcut-0.2.3/element_deeplabcut.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-05 22:31:28.000000 element-deeplabcut-0.2.3/element_deeplabcut.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 22:31:28.000000 element-deeplabcut-0.2.3/element_deeplabcut.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-05 22:31:28.000000 element-deeplabcut-0.2.3/element_deeplabcut.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-05 22:31:28.000000 element-deeplabcut-0.2.3/element_deeplabcut.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 22:31:28.388653 element-deeplabcut-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-05 22:31:25.000000 element-deeplabcut-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:22:20.930919 element-deeplabcut-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-04 22:22:17.000000 element-deeplabcut-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-04 22:22:20.930919 element-deeplabcut-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-08-04 22:22:17.000000 element-deeplabcut-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:22:20.930919 element-deeplabcut-0.2.7/element_deeplabcut/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 22:22:17.000000 element-deeplabcut-0.2.7/element_deeplabcut/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:22:20.930919 element-deeplabcut-0.2.7/element_deeplabcut/export/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 22:22:17.000000 element-deeplabcut-0.2.7/element_deeplabcut/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-08-04 22:22:17.000000 element-deeplabcut-0.2.7/element_deeplabcut/export/nwb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31536 2023-08-04 22:22:17.000000 element-deeplabcut-0.2.7/element_deeplabcut/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:22:20.930919 element-deeplabcut-0.2.7/element_deeplabcut/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 22:22:17.000000 element-deeplabcut-0.2.7/element_deeplabcut/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-08-04 22:22:17.000000 element-deeplabcut-0.2.7/element_deeplabcut/readers/dlc_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-08-04 22:22:17.000000 element-deeplabcut-0.2.7/element_deeplabcut/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-04 22:22:17.000000 element-deeplabcut-0.2.7/element_deeplabcut/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:22:20.930919 element-deeplabcut-0.2.7/element_deeplabcut.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-04 22:22:20.000000 element-deeplabcut-0.2.7/element_deeplabcut.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-04 22:22:20.000000 element-deeplabcut-0.2.7/element_deeplabcut.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 22:22:20.000000 element-deeplabcut-0.2.7/element_deeplabcut.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-04 22:22:20.000000 element-deeplabcut-0.2.7/element_deeplabcut.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-04 22:22:20.000000 element-deeplabcut-0.2.7/element_deeplabcut.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 22:22:20.930919 element-deeplabcut-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-04 22:22:17.000000 element-deeplabcut-0.2.7/setup.py
```

### Comparing `element-deeplabcut-0.2.3/LICENSE` & `element-deeplabcut-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `element-deeplabcut-0.2.3/PKG-INFO` & `element-deeplabcut-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-deeplabcut
-Version: 0.2.3
+Version: 0.2.7
 Summary: DataJoint Element for Continuous Behavior Tracking via DeepLabCut
 Home-page: https://github.com/datajoint/element-deeplabcut
 Author: DataJoint
 Author-email: info@vathes.com
 License: MIT
 Keywords: neuroscience behavior deeplabcut datajoint
 Platform: UNKNOWN
```

### Comparing `element-deeplabcut-0.2.3/README.md` & `element-deeplabcut-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `element-deeplabcut-0.2.3/element_deeplabcut/export/nwb.py` & `element-deeplabcut-0.2.7/element_deeplabcut/export/nwb.py`

 * *Files identical despite different names*

### Comparing `element-deeplabcut-0.2.3/element_deeplabcut/model.py` & `element-deeplabcut-0.2.7/element_deeplabcut/model.py`

 * *Files identical despite different names*

### Comparing `element-deeplabcut-0.2.3/element_deeplabcut/readers/dlc_reader.py` & `element-deeplabcut-0.2.7/element_deeplabcut/readers/dlc_reader.py`

 * *Files identical despite different names*

### Comparing `element-deeplabcut-0.2.3/element_deeplabcut/train.py` & `element-deeplabcut-0.2.7/element_deeplabcut/train.py`

 * *Files 6% similar despite different names*

```diff
@@ -237,21 +237,25 @@
     config_template: longblob     # stored full config file
     """
 
     # To continue from previous training snapshot, devs suggest editing pose_cfg.yml
     # https://github.com/DeepLabCut/DeepLabCut/issues/70
 
     def make(self, key):
-        from deeplabcut import train_network # isort:skip
+        from deeplabcut import train_network  # isort:skip
+
         try:
-            from deeplabcut.utils.auxiliaryfunctions import get_model_folder # isort:skip
+            from deeplabcut.utils.auxiliaryfunctions import (
+                get_model_folder,
+                edit_config,
+            )  # isort:skip
         except ImportError:
             from deeplabcut.utils.auxiliaryfunctions import (
-                GetModelFolder as get_model_folder
-            ) # isort:skip
+                GetModelFolder as get_model_folder,
+            )  # isort:skip
 
         """Launch training for each train.TrainingTask training_id via `.populate()`."""
         project_path, model_prefix = (TrainingTask & key).fetch1(
             "project_path", "model_prefix"
         )
 
         project_path = find_full_path(get_dlc_root_data_dir(), project_path)
@@ -271,40 +275,44 @@
                     for fp in (VideoSet.File & key).fetch("file_path")
                 ],
             }
         )
         # Write dlc config file to base project folder
         dlc_cfg_filepath = dlc_reader.save_yaml(project_path, dlc_config)
 
+        # ---- Update the project path in the DLC pose configuration (yaml) files ----
+        model_folder = get_model_folder(
+            trainFraction=dlc_config["train_fraction"],
+            shuffle=dlc_config["shuffle"],
+            cfg=dlc_config,
+            modelprefix=dlc_config["modelprefix"],
+        )
+        model_train_folder = project_path / model_folder / "train"
+
+        edit_config(
+            model_train_folder / "pose_cfg.yaml",
+            {"project_path": project_path.as_posix()},
+        )
+
         # ---- Trigger DLC model training job ----
         train_network_input_args = list(inspect.signature(train_network).parameters)
         train_network_kwargs = {
-            k: int(v) if k in ("shuffle", "trainingsetindex", "maxiters") else v 
-            for k, v in dlc_config.items() if k in train_network_input_args
+            k: int(v) if k in ("shuffle", "trainingsetindex", "maxiters") else v
+            for k, v in dlc_config.items()
+            if k in train_network_input_args
         }
         for k in ["shuffle", "trainingsetindex", "maxiters"]:
             train_network_kwargs[k] = int(train_network_kwargs[k])
 
         try:
             train_network(dlc_cfg_filepath, **train_network_kwargs)
         except KeyboardInterrupt:  # Instructions indicate to train until interrupt
             print("DLC training stopped via Keyboard Interrupt")
 
-        snapshots = list(
-            (
-                project_path
-                / get_model_folder(
-                    trainFraction=dlc_config["train_fraction"],
-                    shuffle=dlc_config["shuffle"],
-                    cfg=dlc_config,
-                    modelprefix=dlc_config["modelprefix"],
-                )
-                / "train"
-            ).glob("*index*")
-        )
+        snapshots = list(model_train_folder.glob("*index*"))
         max_modified_time = 0
         # DLC goes by snapshot magnitude when judging 'latest' for evaluation
         # Here, we mean most recently generated
         for snapshot in snapshots:
             modified_time = os.path.getmtime(snapshot)
             if modified_time > max_modified_time:
                 latest_snapshot = int(snapshot.stem[9:])
```

### Comparing `element-deeplabcut-0.2.3/element_deeplabcut.egg-info/PKG-INFO` & `element-deeplabcut-0.2.7/element_deeplabcut.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-deeplabcut
-Version: 0.2.3
+Version: 0.2.7
 Summary: DataJoint Element for Continuous Behavior Tracking via DeepLabCut
 Home-page: https://github.com/datajoint/element-deeplabcut
 Author: DataJoint
 Author-email: info@vathes.com
 License: MIT
 Keywords: neuroscience behavior deeplabcut datajoint
 Platform: UNKNOWN
```

### Comparing `element-deeplabcut-0.2.3/setup.py` & `element-deeplabcut-0.2.7/setup.py`

 * *Files identical despite different names*

