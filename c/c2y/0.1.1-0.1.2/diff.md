# Comparing `tmp/c2y-0.1.1.tar.gz` & `tmp/c2y-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c2y-0.1.1.tar", max compression
+gzip compressed data, was "c2y-0.1.2.tar", max compression
```

## Comparing `c2y-0.1.1.tar` & `c2y-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2023-07-31 07:46:08.853000 c2y-0.1.1/LICENSE
--rw-r--r--   0        0        0      519 2023-08-04 15:13:42.677467 c2y-0.1.1/README.md
--rw-r--r--   0        0        0       45 2023-07-31 07:46:09.223000 c2y-0.1.1/c2y/__init__.py
--rw-r--r--   0        0        0      103 2023-07-31 07:46:09.233000 c2y-0.1.1/c2y/__main__.py
--rw-r--r--   0        0        0     9377 2023-07-31 12:10:58.309000 c2y-0.1.1/c2y/utils.py
--rw-r--r--   0        0        0      707 2023-08-04 15:09:08.015926 c2y-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 c2y-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-31 07:46:08.853000 c2y-0.1.2/LICENSE
+-rw-r--r--   0        0        0      519 2023-08-04 15:13:42.677467 c2y-0.1.2/README.md
+-rw-r--r--   0        0        0       45 2023-07-31 07:46:09.223000 c2y-0.1.2/c2y/__init__.py
+-rw-r--r--   0        0        0      103 2023-07-31 07:46:09.233000 c2y-0.1.2/c2y/__main__.py
+-rw-r--r--   0        0        0     9377 2023-07-31 12:10:58.309000 c2y-0.1.2/c2y/utils.py
+-rw-r--r--   0        0        0      488 2023-08-04 15:21:09.041909 c2y-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 c2y-0.1.2/PKG-INFO
```

### Comparing `c2y-0.1.1/LICENSE` & `c2y-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `c2y-0.1.1/README.md` & `c2y-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `c2y-0.1.1/c2y/utils.py` & `c2y-0.1.2/c2y/utils.py`

 * *Files identical despite different names*

### Comparing `c2y-0.1.1/PKG-INFO` & `c2y-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,26 @@
 Metadata-Version: 2.1
 Name: c2y
-Version: 0.1.1
+Version: 0.1.2
 Summary: Convert coco datasets to yolo datasets
 Author: hobbymarks
 Author-email: ihobbymarks@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: coverage (>=7.2.7,<8.0.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
-Requires-Dist: ipywidgets (>=8.0.7,<9.0.0)
-Requires-Dist: isort (>=5.12.0,<6.0.0)
-Requires-Dist: jupyterlab (>=4.0.3,<5.0.0)
-Requires-Dist: jupyterlab-code-formatter (>=2.2.1,<3.0.0)
-Requires-Dist: jupyterlab-execute-time (>=3.0.0,<4.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: mimetypes-magic (>=0.4.30,<0.5.0)
-Requires-Dist: nuitka (>=1.7.8,<2.0.0)
 Requires-Dist: oyaml (>=1.0,<2.0)
-Requires-Dist: plotly-express (>=0.4.1,<0.5.0)
 Requires-Dist: pycocotools (>=2.0.6,<3.0.0)
-Requires-Dist: pyinstaller (>=5.13.0,<6.0.0)
 Requires-Dist: pytest (>=7.4.0,<8.0.0)
 Requires-Dist: pytest-mock (>=3.11.1,<4.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Requires-Dist: yapf (>=0.40.1,<0.41.0)
 Description-Content-Type: text/markdown
 
 # NAME
     c2y
 
 # SYNOPSIS
     c2y <flags>
```

