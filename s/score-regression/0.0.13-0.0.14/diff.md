# Comparing `tmp/score_regression-0.0.13.tar.gz` & `tmp/score_regression-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "score_regression-0.0.13.tar", last modified: Sat Aug  5 02:40:22 2023, max compression
+gzip compressed data, was "score_regression-0.0.14.tar", last modified: Sat Aug  5 02:48:19 2023, max compression
```

## Comparing `score_regression-0.0.13.tar` & `score_regression-0.0.14.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-05 02:40:22.421276 score_regression-0.0.13/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1529 2023-08-02 15:42:42.000000 score_regression-0.0.13/LICENSE
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-08-02 15:42:42.000000 score_regression-0.0.13/MANIFEST.in
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     3000 2023-08-05 02:40:22.421276 score_regression-0.0.13/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2185 2023-08-05 02:29:19.000000 score_regression-0.0.13/README.rst
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      133 2023-08-03 00:34:01.000000 score_regression-0.0.13/requirements.txt
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-05 02:40:22.417276 score_regression-0.0.13/score_regression/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      200 2023-08-04 02:00:42.000000 score_regression-0.0.13/score_regression/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       23 2023-08-05 02:37:07.000000 score_regression-0.0.13/score_regression/_version.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)    12046 2023-08-05 02:37:52.000000 score_regression-0.0.13/score_regression/score_regression.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-05 02:40:22.421276 score_regression-0.0.13/score_regression/tests/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-08-02 15:42:42.000000 score_regression-0.0.13/score_regression/tests/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      321 2023-08-04 02:03:02.000000 score_regression-0.0.13/score_regression/tests/test_common.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1241 2023-08-04 17:23:29.000000 score_regression-0.0.13/score_regression/tests/test_template.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-05 02:40:22.421276 score_regression-0.0.13/score_regression.egg-info/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     3000 2023-08-05 02:40:22.000000 score_regression-0.0.13/score_regression.egg-info/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      512 2023-08-05 02:40:22.000000 score_regression-0.0.13/score_regression.egg-info/SOURCES.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-05 02:40:22.000000 score_regression-0.0.13/score_regression.egg-info/dependency_links.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-05 02:40:22.000000 score_regression-0.0.13/score_regression.egg-info/not-zip-safe
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      119 2023-08-05 02:40:22.000000 score_regression-0.0.13/score_regression.egg-info/requires.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       17 2023-08-05 02:40:22.000000 score_regression-0.0.13/score_regression.egg-info/top_level.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-08-05 02:40:22.425276 score_regression-0.0.13/setup.cfg
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2631 2023-08-05 02:26:20.000000 score_regression-0.0.13/setup.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-05 02:48:19.623899 score_regression-0.0.14/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1529 2023-08-02 15:42:42.000000 score_regression-0.0.14/LICENSE
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-08-02 15:42:42.000000 score_regression-0.0.14/MANIFEST.in
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     3058 2023-08-05 02:48:19.623899 score_regression-0.0.14/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     2243 2023-08-05 02:45:31.000000 score_regression-0.0.14/README.rst
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      133 2023-08-03 00:34:01.000000 score_regression-0.0.14/requirements.txt
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-05 02:48:19.623899 score_regression-0.0.14/score_regression/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      200 2023-08-04 02:00:42.000000 score_regression-0.0.14/score_regression/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       23 2023-08-05 02:46:28.000000 score_regression-0.0.14/score_regression/_version.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)    12046 2023-08-05 02:37:52.000000 score_regression-0.0.14/score_regression/score_regression.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-05 02:48:19.623899 score_regression-0.0.14/score_regression/tests/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-08-02 15:42:42.000000 score_regression-0.0.14/score_regression/tests/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      321 2023-08-04 02:03:02.000000 score_regression-0.0.14/score_regression/tests/test_common.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1241 2023-08-04 17:23:29.000000 score_regression-0.0.14/score_regression/tests/test_template.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-05 02:48:19.623899 score_regression-0.0.14/score_regression.egg-info/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     3058 2023-08-05 02:48:19.000000 score_regression-0.0.14/score_regression.egg-info/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      512 2023-08-05 02:48:19.000000 score_regression-0.0.14/score_regression.egg-info/SOURCES.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-05 02:48:19.000000 score_regression-0.0.14/score_regression.egg-info/dependency_links.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-05 02:40:22.000000 score_regression-0.0.14/score_regression.egg-info/not-zip-safe
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      119 2023-08-05 02:48:19.000000 score_regression-0.0.14/score_regression.egg-info/requires.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       17 2023-08-05 02:48:19.000000 score_regression-0.0.14/score_regression.egg-info/top_level.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-08-05 02:48:19.623899 score_regression-0.0.14/setup.cfg
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     2631 2023-08-05 02:26:20.000000 score_regression-0.0.14/setup.py
```

### Comparing `score_regression-0.0.13/LICENSE` & `score_regression-0.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `score_regression-0.0.13/PKG-INFO` & `score_regression-0.0.14/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: score_regression
-Version: 0.0.13
+Version: 0.0.14
 Summary: A classifier that maximizes AUC
 Home-page: https://github.com/hrolfrc/score_regression
 Download-URL: https://github.com/hrolfrc/score_regression
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
@@ -40,15 +40,15 @@
 ------------------
 Use pip to install score_regression.
 
 ``pip install score_regression``
 
 Introduction
 ------------------
-This is a python implementation of a classifier that maximizes AUC.  The idea is to relax the requirement from CALF_ that the weights be integers in [-1, 0, 1] and allow the weights to be any real number.
+This is a python implementation of a classifier that maximizes AUC.  The idea is to find the features that maximize AUC, analogous to CALF_, but relax the requirement that the weights be integers in [-1, 0, 1] and instead allow the weights to be any real number.
 
 ScoreRegression provides classification and prediction for two classes, the binomial case.  Small to medium problems are supported.  This is research code and a work in progress.
 
 ScoreRegression is designed for use with scikit-learn_ pipelines and composite estimators.
 
 .. _scikit-learn: https://scikit-learn.org
```

