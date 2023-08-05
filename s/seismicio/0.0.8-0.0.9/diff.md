# Comparing `tmp/seismicio-0.0.8.tar.gz` & `tmp/seismicio-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seismicio-0.0.8.tar", last modified: Fri Dec  2 04:02:37 2022, max compression
+gzip compressed data, was "seismicio-0.0.9.tar", last modified: Fri Dec  2 04:07:21 2022, max compression
```

## Comparing `seismicio-0.0.8.tar` & `seismicio-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 jorb      (1000) jorb      (1000)        0 2022-12-02 04:02:37.906533 seismicio-0.0.8/
--rw-r--r--   0 jorb      (1000) jorb      (1000)      138 2022-12-02 03:26:30.000000 seismicio-0.0.8/MANIFEST.in
--rw-r--r--   0 jorb      (1000) jorb      (1000)      515 2022-12-02 04:02:37.906533 seismicio-0.0.8/PKG-INFO
--rw-r--r--   0 jorb      (1000) jorb      (1000)     1105 2022-12-02 03:36:36.000000 seismicio-0.0.8/README.md
-drwxr-xr-x   0 jorb      (1000) jorb      (1000)        0 2022-12-02 04:02:37.896533 seismicio-0.0.8/seismicio/
-drwxr-xr-x   0 jorb      (1000) jorb      (1000)        0 2022-12-02 04:02:37.906533 seismicio-0.0.8/seismicio/Models/
--rw-r--r--   0 jorb      (1000) jorb      (1000)     2177 2022-12-02 01:51:59.000000 seismicio-0.0.8/seismicio/Models/HeadersModel.py
--rw-r--r--   0 jorb      (1000) jorb      (1000)     3758 2022-12-02 01:51:59.000000 seismicio-0.0.8/seismicio/Models/InOutSuModel.py
--rw-r--r--   0 jorb      (1000) jorb      (1000)     4621 2022-12-02 01:51:59.000000 seismicio-0.0.8/seismicio/Models/UtilsModel.py
--rw-r--r--   0 jorb      (1000) jorb      (1000)      180 2022-12-02 04:02:19.000000 seismicio-0.0.8/seismicio/__init__.py
--rw-r--r--   0 jorb      (1000) jorb      (1000)       21 2022-12-02 04:00:57.000000 seismicio-0.0.8/seismicio/__version__.py
-drwxr-xr-x   0 jorb      (1000) jorb      (1000)        0 2022-12-02 04:02:37.906533 seismicio-0.0.8/seismicio/constants/
--rw-r--r--   0 jorb      (1000) jorb      (1000)       47 2022-12-02 01:51:33.000000 seismicio-0.0.8/seismicio/constants/HEADER_FORMAT_STRING.py
--rw-r--r--   0 jorb      (1000) jorb      (1000)       36 2022-12-02 01:51:38.000000 seismicio-0.0.8/seismicio/constants/TRACE_HEADER_SIZE.py
-drwxr-xr-x   0 jorb      (1000) jorb      (1000)        0 2022-12-02 04:02:37.906533 seismicio-0.0.8/seismicio/services/
--rw-r--r--   0 jorb      (1000) jorb      (1000)      172 2022-12-02 01:51:59.000000 seismicio-0.0.8/seismicio/services/readsu.py
--rw-r--r--   0 jorb      (1000) jorb      (1000)      235 2022-12-02 03:45:11.000000 seismicio-0.0.8/seismicio/services/readsuInMemory.py
--rw-r--r--   0 jorb      (1000) jorb      (1000)      216 2022-12-02 01:51:59.000000 seismicio-0.0.8/seismicio/services/writesu.py
--rw-r--r--   0 jorb      (1000) jorb      (1000)      277 2022-12-02 03:45:28.000000 seismicio-0.0.8/seismicio/services/writesuInMemory.py
-drwxr-xr-x   0 jorb      (1000) jorb      (1000)        0 2022-12-02 04:02:37.906533 seismicio-0.0.8/seismicio.egg-info/
--rw-r--r--   0 jorb      (1000) jorb      (1000)      515 2022-12-02 04:02:37.000000 seismicio-0.0.8/seismicio.egg-info/PKG-INFO
--rw-r--r--   0 jorb      (1000) jorb      (1000)      557 2022-12-02 04:02:37.000000 seismicio-0.0.8/seismicio.egg-info/SOURCES.txt
--rw-r--r--   0 jorb      (1000) jorb      (1000)        1 2022-12-02 04:02:37.000000 seismicio-0.0.8/seismicio.egg-info/dependency_links.txt
--rw-r--r--   0 jorb      (1000) jorb      (1000)        9 2022-12-02 04:02:37.000000 seismicio-0.0.8/seismicio.egg-info/requires.txt
--rw-r--r--   0 jorb      (1000) jorb      (1000)       10 2022-12-02 04:02:37.000000 seismicio-0.0.8/seismicio.egg-info/top_level.txt
--rw-r--r--   0 jorb      (1000) jorb      (1000)       38 2022-12-02 04:02:37.906533 seismicio-0.0.8/setup.cfg
--rw-r--r--   0 jorb      (1000) jorb      (1000)      708 2022-12-02 04:01:37.000000 seismicio-0.0.8/setup.py
+drwxr-xr-x   0 jorb      (1000) jorb      (1000)        0 2022-12-02 04:07:21.766533 seismicio-0.0.9/
+-rw-r--r--   0 jorb      (1000) jorb      (1000)      138 2022-12-02 03:26:30.000000 seismicio-0.0.9/MANIFEST.in
+-rw-r--r--   0 jorb      (1000) jorb      (1000)      515 2022-12-02 04:07:21.756533 seismicio-0.0.9/PKG-INFO
+-rw-r--r--   0 jorb      (1000) jorb      (1000)     1105 2022-12-02 03:36:36.000000 seismicio-0.0.9/README.md
+drwxr-xr-x   0 jorb      (1000) jorb      (1000)        0 2022-12-02 04:07:21.756533 seismicio-0.0.9/seismicio/
+drwxr-xr-x   0 jorb      (1000) jorb      (1000)        0 2022-12-02 04:07:21.756533 seismicio-0.0.9/seismicio/Models/
+-rw-r--r--   0 jorb      (1000) jorb      (1000)     2177 2022-12-02 01:51:59.000000 seismicio-0.0.9/seismicio/Models/HeadersModel.py
+-rw-r--r--   0 jorb      (1000) jorb      (1000)     3758 2022-12-02 01:51:59.000000 seismicio-0.0.9/seismicio/Models/InOutSuModel.py
+-rw-r--r--   0 jorb      (1000) jorb      (1000)     4621 2022-12-02 01:51:59.000000 seismicio-0.0.9/seismicio/Models/UtilsModel.py
+-rw-r--r--   0 jorb      (1000) jorb      (1000)      227 2022-12-02 04:07:01.000000 seismicio-0.0.9/seismicio/__init__.py
+drwxr-xr-x   0 jorb      (1000) jorb      (1000)        0 2022-12-02 04:07:21.756533 seismicio-0.0.9/seismicio/constants/
+-rw-r--r--   0 jorb      (1000) jorb      (1000)       47 2022-12-02 01:51:33.000000 seismicio-0.0.9/seismicio/constants/HEADER_FORMAT_STRING.py
+-rw-r--r--   0 jorb      (1000) jorb      (1000)       36 2022-12-02 01:51:38.000000 seismicio-0.0.9/seismicio/constants/TRACE_HEADER_SIZE.py
+-rw-r--r--   0 jorb      (1000) jorb      (1000)       21 2022-12-02 04:00:57.000000 seismicio-0.0.9/seismicio/constants/__version__.py
+drwxr-xr-x   0 jorb      (1000) jorb      (1000)        0 2022-12-02 04:07:21.756533 seismicio-0.0.9/seismicio/services/
+-rw-r--r--   0 jorb      (1000) jorb      (1000)      172 2022-12-02 01:51:59.000000 seismicio-0.0.9/seismicio/services/readsu.py
+-rw-r--r--   0 jorb      (1000) jorb      (1000)      235 2022-12-02 03:45:11.000000 seismicio-0.0.9/seismicio/services/readsuInMemory.py
+-rw-r--r--   0 jorb      (1000) jorb      (1000)      216 2022-12-02 01:51:59.000000 seismicio-0.0.9/seismicio/services/writesu.py
+-rw-r--r--   0 jorb      (1000) jorb      (1000)      277 2022-12-02 03:45:28.000000 seismicio-0.0.9/seismicio/services/writesuInMemory.py
+drwxr-xr-x   0 jorb      (1000) jorb      (1000)        0 2022-12-02 04:07:21.756533 seismicio-0.0.9/seismicio.egg-info/
+-rw-r--r--   0 jorb      (1000) jorb      (1000)      515 2022-12-02 04:07:21.000000 seismicio-0.0.9/seismicio.egg-info/PKG-INFO
+-rw-r--r--   0 jorb      (1000) jorb      (1000)      567 2022-12-02 04:07:21.000000 seismicio-0.0.9/seismicio.egg-info/SOURCES.txt
+-rw-r--r--   0 jorb      (1000) jorb      (1000)        1 2022-12-02 04:07:21.000000 seismicio-0.0.9/seismicio.egg-info/dependency_links.txt
+-rw-r--r--   0 jorb      (1000) jorb      (1000)        9 2022-12-02 04:07:21.000000 seismicio-0.0.9/seismicio.egg-info/requires.txt
+-rw-r--r--   0 jorb      (1000) jorb      (1000)       10 2022-12-02 04:07:21.000000 seismicio-0.0.9/seismicio.egg-info/top_level.txt
+-rw-r--r--   0 jorb      (1000) jorb      (1000)       38 2022-12-02 04:07:21.766533 seismicio-0.0.9/setup.cfg
+-rw-r--r--   0 jorb      (1000) jorb      (1000)      708 2022-12-02 04:06:30.000000 seismicio-0.0.9/setup.py
```

### Comparing `seismicio-0.0.8/PKG-INFO` & `seismicio-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: seismicio
-Version: 0.0.8
+Version: 0.0.9
 Summary: Read and write .su files for seismic data
 Home-page: UNKNOWN
 Author: cadu-sg
 Author-email: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python,io
