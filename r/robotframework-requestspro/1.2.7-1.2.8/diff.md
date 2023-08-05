# Comparing `tmp/robotframework-requestspro-1.2.7.tar.gz` & `tmp/robotframework-requestspro-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-requestspro-1.2.7.tar", last modified: Fri Aug  4 23:30:17 2023, max compression
+gzip compressed data, was "robotframework-requestspro-1.2.8.tar", last modified: Sat Aug  5 01:19:43 2023, max compression
```

## Comparing `robotframework-requestspro-1.2.7.tar` & `robotframework-requestspro-1.2.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 23:30:17.385274 robotframework-requestspro-1.2.7/
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     1069 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.7/LICENSE
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       34 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.7/MANIFEST.in
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-04 23:30:17.385146 robotframework-requestspro-1.2.7/PKG-INFO
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       31 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.7/README.md
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       85 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.7/requirements.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       38 2023-08-04 23:30:17.385319 robotframework-requestspro-1.2.7/setup.cfg
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     1689 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.7/setup.py
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 23:30:17.382434 robotframework-requestspro-1.2.7/src/
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 23:30:17.384154 robotframework-requestspro-1.2.7/src/RequestsProLibrary/
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     2458 2023-08-04 23:28:34.000000 robotframework-requestspro-1.2.7/src/RequestsProLibrary/DynamicTestCases.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)    12747 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.7/src/RequestsProLibrary/RequestsProKeywords.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     1966 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.7/src/RequestsProLibrary/__init__.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      182 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.7/src/RequestsProLibrary/compat.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       18 2023-08-04 23:23:53.000000 robotframework-requestspro-1.2.7/src/RequestsProLibrary/version.py
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 23:30:17.384966 robotframework-requestspro-1.2.7/src/robotframework_requestspro.egg-info/
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-04 23:30:17.000000 robotframework-requestspro-1.2.7/src/robotframework_requestspro.egg-info/PKG-INFO
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      515 2023-08-04 23:30:17.000000 robotframework-requestspro-1.2.7/src/robotframework_requestspro.egg-info/SOURCES.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)        1 2023-08-04 23:30:17.000000 robotframework-requestspro-1.2.7/src/robotframework_requestspro.egg-info/dependency_links.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       74 2023-08-04 23:30:17.000000 robotframework-requestspro-1.2.7/src/robotframework_requestspro.egg-info/requires.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       19 2023-08-04 23:30:17.000000 robotframework-requestspro-1.2.7/src/robotframework_requestspro.egg-info/top_level.txt
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-05 01:19:43.675123 robotframework-requestspro-1.2.8/
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     1069 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.8/LICENSE
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       34 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.8/MANIFEST.in
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-05 01:19:43.674997 robotframework-requestspro-1.2.8/PKG-INFO
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       31 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.8/README.md
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       85 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.8/requirements.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       38 2023-08-05 01:19:43.675168 robotframework-requestspro-1.2.8/setup.cfg
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     1689 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.8/setup.py
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-05 01:19:43.672626 robotframework-requestspro-1.2.8/src/
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-05 01:19:43.674235 robotframework-requestspro-1.2.8/src/RequestsProLibrary/
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     2469 2023-08-05 01:18:46.000000 robotframework-requestspro-1.2.8/src/RequestsProLibrary/DynamicTestCases.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)    12747 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.8/src/RequestsProLibrary/RequestsProKeywords.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     1966 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.8/src/RequestsProLibrary/__init__.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      182 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.8/src/RequestsProLibrary/compat.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       18 2023-08-05 00:37:06.000000 robotframework-requestspro-1.2.8/src/RequestsProLibrary/version.py
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-05 01:19:43.674815 robotframework-requestspro-1.2.8/src/robotframework_requestspro.egg-info/
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-05 01:19:43.000000 robotframework-requestspro-1.2.8/src/robotframework_requestspro.egg-info/PKG-INFO
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      515 2023-08-05 01:19:43.000000 robotframework-requestspro-1.2.8/src/robotframework_requestspro.egg-info/SOURCES.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)        1 2023-08-05 01:19:43.000000 robotframework-requestspro-1.2.8/src/robotframework_requestspro.egg-info/dependency_links.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       74 2023-08-05 01:19:43.000000 robotframework-requestspro-1.2.8/src/robotframework_requestspro.egg-info/requires.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       19 2023-08-05 01:19:43.000000 robotframework-requestspro-1.2.8/src/robotframework_requestspro.egg-info/top_level.txt
```

### Comparing `robotframework-requestspro-1.2.7/LICENSE` & `robotframework-requestspro-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.2.7/PKG-INFO` & `robotframework-requestspro-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-requestspro
-Version: 1.2.7
+Version: 1.2.8
 Summary: Robot Framework keyword library wrapper around requests
 Home-page: https://github.com/sridharvpmca/robotframework-requestspro
 Author: Sridhar VP
 Author-email: sridharvpmca@gmail.com
 License: MIT
 Keywords: robotframework testing test automation http client requests
 Platform: any
