# Comparing `tmp/refineryframe-0.1.4.tar.gz` & `tmp/refineryframe-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refineryframe-0.1.4.tar", last modified: Sat Aug  5 01:10:19 2023, max compression
+gzip compressed data, was "refineryframe-0.1.5.tar", last modified: Sat Aug  5 01:39:26 2023, max compression
```

## Comparing `refineryframe-0.1.4.tar` & `refineryframe-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:10:19.170590 refineryframe-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-05 01:10:06.000000 refineryframe-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    31957 2023-08-05 01:10:19.170590 refineryframe-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31172 2023-08-05 01:10:18.000000 refineryframe-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:10:19.170590 refineryframe-0.1.4/refineryframe/
--rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-08-05 01:10:06.000000 refineryframe-0.1.4/refineryframe/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36509 2023-08-05 01:10:06.000000 refineryframe-0.1.4/refineryframe/detect_unexpected.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12527 2023-08-05 01:10:06.000000 refineryframe-0.1.4/refineryframe/other.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19573 2023-08-05 01:10:06.000000 refineryframe-0.1.4/refineryframe/refiner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14051 2023-08-05 01:10:06.000000 refineryframe-0.1.4/refineryframe/replace_unexpected.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:10:19.170590 refineryframe-0.1.4/refineryframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    31957 2023-08-05 01:10:19.000000 refineryframe-0.1.4/refineryframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-05 01:10:19.000000 refineryframe-0.1.4/refineryframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 01:10:19.000000 refineryframe-0.1.4/refineryframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-05 01:10:19.000000 refineryframe-0.1.4/refineryframe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-05 01:10:19.000000 refineryframe-0.1.4/refineryframe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 01:10:19.170590 refineryframe-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-05 01:10:18.000000 refineryframe-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:10:19.170590 refineryframe-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 01:10:06.000000 refineryframe-0.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-08-05 01:10:06.000000 refineryframe-0.1.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-08-05 01:10:06.000000 refineryframe-0.1.4/tests/test_refiner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:39:26.811550 refineryframe-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-05 01:39:09.000000 refineryframe-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    31957 2023-08-05 01:39:26.811550 refineryframe-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31172 2023-08-05 01:39:09.000000 refineryframe-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:39:26.811550 refineryframe-0.1.5/refineryframe/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-08-05 01:39:09.000000 refineryframe-0.1.5/refineryframe/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36509 2023-08-05 01:39:09.000000 refineryframe-0.1.5/refineryframe/detect_unexpected.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12527 2023-08-05 01:39:09.000000 refineryframe-0.1.5/refineryframe/other.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24540 2023-08-05 01:39:09.000000 refineryframe-0.1.5/refineryframe/refiner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14051 2023-08-05 01:39:09.000000 refineryframe-0.1.5/refineryframe/replace_unexpected.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:39:26.811550 refineryframe-0.1.5/refineryframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    31957 2023-08-05 01:39:26.000000 refineryframe-0.1.5/refineryframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-05 01:39:26.000000 refineryframe-0.1.5/refineryframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 01:39:26.000000 refineryframe-0.1.5/refineryframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-05 01:39:26.000000 refineryframe-0.1.5/refineryframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-05 01:39:26.000000 refineryframe-0.1.5/refineryframe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 01:39:26.811550 refineryframe-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-05 01:39:25.000000 refineryframe-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:39:26.811550 refineryframe-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 01:39:09.000000 refineryframe-0.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-08-05 01:39:09.000000 refineryframe-0.1.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-08-05 01:39:09.000000 refineryframe-0.1.5/tests/test_refiner.py
```

### Comparing `refineryframe-0.1.4/LICENSE` & `refineryframe-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.4/PKG-INFO` & `refineryframe-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refineryframe
-Version: 0.1.4
+Version: 0.1.5
 Summary: Cleans data, best to be used as a part of initial preprocessor
 Home-page: UNKNOWN
 Author: Kyrylo Mordan
 Author-email: <parachute.repo@gmail.com>
 License: UNKNOWN
 Keywords: python,data cleaning,safeguards
 Platform: UNKNOWN
