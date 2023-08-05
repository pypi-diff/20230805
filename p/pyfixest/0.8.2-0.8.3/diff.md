# Comparing `tmp/pyfixest-0.8.2.tar.gz` & `tmp/pyfixest-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfixest-0.8.2.tar", max compression
+gzip compressed data, was "pyfixest-0.8.3.tar", max compression
```

## Comparing `pyfixest-0.8.2.tar` & `pyfixest-0.8.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1096 2022-11-19 12:53:04.921992 pyfixest-0.8.2/LICENSE.md
--rw-r--r--   0        0        0       26 2023-03-16 21:51:51.234748 pyfixest-0.8.2/pyfixest/__init__.py
--rw-r--r--   0        0        0     4450 2023-07-18 14:22:36.978128 pyfixest-0.8.2/pyfixest/demean.py
--rw-r--r--   0        0        0      769 2023-07-30 17:03:37.074674 pyfixest-0.8.2/pyfixest/exceptions.py
--rw-r--r--   0        0        0    30093 2023-08-02 21:12:45.857216 pyfixest-0.8.2/pyfixest/feols.py
--rw-r--r--   0        0        0    17531 2023-08-05 15:52:17.429713 pyfixest-0.8.2/pyfixest/fepois.py
--rw-r--r--   0        0        0    53400 2023-08-05 17:15:59.208832 pyfixest-0.8.2/pyfixest/fixest.py
--rw-r--r--   0        0        0    17648 2023-08-02 20:40:23.776371 pyfixest-0.8.2/pyfixest/FormulaParser.py
--rw-r--r--   0        0        0     3426 2023-04-27 19:03:35.062476 pyfixest-0.8.2/pyfixest/ssc_utils.py
--rw-r--r--   0        0        0     2385 2023-08-01 17:00:38.612293 pyfixest-0.8.2/pyfixest/utils.py
--rw-r--r--   0        0        0      939 2023-08-05 17:17:22.448911 pyfixest-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     2590 2023-08-05 17:22:41.325513 pyfixest-0.8.2/readme.md
--rw-r--r--   0        0        0     3560 1970-01-01 00:00:00.000000 pyfixest-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1096 2022-11-19 12:53:04.921992 pyfixest-0.8.3/LICENSE.md
+-rw-r--r--   0        0        0       26 2023-03-16 21:51:51.234748 pyfixest-0.8.3/pyfixest/__init__.py
+-rw-r--r--   0        0        0     4450 2023-07-18 14:22:36.978128 pyfixest-0.8.3/pyfixest/demean.py
+-rw-r--r--   0        0        0      769 2023-07-30 17:03:37.074674 pyfixest-0.8.3/pyfixest/exceptions.py
+-rw-r--r--   0        0        0    30093 2023-08-02 21:12:45.857216 pyfixest-0.8.3/pyfixest/feols.py
+-rw-r--r--   0        0        0    17531 2023-08-05 15:52:17.429713 pyfixest-0.8.3/pyfixest/fepois.py
+-rw-r--r--   0        0        0    53400 2023-08-05 17:15:59.208832 pyfixest-0.8.3/pyfixest/fixest.py
+-rw-r--r--   0        0        0    17648 2023-08-02 20:40:23.776371 pyfixest-0.8.3/pyfixest/FormulaParser.py
+-rw-r--r--   0        0        0     3426 2023-04-27 19:03:35.062476 pyfixest-0.8.3/pyfixest/ssc_utils.py
+-rw-r--r--   0        0        0     2385 2023-08-01 17:00:38.612293 pyfixest-0.8.3/pyfixest/utils.py
+-rw-r--r--   0        0        0      939 2023-08-05 17:45:26.895258 pyfixest-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     2590 2023-08-05 17:22:41.325513 pyfixest-0.8.3/readme.md
+-rw-r--r--   0        0        0     3560 1970-01-01 00:00:00.000000 pyfixest-0.8.3/PKG-INFO
```

### Comparing `pyfixest-0.8.2/LICENSE.md` & `pyfixest-0.8.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyfixest-0.8.2/pyfixest/demean.py` & `pyfixest-0.8.3/pyfixest/demean.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.8.2/pyfixest/exceptions.py` & `pyfixest-0.8.3/pyfixest/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.8.2/pyfixest/feols.py` & `pyfixest-0.8.3/pyfixest/feols.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.8.2/pyfixest/fepois.py` & `pyfixest-0.8.3/pyfixest/fepois.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.8.2/pyfixest/fixest.py` & `pyfixest-0.8.3/pyfixest/fixest.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.8.2/pyfixest/FormulaParser.py` & `pyfixest-0.8.3/pyfixest/FormulaParser.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.8.2/pyfixest/ssc_utils.py` & `pyfixest-0.8.3/pyfixest/ssc_utils.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.8.2/pyfixest/utils.py` & `pyfixest-0.8.3/pyfixest/utils.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.8.2/pyproject.toml` & `pyfixest-0.8.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyfixest"
-version = "0.8.2"
+version = "0.8.3"
 
 description = "Experimental draft package for high dimensional fixed effect estimation. Supports OLS and IV estimation."
 authors = ["Alexander Fischer <alexander-fischer1801@t-online.de>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://s3alfisc.github.io/pyfixest/"
 repository = "https://github.com/s3alfisc/pyfixest"
```

### Comparing `pyfixest-0.8.2/readme.md` & `pyfixest-0.8.3/readme.md`

 * *Files identical despite different names*

### Comparing `pyfixest-0.8.2/PKG-INFO` & `pyfixest-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfixest
-Version: 0.8.2
+Version: 0.8.3
 Summary: Experimental draft package for high dimensional fixed effect estimation. Supports OLS and IV estimation.
 Home-page: https://s3alfisc.github.io/pyfixest/
 License: MIT
 Author: Alexander Fischer
 Author-email: alexander-fischer1801@t-online.de
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