```

### Comparing `seismicio-0.0.8/README.md` & `seismicio-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `seismicio-0.0.8/seismicio/Models/HeadersModel.py` & `seismicio-0.0.9/seismicio/Models/HeadersModel.py`

 * *Files identical despite different names*

### Comparing `seismicio-0.0.8/seismicio/Models/InOutSuModel.py` & `seismicio-0.0.9/seismicio/Models/InOutSuModel.py`

 * *Files identical despite different names*

### Comparing `seismicio-0.0.8/seismicio/Models/UtilsModel.py` & `seismicio-0.0.9/seismicio/Models/UtilsModel.py`

 * *Files identical despite different names*

### Comparing `seismicio-0.0.8/seismicio.egg-info/PKG-INFO` & `seismicio-0.0.9/seismicio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: seismicio
-Version: 0.0.8
+Version: 0.0.9
 Summary: Read and write .su files for seismic data
 Home-page: UNKNOWN
 Author: cadu-sg
 Author-email: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python,io
```

### Comparing `seismicio-0.0.8/seismicio.egg-info/SOURCES.txt` & `seismicio-0.0.9/seismicio.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 MANIFEST.in
 README.md
 setup.py
 seismicio/__init__.py
-seismicio/__version__.py
 seismicio.egg-info/PKG-INFO
 seismicio.egg-info/SOURCES.txt
 seismicio.egg-info/dependency_links.txt
 seismicio.egg-info/requires.txt
 seismicio.egg-info/top_level.txt
 seismicio/Models/HeadersModel.py
 seismicio/Models/InOutSuModel.py
 seismicio/Models/UtilsModel.py
 seismicio/constants/HEADER_FORMAT_STRING.py
 seismicio/constants/TRACE_HEADER_SIZE.py
+seismicio/constants/__version__.py
 seismicio/services/readsu.py
 seismicio/services/readsuInMemory.py
 seismicio/services/writesu.py
 seismicio/services/writesuInMemory.py
```

### Comparing `seismicio-0.0.8/setup.py` & `seismicio-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Read and write .su files for seismic data'
 
 # Setting up
 setup(
     name="seismicio",
     version=VERSION,
     author="cadu-sg",
```

