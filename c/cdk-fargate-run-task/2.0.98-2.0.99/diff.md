# Comparing `tmp/cdk-fargate-run-task-2.0.98.tar.gz` & `tmp/cdk-fargate-run-task-2.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-fargate-run-task-2.0.98.tar", last modified: Mon Aug  1 00:11:17 2022, max compression
+gzip compressed data, was "cdk-fargate-run-task-2.0.99.tar", last modified: Tue Aug  2 00:12:24 2022, max compression
```

## Comparing `cdk-fargate-run-task-2.0.98.tar` & `cdk-fargate-run-task-2.0.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 00:11:17.102134 cdk-fargate-run-task-2.0.98/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-08-01 00:11:03.000000 cdk-fargate-run-task-2.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-01 00:11:03.000000 cdk-fargate-run-task-2.0.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4158 2022-08-01 00:11:17.102134 cdk-fargate-run-task-2.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3196 2022-08-01 00:11:03.000000 cdk-fargate-run-task-2.0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-08-01 00:11:03.000000 cdk-fargate-run-task-2.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-01 00:11:17.102134 cdk-fargate-run-task-2.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-08-01 00:11:03.000000 cdk-fargate-run-task-2.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 00:11:17.098134 cdk-fargate-run-task-2.0.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 00:11:17.098134 cdk-fargate-run-task-2.0.98/src/cdk_fargate_run_task/
--rw-r--r--   0 runner    (1001) docker     (121)    19798 2022-08-01 00:11:03.000000 cdk-fargate-run-task-2.0.98/src/cdk_fargate_run_task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 00:11:17.102134 cdk-fargate-run-task-2.0.98/src/cdk_fargate_run_task/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-08-01 00:11:03.000000 cdk-fargate-run-task-2.0.98/src/cdk_fargate_run_task/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29204 2022-08-01 00:11:03.000000 cdk-fargate-run-task-2.0.98/src/cdk_fargate_run_task/_jsii/cdk-fargate-run-task@2.0.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-01 00:11:03.000000 cdk-fargate-run-task-2.0.98/src/cdk_fargate_run_task/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 00:11:17.098134 cdk-fargate-run-task-2.0.98/src/cdk_fargate_run_task.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4158 2022-08-01 00:11:16.000000 cdk-fargate-run-task-2.0.98/src/cdk_fargate_run_task.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-08-01 00:11:17.000000 cdk-fargate-run-task-2.0.98/src/cdk_fargate_run_task.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-01 00:11:16.000000 cdk-fargate-run-task-2.0.98/src/cdk_fargate_run_task.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-08-01 00:11:16.000000 cdk-fargate-run-task-2.0.98/src/cdk_fargate_run_task.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-08-01 00:11:16.000000 cdk-fargate-run-task-2.0.98/src/cdk_fargate_run_task.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 00:12:24.390334 cdk-fargate-run-task-2.0.99/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-08-02 00:12:07.000000 cdk-fargate-run-task-2.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-02 00:12:07.000000 cdk-fargate-run-task-2.0.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4158 2022-08-02 00:12:24.390334 cdk-fargate-run-task-2.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3196 2022-08-02 00:12:07.000000 cdk-fargate-run-task-2.0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-08-02 00:12:07.000000 cdk-fargate-run-task-2.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-02 00:12:24.390334 cdk-fargate-run-task-2.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-08-02 00:12:07.000000 cdk-fargate-run-task-2.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 00:12:24.386333 cdk-fargate-run-task-2.0.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 00:12:24.390334 cdk-fargate-run-task-2.0.99/src/cdk_fargate_run_task/
+-rw-r--r--   0 runner    (1001) docker     (121)    19798 2022-08-02 00:12:07.000000 cdk-fargate-run-task-2.0.99/src/cdk_fargate_run_task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 00:12:24.390334 cdk-fargate-run-task-2.0.99/src/cdk_fargate_run_task/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      422 2022-08-02 00:12:07.000000 cdk-fargate-run-task-2.0.99/src/cdk_fargate_run_task/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29204 2022-08-02 00:12:07.000000 cdk-fargate-run-task-2.0.99/src/cdk_fargate_run_task/_jsii/cdk-fargate-run-task@2.0.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-02 00:12:07.000000 cdk-fargate-run-task-2.0.99/src/cdk_fargate_run_task/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 00:12:24.390334 cdk-fargate-run-task-2.0.99/src/cdk_fargate_run_task.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4158 2022-08-02 00:12:23.000000 cdk-fargate-run-task-2.0.99/src/cdk_fargate_run_task.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2022-08-02 00:12:24.000000 cdk-fargate-run-task-2.0.99/src/cdk_fargate_run_task.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-02 00:12:23.000000 cdk-fargate-run-task-2.0.99/src/cdk_fargate_run_task.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2022-08-02 00:12:24.000000 cdk-fargate-run-task-2.0.99/src/cdk_fargate_run_task.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-08-02 00:12:24.000000 cdk-fargate-run-task-2.0.99/src/cdk_fargate_run_task.egg-info/top_level.txt
```

### Comparing `cdk-fargate-run-task-2.0.98/LICENSE` & `cdk-fargate-run-task-2.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-fargate-run-task-2.0.98/PKG-INFO` & `cdk-fargate-run-task-2.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-fargate-run-task
-Version: 2.0.98
+Version: 2.0.99
 Summary: Define and run container tasks on AWS Fargate immediately or with schedule
 Home-page: https://github.com/pahud/cdk-fargate-run-task.git
 Author: Pahud Hsieh<pahudnet@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/pahud/cdk-fargate-run-task.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk-fargate-run-task-2.0.98/README.md` & `cdk-fargate-run-task-2.0.99/README.md`

 * *Files identical despite different names*

### Comparing `cdk-fargate-run-task-2.0.98/setup.py` & `cdk-fargate-run-task-2.0.99/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-fargate-run-task",
-    "version": "2.0.98",
+    "version": "2.0.99",
     "description": "Define and run container tasks on AWS Fargate immediately or with schedule",
     "license": "Apache-2.0",
     "url": "https://github.com/pahud/cdk-fargate-run-task.git",
     "long_description_content_type": "text/markdown",
     "author": "Pahud Hsieh<pahudnet@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_fargate_run_task",
         "cdk_fargate_run_task._jsii"
     ],
     "package_data": {
         "cdk_fargate_run_task._jsii": [
-            "cdk-fargate-run-task@2.0.98.jsii.tgz"
+            "cdk-fargate-run-task@2.0.99.jsii.tgz"
         ],
         "cdk_fargate_run_task": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-fargate-run-task-2.0.98/src/cdk_fargate_run_task/__init__.py` & `cdk-fargate-run-task-2.0.99/src/cdk_fargate_run_task/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-fargate-run-task-2.0.98/src/cdk_fargate_run_task.egg-info/PKG-INFO` & `cdk-fargate-run-task-2.0.99/src/cdk_fargate_run_task.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-fargate-run-task
-Version: 2.0.98
+Version: 2.0.99
 Summary: Define and run container tasks on AWS Fargate immediately or with schedule
 Home-page: https://github.com/pahud/cdk-fargate-run-task.git
 Author: Pahud Hsieh<pahudnet@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/pahud/cdk-fargate-run-task.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

