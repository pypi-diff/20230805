# Comparing `tmp/refineryframe-0.1.5.tar.gz` & `tmp/refineryframe-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refineryframe-0.1.5.tar", last modified: Sat Aug  5 01:39:26 2023, max compression
+gzip compressed data, was "refineryframe-0.1.6.tar", last modified: Sat Aug  5 13:29:42 2023, max compression
```

## Comparing `refineryframe-0.1.5.tar` & `refineryframe-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:39:26.811550 refineryframe-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-05 01:39:09.000000 refineryframe-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    31957 2023-08-05 01:39:26.811550 refineryframe-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31172 2023-08-05 01:39:09.000000 refineryframe-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:39:26.811550 refineryframe-0.1.5/refineryframe/
--rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-08-05 01:39:09.000000 refineryframe-0.1.5/refineryframe/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36509 2023-08-05 01:39:09.000000 refineryframe-0.1.5/refineryframe/detect_unexpected.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12527 2023-08-05 01:39:09.000000 refineryframe-0.1.5/refineryframe/other.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24540 2023-08-05 01:39:09.000000 refineryframe-0.1.5/refineryframe/refiner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14051 2023-08-05 01:39:09.000000 refineryframe-0.1.5/refineryframe/replace_unexpected.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:39:26.811550 refineryframe-0.1.5/refineryframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    31957 2023-08-05 01:39:26.000000 refineryframe-0.1.5/refineryframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-05 01:39:26.000000 refineryframe-0.1.5/refineryframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 01:39:26.000000 refineryframe-0.1.5/refineryframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-05 01:39:26.000000 refineryframe-0.1.5/refineryframe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-05 01:39:26.000000 refineryframe-0.1.5/refineryframe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 01:39:26.811550 refineryframe-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-05 01:39:25.000000 refineryframe-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:39:26.811550 refineryframe-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 01:39:09.000000 refineryframe-0.1.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-08-05 01:39:09.000000 refineryframe-0.1.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-08-05 01:39:09.000000 refineryframe-0.1.5/tests/test_refiner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:29:42.253757 refineryframe-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-05 13:29:31.000000 refineryframe-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    31957 2023-08-05 13:29:42.253757 refineryframe-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31172 2023-08-05 13:29:31.000000 refineryframe-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:29:42.253757 refineryframe-0.1.6/refineryframe/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-08-05 13:29:31.000000 refineryframe-0.1.6/refineryframe/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36563 2023-08-05 13:29:31.000000 refineryframe-0.1.6/refineryframe/detect_unexpected.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12527 2023-08-05 13:29:31.000000 refineryframe-0.1.6/refineryframe/other.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24612 2023-08-05 13:29:31.000000 refineryframe-0.1.6/refineryframe/refiner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14051 2023-08-05 13:29:31.000000 refineryframe-0.1.6/refineryframe/replace_unexpected.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:29:42.253757 refineryframe-0.1.6/refineryframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    31957 2023-08-05 13:29:42.000000 refineryframe-0.1.6/refineryframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-05 13:29:42.000000 refineryframe-0.1.6/refineryframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 13:29:42.000000 refineryframe-0.1.6/refineryframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-05 13:29:42.000000 refineryframe-0.1.6/refineryframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-05 13:29:42.000000 refineryframe-0.1.6/refineryframe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 13:29:42.253757 refineryframe-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-05 13:29:41.000000 refineryframe-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:29:42.253757 refineryframe-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 13:29:31.000000 refineryframe-0.1.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-08-05 13:29:31.000000 refineryframe-0.1.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-08-05 13:29:31.000000 refineryframe-0.1.6/tests/test_refiner.py
```

### Comparing `refineryframe-0.1.5/LICENSE` & `refineryframe-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.5/PKG-INFO` & `refineryframe-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refineryframe
-Version: 0.1.5
+Version: 0.1.6
 Summary: Cleans data, best to be used as a part of initial preprocessor
 Home-page: UNKNOWN
 Author: Kyrylo Mordan
 Author-email: <parachute.repo@gmail.com>
 License: UNKNOWN
 Keywords: python,data cleaning,safeguards
 Platform: UNKNOWN