```

### Comparing `refineryframe-0.1.4/README.md` & `refineryframe-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.4/refineryframe/detect_unexpected.py` & `refineryframe-0.1.5/refineryframe/detect_unexpected.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.4/refineryframe/other.py` & `refineryframe-0.1.5/refineryframe/other.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.4/refineryframe/refiner.py` & `refineryframe-0.1.5/refineryframe/refiner.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,68 @@
             check_missing_types, detect_unexpected_values
 from refineryframe.replace_unexpected import replace_unexpected_values
 
 @attr.s
 class Refiner:
 
     """
-    Class that encapsulates funtions from refineryframe.
+    Class that encapsulates functions for data refining and validation.
+
+    Attributes:
+        dataframe (pd.DataFrame): The input pandas DataFrame to be processed.
+        replace_dict (dict, optional): A dictionary to define replacements for specific values in the DataFrame.
+        MISSING_TYPES (dict, optional): Default values for missing types in different columns of the DataFrame.
+        expected_date_format (str, optional): The expected date format for date columns in the DataFrame.
+        mess (str, optional): A custom message used in the `shout` method for printing.
+        shout_type (str, optional): The type of output for the `shout` method (e.g., 'HEAD2').
+        logger (logging.Logger, optional): A custom logger object for logging messages.
+        logger_name (str, optional): The name of the logger for the class instance.
+        loggerLvl (int, optional): The logging level for the logger.
+        dotline_length (int, optional): The length of the line to be printed in the `shout` method.
+        lower_bound (float, optional): The lower bound for numeric range validation.
+        upper_bound (float, optional): The upper bound for numeric range validation.
+        earliest_date (str, optional): The earliest allowed date for date range validation.
+        latest_date (str, optional): The latest allowed date for date range validation.
+        ids_for_dedup (list, optional): A list of column names to be used for duplicate detection.
+        unexpected_exceptions_duv (dict, optional): A dictionary of unexpected exceptions for data value validation.
+        unexpected_exceptions_ruv (dict, optional): A dictionary of unexpected exceptions for data replacement validation.
+        unexpected_conditions (None or callable, optional): A callable function for custom unexpected conditions.
+        ignore_values (list, optional): A list of values to ignore during numeric range validation.
+        ignore_dates (list, optional): A list of dates to ignore during date range validation.
+
+    Methods:
+        shout(mess=None): Prints a line of text with a specified length and format.
+        get_type_dict_from_dataframe(explicit=True, stringout=False): Returns a dictionary containing the data types
+            of each column in the given pandas DataFrame.
+        set_type_dict(type_dict=None, explicit=True, stringout=False): Changes the data types of the columns in the
+            DataFrame based on a dictionary of intended data types.
+        set_types(type_dict=None, replace_dict=None, expected_date_format=None): Changes the data types of the columns
+            in the DataFrame based on a dictionary of intended data types.
+        get_refiner_settings(): Extracts values of parameters from the Refiner and saves them in a dictionary for later use.
+        set_refiner_settings(settings: dict): Updates input parameters with values from the provided settings dict.
+        check_missing_types(): Searches for instances of missing types in each column of the DataFrame.
+        check_missing_values(): Counts the number of NaN, None, and NaT values in each column of the DataFrame.
+        check_inf_values(): Counts the inf values in each column of the DataFrame.
+        check_date_format(): Checks if the values in the datetime columns have the expected 'YYYY-MM-DD' format.
+        check_duplicates(subset=None): Checks for duplicates in the DataFrame.
+        check_col_names_types(): Checks if the DataFrame has the same column names as the types_dict_str dictionary
+            and those columns have the same types as items in the dictionary.
+        check_numeric_range(numeric_cols=None, lower_bound=None, upper_bound=None, ignore_values=None): Checks if
+            numeric values are in expected ranges.
+        check_date_range(earliest_date=None, latest_date=None, ignore_dates=None): Checks if dates are in expected ranges.
+        detect_unexpected_values(MISSING_TYPES=None, unexpected_exceptions=None, unexpected_conditions=None,
+                                 ids_for_dedup=None, TEST_DUV_FLAGS_PATH=None, types_dict_str=None,
+                                 expected_date_format=None, earliest_date=None, latest_date=None, numeric_lower_bound=None,
+                                 numeric_upper_bound=None, print_score=True): Detects unexpected values in the DataFrame.
+        get_unexpected_exceptions_scaned(dataframe=None): Returns unexpected_exceptions with appropriate settings for the
+            values in the DataFrame.
+        replace_unexpected_values(MISSING_TYPES=None, unexpected_exceptions=None, unexpected_conditions=None,
+                                  TEST_RUV_FLAGS_PATH=None, earliest_date=None, latest_date=None, numeric_lower_bound=None,
+                                  numeric_upper_bound=None): Replaces unexpected values in the DataFrame with missing types
+                                  based on a dictionary of unexpected exceptions.
     """
 
 
     # inputs
     dataframe = attr.ib(type=pd.DataFrame)
     replace_dict = attr.ib(default=None, type=dict)
 
