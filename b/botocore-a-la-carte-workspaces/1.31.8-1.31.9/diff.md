# Comparing `tmp/botocore-a-la-carte-workspaces-1.31.8.tar.gz` & `tmp/botocore-a-la-carte-workspaces-1.31.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-workspaces-1.31.8.tar", last modified: Fri Jul 21 01:22:00 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-workspaces-1.31.9.tar", last modified: Sat Jul 22 01:21:00 2023, max compression
```

## Comparing `botocore-a-la-carte-workspaces-1.31.8.tar` & `botocore-a-la-carte-workspaces-1.31.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:22:00.015627 botocore-a-la-carte-workspaces-1.31.8/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-21 01:21:59.000000 botocore-a-la-carte-workspaces-1.31.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-21 01:22:00.015627 botocore-a-la-carte-workspaces-1.31.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:22:00.015627 botocore-a-la-carte-workspaces-1.31.8/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:22:00.015627 botocore-a-la-carte-workspaces-1.31.8/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:22:00.015627 botocore-a-la-carte-workspaces-1.31.8/botocore/data/workspaces/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:22:00.015627 botocore-a-la-carte-workspaces-1.31.8/botocore/data/workspaces/2015-04-08/
--rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-07-21 01:21:06.000000 botocore-a-la-carte-workspaces-1.31.8/botocore/data/workspaces/2015-04-08/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 01:21:06.000000 botocore-a-la-carte-workspaces-1.31.8/botocore/data/workspaces/2015-04-08/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-21 01:21:06.000000 botocore-a-la-carte-workspaces-1.31.8/botocore/data/workspaces/2015-04-08/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   199316 2023-07-21 01:21:06.000000 botocore-a-la-carte-workspaces-1.31.8/botocore/data/workspaces/2015-04-08/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:22:00.015627 botocore-a-la-carte-workspaces-1.31.8/botocore_a_la_carte_workspaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-21 01:21:59.000000 botocore-a-la-carte-workspaces-1.31.8/botocore_a_la_carte_workspaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-21 01:21:59.000000 botocore-a-la-carte-workspaces-1.31.8/botocore_a_la_carte_workspaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:21:59.000000 botocore-a-la-carte-workspaces-1.31.8/botocore_a_la_carte_workspaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 01:21:59.000000 botocore-a-la-carte-workspaces-1.31.8/botocore_a_la_carte_workspaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:22:00.015627 botocore-a-la-carte-workspaces-1.31.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-21 01:21:59.000000 botocore-a-la-carte-workspaces-1.31.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:21:00.509463 botocore-a-la-carte-workspaces-1.31.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-22 01:21:00.000000 botocore-a-la-carte-workspaces-1.31.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-22 01:21:00.509463 botocore-a-la-carte-workspaces-1.31.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:21:00.509463 botocore-a-la-carte-workspaces-1.31.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:21:00.509463 botocore-a-la-carte-workspaces-1.31.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:21:00.509463 botocore-a-la-carte-workspaces-1.31.9/botocore/data/workspaces/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:21:00.509463 botocore-a-la-carte-workspaces-1.31.9/botocore/data/workspaces/2015-04-08/
+-rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-07-22 01:20:09.000000 botocore-a-la-carte-workspaces-1.31.9/botocore/data/workspaces/2015-04-08/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-22 01:20:09.000000 botocore-a-la-carte-workspaces-1.31.9/botocore/data/workspaces/2015-04-08/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-22 01:20:09.000000 botocore-a-la-carte-workspaces-1.31.9/botocore/data/workspaces/2015-04-08/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   199338 2023-07-22 01:20:09.000000 botocore-a-la-carte-workspaces-1.31.9/botocore/data/workspaces/2015-04-08/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:21:00.509463 botocore-a-la-carte-workspaces-1.31.9/botocore_a_la_carte_workspaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-22 01:21:00.000000 botocore-a-la-carte-workspaces-1.31.9/botocore_a_la_carte_workspaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-22 01:21:00.000000 botocore-a-la-carte-workspaces-1.31.9/botocore_a_la_carte_workspaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 01:21:00.000000 botocore-a-la-carte-workspaces-1.31.9/botocore_a_la_carte_workspaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 01:21:00.000000 botocore-a-la-carte-workspaces-1.31.9/botocore_a_la_carte_workspaces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 01:21:00.509463 botocore-a-la-carte-workspaces-1.31.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-22 01:21:00.000000 botocore-a-la-carte-workspaces-1.31.9/setup.py
```

### Comparing `botocore-a-la-carte-workspaces-1.31.8/LICENSE.txt` & `botocore-a-la-carte-workspaces-1.31.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-workspaces-1.31.8/PKG-INFO` & `botocore-a-la-carte-workspaces-1.31.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-workspaces
-Version: 1.31.8
+Version: 1.31.9
 Summary: workspaces data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-workspaces-1.31.8/botocore/data/workspaces/2015-04-08/endpoint-rule-set-1.json` & `botocore-a-la-carte-workspaces-1.31.9/botocore/data/workspaces/2015-04-08/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-workspaces-1.31.8/botocore/data/workspaces/2015-04-08/paginators-1.json` & `botocore-a-la-carte-workspaces-1.31.9/botocore/data/workspaces/2015-04-08/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-workspaces-1.31.8/botocore/data/workspaces/2015-04-08/service-2.json` & `botocore-a-la-carte-workspaces-1.31.9/botocore/data/workspaces/2015-04-08/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999995184603057%*

 * *Differences: {"'shapes'": "{'Workspace': {'members': {'VolumeEncryptionKey': {'documentation': '<p>The ARN of "*

 * *             'the symmetric KMS key used to encrypt data stored on your WorkSpace. Amazon '*

 * *             "WorkSpaces does not support asymmetric KMS keys.</p>'}}}, 'WorkspaceRequest': "*

 * *             "{'members': {'VolumeEncryptionKey': {'documentation': '<p>The ARN of the symmetric "*

 * *             'KMS key used to encrypt data stored on your WorkSpace. Amazon WorkSpaces does not '*

 * *             "support asymmetr […]*

```diff
@@ -5092,15 +5092,15 @@
                     "shape": "UserName"
                 },
                 "UserVolumeEncryptionEnabled": {
                     "documentation": "<p>Indicates whether the data stored on the user volume is encrypted.</p>",
                     "shape": "BooleanObject"
                 },
                 "VolumeEncryptionKey": {
-                    "documentation": "<p>The symmetric KMS key used to encrypt data stored on your WorkSpace. Amazon WorkSpaces does not support asymmetric KMS keys.</p>",
+                    "documentation": "<p>The ARN of the symmetric KMS key used to encrypt data stored on your WorkSpace. Amazon WorkSpaces does not support asymmetric KMS keys.</p>",
                     "shape": "VolumeEncryptionKey"
                 },
                 "WorkspaceId": {
                     "documentation": "<p>The identifier of the WorkSpace.</p>",
                     "shape": "WorkspaceId"
                 },
                 "WorkspaceProperties": {
@@ -5560,15 +5560,15 @@
                     "shape": "UserName"
                 },
                 "UserVolumeEncryptionEnabled": {
                     "documentation": "<p>Indicates whether the data stored on the user volume is encrypted.</p>",
                     "shape": "BooleanObject"
                 },
                 "VolumeEncryptionKey": {
-                    "documentation": "<p>The symmetric KMS key used to encrypt data stored on your WorkSpace. Amazon WorkSpaces does not support asymmetric KMS keys.</p>",
+                    "documentation": "<p>The ARN of the symmetric KMS key used to encrypt data stored on your WorkSpace. Amazon WorkSpaces does not support asymmetric KMS keys.</p>",
                     "shape": "VolumeEncryptionKey"
                 },
                 "WorkspaceProperties": {
                     "documentation": "<p>The WorkSpace properties.</p>",
                     "shape": "WorkspaceProperties"
                 }
             },
```

### Comparing `botocore-a-la-carte-workspaces-1.31.8/botocore_a_la_carte_workspaces.egg-info/PKG-INFO` & `botocore-a-la-carte-workspaces-1.31.9/botocore_a_la_carte_workspaces.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-workspaces
-Version: 1.31.8
+Version: 1.31.9
 Summary: workspaces data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-workspaces-1.31.8/setup.py` & `botocore-a-la-carte-workspaces-1.31.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-workspaces',
-    version="1.31.8",
+    version="1.31.9",
     description='workspaces data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/workspaces/*/*.json'],
```