```

### Comparing `refineryframe-0.1.5/README.md` & `refineryframe-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.5/refineryframe/detect_unexpected.py` & `refineryframe-0.1.6/refineryframe/detect_unexpected.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,15 +318,15 @@
 
         ROW_DUPLICATES = False
         KEY_DUPLICATES = False
 
         duplicates = dataframe.duplicated()
         n_duplicates = duplicates.sum()
 
-        if subset is not None:
+        if (subset is not None) and (subset in list(dataframe.columns)):
             subset_duplicates = dataframe.duplicated(subset=subset)
             n_subset_duplicates = subset_duplicates.sum()
 
             if n_subset_duplicates > 0:
                 logger.warning(f"There are {n_subset_duplicates} duplicate keys : {n_subset_duplicates/dataframe.shape[0]*100:.2f}%")
 
                 n_true_dup = n_subset_duplicates - n_duplicates
@@ -609,15 +609,15 @@
                                                       "missing_types": "NONE",
                                                       "inf_values": "NONE",
                                                       "date_format": "NONE",
                                                       "duplicates": "NONE",
                                                       "date_range": "NONE",
                                                       "numeric_range": "NONE"},
                              unexpected_conditions : dict = None,
-                             ids_for_dup : list = None,
+                             ids_for_dedup : list = None,
                              TEST_DUV_FLAGS_PATH : str = None,
                              types_dict_str : dict = None,
                              expected_date_format : str = '%Y-%m-%d',
                              earliest_date : str = "1900-08-25",
                              latest_date : str = "2100-01-01",
                              numeric_lower_bound : float = 0,
                              numeric_upper_bound : float = float("inf"),
@@ -632,15 +632,15 @@
 
     dataframe (pandas DataFrame): The DataFrame to be checked.
     MISSING_TYPES (dict): Dictionary that maps column names to the values considered as missing
                               for that column.
     unexpected_exceptions (dict): Dictionary that lists column exceptions for each of the
                                       following checks: col_names_types, missing_values, missing_types,
                                       inf_values, date_format, duplicates, date_range, and numeric_range.
-    ids_for_dup (list): List of columns to identify duplicates (default is None).
+    ids_for_dedup (list): List of columns to identify duplicates (default is None).
     TEST_DUV_FLAGS_PATH (str): Path for checking unexpected values (default is None).
     types_dict_str (str): String that describes the expected types of the columns (default is None).
     expected_date_format (str): The expected date format (default is '%Y-%m-%d').
     earliest_date (str): The earliest acceptable date (default is "1900-08-25").
     latest_date (str): The latest acceptable date (default is "2100-01-01").
     numeric_lower_bound (float): The lowest acceptable value for numeric columns (default is 0).
     numeric_upper_bound (float): The highest acceptable value for numeric columns
@@ -705,20 +705,20 @@
 
         if unexpected_conditions:
             run_check_additional_cons = sum([unexpected_conditions[i]['warning'] for i in unexpected_conditions]) > 0
         else:
             run_check_additional_cons = False
 
 
-        if ids_for_dup is None:
+        if ids_for_dedup is None:
 
             if len(index_cols) > 0:
-                ids_for_dup = index_cols
+                ids_for_dedup = index_cols
             else:
-                ids_for_dup = all_columns
+                ids_for_dedup = all_columns
 
 
         # Checks scan
         unexpected_exceptions_scaned = {
             "col_names_types": "NONE",
             "missing_values": "NONE",
             "missing_types": "NONE",
@@ -796,15 +796,15 @@
                 unexpected_exceptions_scaned["date_range"] = "ALL"
 
         if run_check_duplicates:
 
             logger.debug("=== checking for duplicates")
 
             checks_list.extend(check_duplicates(dataframe = dataframe[cols_check_duplicates],
-                             subset = ids_for_dup,
+                             subset = ids_for_dedup,
                              independent = False,
                              logger = logger))
 
             if not checks_list[-1]:
                 unexpected_exceptions_scaned["duplicates"] = "ALL"
```

### Comparing `refineryframe-0.1.5/refineryframe/other.py` & `refineryframe-0.1.6/refineryframe/other.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.5/refineryframe/refiner.py` & `refineryframe-0.1.6/refineryframe/refiner.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,14 +325,17 @@
     def check_duplicates(self,
                          subset = None) -> None:
 
         """
         Checks for duplicates in a pandas DataFrame.
         """
 
+        if subset is None:
+            subset = self.ids_for_dedup
+
         self.DUPLICATES_TEST = check_duplicates(dataframe = self.dataframe,
                                                  subset = subset,
                                                  independent = True,
                                                  logger = self.logger)
 
     def check_col_names_types(self) -> None:
 
@@ -433,15 +436,15 @@
         if numeric_upper_bound is None:
             numeric_upper_bound = self.upper_bound
 
         duv_obj = detect_unexpected_values(dataframe = self.dataframe,
                                                  MISSING_TYPES = MISSING_TYPES,
                                                  unexpected_exceptions = unexpected_exceptions,
                                                  unexpected_conditions = unexpected_conditions,
-                                                 ids_for_dup = ids_for_dedup,
+                                                 ids_for_dedup = ids_for_dedup,
                                                  TEST_DUV_FLAGS_PATH = TEST_DUV_FLAGS_PATH,
                                                  types_dict_str = types_dict_str,
                                                  expected_date_format = expected_date_format,
                                                  earliest_date = earliest_date,
                                                  latest_date = latest_date,
                                                  numeric_lower_bound = numeric_lower_bound,
                                                  numeric_upper_bound = numeric_upper_bound,
@@ -460,15 +463,15 @@
         if dataframe is None:
             dataframe = self.dataframe
 
         duv_obj = detect_unexpected_values(dataframe = dataframe,
                                                  MISSING_TYPES = self.MISSING_TYPES,
                                                  unexpected_exceptions = self.unexpected_exceptions_duv,
                                                  unexpected_conditions = self.unexpected_conditions,
-                                                 ids_for_dup = self.ids_for_dedup,
+                                                 ids_for_dedup = self.ids_for_dedup,
                                                  TEST_DUV_FLAGS_PATH = None,
                                                  types_dict_str = self.type_dict,
                                                  expected_date_format = self.expected_date_format,
                                                  earliest_date = self.earliest_date,
                                                  latest_date = self.latest_date,
                                                  numeric_lower_bound = self.lower_bound,
                                                  numeric_upper_bound = self.upper_bound,
```

### Comparing `refineryframe-0.1.5/refineryframe/replace_unexpected.py` & `refineryframe-0.1.6/refineryframe/replace_unexpected.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.5/refineryframe.egg-info/PKG-INFO` & `refineryframe-0.1.6/refineryframe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refineryframe
-Version: 0.1.5
+Version: 0.1.6
 Summary: Cleans data, best to be used as a part of initial preprocessor
 Home-page: UNKNOWN
 Author: Kyrylo Mordan
 Author-email: <parachute.repo@gmail.com>
 License: UNKNOWN
 Keywords: python,data cleaning,safeguards
 Platform: UNKNOWN
```

### Comparing `refineryframe-0.1.5/setup.py` & `refineryframe-0.1.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "attrs>=22.2.0",
     "datetime",
     "pandas",
     "numpy",
     "unidecode"
 ]
 
-VERSION = '0.1.5'
+VERSION = '0.1.6'
 DESCRIPTION = 'Cleans data, best to be used as a part of initial preprocessor'
 LONG_DESCRIPTION = 'A package that allows to detect unexpected values in data and clean them according to set of predefined rules'
 
 # Setting up
 setup(
     name="refineryframe",
     #use_scm_version=True,
```

### Comparing `refineryframe-0.1.5/tests/conftest.py` & `refineryframe-0.1.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.5/tests/test_refiner.py` & `refineryframe-0.1.6/tests/test_refiner.py`

 * *Files identical despite different names*

