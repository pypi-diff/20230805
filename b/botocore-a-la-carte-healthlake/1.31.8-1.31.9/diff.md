# Comparing `tmp/botocore-a-la-carte-healthlake-1.31.8.tar.gz` & `tmp/botocore-a-la-carte-healthlake-1.31.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-healthlake-1.31.8.tar", last modified: Fri Jul 21 01:21:25 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-healthlake-1.31.9.tar", last modified: Sat Jul 22 01:20:28 2023, max compression
```

## Comparing `botocore-a-la-carte-healthlake-1.31.8.tar` & `botocore-a-la-carte-healthlake-1.31.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:25.747011 botocore-a-la-carte-healthlake-1.31.8/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-21 01:21:25.000000 botocore-a-la-carte-healthlake-1.31.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-21 01:21:25.747011 botocore-a-la-carte-healthlake-1.31.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:25.747011 botocore-a-la-carte-healthlake-1.31.8/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:25.747011 botocore-a-la-carte-healthlake-1.31.8/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:25.747011 botocore-a-la-carte-healthlake-1.31.8/botocore/data/healthlake/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:25.747011 botocore-a-la-carte-healthlake-1.31.8/botocore/data/healthlake/2017-07-01/
--rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-07-21 01:21:06.000000 botocore-a-la-carte-healthlake-1.31.8/botocore/data/healthlake/2017-07-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 01:21:06.000000 botocore-a-la-carte-healthlake-1.31.8/botocore/data/healthlake/2017-07-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 01:21:06.000000 botocore-a-la-carte-healthlake-1.31.8/botocore/data/healthlake/2017-07-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    42875 2023-07-21 01:21:06.000000 botocore-a-la-carte-healthlake-1.31.8/botocore/data/healthlake/2017-07-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:25.747011 botocore-a-la-carte-healthlake-1.31.8/botocore_a_la_carte_healthlake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-21 01:21:25.000000 botocore-a-la-carte-healthlake-1.31.8/botocore_a_la_carte_healthlake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-21 01:21:25.000000 botocore-a-la-carte-healthlake-1.31.8/botocore_a_la_carte_healthlake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:21:25.000000 botocore-a-la-carte-healthlake-1.31.8/botocore_a_la_carte_healthlake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 01:21:25.000000 botocore-a-la-carte-healthlake-1.31.8/botocore_a_la_carte_healthlake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:21:25.747011 botocore-a-la-carte-healthlake-1.31.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-21 01:21:25.000000 botocore-a-la-carte-healthlake-1.31.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:28.260970 botocore-a-la-carte-healthlake-1.31.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-22 01:20:28.000000 botocore-a-la-carte-healthlake-1.31.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-22 01:20:28.260970 botocore-a-la-carte-healthlake-1.31.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:28.256970 botocore-a-la-carte-healthlake-1.31.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:28.256970 botocore-a-la-carte-healthlake-1.31.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:28.256970 botocore-a-la-carte-healthlake-1.31.9/botocore/data/healthlake/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:28.260970 botocore-a-la-carte-healthlake-1.31.9/botocore/data/healthlake/2017-07-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-07-22 01:20:09.000000 botocore-a-la-carte-healthlake-1.31.9/botocore/data/healthlake/2017-07-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-22 01:20:09.000000 botocore-a-la-carte-healthlake-1.31.9/botocore/data/healthlake/2017-07-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-22 01:20:09.000000 botocore-a-la-carte-healthlake-1.31.9/botocore/data/healthlake/2017-07-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    42875 2023-07-22 01:20:09.000000 botocore-a-la-carte-healthlake-1.31.9/botocore/data/healthlake/2017-07-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:28.260970 botocore-a-la-carte-healthlake-1.31.9/botocore_a_la_carte_healthlake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-22 01:20:28.000000 botocore-a-la-carte-healthlake-1.31.9/botocore_a_la_carte_healthlake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-22 01:20:28.000000 botocore-a-la-carte-healthlake-1.31.9/botocore_a_la_carte_healthlake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 01:20:28.000000 botocore-a-la-carte-healthlake-1.31.9/botocore_a_la_carte_healthlake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 01:20:28.000000 botocore-a-la-carte-healthlake-1.31.9/botocore_a_la_carte_healthlake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 01:20:28.260970 botocore-a-la-carte-healthlake-1.31.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-22 01:20:28.000000 botocore-a-la-carte-healthlake-1.31.9/setup.py
```

### Comparing `botocore-a-la-carte-healthlake-1.31.8/LICENSE.txt` & `botocore-a-la-carte-healthlake-1.31.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-healthlake-1.31.8/PKG-INFO` & `botocore-a-la-carte-healthlake-1.31.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-healthlake
-Version: 1.31.8
+Version: 1.31.9
 Summary: healthlake data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-healthlake-1.31.8/botocore/data/healthlake/2017-07-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-healthlake-1.31.9/botocore/data/healthlake/2017-07-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-healthlake-1.31.8/botocore/data/healthlake/2017-07-01/service-2.json` & `botocore-a-la-carte-healthlake-1.31.9/botocore/data/healthlake/2017-07-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-healthlake-1.31.8/botocore_a_la_carte_healthlake.egg-info/PKG-INFO` & `botocore-a-la-carte-healthlake-1.31.9/botocore_a_la_carte_healthlake.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-healthlake
-Version: 1.31.8
+Version: 1.31.9
 Summary: healthlake data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-healthlake-1.31.8/setup.py` & `botocore-a-la-carte-healthlake-1.31.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-healthlake',
-    version="1.31.8",
+    version="1.31.9",
     description='healthlake data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/healthlake/*/*.json'],
```

