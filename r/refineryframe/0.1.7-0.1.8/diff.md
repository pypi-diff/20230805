# Comparing `tmp/refineryframe-0.1.7.tar.gz` & `tmp/refineryframe-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refineryframe-0.1.7.tar", last modified: Sat Aug  5 13:47:34 2023, max compression
+gzip compressed data, was "refineryframe-0.1.8.tar", last modified: Sat Aug  5 14:04:51 2023, max compression
```

## Comparing `refineryframe-0.1.7.tar` & `refineryframe-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:47:34.557942 refineryframe-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-05 13:47:21.000000 refineryframe-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    31901 2023-08-05 13:47:34.557942 refineryframe-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31172 2023-08-05 13:47:21.000000 refineryframe-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:47:34.553942 refineryframe-0.1.7/refineryframe/
--rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-08-05 13:47:21.000000 refineryframe-0.1.7/refineryframe/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36563 2023-08-05 13:47:21.000000 refineryframe-0.1.7/refineryframe/detect_unexpected.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12527 2023-08-05 13:47:21.000000 refineryframe-0.1.7/refineryframe/other.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24623 2023-08-05 13:47:21.000000 refineryframe-0.1.7/refineryframe/refiner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14051 2023-08-05 13:47:21.000000 refineryframe-0.1.7/refineryframe/replace_unexpected.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:47:34.557942 refineryframe-0.1.7/refineryframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    31901 2023-08-05 13:47:34.000000 refineryframe-0.1.7/refineryframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-05 13:47:34.000000 refineryframe-0.1.7/refineryframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 13:47:34.000000 refineryframe-0.1.7/refineryframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-05 13:47:34.000000 refineryframe-0.1.7/refineryframe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-05 13:47:34.000000 refineryframe-0.1.7/refineryframe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 13:47:34.557942 refineryframe-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-05 13:47:32.000000 refineryframe-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:47:34.557942 refineryframe-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 13:47:21.000000 refineryframe-0.1.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-08-05 13:47:21.000000 refineryframe-0.1.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-08-05 13:47:21.000000 refineryframe-0.1.7/tests/test_refiner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:04:51.067758 refineryframe-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-05 14:04:38.000000 refineryframe-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    31901 2023-08-05 14:04:51.063758 refineryframe-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31172 2023-08-05 14:04:38.000000 refineryframe-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:04:51.063758 refineryframe-0.1.8/refineryframe/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-08-05 14:04:38.000000 refineryframe-0.1.8/refineryframe/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36627 2023-08-05 14:04:38.000000 refineryframe-0.1.8/refineryframe/detect_unexpected.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12527 2023-08-05 14:04:38.000000 refineryframe-0.1.8/refineryframe/other.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24623 2023-08-05 14:04:38.000000 refineryframe-0.1.8/refineryframe/refiner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14051 2023-08-05 14:04:38.000000 refineryframe-0.1.8/refineryframe/replace_unexpected.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:04:51.063758 refineryframe-0.1.8/refineryframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    31901 2023-08-05 14:04:50.000000 refineryframe-0.1.8/refineryframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-05 14:04:51.000000 refineryframe-0.1.8/refineryframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 14:04:50.000000 refineryframe-0.1.8/refineryframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-05 14:04:50.000000 refineryframe-0.1.8/refineryframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-05 14:04:50.000000 refineryframe-0.1.8/refineryframe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 14:04:51.067758 refineryframe-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-05 14:04:50.000000 refineryframe-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:04:51.063758 refineryframe-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 14:04:38.000000 refineryframe-0.1.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-08-05 14:04:38.000000 refineryframe-0.1.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-08-05 14:04:38.000000 refineryframe-0.1.8/tests/test_refiner.py
```

### Comparing `refineryframe-0.1.7/LICENSE` & `refineryframe-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.7/PKG-INFO` & `refineryframe-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refineryframe
-Version: 0.1.7
+Version: 0.1.8
 Summary: Cleans data, best to be used as a part of initial preprocessor
 Author: Kyrylo Mordan
 Author-email: <parachute.repo@gmail.com>
 Keywords: python,data cleaning,safeguards
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `refineryframe-0.1.7/README.md` & `refineryframe-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.7/refineryframe/detect_unexpected.py` & `refineryframe-0.1.8/refineryframe/detect_unexpected.py`

 * *Files 1% similar despite different names*

```diff
@@ -707,18 +707,18 @@
             run_check_additional_cons = sum([unexpected_conditions[i]['warning'] for i in unexpected_conditions]) > 0
         else:
             run_check_additional_cons = False
 
 
         if ids_for_dedup is None:
 
-            if len(index_cols) > 0:
-                ids_for_dedup = index_cols
+            if (len(index_cols) > 0) and (index_cols in list(dataframe.columns)):
+                ids_for_dedup = list(index_cols)
             else:
-                ids_for_dedup = all_columns
+                ids_for_dedup = list(dataframe.columns)
 
 
         # Checks scan
         unexpected_exceptions_scaned = {
             "col_names_types": "NONE",
             "missing_values": "NONE",
             "missing_types": "NONE",
```

### Comparing `refineryframe-0.1.7/refineryframe/other.py` & `refineryframe-0.1.8/refineryframe/other.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.7/refineryframe/refiner.py` & `refineryframe-0.1.8/refineryframe/refiner.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.7/refineryframe/replace_unexpected.py` & `refineryframe-0.1.8/refineryframe/replace_unexpected.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.7/refineryframe.egg-info/PKG-INFO` & `refineryframe-0.1.8/refineryframe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refineryframe
-Version: 0.1.7
+Version: 0.1.8
 Summary: Cleans data, best to be used as a part of initial preprocessor
 Author: Kyrylo Mordan
 Author-email: <parachute.repo@gmail.com>
 Keywords: python,data cleaning,safeguards
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `refineryframe-0.1.7/setup.py` & `refineryframe-0.1.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "attrs>=22.2.0",
     "datetime",
     "pandas",
     "numpy",
     "unidecode"
 ]
 
-VERSION = '0.1.7'
+VERSION = '0.1.8'
 DESCRIPTION = 'Cleans data, best to be used as a part of initial preprocessor'
 LONG_DESCRIPTION = 'A package that allows to detect unexpected values in data and clean them according to set of predefined rules'
 
 # Setting up
 setup(
     name="refineryframe",
     #use_scm_version=True,
```

### Comparing `refineryframe-0.1.7/tests/conftest.py` & `refineryframe-0.1.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.7/tests/test_refiner.py` & `refineryframe-0.1.8/tests/test_refiner.py`

 * *Files identical despite different names*