@@ -341,15 +394,15 @@
                                                  ignore_dates = ignore_dates,
                                                 logger = self.logger)
 
     def detect_unexpected_values(self,
                                  MISSING_TYPES = None,
                                  unexpected_exceptions = None,
                                  unexpected_conditions = None,
-                                 ids_for_dup = None,
+                                 ids_for_dedup = None,
                                  TEST_DUV_FLAGS_PATH = None,
                                  types_dict_str = None,
                                  expected_date_format = None,
                                  earliest_date = None,
                                  latest_date = None,
                                  numeric_lower_bound = None,
                                  numeric_upper_bound = None,
@@ -363,14 +416,16 @@
             MISSING_TYPES = self.MISSING_TYPES
         if unexpected_exceptions is None:
             unexpected_exceptions = self.unexpected_exceptions_duv
         if unexpected_conditions is None:
             unexpected_conditions = self.unexpected_conditions
         if types_dict_str is None:
             types_dict_str = self.type_dict
+        if ids_for_dedup is None:
+            ids_for_dedup = self.ids_for_dedup
         if expected_date_format is None:
             expected_date_format = self.expected_date_format
         if earliest_date is None:
             earliest_date = self.earliest_date
         if latest_date is None:
             latest_date = self.latest_date
         if numeric_lower_bound is None:
@@ -378,15 +433,15 @@
         if numeric_upper_bound is None:
             numeric_upper_bound = self.upper_bound
 
         duv_obj = detect_unexpected_values(dataframe = self.dataframe,
                                                  MISSING_TYPES = MISSING_TYPES,
                                                  unexpected_exceptions = unexpected_exceptions,
                                                  unexpected_conditions = unexpected_conditions,
-                                                 ids_for_dup = ids_for_dup,
+                                                 ids_for_dup = ids_for_dedup,
                                                  TEST_DUV_FLAGS_PATH = TEST_DUV_FLAGS_PATH,
                                                  types_dict_str = types_dict_str,
                                                  expected_date_format = expected_date_format,
                                                  earliest_date = earliest_date,
                                                  latest_date = latest_date,
                                                  numeric_lower_bound = numeric_lower_bound,
                                                  numeric_upper_bound = numeric_upper_bound,
```

### Comparing `refineryframe-0.1.4/refineryframe/replace_unexpected.py` & `refineryframe-0.1.5/refineryframe/replace_unexpected.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.4/refineryframe.egg-info/PKG-INFO` & `refineryframe-0.1.5/refineryframe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refineryframe
-Version: 0.1.4
+Version: 0.1.5
 Summary: Cleans data, best to be used as a part of initial preprocessor
 Home-page: UNKNOWN
 Author: Kyrylo Mordan
 Author-email: <parachute.repo@gmail.com>
 License: UNKNOWN
 Keywords: python,data cleaning,safeguards
 Platform: UNKNOWN
```

### Comparing `refineryframe-0.1.4/setup.py` & `refineryframe-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "attrs>=22.2.0",
     "datetime",
     "pandas",
     "numpy",
     "unidecode"
 ]
 
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 DESCRIPTION = 'Cleans data, best to be used as a part of initial preprocessor'
 LONG_DESCRIPTION = 'A package that allows to detect unexpected values in data and clean them according to set of predefined rules'
 
 # Setting up
 setup(
     name="refineryframe",
     #use_scm_version=True,
```

### Comparing `refineryframe-0.1.4/tests/conftest.py` & `refineryframe-0.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.4/tests/test_refiner.py` & `refineryframe-0.1.5/tests/test_refiner.py`

 * *Files identical despite different names*

