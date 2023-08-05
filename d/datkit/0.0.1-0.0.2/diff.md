# Comparing `tmp/datkit-0.0.1.tar.gz` & `tmp/datkit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datkit-0.0.1.tar", last modified: Sat Aug  5 15:56:43 2023, max compression
+gzip compressed data, was "datkit-0.0.2.tar", last modified: Sat Aug  5 16:17:32 2023, max compression
```

## Comparing `datkit-0.0.1.tar` & `datkit-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-05 15:56:43.029075 datkit-0.0.1/
--rw-r--r--   0 michael   (1000) michael   (1000)     1532 2023-08-04 17:27:22.000000 datkit-0.0.1/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)     1283 2023-08-05 15:56:43.029075 datkit-0.0.1/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      522 2023-08-05 15:55:22.000000 datkit-0.0.1/README.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-05 15:56:43.027075 datkit-0.0.1/datkit/
--rw-r--r--   0 michael   (1000) michael   (1000)     1013 2023-08-05 15:41:13.000000 datkit-0.0.1/datkit/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1588 2023-08-05 15:41:15.000000 datkit-0.0.1/datkit/_check_times.py
--rw-r--r--   0 michael   (1000) michael   (1000)      551 2023-08-05 15:41:18.000000 datkit-0.0.1/datkit/_datkit_version.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5111 2023-08-05 15:47:53.000000 datkit-0.0.1/datkit/_points.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-05 15:56:43.029075 datkit-0.0.1/datkit/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)      241 2023-08-05 15:41:23.000000 datkit-0.0.1/datkit/tests/__init__.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3346 2023-08-05 15:41:27.000000 datkit-0.0.1/datkit/tests/test_check_times.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     9668 2023-08-05 15:41:01.000000 datkit-0.0.1/datkit/tests/test_points.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-05 15:56:43.029075 datkit-0.0.1/datkit.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     1283 2023-08-05 15:56:42.000000 datkit-0.0.1/datkit.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      347 2023-08-05 15:56:42.000000 datkit-0.0.1/datkit.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-08-05 15:56:42.000000 datkit-0.0.1/datkit.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-08-05 15:56:42.000000 datkit-0.0.1/datkit.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        7 2023-08-05 15:56:42.000000 datkit-0.0.1/datkit.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-08-05 15:56:43.029075 datkit-0.0.1/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     2137 2023-08-05 15:50:26.000000 datkit-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:17:32.334106 datkit-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-08-05 16:17:22.000000 datkit-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-08-05 16:17:32.334106 datkit-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-05 16:17:22.000000 datkit-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:17:32.334106 datkit-0.0.2/datkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-05 16:17:22.000000 datkit-0.0.2/datkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-05 16:17:22.000000 datkit-0.0.2/datkit/_check_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-05 16:17:22.000000 datkit-0.0.2/datkit/_datkit_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-08-05 16:17:22.000000 datkit-0.0.2/datkit/_points.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:17:32.334106 datkit-0.0.2/datkit/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-05 16:17:22.000000 datkit-0.0.2/datkit/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3346 2023-08-05 16:17:22.000000 datkit-0.0.2/datkit/tests/test_check_times.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9668 2023-08-05 16:17:22.000000 datkit-0.0.2/datkit/tests/test_points.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:17:32.334106 datkit-0.0.2/datkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-08-05 16:17:32.000000 datkit-0.0.2/datkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-05 16:17:32.000000 datkit-0.0.2/datkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 16:17:32.000000 datkit-0.0.2/datkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-05 16:17:32.000000 datkit-0.0.2/datkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-05 16:17:32.000000 datkit-0.0.2/datkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 16:17:32.334106 datkit-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-08-05 16:17:22.000000 datkit-0.0.2/setup.py
```

### Comparing `datkit-0.0.1/LICENSE` & `datkit-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datkit-0.0.1/PKG-INFO` & `datkit-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datkit
-Version: 0.0.1
+Version: 0.0.2
 Summary: A bunch of scripts
 Author: Michael Clerx
 Author-email: michael@myokit.org
 License: BSD 3-clause license
 Project-URL: Bug Tracker, https://github.com/myokit/datkit/issues
 Project-URL: Documentation, http://datkit.readthedocs.io/
 Project-URL: Source Code, https://github.com/myokit/datkit
```

### Comparing `datkit-0.0.1/README.md` & `datkit-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `datkit-0.0.1/datkit/__init__.py` & `datkit-0.0.2/datkit/__init__.py`

 * *Files identical despite different names*

### Comparing `datkit-0.0.1/datkit/_check_times.py` & `datkit-0.0.2/datkit/_check_times.py`

 * *Files identical despite different names*

### Comparing `datkit-0.0.1/datkit/_datkit_version.py` & `datkit-0.0.2/datkit/_datkit_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,12 +7,12 @@
 
 # Version as a tuple (major, minor, revision)
 #  - Changes to major are rare
 #  - Changes to minor indicate new features, possible slight backwards
 #    incompatibility
 #  - Changes to revision indicate bugfixes, tiny new features
 #  - There is no significance to odd/even numbers
-__version_tuple__ = 0, 0, 1
+__version_tuple__ = 0, 0, 2
 
 # String version of the version number
 __version__ = '.'.join([str(x) for x in __version_tuple__])
```

### Comparing `datkit-0.0.1/datkit/_points.py` & `datkit-0.0.2/datkit/_points.py`

 * *Files identical despite different names*

### Comparing `datkit-0.0.1/datkit/tests/test_check_times.py` & `datkit-0.0.2/datkit/tests/test_check_times.py`

 * *Files identical despite different names*

### Comparing `datkit-0.0.1/datkit/tests/test_points.py` & `datkit-0.0.2/datkit/tests/test_points.py`

 * *Files identical despite different names*

### Comparing `datkit-0.0.1/datkit.egg-info/PKG-INFO` & `datkit-0.0.2/datkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datkit
-Version: 0.0.1
+Version: 0.0.2
 Summary: A bunch of scripts
 Author: Michael Clerx
 Author-email: michael@myokit.org
 License: BSD 3-clause license
 Project-URL: Bug Tracker, https://github.com/myokit/datkit/issues
 Project-URL: Documentation, http://datkit.readthedocs.io/
 Project-URL: Source Code, https://github.com/myokit/datkit
```

### Comparing `datkit-0.0.1/setup.py` & `datkit-0.0.2/setup.py`

 * *Files identical despite different names*