```

### Comparing `robotframework-requestspro-1.2.7/setup.py` & `robotframework-requestspro-1.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.2.7/src/RequestsProLibrary/DynamicTestCases.py` & `robotframework-requestspro-1.2.8/src/RequestsProLibrary/DynamicTestCases.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from robot.api import logger
 from typing import List
 import pandas as pd
 
 
 class DynamicTestCases(object):
     """A Robot Framework test library to dynamically add test cases to the current suite."""
-    ROBOT_LIBRARY_API_VERSION = 3
+    ROBOT_LISTENER_API_VERSION = 3
     ROBOT_LIBRARY_SCOPE = 'TEST SUITE'
 
     def __init__(self):
         self.ROBOT_LIBRARY_LISTENER = self
-        self.suite = None
+        self.current_suite = None
 
     def _start_suite(self, suite, result):
         self.current_suite = suite
 
     def add_test_case(self, name: str, doc: str, tags: List[str], kwname: str, **kwargs):
         """Adds a test case to the current suite.
 
@@ -28,15 +28,15 @@
         | Add Test Case | Example Test Case | This is a dynamic test case | ['smoke'] | My Keyword | arg1=value1 | arg2=value2 |
         """
         test_case = self.current_suite.tests.create(name=name, doc=doc, tags=tags)
         args = []
         for arg_name, arg_value in kwargs.items():
             args.append(f'{arg_name}={arg_value}')
         test_case.body.create_keyword(name=kwname, args=args)
-        self.suite.tests.append(test_case)
+        # self.suite.tests.append(test_case)
         logger.info(f"Added test case '{name}' with keyword '{kwname}' and keyword arguments: {kwargs}")
 
     def read_test_data_and_add_test_cases(self, csv_file_path: str):
         """Reads test data from a CSV file and adds test cases dynamically.
 
         `csv_file_path`: The path to the CSV file containing test data.
```

### Comparing `robotframework-requestspro-1.2.7/src/RequestsProLibrary/RequestsProKeywords.py` & `robotframework-requestspro-1.2.8/src/RequestsProLibrary/RequestsProKeywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.2.7/src/RequestsProLibrary/__init__.py` & `robotframework-requestspro-1.2.8/src/RequestsProLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.2.7/src/robotframework_requestspro.egg-info/PKG-INFO` & `robotframework-requestspro-1.2.8/src/robotframework_requestspro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-requestspro
-Version: 1.2.7
+Version: 1.2.8
 Summary: Robot Framework keyword library wrapper around requests
 Home-page: https://github.com/sridharvpmca/robotframework-requestspro
 Author: Sridhar VP
 Author-email: sridharvpmca@gmail.com
 License: MIT
 Keywords: robotframework testing test automation http client requests
 Platform: any
```

### Comparing `robotframework-requestspro-1.2.7/src/robotframework_requestspro.egg-info/SOURCES.txt` & `robotframework-requestspro-1.2.8/src/robotframework_requestspro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

