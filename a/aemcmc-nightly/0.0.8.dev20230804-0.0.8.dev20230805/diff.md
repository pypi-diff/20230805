# Comparing `tmp/aemcmc-nightly-0.0.8.dev20230804.tar.gz` & `tmp/aemcmc-nightly-0.0.8.dev20230805.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aemcmc-nightly-0.0.8.dev20230804.tar", last modified: Fri Aug  4 01:00:08 2023, max compression
+gzip compressed data, was "aemcmc-nightly-0.0.8.dev20230805.tar", last modified: Sat Aug  5 00:56:37 2023, max compression
```

## Comparing `aemcmc-nightly-0.0.8.dev20230804.tar` & `aemcmc-nightly-0.0.8.dev20230805.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 01:00:08.743510 aemcmc-nightly-0.0.8.dev20230804/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-04 01:00:08.743510 aemcmc-nightly-0.0.8.dev20230804/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 01:00:08.743510 aemcmc-nightly-0.0.8.dev20230804/aemcmc/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/aemcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-04 01:00:08.743510 aemcmc-nightly-0.0.8.dev20230804/aemcmc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/aemcmc/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/aemcmc/conjugates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/aemcmc/dists.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/aemcmc/ffbs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24238 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/aemcmc/gibbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/aemcmc/nuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/aemcmc/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/aemcmc/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/aemcmc/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/aemcmc/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/aemcmc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 01:00:08.743510 aemcmc-nightly-0.0.8.dev20230804/aemcmc_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-04 01:00:08.000000 aemcmc-nightly-0.0.8.dev20230804/aemcmc_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-08-04 01:00:08.000000 aemcmc-nightly-0.0.8.dev20230804/aemcmc_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 01:00:08.000000 aemcmc-nightly-0.0.8.dev20230804/aemcmc_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 01:00:08.000000 aemcmc-nightly-0.0.8.dev20230804/aemcmc_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-04 01:00:08.000000 aemcmc-nightly-0.0.8.dev20230804/aemcmc_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 01:00:08.000000 aemcmc-nightly-0.0.8.dev20230804/aemcmc_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-08-04 01:00:08.743510 aemcmc-nightly-0.0.8.dev20230804/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 01:00:08.743510 aemcmc-nightly-0.0.8.dev20230804/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/tests/test_conjugates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/tests/test_dists.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/tests/test_ffbs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/tests/test_gibbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/tests/test_nuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/tests/test_rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-08-04 00:59:57.000000 aemcmc-nightly-0.0.8.dev20230804/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:56:37.616791 aemcmc-nightly-0.0.8.dev20230805/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-05 00:56:37.616791 aemcmc-nightly-0.0.8.dev20230805/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:56:37.616791 aemcmc-nightly-0.0.8.dev20230805/aemcmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/aemcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-05 00:56:37.616791 aemcmc-nightly-0.0.8.dev20230805/aemcmc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/aemcmc/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/aemcmc/conjugates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/aemcmc/dists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/aemcmc/ffbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24238 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/aemcmc/gibbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/aemcmc/nuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/aemcmc/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/aemcmc/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/aemcmc/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/aemcmc/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/aemcmc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:56:37.612791 aemcmc-nightly-0.0.8.dev20230805/aemcmc_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-05 00:56:37.000000 aemcmc-nightly-0.0.8.dev20230805/aemcmc_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-08-05 00:56:37.000000 aemcmc-nightly-0.0.8.dev20230805/aemcmc_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 00:56:37.000000 aemcmc-nightly-0.0.8.dev20230805/aemcmc_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 00:56:37.000000 aemcmc-nightly-0.0.8.dev20230805/aemcmc_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-05 00:56:37.000000 aemcmc-nightly-0.0.8.dev20230805/aemcmc_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-05 00:56:37.000000 aemcmc-nightly-0.0.8.dev20230805/aemcmc_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-08-05 00:56:37.616791 aemcmc-nightly-0.0.8.dev20230805/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:56:37.616791 aemcmc-nightly-0.0.8.dev20230805/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/tests/test_conjugates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/tests/test_dists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/tests/test_ffbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/tests/test_gibbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/tests/test_nuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/tests/test_rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-08-05 00:56:25.000000 aemcmc-nightly-0.0.8.dev20230805/versioneer.py
```

### Comparing `aemcmc-nightly-0.0.8.dev20230804/LICENSE` & `aemcmc-nightly-0.0.8.dev20230805/LICENSE`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/PKG-INFO` & `aemcmc-nightly-0.0.8.dev20230805/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aemcmc-nightly
-Version: 0.0.8.dev20230804
+Version: 0.0.8.dev20230805
 Summary: Miscellaneous MCMC samplers written in Aesara
 Home-page: http://github.com/aesara-devs/aemcmc
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: math,probability,numerical,symbolic,MCMC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aemcmc-nightly-0.0.8.dev20230804/README.md` & `aemcmc-nightly-0.0.8.dev20230805/README.md`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/aemcmc/basic.py` & `aemcmc-nightly-0.0.8.dev20230805/aemcmc/basic.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/aemcmc/conjugates.py` & `aemcmc-nightly-0.0.8.dev20230805/aemcmc/conjugates.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/aemcmc/dists.py` & `aemcmc-nightly-0.0.8.dev20230805/aemcmc/dists.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/aemcmc/ffbs.py` & `aemcmc-nightly-0.0.8.dev20230805/aemcmc/ffbs.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/aemcmc/gibbs.py` & `aemcmc-nightly-0.0.8.dev20230805/aemcmc/gibbs.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/aemcmc/nuts.py` & `aemcmc-nightly-0.0.8.dev20230805/aemcmc/nuts.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/aemcmc/rewriting.py` & `aemcmc-nightly-0.0.8.dev20230805/aemcmc/rewriting.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/aemcmc/sample.py` & `aemcmc-nightly-0.0.8.dev20230805/aemcmc/sample.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/aemcmc/transforms.py` & `aemcmc-nightly-0.0.8.dev20230805/aemcmc/transforms.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/aemcmc/types.py` & `aemcmc-nightly-0.0.8.dev20230805/aemcmc/types.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/aemcmc/utils.py` & `aemcmc-nightly-0.0.8.dev20230805/aemcmc/utils.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/aemcmc_nightly.egg-info/PKG-INFO` & `aemcmc-nightly-0.0.8.dev20230805/aemcmc_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aemcmc-nightly
-Version: 0.0.8.dev20230804
+Version: 0.0.8.dev20230805
 Summary: Miscellaneous MCMC samplers written in Aesara
 Home-page: http://github.com/aesara-devs/aemcmc
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: math,probability,numerical,symbolic,MCMC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aemcmc-nightly-0.0.8.dev20230804/aemcmc_nightly.egg-info/SOURCES.txt` & `aemcmc-nightly-0.0.8.dev20230805/aemcmc_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/setup.cfg` & `aemcmc-nightly-0.0.8.dev20230805/setup.cfg`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/setup.py` & `aemcmc-nightly-0.0.8.dev20230805/setup.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/tests/test_basic.py` & `aemcmc-nightly-0.0.8.dev20230805/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/tests/test_conjugates.py` & `aemcmc-nightly-0.0.8.dev20230805/tests/test_conjugates.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/tests/test_dists.py` & `aemcmc-nightly-0.0.8.dev20230805/tests/test_dists.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/tests/test_ffbs.py` & `aemcmc-nightly-0.0.8.dev20230805/tests/test_ffbs.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/tests/test_gibbs.py` & `aemcmc-nightly-0.0.8.dev20230805/tests/test_gibbs.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/tests/test_nuts.py` & `aemcmc-nightly-0.0.8.dev20230805/tests/test_nuts.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/tests/test_rewriting.py` & `aemcmc-nightly-0.0.8.dev20230805/tests/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/tests/test_sample.py` & `aemcmc-nightly-0.0.8.dev20230805/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/tests/test_transforms.py` & `aemcmc-nightly-0.0.8.dev20230805/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/tests/test_utils.py` & `aemcmc-nightly-0.0.8.dev20230805/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230804/versioneer.py` & `aemcmc-nightly-0.0.8.dev20230805/versioneer.py`

 * *Files identical despite different names*

