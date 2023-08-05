# Comparing `tmp/botocore-a-la-carte-cognito-sync-1.31.8.tar.gz` & `tmp/botocore-a-la-carte-cognito-sync-1.31.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-cognito-sync-1.31.8.tar", last modified: Fri Jul 21 01:21:17 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-cognito-sync-1.31.9.tar", last modified: Sat Jul 22 01:20:20 2023, max compression
```

## Comparing `botocore-a-la-carte-cognito-sync-1.31.8.tar` & `botocore-a-la-carte-cognito-sync-1.31.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:17.982859 botocore-a-la-carte-cognito-sync-1.31.8/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-21 01:21:17.000000 botocore-a-la-carte-cognito-sync-1.31.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-21 01:21:17.982859 botocore-a-la-carte-cognito-sync-1.31.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:17.978859 botocore-a-la-carte-cognito-sync-1.31.8/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:17.978859 botocore-a-la-carte-cognito-sync-1.31.8/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:17.978859 botocore-a-la-carte-cognito-sync-1.31.8/botocore/data/cognito-sync/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:17.978859 botocore-a-la-carte-cognito-sync-1.31.8/botocore/data/cognito-sync/2014-06-30/
--rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-07-21 01:21:06.000000 botocore-a-la-carte-cognito-sync-1.31.8/botocore/data/cognito-sync/2014-06-30/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 01:21:06.000000 botocore-a-la-carte-cognito-sync-1.31.8/botocore/data/cognito-sync/2014-06-30/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 01:21:06.000000 botocore-a-la-carte-cognito-sync-1.31.8/botocore/data/cognito-sync/2014-06-30/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    59424 2023-07-21 01:21:06.000000 botocore-a-la-carte-cognito-sync-1.31.8/botocore/data/cognito-sync/2014-06-30/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:17.978859 botocore-a-la-carte-cognito-sync-1.31.8/botocore_a_la_carte_cognito_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-21 01:21:17.000000 botocore-a-la-carte-cognito-sync-1.31.8/botocore_a_la_carte_cognito_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-21 01:21:17.000000 botocore-a-la-carte-cognito-sync-1.31.8/botocore_a_la_carte_cognito_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:21:17.000000 botocore-a-la-carte-cognito-sync-1.31.8/botocore_a_la_carte_cognito_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 01:21:17.000000 botocore-a-la-carte-cognito-sync-1.31.8/botocore_a_la_carte_cognito_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:21:17.982859 botocore-a-la-carte-cognito-sync-1.31.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-21 01:21:17.000000 botocore-a-la-carte-cognito-sync-1.31.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:20.988847 botocore-a-la-carte-cognito-sync-1.31.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-22 01:20:20.000000 botocore-a-la-carte-cognito-sync-1.31.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-22 01:20:20.984847 botocore-a-la-carte-cognito-sync-1.31.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:20.984847 botocore-a-la-carte-cognito-sync-1.31.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:20.984847 botocore-a-la-carte-cognito-sync-1.31.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:20.984847 botocore-a-la-carte-cognito-sync-1.31.9/botocore/data/cognito-sync/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:20.984847 botocore-a-la-carte-cognito-sync-1.31.9/botocore/data/cognito-sync/2014-06-30/
+-rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-07-22 01:20:09.000000 botocore-a-la-carte-cognito-sync-1.31.9/botocore/data/cognito-sync/2014-06-30/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-22 01:20:09.000000 botocore-a-la-carte-cognito-sync-1.31.9/botocore/data/cognito-sync/2014-06-30/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-22 01:20:09.000000 botocore-a-la-carte-cognito-sync-1.31.9/botocore/data/cognito-sync/2014-06-30/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    59424 2023-07-22 01:20:09.000000 botocore-a-la-carte-cognito-sync-1.31.9/botocore/data/cognito-sync/2014-06-30/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:20.984847 botocore-a-la-carte-cognito-sync-1.31.9/botocore_a_la_carte_cognito_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-22 01:20:20.000000 botocore-a-la-carte-cognito-sync-1.31.9/botocore_a_la_carte_cognito_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-22 01:20:20.000000 botocore-a-la-carte-cognito-sync-1.31.9/botocore_a_la_carte_cognito_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 01:20:20.000000 botocore-a-la-carte-cognito-sync-1.31.9/botocore_a_la_carte_cognito_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 01:20:20.000000 botocore-a-la-carte-cognito-sync-1.31.9/botocore_a_la_carte_cognito_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 01:20:20.988847 botocore-a-la-carte-cognito-sync-1.31.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-22 01:20:20.000000 botocore-a-la-carte-cognito-sync-1.31.9/setup.py
```

### Comparing `botocore-a-la-carte-cognito-sync-1.31.8/LICENSE.txt` & `botocore-a-la-carte-cognito-sync-1.31.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cognito-sync-1.31.8/PKG-INFO` & `botocore-a-la-carte-cognito-sync-1.31.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-cognito-sync
-Version: 1.31.8
+Version: 1.31.9
 Summary: cognito-sync data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-cognito-sync-1.31.8/botocore/data/cognito-sync/2014-06-30/endpoint-rule-set-1.json` & `botocore-a-la-carte-cognito-sync-1.31.9/botocore/data/cognito-sync/2014-06-30/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cognito-sync-1.31.8/botocore/data/cognito-sync/2014-06-30/service-2.json` & `botocore-a-la-carte-cognito-sync-1.31.9/botocore/data/cognito-sync/2014-06-30/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cognito-sync-1.31.8/botocore_a_la_carte_cognito_sync.egg-info/PKG-INFO` & `botocore-a-la-carte-cognito-sync-1.31.9/botocore_a_la_carte_cognito_sync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-cognito-sync
-Version: 1.31.8
+Version: 1.31.9
 Summary: cognito-sync data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-cognito-sync-1.31.8/setup.py` & `botocore-a-la-carte-cognito-sync-1.31.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-cognito-sync',
-    version="1.31.8",
+    version="1.31.9",
     description='cognito-sync data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/cognito-sync/*/*.json'],
```

