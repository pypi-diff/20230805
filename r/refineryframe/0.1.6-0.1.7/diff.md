# Comparing `tmp/refineryframe-0.1.6.tar.gz` & `tmp/refineryframe-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refineryframe-0.1.6.tar", last modified: Sat Aug  5 13:29:42 2023, max compression
+gzip compressed data, was "refineryframe-0.1.7.tar", last modified: Sat Aug  5 13:47:34 2023, max compression
```

## Comparing `refineryframe-0.1.6.tar` & `refineryframe-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:29:42.253757 refineryframe-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-05 13:29:31.000000 refineryframe-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    31957 2023-08-05 13:29:42.253757 refineryframe-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31172 2023-08-05 13:29:31.000000 refineryframe-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:29:42.253757 refineryframe-0.1.6/refineryframe/
--rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-08-05 13:29:31.000000 refineryframe-0.1.6/refineryframe/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36563 2023-08-05 13:29:31.000000 refineryframe-0.1.6/refineryframe/detect_unexpected.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12527 2023-08-05 13:29:31.000000 refineryframe-0.1.6/refineryframe/other.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24612 2023-08-05 13:29:31.000000 refineryframe-0.1.6/refineryframe/refiner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14051 2023-08-05 13:29:31.000000 refineryframe-0.1.6/refineryframe/replace_unexpected.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:29:42.253757 refineryframe-0.1.6/refineryframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    31957 2023-08-05 13:29:42.000000 refineryframe-0.1.6/refineryframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-05 13:29:42.000000 refineryframe-0.1.6/refineryframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 13:29:42.000000 refineryframe-0.1.6/refineryframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-05 13:29:42.000000 refineryframe-0.1.6/refineryframe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-05 13:29:42.000000 refineryframe-0.1.6/refineryframe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 13:29:42.253757 refineryframe-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-05 13:29:41.000000 refineryframe-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:29:42.253757 refineryframe-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 13:29:31.000000 refineryframe-0.1.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-08-05 13:29:31.000000 refineryframe-0.1.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-08-05 13:29:31.000000 refineryframe-0.1.6/tests/test_refiner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:47:34.557942 refineryframe-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-05 13:47:21.000000 refineryframe-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    31901 2023-08-05 13:47:34.557942 refineryframe-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31172 2023-08-05 13:47:21.000000 refineryframe-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:47:34.553942 refineryframe-0.1.7/refineryframe/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-08-05 13:47:21.000000 refineryframe-0.1.7/refineryframe/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36563 2023-08-05 13:47:21.000000 refineryframe-0.1.7/refineryframe/detect_unexpected.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12527 2023-08-05 13:47:21.000000 refineryframe-0.1.7/refineryframe/other.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24623 2023-08-05 13:47:21.000000 refineryframe-0.1.7/refineryframe/refiner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14051 2023-08-05 13:47:21.000000 refineryframe-0.1.7/refineryframe/replace_unexpected.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:47:34.557942 refineryframe-0.1.7/refineryframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    31901 2023-08-05 13:47:34.000000 refineryframe-0.1.7/refineryframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-05 13:47:34.000000 refineryframe-0.1.7/refineryframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 13:47:34.000000 refineryframe-0.1.7/refineryframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-05 13:47:34.000000 refineryframe-0.1.7/refineryframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-05 13:47:34.000000 refineryframe-0.1.7/refineryframe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 13:47:34.557942 refineryframe-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-05 13:47:32.000000 refineryframe-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:47:34.557942 refineryframe-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 13:47:21.000000 refineryframe-0.1.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-08-05 13:47:21.000000 refineryframe-0.1.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-08-05 13:47:21.000000 refineryframe-0.1.7/tests/test_refiner.py
```

### Comparing `refineryframe-0.1.6/LICENSE` & `refineryframe-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.6/PKG-INFO` & `refineryframe-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 Metadata-Version: 2.1
 Name: refineryframe
-Version: 0.1.6
+Version: 0.1.7
 Summary: Cleans data, best to be used as a part of initial preprocessor
-Home-page: UNKNOWN
 Author: Kyrylo Mordan
 Author-email: <parachute.repo@gmail.com>
-License: UNKNOWN
 Keywords: python,data cleaning,safeguards
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -1043,9 +1040,7 @@
 * RUV_score2 takes advantage of the fact that if one has too many rows or columns of data that are completly unusable or some kind of mix of those situations, the dataset does become unusable. The values below 0.5 supposedly indicate completelly unusable dataset.
 
 $$
 score_{ruv2} =  1 - \frac{med_{col}^2 + med_{row}^2}{2}
 $$
 
 
-
-
```

### Comparing `refineryframe-0.1.6/README.md` & `refineryframe-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.6/refineryframe/detect_unexpected.py` & `refineryframe-0.1.7/refineryframe/detect_unexpected.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.6/refineryframe/other.py` & `refineryframe-0.1.7/refineryframe/other.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.6/refineryframe/refiner.py` & `refineryframe-0.1.7/refineryframe/refiner.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     dotline_length = attr.ib(default=50, type=int)
 
     lower_bound = attr.ib(default=-float("inf"))
     upper_bound = attr.ib(default=float("inf"))
     earliest_date = attr.ib(default="1900-08-25")
     latest_date = attr.ib(default="2100-01-01")
 
-    ids_for_dedup = attr.ib(default=None)
+    ids_for_dedup = attr.ib(default=None, type=list)
 
     unexpected_exceptions_duv = attr.ib(default={"col_names_types": "NONE",
                                               "missing_values": "NONE",
                                               "missing_types": "NONE",
                                               "inf_values": "NONE",
                                               "date_format": "NONE",
                                               "duplicates": "NONE",
```

### Comparing `refineryframe-0.1.6/refineryframe/replace_unexpected.py` & `refineryframe-0.1.7/refineryframe/replace_unexpected.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.6/refineryframe.egg-info/PKG-INFO` & `refineryframe-0.1.7/refineryframe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 Metadata-Version: 2.1
 Name: refineryframe
-Version: 0.1.6
+Version: 0.1.7
 Summary: Cleans data, best to be used as a part of initial preprocessor
-Home-page: UNKNOWN
 Author: Kyrylo Mordan
 Author-email: <parachute.repo@gmail.com>
-License: UNKNOWN
 Keywords: python,data cleaning,safeguards
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -1043,9 +1040,7 @@
 * RUV_score2 takes advantage of the fact that if one has too many rows or columns of data that are completly unusable or some kind of mix of those situations, the dataset does become unusable. The values below 0.5 supposedly indicate completelly unusable dataset.
 
 $$
 score_{ruv2} =  1 - \frac{med_{col}^2 + med_{row}^2}{2}
 $$
 
 
-
-
```

### Comparing `refineryframe-0.1.6/setup.py` & `refineryframe-0.1.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "attrs>=22.2.0",
     "datetime",
     "pandas",
     "numpy",
     "unidecode"
 ]
 
-VERSION = '0.1.6'
+VERSION = '0.1.7'
 DESCRIPTION = 'Cleans data, best to be used as a part of initial preprocessor'
 LONG_DESCRIPTION = 'A package that allows to detect unexpected values in data and clean them according to set of predefined rules'
 
 # Setting up
 setup(
     name="refineryframe",
     #use_scm_version=True,
```

### Comparing `refineryframe-0.1.6/tests/conftest.py` & `refineryframe-0.1.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.6/tests/test_refiner.py` & `refineryframe-0.1.7/tests/test_refiner.py`

 * *Files identical despite different names*

