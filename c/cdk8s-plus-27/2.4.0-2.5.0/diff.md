# Comparing `tmp/cdk8s-plus-27-2.4.0.tar.gz` & `tmp/cdk8s-plus-27-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-plus-27-2.4.0.tar", last modified: Thu Aug  3 00:38:05 2023, max compression
+gzip compressed data, was "cdk8s-plus-27-2.5.0.tar", last modified: Sat Aug  5 12:13:47 2023, max compression
```

## Comparing `cdk8s-plus-27-2.4.0.tar` & `cdk8s-plus-27-2.5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:38:05.067807 cdk8s-plus-27-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-03 00:37:52.000000 cdk8s-plus-27-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-03 00:37:52.000000 cdk8s-plus-27-2.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-03 00:37:52.000000 cdk8s-plus-27-2.4.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-08-03 00:38:05.067807 cdk8s-plus-27-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-03 00:37:52.000000 cdk8s-plus-27-2.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-03 00:37:52.000000 cdk8s-plus-27-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 00:38:05.067807 cdk8s-plus-27-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-08-03 00:37:52.000000 cdk8s-plus-27-2.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:38:05.059807 cdk8s-plus-27-2.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:38:05.063807 cdk8s-plus-27-2.4.0/src/cdk8s_plus_27/
--rw-r--r--   0 runner    (1001) docker     (123)  1166210 2023-08-03 00:37:52.000000 cdk8s-plus-27-2.4.0/src/cdk8s_plus_27/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:38:05.063807 cdk8s-plus-27-2.4.0/src/cdk8s_plus_27/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-03 00:37:52.000000 cdk8s-plus-27-2.4.0/src/cdk8s_plus_27/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1316364 2023-08-03 00:37:52.000000 cdk8s-plus-27-2.4.0/src/cdk8s_plus_27/_jsii/cdk8s-plus-27@2.4.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:38:05.063807 cdk8s-plus-27-2.4.0/src/cdk8s_plus_27/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)  2838846 2023-08-03 00:37:52.000000 cdk8s-plus-27-2.4.0/src/cdk8s_plus_27/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 00:37:52.000000 cdk8s-plus-27-2.4.0/src/cdk8s_plus_27/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:38:05.063807 cdk8s-plus-27-2.4.0/src/cdk8s_plus_27.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-08-03 00:38:05.000000 cdk8s-plus-27-2.4.0/src/cdk8s_plus_27.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-03 00:38:05.000000 cdk8s-plus-27-2.4.0/src/cdk8s_plus_27.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 00:38:05.000000 cdk8s-plus-27-2.4.0/src/cdk8s_plus_27.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-03 00:38:05.000000 cdk8s-plus-27-2.4.0/src/cdk8s_plus_27.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-03 00:38:05.000000 cdk8s-plus-27-2.4.0/src/cdk8s_plus_27.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:13:47.419739 cdk8s-plus-27-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-05 12:13:35.000000 cdk8s-plus-27-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-05 12:13:35.000000 cdk8s-plus-27-2.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-05 12:13:35.000000 cdk8s-plus-27-2.5.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-08-05 12:13:47.419739 cdk8s-plus-27-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-05 12:13:35.000000 cdk8s-plus-27-2.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-05 12:13:35.000000 cdk8s-plus-27-2.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 12:13:47.419739 cdk8s-plus-27-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-08-05 12:13:35.000000 cdk8s-plus-27-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:13:47.411738 cdk8s-plus-27-2.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:13:47.415739 cdk8s-plus-27-2.5.0/src/cdk8s_plus_27/
+-rw-r--r--   0 runner    (1001) docker     (123)  1166210 2023-08-05 12:13:35.000000 cdk8s-plus-27-2.5.0/src/cdk8s_plus_27/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:13:47.415739 cdk8s-plus-27-2.5.0/src/cdk8s_plus_27/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-05 12:13:35.000000 cdk8s-plus-27-2.5.0/src/cdk8s_plus_27/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1316367 2023-08-05 12:13:35.000000 cdk8s-plus-27-2.5.0/src/cdk8s_plus_27/_jsii/cdk8s-plus-27@2.5.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:13:47.419739 cdk8s-plus-27-2.5.0/src/cdk8s_plus_27/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)  2838846 2023-08-05 12:13:35.000000 cdk8s-plus-27-2.5.0/src/cdk8s_plus_27/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 12:13:35.000000 cdk8s-plus-27-2.5.0/src/cdk8s_plus_27/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:13:47.415739 cdk8s-plus-27-2.5.0/src/cdk8s_plus_27.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-08-05 12:13:47.000000 cdk8s-plus-27-2.5.0/src/cdk8s_plus_27.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-05 12:13:47.000000 cdk8s-plus-27-2.5.0/src/cdk8s_plus_27.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 12:13:47.000000 cdk8s-plus-27-2.5.0/src/cdk8s_plus_27.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-05 12:13:47.000000 cdk8s-plus-27-2.5.0/src/cdk8s_plus_27.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-05 12:13:47.000000 cdk8s-plus-27-2.5.0/src/cdk8s_plus_27.egg-info/top_level.txt
```

### Comparing `cdk8s-plus-27-2.4.0/LICENSE` & `cdk8s-plus-27-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-27-2.4.0/PKG-INFO` & `cdk8s-plus-27-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-27
-Version: 2.4.0
+Version: 2.5.0
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-27 synthesizes Kubernetes manifests for Kubernetes 1.27.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-plus-27-2.4.0/README.md` & `cdk8s-plus-27-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-27-2.4.0/setup.py` & `cdk8s-plus-27-2.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-plus-27",
-    "version": "2.4.0",
+    "version": "2.5.0",
     "description": "cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-27 synthesizes Kubernetes manifests for Kubernetes 1.27.0",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-plus.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -23,15 +23,15 @@
     "packages": [
         "cdk8s_plus_27",
         "cdk8s_plus_27._jsii",
         "cdk8s_plus_27.k8s"
     ],
     "package_data": {
         "cdk8s_plus_27._jsii": [
-            "cdk8s-plus-27@2.4.0.jsii.tgz"
+            "cdk8s-plus-27@2.5.0.jsii.tgz"
         ],
         "cdk8s_plus_27": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk8s-plus-27-2.4.0/src/cdk8s_plus_27/__init__.py` & `cdk8s-plus-27-2.5.0/src/cdk8s_plus_27/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-27-2.4.0/src/cdk8s_plus_27/k8s/__init__.py` & `cdk8s-plus-27-2.5.0/src/cdk8s_plus_27/k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-27-2.4.0/src/cdk8s_plus_27.egg-info/PKG-INFO` & `cdk8s-plus-27-2.5.0/src/cdk8s_plus_27.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-27
-Version: 2.4.0
+Version: 2.5.0
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-27 synthesizes Kubernetes manifests for Kubernetes 1.27.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

