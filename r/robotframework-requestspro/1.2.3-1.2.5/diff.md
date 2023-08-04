# Comparing `tmp/robotframework-requestspro-1.2.3.tar.gz` & `tmp/robotframework-requestspro-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-requestspro-1.2.3.tar", last modified: Fri Aug  4 13:32:10 2023, max compression
+gzip compressed data, was "robotframework-requestspro-1.2.5.tar", last modified: Fri Aug  4 14:22:34 2023, max compression
```

## Comparing `robotframework-requestspro-1.2.3.tar` & `robotframework-requestspro-1.2.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 13:32:10.456910 robotframework-requestspro-1.2.3/
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     1069 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.3/LICENSE
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       34 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.3/MANIFEST.in
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-04 13:32:10.456795 robotframework-requestspro-1.2.3/PKG-INFO
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       31 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.3/README.md
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       85 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.3/requirements.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       38 2023-08-04 13:32:10.456951 robotframework-requestspro-1.2.3/setup.cfg
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     1689 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.3/setup.py
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 13:32:10.454405 robotframework-requestspro-1.2.3/src/
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 13:32:10.456001 robotframework-requestspro-1.2.3/src/RequestsProLibrary/
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     2818 2023-08-04 13:31:45.000000 robotframework-requestspro-1.2.3/src/RequestsProLibrary/DynamicTestCases.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)    12747 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.3/src/RequestsProLibrary/RequestsProKeywords.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     1966 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.3/src/RequestsProLibrary/__init__.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      182 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.3/src/RequestsProLibrary/compat.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       18 2023-08-04 13:31:54.000000 robotframework-requestspro-1.2.3/src/RequestsProLibrary/version.py
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 13:32:10.456636 robotframework-requestspro-1.2.3/src/robotframework_requestspro.egg-info/
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-04 13:32:10.000000 robotframework-requestspro-1.2.3/src/robotframework_requestspro.egg-info/PKG-INFO
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      515 2023-08-04 13:32:10.000000 robotframework-requestspro-1.2.3/src/robotframework_requestspro.egg-info/SOURCES.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)        1 2023-08-04 13:32:10.000000 robotframework-requestspro-1.2.3/src/robotframework_requestspro.egg-info/dependency_links.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       74 2023-08-04 13:32:10.000000 robotframework-requestspro-1.2.3/src/robotframework_requestspro.egg-info/requires.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       19 2023-08-04 13:32:10.000000 robotframework-requestspro-1.2.3/src/robotframework_requestspro.egg-info/top_level.txt
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 14:22:34.712310 robotframework-requestspro-1.2.5/
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     1069 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.5/LICENSE
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       34 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.5/MANIFEST.in
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-04 14:22:34.712190 robotframework-requestspro-1.2.5/PKG-INFO
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       31 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.5/README.md
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       85 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.5/requirements.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       38 2023-08-04 14:22:34.712351 robotframework-requestspro-1.2.5/setup.cfg
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     1689 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.5/setup.py
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 14:22:34.709834 robotframework-requestspro-1.2.5/src/
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 14:22:34.711433 robotframework-requestspro-1.2.5/src/RequestsProLibrary/
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     1918 2023-08-04 14:21:57.000000 robotframework-requestspro-1.2.5/src/RequestsProLibrary/DynamicTestCases.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)    12747 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.5/src/RequestsProLibrary/RequestsProKeywords.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     1966 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.5/src/RequestsProLibrary/__init__.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      182 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.5/src/RequestsProLibrary/compat.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       18 2023-08-04 14:17:52.000000 robotframework-requestspro-1.2.5/src/RequestsProLibrary/version.py
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 14:22:34.712018 robotframework-requestspro-1.2.5/src/robotframework_requestspro.egg-info/
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-04 14:22:34.000000 robotframework-requestspro-1.2.5/src/robotframework_requestspro.egg-info/PKG-INFO
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      515 2023-08-04 14:22:34.000000 robotframework-requestspro-1.2.5/src/robotframework_requestspro.egg-info/SOURCES.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)        1 2023-08-04 14:22:34.000000 robotframework-requestspro-1.2.5/src/robotframework_requestspro.egg-info/dependency_links.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       74 2023-08-04 14:22:34.000000 robotframework-requestspro-1.2.5/src/robotframework_requestspro.egg-info/requires.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       19 2023-08-04 14:22:34.000000 robotframework-requestspro-1.2.5/src/robotframework_requestspro.egg-info/top_level.txt
```

### Comparing `robotframework-requestspro-1.2.3/LICENSE` & `robotframework-requestspro-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.2.3/PKG-INFO` & `robotframework-requestspro-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-requestspro
-Version: 1.2.3
+Version: 1.2.5
 Summary: Robot Framework keyword library wrapper around requests
 Home-page: https://github.com/sridharvpmca/robotframework-requestspro
 Author: Sridhar VP
 Author-email: sridharvpmca@gmail.com
 License: MIT
 Keywords: robotframework testing test automation http client requests
 Platform: any
```

### Comparing `robotframework-requestspro-1.2.3/setup.py` & `robotframework-requestspro-1.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.2.3/src/RequestsProLibrary/RequestsProKeywords.py` & `robotframework-requestspro-1.2.5/src/RequestsProLibrary/RequestsProKeywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.2.3/src/RequestsProLibrary/__init__.py` & `robotframework-requestspro-1.2.5/src/RequestsProLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.2.3/src/robotframework_requestspro.egg-info/PKG-INFO` & `robotframework-requestspro-1.2.5/src/robotframework_requestspro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-requestspro
-Version: 1.2.3
+Version: 1.2.5
 Summary: Robot Framework keyword library wrapper around requests
 Home-page: https://github.com/sridharvpmca/robotframework-requestspro
 Author: Sridhar VP
 Author-email: sridharvpmca@gmail.com
 License: MIT
 Keywords: robotframework testing test automation http client requests
 Platform: any
```

### Comparing `robotframework-requestspro-1.2.3/src/robotframework_requestspro.egg-info/SOURCES.txt` & `robotframework-requestspro-1.2.5/src/robotframework_requestspro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

