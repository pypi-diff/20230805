# Comparing `tmp/smltheory-0.1.1.tar.gz` & `tmp/smltheory-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smltheory-0.1.1.tar", max compression
+gzip compressed data, was "smltheory-0.1.2.tar", max compression
```

## Comparing `smltheory-0.1.1.tar` & `smltheory-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rwxr-xr-x   0        0        0     1076 2023-08-01 20:38:18.331005 smltheory-0.1.1/LICENSE
--rw-r--r--   0        0        0      926 2023-08-02 15:34:34.623560 smltheory-0.1.1/README.md
--rw-r--r--   0        0        0      592 2023-08-04 21:27:58.158750 smltheory-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      278 2023-08-02 17:13:55.577493 smltheory-0.1.1/src/smltheory/__init__.py
--rw-r--r--   0        0        0     5122 2023-08-04 17:25:51.083724 smltheory-0.1.1/src/smltheory/bayes_decision.py
--rw-r--r--   0        0        0     4012 2023-08-03 14:23:13.848664 smltheory-0.1.1/src/smltheory/est_error.py
--rw-r--r--   0        0        0    12719 2023-08-03 20:10:07.529472 smltheory-0.1.1/src/smltheory/generate_data.py
--rw-r--r--   0        0        0     9449 2023-08-04 14:15:40.598616 smltheory-0.1.1/src/smltheory/gradient_descent.py
--rw-r--r--   0        0        0     9377 2023-08-04 16:14:40.063052 smltheory-0.1.1/src/smltheory/least_squares.py
--rw-r--r--   0        0        0    11041 2023-08-04 17:10:38.427385 smltheory-0.1.1/src/smltheory/opt_error.py
--rw-r--r--   0        0        0     7590 2023-08-04 17:04:40.592233 smltheory-0.1.1/src/smltheory/overfitting.py
--rw-r--r--   0        0        0    15886 2023-08-04 17:06:08.189243 smltheory-0.1.1/src/smltheory/trun_mvnt.py
--rw-r--r--   0        0        0     1509 1970-01-01 00:00:00.000000 smltheory-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1076 2023-08-01 20:38:18.331005 smltheory-0.1.2/LICENSE
+-rw-r--r--   0        0        0      926 2023-08-02 15:34:34.623560 smltheory-0.1.2/README.md
+-rw-r--r--   0        0        0      592 2023-08-04 21:53:32.624609 smltheory-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      139 2023-08-04 21:53:03.857138 smltheory-0.1.2/src/smltheory/__init__.py
+-rw-r--r--   0        0        0     5122 2023-08-04 17:25:51.083724 smltheory-0.1.2/src/smltheory/bayes_decision.py
+-rw-r--r--   0        0        0     4012 2023-08-03 14:23:13.848664 smltheory-0.1.2/src/smltheory/est_error.py
+-rw-r--r--   0        0        0    12719 2023-08-03 20:10:07.529472 smltheory-0.1.2/src/smltheory/generate_data.py
+-rw-r--r--   0        0        0     9449 2023-08-04 14:15:40.598616 smltheory-0.1.2/src/smltheory/gradient_descent.py
+-rw-r--r--   0        0        0     9377 2023-08-04 16:14:40.063052 smltheory-0.1.2/src/smltheory/least_squares.py
+-rw-r--r--   0        0        0    11041 2023-08-04 17:10:38.427385 smltheory-0.1.2/src/smltheory/opt_error.py
+-rw-r--r--   0        0        0     7590 2023-08-04 17:04:40.592233 smltheory-0.1.2/src/smltheory/overfitting.py
+-rw-r--r--   0        0        0    15886 2023-08-04 17:06:08.189243 smltheory-0.1.2/src/smltheory/trun_mvnt.py
+-rw-r--r--   0        0        0     1509 1970-01-01 00:00:00.000000 smltheory-0.1.2/PKG-INFO
```

### Comparing `smltheory-0.1.1/LICENSE` & `smltheory-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.1/README.md` & `smltheory-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.1/pyproject.toml` & `smltheory-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smltheory"
-version = "0.1.1"
+version = "0.1.2"
 description = "Demonstrates propositions of supervised machine learning theories"
 authors = ["Sebastian Sciarra"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
```

### Comparing `smltheory-0.1.1/src/smltheory/bayes_decision.py` & `smltheory-0.1.2/src/smltheory/bayes_decision.py`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.1/src/smltheory/est_error.py` & `smltheory-0.1.2/src/smltheory/est_error.py`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.1/src/smltheory/generate_data.py` & `smltheory-0.1.2/src/smltheory/generate_data.py`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.1/src/smltheory/gradient_descent.py` & `smltheory-0.1.2/src/smltheory/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.1/src/smltheory/least_squares.py` & `smltheory-0.1.2/src/smltheory/least_squares.py`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.1/src/smltheory/opt_error.py` & `smltheory-0.1.2/src/smltheory/opt_error.py`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.1/src/smltheory/overfitting.py` & `smltheory-0.1.2/src/smltheory/overfitting.py`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.1/src/smltheory/trun_mvnt.py` & `smltheory-0.1.2/src/smltheory/trun_mvnt.py`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.1/PKG-INFO` & `smltheory-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smltheory
-Version: 0.1.1
+Version: 0.1.2
 Summary: Demonstrates propositions of supervised machine learning theories
 License: MIT
 Author: Sebastian Sciarra
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

