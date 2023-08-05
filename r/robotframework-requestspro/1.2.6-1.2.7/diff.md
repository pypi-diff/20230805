# Comparing `tmp/robotframework-requestspro-1.2.6.tar.gz` & `tmp/robotframework-requestspro-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-requestspro-1.2.6.tar", last modified: Fri Aug  4 22:50:59 2023, max compression
+gzip compressed data, was "robotframework-requestspro-1.2.7.tar", last modified: Fri Aug  4 23:30:17 2023, max compression
```

## Comparing `robotframework-requestspro-1.2.6.tar` & `robotframework-requestspro-1.2.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 22:50:59.354065 robotframework-requestspro-1.2.6/
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     1069 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.6/LICENSE
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       34 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.6/MANIFEST.in
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-04 22:50:59.353908 robotframework-requestspro-1.2.6/PKG-INFO
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       31 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.6/README.md
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       85 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.6/requirements.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       38 2023-08-04 22:50:59.354118 robotframework-requestspro-1.2.6/setup.cfg
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     1689 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.6/setup.py
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 22:50:59.349219 robotframework-requestspro-1.2.6/src/
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 22:50:59.352535 robotframework-requestspro-1.2.6/src/RequestsProLibrary/
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     2356 2023-08-04 22:48:32.000000 robotframework-requestspro-1.2.6/src/RequestsProLibrary/DynamicTestCases.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)    12747 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.6/src/RequestsProLibrary/RequestsProKeywords.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     1966 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.6/src/RequestsProLibrary/__init__.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      182 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.6/src/RequestsProLibrary/compat.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       18 2023-08-04 22:48:39.000000 robotframework-requestspro-1.2.6/src/RequestsProLibrary/version.py
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 22:50:59.353675 robotframework-requestspro-1.2.6/src/robotframework_requestspro.egg-info/
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-04 22:50:59.000000 robotframework-requestspro-1.2.6/src/robotframework_requestspro.egg-info/PKG-INFO
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      515 2023-08-04 22:50:59.000000 robotframework-requestspro-1.2.6/src/robotframework_requestspro.egg-info/SOURCES.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)        1 2023-08-04 22:50:59.000000 robotframework-requestspro-1.2.6/src/robotframework_requestspro.egg-info/dependency_links.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       74 2023-08-04 22:50:59.000000 robotframework-requestspro-1.2.6/src/robotframework_requestspro.egg-info/requires.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       19 2023-08-04 22:50:59.000000 robotframework-requestspro-1.2.6/src/robotframework_requestspro.egg-info/top_level.txt
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 23:30:17.385274 robotframework-requestspro-1.2.7/
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     1069 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.7/LICENSE
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       34 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.7/MANIFEST.in
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-04 23:30:17.385146 robotframework-requestspro-1.2.7/PKG-INFO
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       31 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.7/README.md
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       85 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.7/requirements.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       38 2023-08-04 23:30:17.385319 robotframework-requestspro-1.2.7/setup.cfg
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     1689 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.7/setup.py
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 23:30:17.382434 robotframework-requestspro-1.2.7/src/
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 23:30:17.384154 robotframework-requestspro-1.2.7/src/RequestsProLibrary/
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     2458 2023-08-04 23:28:34.000000 robotframework-requestspro-1.2.7/src/RequestsProLibrary/DynamicTestCases.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)    12747 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.7/src/RequestsProLibrary/RequestsProKeywords.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     1966 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.7/src/RequestsProLibrary/__init__.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      182 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.7/src/RequestsProLibrary/compat.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       18 2023-08-04 23:23:53.000000 robotframework-requestspro-1.2.7/src/RequestsProLibrary/version.py
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 23:30:17.384966 robotframework-requestspro-1.2.7/src/robotframework_requestspro.egg-info/
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-04 23:30:17.000000 robotframework-requestspro-1.2.7/src/robotframework_requestspro.egg-info/PKG-INFO
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      515 2023-08-04 23:30:17.000000 robotframework-requestspro-1.2.7/src/robotframework_requestspro.egg-info/SOURCES.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)        1 2023-08-04 23:30:17.000000 robotframework-requestspro-1.2.7/src/robotframework_requestspro.egg-info/dependency_links.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       74 2023-08-04 23:30:17.000000 robotframework-requestspro-1.2.7/src/robotframework_requestspro.egg-info/requires.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       19 2023-08-04 23:30:17.000000 robotframework-requestspro-1.2.7/src/robotframework_requestspro.egg-info/top_level.txt
```

### Comparing `robotframework-requestspro-1.2.6/LICENSE` & `robotframework-requestspro-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.2.6/PKG-INFO` & `robotframework-requestspro-1.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-requestspro
-Version: 1.2.6
+Version: 1.2.7
 Summary: Robot Framework keyword library wrapper around requests
 Home-page: https://github.com/sridharvpmca/robotframework-requestspro
 Author: Sridhar VP
 Author-email: sridharvpmca@gmail.com
 License: MIT
 Keywords: robotframework testing test automation http client requests
 Platform: any
```

### Comparing `robotframework-requestspro-1.2.6/setup.py` & `robotframework-requestspro-1.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.2.6/src/RequestsProLibrary/DynamicTestCases.py` & `robotframework-requestspro-1.2.7/src/RequestsProLibrary/DynamicTestCases.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,16 @@
         `**kwargs`: Keyword arguments to be passed to the keyword.
 
         Example:
         | Add Test Case | Example Test Case | This is a dynamic test case | ['smoke'] | My Keyword | arg1=value1 | arg2=value2 |
         """
         test_case = self.current_suite.tests.create(name=name, doc=doc, tags=tags)
         args = []
+        for arg_name, arg_value in kwargs.items():
+            args.append(f'{arg_name}={arg_value}')
         test_case.body.create_keyword(name=kwname, args=args)
         self.suite.tests.append(test_case)
         logger.info(f"Added test case '{name}' with keyword '{kwname}' and keyword arguments: {kwargs}")
 
     def read_test_data_and_add_test_cases(self, csv_file_path: str):
         """Reads test data from a CSV file and adds test cases dynamically.
```

### Comparing `robotframework-requestspro-1.2.6/src/RequestsProLibrary/RequestsProKeywords.py` & `robotframework-requestspro-1.2.7/src/RequestsProLibrary/RequestsProKeywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.2.6/src/RequestsProLibrary/__init__.py` & `robotframework-requestspro-1.2.7/src/RequestsProLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.2.6/src/robotframework_requestspro.egg-info/PKG-INFO` & `robotframework-requestspro-1.2.7/src/robotframework_requestspro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-requestspro
-Version: 1.2.6
+Version: 1.2.7
 Summary: Robot Framework keyword library wrapper around requests
 Home-page: https://github.com/sridharvpmca/robotframework-requestspro
 Author: Sridhar VP
 Author-email: sridharvpmca@gmail.com
 License: MIT
 Keywords: robotframework testing test automation http client requests
 Platform: any
```

### Comparing `robotframework-requestspro-1.2.6/src/robotframework_requestspro.egg-info/SOURCES.txt` & `robotframework-requestspro-1.2.7/src/robotframework_requestspro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

