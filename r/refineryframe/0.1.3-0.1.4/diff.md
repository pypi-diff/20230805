# Comparing `tmp/refineryframe-0.1.3.tar.gz` & `tmp/refineryframe-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refineryframe-0.1.3.tar", last modified: Thu Aug  3 21:55:56 2023, max compression
+gzip compressed data, was "refineryframe-0.1.4.tar", last modified: Sat Aug  5 01:10:19 2023, max compression
```

## Comparing `refineryframe-0.1.3.tar` & `refineryframe-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:55:56.829678 refineryframe-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-03 21:55:43.000000 refineryframe-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    31929 2023-08-03 21:55:56.829678 refineryframe-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31144 2023-08-03 21:55:43.000000 refineryframe-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:55:56.829678 refineryframe-0.1.3/refineryframe/
--rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-08-03 21:55:43.000000 refineryframe-0.1.3/refineryframe/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36432 2023-08-03 21:55:43.000000 refineryframe-0.1.3/refineryframe/detect_unexpected.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12527 2023-08-03 21:55:43.000000 refineryframe-0.1.3/refineryframe/other.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19516 2023-08-03 21:55:43.000000 refineryframe-0.1.3/refineryframe/refiner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14051 2023-08-03 21:55:43.000000 refineryframe-0.1.3/refineryframe/replace_unexpected.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:55:56.829678 refineryframe-0.1.3/refineryframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    31929 2023-08-03 21:55:56.000000 refineryframe-0.1.3/refineryframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-03 21:55:56.000000 refineryframe-0.1.3/refineryframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 21:55:56.000000 refineryframe-0.1.3/refineryframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-03 21:55:56.000000 refineryframe-0.1.3/refineryframe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-03 21:55:56.000000 refineryframe-0.1.3/refineryframe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 21:55:56.829678 refineryframe-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-03 21:55:55.000000 refineryframe-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:55:56.829678 refineryframe-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 21:55:43.000000 refineryframe-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-08-03 21:55:43.000000 refineryframe-0.1.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-08-03 21:55:43.000000 refineryframe-0.1.3/tests/test_refiner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:10:19.170590 refineryframe-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-05 01:10:06.000000 refineryframe-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    31957 2023-08-05 01:10:19.170590 refineryframe-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31172 2023-08-05 01:10:18.000000 refineryframe-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:10:19.170590 refineryframe-0.1.4/refineryframe/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-08-05 01:10:06.000000 refineryframe-0.1.4/refineryframe/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36509 2023-08-05 01:10:06.000000 refineryframe-0.1.4/refineryframe/detect_unexpected.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12527 2023-08-05 01:10:06.000000 refineryframe-0.1.4/refineryframe/other.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19573 2023-08-05 01:10:06.000000 refineryframe-0.1.4/refineryframe/refiner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14051 2023-08-05 01:10:06.000000 refineryframe-0.1.4/refineryframe/replace_unexpected.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:10:19.170590 refineryframe-0.1.4/refineryframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    31957 2023-08-05 01:10:19.000000 refineryframe-0.1.4/refineryframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-05 01:10:19.000000 refineryframe-0.1.4/refineryframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 01:10:19.000000 refineryframe-0.1.4/refineryframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-05 01:10:19.000000 refineryframe-0.1.4/refineryframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-05 01:10:19.000000 refineryframe-0.1.4/refineryframe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 01:10:19.170590 refineryframe-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-05 01:10:18.000000 refineryframe-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:10:19.170590 refineryframe-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 01:10:06.000000 refineryframe-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-08-05 01:10:06.000000 refineryframe-0.1.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-08-05 01:10:06.000000 refineryframe-0.1.4/tests/test_refiner.py
```

### Comparing `refineryframe-0.1.3/LICENSE` & `refineryframe-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.3/PKG-INFO` & `refineryframe-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refineryframe
-Version: 0.1.3
+Version: 0.1.4
 Summary: Cleans data, best to be used as a part of initial preprocessor
 Home-page: UNKNOWN
 Author: Kyrylo Mordan
 Author-email: <parachute.repo@gmail.com>
 License: UNKNOWN
 Keywords: python,data cleaning,safeguards
 Platform: UNKNOWN
@@ -879,14 +879,15 @@
      'logger_name': 'Refiner',
      'loggerLvl': 10,
      'dotline_length': 50,
      'lower_bound': -inf,
      'upper_bound': inf,
      'earliest_date': '1900-08-25',
      'latest_date': '2100-01-01',