### Comparing `score_regression-0.0.13/README.rst` & `score_regression-0.0.14/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ------------------
 Use pip to install score_regression.
 
 ``pip install score_regression``
 
 Introduction
 ------------------
-This is a python implementation of a classifier that maximizes AUC.  The idea is to relax the requirement from CALF_ that the weights be integers in [-1, 0, 1] and allow the weights to be any real number.
+This is a python implementation of a classifier that maximizes AUC.  The idea is to find the features that maximize AUC, analogous to CALF_, but relax the requirement that the weights be integers in [-1, 0, 1] and instead allow the weights to be any real number.
 
 ScoreRegression provides classification and prediction for two classes, the binomial case.  Small to medium problems are supported.  This is research code and a work in progress.
 
 ScoreRegression is designed for use with scikit-learn_ pipelines and composite estimators.
 
 .. _scikit-learn: https://scikit-learn.org
```

### Comparing `score_regression-0.0.13/score_regression/score_regression.py` & `score_regression-0.0.14/score_regression/score_regression.py`

 * *Files identical despite different names*

### Comparing `score_regression-0.0.13/score_regression/tests/test_template.py` & `score_regression-0.0.14/score_regression/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `score_regression-0.0.13/score_regression.egg-info/PKG-INFO` & `score_regression-0.0.14/score_regression.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: score-regression
-Version: 0.0.13
+Version: 0.0.14
 Summary: A classifier that maximizes AUC
 Home-page: https://github.com/hrolfrc/score_regression
 Download-URL: https://github.com/hrolfrc/score_regression
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
@@ -40,15 +40,15 @@
 ------------------
 Use pip to install score_regression.
 
 ``pip install score_regression``
 
 Introduction
 ------------------
-This is a python implementation of a classifier that maximizes AUC.  The idea is to relax the requirement from CALF_ that the weights be integers in [-1, 0, 1] and allow the weights to be any real number.
+This is a python implementation of a classifier that maximizes AUC.  The idea is to find the features that maximize AUC, analogous to CALF_, but relax the requirement that the weights be integers in [-1, 0, 1] and instead allow the weights to be any real number.
 
 ScoreRegression provides classification and prediction for two classes, the binomial case.  Small to medium problems are supported.  This is research code and a work in progress.
 
 ScoreRegression is designed for use with scikit-learn_ pipelines and composite estimators.
 
 .. _scikit-learn: https://scikit-learn.org
```

### Comparing `score_regression-0.0.13/score_regression.egg-info/SOURCES.txt` & `score_regression-0.0.14/score_regression.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `score_regression-0.0.13/setup.py` & `score_regression-0.0.14/setup.py`

 * *Files identical despite different names*

