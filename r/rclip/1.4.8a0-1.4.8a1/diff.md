# Comparing `tmp/rclip-1.4.8a0.tar.gz` & `tmp/rclip-1.4.8a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rclip-1.4.8a0.tar", max compression
+gzip compressed data, was "rclip-1.4.8a1.tar", max compression
```

## Comparing `rclip-1.4.8a0.tar` & `rclip-1.4.8a1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-08-05 18:50:57.620922 rclip-1.4.8a0/LICENSE
--rw-r--r--   0        0        0     5203 2023-08-05 18:50:57.620922 rclip-1.4.8a0/README.md
--rw-r--r--   0        0        0     1051 2023-08-05 18:50:57.620922 rclip-1.4.8a0/pyproject.toml
--rw-r--r--   0        0        0     2940 2023-08-05 18:50:57.620922 rclip-1.4.8a0/rclip/db.py
--rw-r--r--   0        0        0     5586 2023-08-05 18:50:57.620922 rclip-1.4.8a0/rclip/main.py
--rw-r--r--   0        0        0     5270 2023-08-05 18:50:57.620922 rclip-1.4.8a0/rclip/model.py
--rw-r--r--   0        0        0     4746 2023-08-05 18:50:57.620922 rclip-1.4.8a0/rclip/utils.py
--rw-r--r--   0        0        0     6530 1970-01-01 00:00:00.000000 rclip-1.4.8a0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-08-05 19:07:26.287503 rclip-1.4.8a1/LICENSE
+-rw-r--r--   0        0        0     5203 2023-08-05 19:07:26.287503 rclip-1.4.8a1/README.md
+-rw-r--r--   0        0        0     1693 2023-08-05 19:07:26.287503 rclip-1.4.8a1/pyproject.toml
+-rw-r--r--   0        0        0     2940 2023-08-05 19:07:26.287503 rclip-1.4.8a1/rclip/db.py
+-rw-r--r--   0        0        0     5586 2023-08-05 19:07:26.287503 rclip-1.4.8a1/rclip/main.py
+-rw-r--r--   0        0        0     5270 2023-08-05 19:07:26.287503 rclip-1.4.8a1/rclip/model.py
+-rw-r--r--   0        0        0     4746 2023-08-05 19:07:26.287503 rclip-1.4.8a1/rclip/utils.py
+-rw-r--r--   0        0        0     6845 1970-01-01 00:00:00.000000 rclip-1.4.8a1/PKG-INFO
```

### Comparing `rclip-1.4.8a0/LICENSE` & `rclip-1.4.8a1/LICENSE`

 * *Files identical despite different names*

### Comparing `rclip-1.4.8a0/README.md` & `rclip-1.4.8a1/README.md`

 * *Files identical despite different names*

### Comparing `rclip-1.4.8a0/rclip/db.py` & `rclip-1.4.8a1/rclip/db.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.8a0/rclip/main.py` & `rclip-1.4.8a1/rclip/main.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.8a0/rclip/model.py` & `rclip-1.4.8a1/rclip/model.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.8a0/rclip/utils.py` & `rclip-1.4.8a1/rclip/utils.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.8a0/PKG-INFO` & `rclip-1.4.8a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclip
-Version: 1.4.8a0
+Version: 1.4.8a1
 Summary: AI-Powered Command-Line Photo Search Tool
 Home-page: https://github.com/yurijmikhalevich/rclip
 License: MIT
 Keywords: image search,computer vision,photography
 Author: Yurij Mikhalevich
 Author-email: yurij@mikhalevi.ch
 Requires-Python: >=3.8,<4.0
@@ -20,16 +20,18 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Utilities
 Requires-Dist: open_clip_torch (>=2.20.0,<3.0.0)
 Requires-Dist: pillow (>=10.0.0,<11.0.0)
 Requires-Dist: requests (>=2.26,<3.0)
-Requires-Dist: torch (==2.0.1)
-Requires-Dist: torchvision (==0.15.2)
+Requires-Dist: torch (==2.0.1) ; sys_platform != "linux" or platform_machine == "aarch64"
+Requires-Dist: torch (==2.0.1+cpu) ; sys_platform == "linux" and platform_machine != "aarch64"
+Requires-Dist: torchvision (==0.15.2) ; sys_platform != "linux" or platform_machine == "aarch64"
+Requires-Dist: torchvision (==0.15.2+cpu) ; sys_platform == "linux" and platform_machine != "aarch64"
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/yurijmikhalevich/rclip
 Description-Content-Type: text/markdown
 
 # rclip - AI-Powered Command-Line Photo Search Tool
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)
```

