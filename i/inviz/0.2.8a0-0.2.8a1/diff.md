# Comparing `tmp/inviz-0.2.8a0.tar.gz` & `tmp/inviz-0.2.8a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inviz-0.2.8a0.tar", last modified: Sat Aug  5 07:11:10 2023, max compression
+gzip compressed data, was "inviz-0.2.8a1.tar", last modified: Sat Aug  5 07:25:21 2023, max compression
```

## Comparing `inviz-0.2.8a0.tar` & `inviz-0.2.8a1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-05 07:11:10.065803 inviz-0.2.8a0/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-03-27 21:46:04.000000 inviz-0.2.8a0/LICENSE
--rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-03-27 21:46:04.000000 inviz-0.2.8a0/MANIFEST.in
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2165 2023-08-05 07:11:10.065803 inviz-0.2.8a0/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1642 2023-07-13 22:19:19.000000 inviz-0.2.8a0/README.md
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-05 07:11:10.055803 inviz-0.2.8a0/inviz.egg-info/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2165 2023-08-05 07:11:10.000000 inviz-0.2.8a0/inviz.egg-info/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)      252 2023-08-05 07:11:10.000000 inviz-0.2.8a0/inviz.egg-info/SOURCES.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-08-05 07:11:10.000000 inviz-0.2.8a0/inviz.egg-info/dependency_links.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)      119 2023-08-05 07:11:10.000000 inviz-0.2.8a0/inviz.egg-info/requires.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-08-05 07:11:10.000000 inviz-0.2.8a0/inviz.egg-info/top_level.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-08-05 07:11:10.065803 inviz-0.2.8a0/setup.cfg
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1154 2023-08-05 07:11:03.000000 inviz-0.2.8a0/setup.py
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-05 07:11:10.065803 inviz-0.2.8a0/src/
--rw-r--r--   0 jswen     (1000) jswen     (1000)        0 2023-08-04 04:36:54.000000 inviz-0.2.8a0/src/__init__.py
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-05 07:11:10.065803 inviz-0.2.8a0/src/cosmo/
--rw-r--r--   0 jswen     (1000) jswen     (1000)        0 2023-08-04 04:36:54.000000 inviz-0.2.8a0/src/cosmo/__init__.py
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2605 2023-08-04 04:36:54.000000 inviz-0.2.8a0/src/cosmo/cosmo.py
--rwxr-xr-x   0 jswen     (1000) jswen     (1000)    11241 2023-08-04 04:36:54.000000 inviz-0.2.8a0/src/inviz.py
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-05 07:25:21.576574 inviz-0.2.8a1/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-03-27 21:46:04.000000 inviz-0.2.8a1/LICENSE
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-03-27 21:46:04.000000 inviz-0.2.8a1/MANIFEST.in
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2165 2023-08-05 07:25:21.576574 inviz-0.2.8a1/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1642 2023-07-13 22:19:19.000000 inviz-0.2.8a1/README.md
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-05 07:25:21.576574 inviz-0.2.8a1/inviz.egg-info/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2165 2023-08-05 07:25:21.000000 inviz-0.2.8a1/inviz.egg-info/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)      252 2023-08-05 07:25:21.000000 inviz-0.2.8a1/inviz.egg-info/SOURCES.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-08-05 07:25:21.000000 inviz-0.2.8a1/inviz.egg-info/dependency_links.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)      119 2023-08-05 07:25:21.000000 inviz-0.2.8a1/inviz.egg-info/requires.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-08-05 07:25:21.000000 inviz-0.2.8a1/inviz.egg-info/top_level.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-08-05 07:25:21.576574 inviz-0.2.8a1/setup.cfg
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1155 2023-08-05 07:25:14.000000 inviz-0.2.8a1/setup.py
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-05 07:25:21.576574 inviz-0.2.8a1/src/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       20 2023-08-05 07:23:00.000000 inviz-0.2.8a1/src/__init__.py
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-05 07:25:21.576574 inviz-0.2.8a1/src/cosmo/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       20 2023-08-05 07:23:40.000000 inviz-0.2.8a1/src/cosmo/__init__.py
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2605 2023-08-04 04:36:54.000000 inviz-0.2.8a1/src/cosmo/cosmo.py
+-rwxr-xr-x   0 jswen     (1000) jswen     (1000)    11241 2023-08-04 04:36:54.000000 inviz-0.2.8a1/src/inviz.py
```

### Comparing `inviz-0.2.8a0/LICENSE` & `inviz-0.2.8a1/LICENSE`

 * *Files identical despite different names*

### Comparing `inviz-0.2.8a0/PKG-INFO` & `inviz-0.2.8a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.2.8a0
+Version: 0.2.8a1
 Summary: An interactive visualizer to help explore high-dimensional data and its observables.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inviz-0.2.8a0/README.md` & `inviz-0.2.8a1/README.md`

 * *Files identical despite different names*

### Comparing `inviz-0.2.8a0/inviz.egg-info/PKG-INFO` & `inviz-0.2.8a1/inviz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.2.8a0
+Version: 0.2.8a1
 Summary: An interactive visualizer to help explore high-dimensional data and its observables.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inviz-0.2.8a0/setup.py` & `inviz-0.2.8a1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "inviz",
-    version = "0.2.8a",
+    version = "0.2.8a1",
     author = "James Wen",
     author_email = "jswen@usc.edu",
     description = ("An interactive visualizer to help explore high-dimensional data and its observables."),
     license = "MIT",
     keywords = "interactive visualizer cosmology",
     url = "http://packages.python.org/inviz",
     # packages=setuptools.find_packages(where='src'),
```

### Comparing `inviz-0.2.8a0/src/cosmo/cosmo.py` & `inviz-0.2.8a1/src/cosmo/cosmo.py`

 * *Files identical despite different names*

### Comparing `inviz-0.2.8a0/src/inviz.py` & `inviz-0.2.8a1/src/inviz.py`

 * *Files identical despite different names*

