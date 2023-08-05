# Comparing `tmp/botocore-a-la-carte-codedeploy-1.31.8.tar.gz` & `tmp/botocore-a-la-carte-codedeploy-1.31.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-codedeploy-1.31.8.tar", last modified: Fri Jul 21 01:21:15 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-codedeploy-1.31.9.tar", last modified: Sat Jul 22 01:20:18 2023, max compression
```

## Comparing `botocore-a-la-carte-codedeploy-1.31.8.tar` & `botocore-a-la-carte-codedeploy-1.31.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:15.170809 botocore-a-la-carte-codedeploy-1.31.8/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-21 01:21:14.000000 botocore-a-la-carte-codedeploy-1.31.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-21 01:21:15.170809 botocore-a-la-carte-codedeploy-1.31.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:15.170809 botocore-a-la-carte-codedeploy-1.31.8/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:15.170809 botocore-a-la-carte-codedeploy-1.31.8/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:15.170809 botocore-a-la-carte-codedeploy-1.31.8/botocore/data/codedeploy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:15.170809 botocore-a-la-carte-codedeploy-1.31.8/botocore/data/codedeploy/2014-10-06/
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-07-21 01:21:06.000000 botocore-a-la-carte-codedeploy-1.31.8/botocore/data/codedeploy/2014-10-06/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 01:21:06.000000 botocore-a-la-carte-codedeploy-1.31.8/botocore/data/codedeploy/2014-10-06/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-21 01:21:06.000000 botocore-a-la-carte-codedeploy-1.31.8/botocore/data/codedeploy/2014-10-06/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   221635 2023-07-21 01:21:06.000000 botocore-a-la-carte-codedeploy-1.31.8/botocore/data/codedeploy/2014-10-06/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-21 01:21:06.000000 botocore-a-la-carte-codedeploy-1.31.8/botocore/data/codedeploy/2014-10-06/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:15.170809 botocore-a-la-carte-codedeploy-1.31.8/botocore_a_la_carte_codedeploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-21 01:21:15.000000 botocore-a-la-carte-codedeploy-1.31.8/botocore_a_la_carte_codedeploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-21 01:21:15.000000 botocore-a-la-carte-codedeploy-1.31.8/botocore_a_la_carte_codedeploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:21:15.000000 botocore-a-la-carte-codedeploy-1.31.8/botocore_a_la_carte_codedeploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 01:21:15.000000 botocore-a-la-carte-codedeploy-1.31.8/botocore_a_la_carte_codedeploy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:21:15.170809 botocore-a-la-carte-codedeploy-1.31.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-21 01:21:14.000000 botocore-a-la-carte-codedeploy-1.31.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:18.356806 botocore-a-la-carte-codedeploy-1.31.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-22 01:20:18.000000 botocore-a-la-carte-codedeploy-1.31.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-22 01:20:18.356806 botocore-a-la-carte-codedeploy-1.31.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:18.356806 botocore-a-la-carte-codedeploy-1.31.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:18.356806 botocore-a-la-carte-codedeploy-1.31.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:18.356806 botocore-a-la-carte-codedeploy-1.31.9/botocore/data/codedeploy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:18.356806 botocore-a-la-carte-codedeploy-1.31.9/botocore/data/codedeploy/2014-10-06/
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-07-22 01:20:09.000000 botocore-a-la-carte-codedeploy-1.31.9/botocore/data/codedeploy/2014-10-06/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-22 01:20:09.000000 botocore-a-la-carte-codedeploy-1.31.9/botocore/data/codedeploy/2014-10-06/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-22 01:20:09.000000 botocore-a-la-carte-codedeploy-1.31.9/botocore/data/codedeploy/2014-10-06/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   221635 2023-07-22 01:20:09.000000 botocore-a-la-carte-codedeploy-1.31.9/botocore/data/codedeploy/2014-10-06/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-22 01:20:09.000000 botocore-a-la-carte-codedeploy-1.31.9/botocore/data/codedeploy/2014-10-06/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:18.356806 botocore-a-la-carte-codedeploy-1.31.9/botocore_a_la_carte_codedeploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-22 01:20:18.000000 botocore-a-la-carte-codedeploy-1.31.9/botocore_a_la_carte_codedeploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-22 01:20:18.000000 botocore-a-la-carte-codedeploy-1.31.9/botocore_a_la_carte_codedeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 01:20:18.000000 botocore-a-la-carte-codedeploy-1.31.9/botocore_a_la_carte_codedeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 01:20:18.000000 botocore-a-la-carte-codedeploy-1.31.9/botocore_a_la_carte_codedeploy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 01:20:18.356806 botocore-a-la-carte-codedeploy-1.31.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-22 01:20:18.000000 botocore-a-la-carte-codedeploy-1.31.9/setup.py
```

### Comparing `botocore-a-la-carte-codedeploy-1.31.8/LICENSE.txt` & `botocore-a-la-carte-codedeploy-1.31.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-codedeploy-1.31.8/PKG-INFO` & `botocore-a-la-carte-codedeploy-1.31.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-codedeploy
-Version: 1.31.8
+Version: 1.31.9
 Summary: codedeploy data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-codedeploy-1.31.8/botocore/data/codedeploy/2014-10-06/endpoint-rule-set-1.json` & `botocore-a-la-carte-codedeploy-1.31.9/botocore/data/codedeploy/2014-10-06/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-codedeploy-1.31.8/botocore/data/codedeploy/2014-10-06/paginators-1.json` & `botocore-a-la-carte-codedeploy-1.31.9/botocore/data/codedeploy/2014-10-06/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-codedeploy-1.31.8/botocore/data/codedeploy/2014-10-06/service-2.json` & `botocore-a-la-carte-codedeploy-1.31.9/botocore/data/codedeploy/2014-10-06/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-codedeploy-1.31.8/botocore/data/codedeploy/2014-10-06/waiters-2.json` & `botocore-a-la-carte-codedeploy-1.31.9/botocore/data/codedeploy/2014-10-06/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-codedeploy-1.31.8/botocore_a_la_carte_codedeploy.egg-info/PKG-INFO` & `botocore-a-la-carte-codedeploy-1.31.9/botocore_a_la_carte_codedeploy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-codedeploy
-Version: 1.31.8
+Version: 1.31.9
 Summary: codedeploy data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-codedeploy-1.31.8/setup.py` & `botocore-a-la-carte-codedeploy-1.31.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-codedeploy',
-    version="1.31.8",
+    version="1.31.9",
     description='codedeploy data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/codedeploy/*/*.json'],
```

