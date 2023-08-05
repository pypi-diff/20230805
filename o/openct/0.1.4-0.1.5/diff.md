# Comparing `tmp/openct-0.1.4.tar.gz` & `tmp/openct-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openct-0.1.4.tar", max compression
+gzip compressed data, was "openct-0.1.5.tar", max compression
```

## Comparing `openct-0.1.4.tar` & `openct-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-08-04 23:26:09.325491 openct-0.1.4/LICENSE
--rw-r--r--   0        0        0     1693 2023-08-04 23:26:09.325491 openct-0.1.4/README.md
--rw-r--r--   0        0        0       89 2023-08-04 23:26:09.325491 openct-0.1.4/openct/__init__.py
--rw-r--r--   0        0        0      649 2023-08-04 23:26:09.325491 openct-0.1.4/openct/__main__.py
--rw-r--r--   0        0        0       83 2023-08-04 23:26:09.325491 openct-0.1.4/openct/connections/__init__.py
--rw-r--r--   0        0        0     2723 2023-08-04 23:26:09.329491 openct-0.1.4/openct/connections/connections.py
--rw-r--r--   0        0        0       73 2023-08-04 23:26:09.329491 openct-0.1.4/openct/datastore/__init__.py
--rw-r--r--   0        0        0     1359 2023-08-04 23:26:09.329491 openct-0.1.4/openct/datastore/datastore.py
--rw-r--r--   0        0        0       65 2023-08-04 23:26:09.329491 openct-0.1.4/openct/devices/__init__.py
--rw-r--r--   0        0        0      743 2023-08-04 23:26:09.329491 openct-0.1.4/openct/devices/devices.py
--rw-r--r--   0        0        0      201 2023-08-04 23:26:09.329491 openct-0.1.4/openct/setup/__init__.py
--rw-r--r--   0        0        0      556 2023-08-04 23:26:09.329491 openct-0.1.4/openct/setup/__main__.py
--rw-r--r--   0        0        0     1440 2023-08-04 23:26:09.329491 openct-0.1.4/openct/setup/config.py
--rw-r--r--   0        0        0      626 2023-08-04 23:26:09.329491 openct-0.1.4/openct/setup/config_schema.py
--rw-r--r--   0        0        0     1354 2023-08-04 23:26:09.329491 openct-0.1.4/openct/setup/setup.py
--rw-r--r--   0        0        0      592 2023-08-04 23:26:09.329491 openct-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2341 1970-01-01 00:00:00.000000 openct-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-05 00:58:12.244308 openct-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1693 2023-08-05 00:58:12.244308 openct-0.1.5/README.md
+-rw-r--r--   0        0        0      112 2023-08-05 00:58:25.700403 openct-0.1.5/openct/__init__.py
+-rw-r--r--   0        0        0      649 2023-08-05 00:58:12.244308 openct-0.1.5/openct/__main__.py
+-rw-r--r--   0        0        0       83 2023-08-05 00:58:12.248309 openct-0.1.5/openct/connections/__init__.py
+-rw-r--r--   0        0        0     2723 2023-08-05 00:58:12.248309 openct-0.1.5/openct/connections/connections.py
+-rw-r--r--   0        0        0       73 2023-08-05 00:58:12.248309 openct-0.1.5/openct/datastore/__init__.py
+-rw-r--r--   0        0        0     1359 2023-08-05 00:58:12.248309 openct-0.1.5/openct/datastore/datastore.py
+-rw-r--r--   0        0        0       65 2023-08-05 00:58:12.248309 openct-0.1.5/openct/devices/__init__.py
+-rw-r--r--   0        0        0      743 2023-08-05 00:58:12.248309 openct-0.1.5/openct/devices/devices.py
+-rw-r--r--   0        0        0      201 2023-08-05 00:58:12.248309 openct-0.1.5/openct/setup/__init__.py
+-rw-r--r--   0        0        0      556 2023-08-05 00:58:12.248309 openct-0.1.5/openct/setup/__main__.py
+-rw-r--r--   0        0        0     1440 2023-08-05 00:58:12.248309 openct-0.1.5/openct/setup/config.py
+-rw-r--r--   0        0        0      626 2023-08-05 00:58:12.248309 openct-0.1.5/openct/setup/config_schema.py
+-rw-r--r--   0        0        0     1696 2023-08-05 00:58:12.248309 openct-0.1.5/openct/setup/setup.py
+-rw-r--r--   0        0        0      645 2023-08-05 00:58:25.696403 openct-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2341 1970-01-01 00:00:00.000000 openct-0.1.5/PKG-INFO
```

### Comparing `openct-0.1.4/LICENSE` & `openct-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openct-0.1.4/README.md` & `openct-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `openct-0.1.4/openct/__main__.py` & `openct-0.1.5/openct/__main__.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.4/openct/connections/connections.py` & `openct-0.1.5/openct/connections/connections.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.4/openct/datastore/datastore.py` & `openct-0.1.5/openct/datastore/datastore.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.4/openct/devices/devices.py` & `openct-0.1.5/openct/devices/devices.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.4/openct/setup/__main__.py` & `openct-0.1.5/openct/setup/__main__.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.4/openct/setup/config.py` & `openct-0.1.5/openct/setup/config.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.4/openct/setup/config_schema.py` & `openct-0.1.5/openct/setup/config_schema.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.4/openct/setup/setup.py` & `openct-0.1.5/openct/setup/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Setup
 """
 
 import os
 import time
 import logging
 import argparse
+import platform
 
+import openct
 from .config_schema import Config
 from .config import load_config
 
 
 def setup_config() -> Config:
     args = parse_args()
 
@@ -44,14 +46,22 @@
     args = parser.parse_args()
     return args
 
 
 def init_logging(log_dir: str) -> None:
     log_file = os.path.join(log_dir, f"ocb_{time.strftime('%Y%m%d_%H%M%S')}.log")
 
+    header_info = f"Package Version: {openct.__version__}\n"
+    header_info += f"OS: {platform.system()} {platform.release()}\n"
+    header_info += f"Python Version: {platform.python_version()}\n"
+    header_info += "\n"
+
+    with open(log_file, "a", encoding="utf-8") as file:
+        file.write(header_info)
+
     logging.basicConfig(
         level=logging.INFO,
         format="%(asctime)s [%(module)s] [%(levelname)s] %(message)s",
         filename=log_file,
         filemode="a",
         encoding="utf-8",
     )
```

### Comparing `openct-0.1.4/pyproject.toml` & `openct-0.1.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openct"
-version = "0.1.4"
+version = "0.1.5"
 description = "Configuration backup and analysis tools for devices running pfSense and RouterOS"
 authors = ["Weehooey <info@weehooey.com>"]
 license = "GNU GPL v3.0"
 readme = "README.md"
 repository = "https://github.com/weehooey/openct"
 
 [tool.poetry.dependencies]
@@ -19,7 +19,9 @@
 pytest = "^7.4.0"
 wrapt = "^1.15.0"
 dill = "^0.3.6"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry_bumpversion.file."openct/__init__.py"]
```

### Comparing `openct-0.1.4/PKG-INFO` & `openct-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openct
-Version: 0.1.4
+Version: 0.1.5
 Summary: Configuration backup and analysis tools for devices running pfSense and RouterOS
 Home-page: https://github.com/weehooey/openct
 License: GNU GPL v3.0
 Author: Weehooey
 Author-email: info@weehooey.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
```