+     'ids_for_dedup': None,
      'unexpected_exceptions_duv': {'col_names_types': 'NONE',
       'missing_values': 'ALL',
       'missing_types': 'ALL',
       'inf_values': 'NONE',
       'date_format': 'NONE',
       'duplicates': 'ALL',
       'date_range': 'NONE',
```

### Comparing `refineryframe-0.1.3/README.md` & `refineryframe-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -856,14 +856,15 @@
      'logger_name': 'Refiner',
      'loggerLvl': 10,
      'dotline_length': 50,
      'lower_bound': -inf,
      'upper_bound': inf,
      'earliest_date': '1900-08-25',
      'latest_date': '2100-01-01',
+     'ids_for_dedup': None,
      'unexpected_exceptions_duv': {'col_names_types': 'NONE',
       'missing_values': 'ALL',
       'missing_types': 'ALL',
       'inf_values': 'NONE',
       'date_format': 'NONE',
       'duplicates': 'ALL',
       'date_range': 'NONE',
```

### Comparing `refineryframe-0.1.3/refineryframe/detect_unexpected.py` & `refineryframe-0.1.4/refineryframe/detect_unexpected.py`

 * *Files 0% similar despite different names*

```diff
@@ -705,16 +705,20 @@
 
         if unexpected_conditions:
             run_check_additional_cons = sum([unexpected_conditions[i]['warning'] for i in unexpected_conditions]) > 0
         else:
             run_check_additional_cons = False
 
 
-        if ids_for_dup is None and len(index_cols) > 0:
-            ids_for_dup = index_cols
+        if ids_for_dup is None:
+
+            if len(index_cols) > 0:
+                ids_for_dup = index_cols
+            else:
+                ids_for_dup = all_columns
 
 
         # Checks scan
         unexpected_exceptions_scaned = {
             "col_names_types": "NONE",
             "missing_values": "NONE",
             "missing_types": "NONE",
```

### Comparing `refineryframe-0.1.3/refineryframe/other.py` & `refineryframe-0.1.4/refineryframe/other.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.3/refineryframe/refiner.py` & `refineryframe-0.1.4/refineryframe/refiner.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,16 @@
     dotline_length = attr.ib(default=50, type=int)
 
     lower_bound = attr.ib(default=-float("inf"))
     upper_bound = attr.ib(default=float("inf"))
     earliest_date = attr.ib(default="1900-08-25")
     latest_date = attr.ib(default="2100-01-01")
 
+    ids_for_dedup = attr.ib(default=None)
+
     unexpected_exceptions_duv = attr.ib(default={"col_names_types": "NONE",
                                               "missing_values": "NONE",
                                               "missing_types": "NONE",
                                               "inf_values": "NONE",
                                               "date_format": "NONE",
                                               "duplicates": "NONE",
                                               "date_range": "NONE",
@@ -403,15 +405,15 @@
         if dataframe is None:
             dataframe = self.dataframe
 
         duv_obj = detect_unexpected_values(dataframe = dataframe,
                                                  MISSING_TYPES = self.MISSING_TYPES,
                                                  unexpected_exceptions = self.unexpected_exceptions_duv,
                                                  unexpected_conditions = self.unexpected_conditions,
-                                                 ids_for_dup = None,
+                                                 ids_for_dup = self.ids_for_dedup,
                                                  TEST_DUV_FLAGS_PATH = None,
                                                  types_dict_str = self.type_dict,
                                                  expected_date_format = self.expected_date_format,
                                                  earliest_date = self.earliest_date,
                                                  latest_date = self.latest_date,
                                                  numeric_lower_bound = self.lower_bound,
                                                  numeric_upper_bound = self.upper_bound,
```

### Comparing `refineryframe-0.1.3/refineryframe/replace_unexpected.py` & `refineryframe-0.1.4/refineryframe/replace_unexpected.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.3/refineryframe.egg-info/PKG-INFO` & `refineryframe-0.1.4/refineryframe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refineryframe
-Version: 0.1.3
+Version: 0.1.4
 Summary: Cleans data, best to be used as a part of initial preprocessor
 Home-page: UNKNOWN
 Author: Kyrylo Mordan
 Author-email: <parachute.repo@gmail.com>
 License: UNKNOWN
 Keywords: python,data cleaning,safeguards
 Platform: UNKNOWN
@@ -879,14 +879,15 @@
      'logger_name': 'Refiner',
      'loggerLvl': 10,
      'dotline_length': 50,
      'lower_bound': -inf,
      'upper_bound': inf,
      'earliest_date': '1900-08-25',
      'latest_date': '2100-01-01',
+     'ids_for_dedup': None,
      'unexpected_exceptions_duv': {'col_names_types': 'NONE',
       'missing_values': 'ALL',
       'missing_types': 'ALL',
       'inf_values': 'NONE',
       'date_format': 'NONE',
       'duplicates': 'ALL',
       'date_range': 'NONE',
```

### Comparing `refineryframe-0.1.3/setup.py` & `refineryframe-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "attrs>=22.2.0",
     "datetime",
     "pandas",
     "numpy",
     "unidecode"
 ]
 
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 DESCRIPTION = 'Cleans data, best to be used as a part of initial preprocessor'
 LONG_DESCRIPTION = 'A package that allows to detect unexpected values in data and clean them according to set of predefined rules'
 
 # Setting up
 setup(
     name="refineryframe",
     #use_scm_version=True,
```

### Comparing `refineryframe-0.1.3/tests/conftest.py` & `refineryframe-0.1.4/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,15 @@
                         'logger_name': 'Refiner',
                         'loggerLvl': 10,
                         'dotline_length': 50,
                         'lower_bound': -np.inf,
                         'upper_bound': np.inf,
                         'earliest_date': '1900-08-25',
                         'latest_date': '2100-01-01',
+                        'ids_for_dedup': None,
                         'unexpected_exceptions_duv': {'col_names_types': 'NONE',
                         'missing_values': 'ALL',
                         'missing_types': 'ALL',
                         'inf_values': 'NONE',
                         'date_format': 'NONE',
                         'duplicates': 'ALL',
                         'date_range': 'NONE',
```

### Comparing `refineryframe-0.1.3/tests/test_refiner.py` & `refineryframe-0.1.4/tests/test_refiner.py`

 * *Files identical despite different names*

