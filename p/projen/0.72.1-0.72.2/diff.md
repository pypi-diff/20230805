# Comparing `tmp/projen-0.72.1.tar.gz` & `tmp/projen-0.72.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projen-0.72.1.tar", last modified: Thu Aug  3 12:51:56 2023, max compression
+gzip compressed data, was "projen-0.72.2.tar", last modified: Fri Aug  4 12:35:59 2023, max compression
```

## Comparing `projen-0.72.1.tar` & `projen-0.72.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:56.115465 projen-0.72.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-03 12:51:38.000000 projen-0.72.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-03 12:51:38.000000 projen-0.72.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    55403 2023-08-03 12:51:56.111465 projen-0.72.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    54524 2023-08-03 12:51:38.000000 projen-0.72.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-03 12:51:38.000000 projen-0.72.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 12:51:56.115465 projen-0.72.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-03 12:51:38.000000 projen-0.72.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:56.099465 projen-0.72.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:56.099465 projen-0.72.1/src/projen/
--rw-r--r--   0 runner    (1001) docker     (123)   601934 2023-08-03 12:51:38.000000 projen-0.72.1/src/projen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:56.103465 projen-0.72.1/src/projen/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-03 12:51:38.000000 projen-0.72.1/src/projen/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:56.103465 projen-0.72.1/src/projen/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-03 12:51:38.000000 projen-0.72.1/src/projen/_jsii/bin/projen
--rw-r--r--   0 runner    (1001) docker     (123)  2754031 2023-08-03 12:51:38.000000 projen-0.72.1/src/projen/_jsii/projen@0.72.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:56.103465 projen-0.72.1/src/projen/awscdk/
--rw-r--r--   0 runner    (1001) docker     (123)  1040675 2023-08-03 12:51:38.000000 projen-0.72.1/src/projen/awscdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:56.107465 projen-0.72.1/src/projen/build/
--rw-r--r--   0 runner    (1001) docker     (123)    40847 2023-08-03 12:51:38.000000 projen-0.72.1/src/projen/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:56.107465 projen-0.72.1/src/projen/cdk/
--rw-r--r--   0 runner    (1001) docker     (123)   480911 2023-08-03 12:51:38.000000 projen-0.72.1/src/projen/cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:56.107465 projen-0.72.1/src/projen/cdk8s/
--rw-r--r--   0 runner    (1001) docker     (123)   575465 2023-08-03 12:51:38.000000 projen-0.72.1/src/projen/cdk8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:56.107465 projen-0.72.1/src/projen/cdktf/
--rw-r--r--   0 runner    (1001) docker     (123)   213323 2023-08-03 12:51:38.000000 projen-0.72.1/src/projen/cdktf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:56.107465 projen-0.72.1/src/projen/circleci/
--rw-r--r--   0 runner    (1001) docker     (123)    75837 2023-08-03 12:51:38.000000 projen-0.72.1/src/projen/circleci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:56.107465 projen-0.72.1/src/projen/github/
--rw-r--r--   0 runner    (1001) docker     (123)   291142 2023-08-03 12:51:38.000000 projen-0.72.1/src/projen/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:56.107465 projen-0.72.1/src/projen/github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)   235582 2023-08-03 12:51:38.000000 projen-0.72.1/src/projen/github/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:56.107465 projen-0.72.1/src/projen/gitlab/
--rw-r--r--   0 runner    (1001) docker     (123)   196190 2023-08-03 12:51:38.000000 projen-0.72.1/src/projen/gitlab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:56.111465 projen-0.72.1/src/projen/java/
--rw-r--r--   0 runner    (1001) docker     (123)   175246 2023-08-03 12:51:38.000000 projen-0.72.1/src/projen/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:56.111465 projen-0.72.1/src/projen/javascript/
--rw-r--r--   0 runner    (1001) docker     (123)   607210 2023-08-03 12:51:38.000000 projen-0.72.1/src/projen/javascript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:51:38.000000 projen-0.72.1/src/projen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:56.111465 projen-0.72.1/src/projen/python/
--rw-r--r--   0 runner    (1001) docker     (123)   190514 2023-08-03 12:51:38.000000 projen-0.72.1/src/projen/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:56.111465 projen-0.72.1/src/projen/release/
--rw-r--r--   0 runner    (1001) docker     (123)   248786 2023-08-03 12:51:38.000000 projen-0.72.1/src/projen/release/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:56.111465 projen-0.72.1/src/projen/typescript/
--rw-r--r--   0 runner    (1001) docker     (123)   430274 2023-08-03 12:51:38.000000 projen-0.72.1/src/projen/typescript/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:56.111465 projen-0.72.1/src/projen/vscode/
--rw-r--r--   0 runner    (1001) docker     (123)    54316 2023-08-03 12:51:38.000000 projen-0.72.1/src/projen/vscode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:56.111465 projen-0.72.1/src/projen/web/
--rw-r--r--   0 runner    (1001) docker     (123)   756498 2023-08-03 12:51:38.000000 projen-0.72.1/src/projen/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:51:56.103465 projen-0.72.1/src/projen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    55403 2023-08-03 12:51:56.000000 projen-0.72.1/src/projen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-03 12:51:56.000000 projen-0.72.1/src/projen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:51:56.000000 projen-0.72.1/src/projen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-03 12:51:56.000000 projen-0.72.1/src/projen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 12:51:56.000000 projen-0.72.1/src/projen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:35:59.001876 projen-0.72.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-04 12:35:43.000000 projen-0.72.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-04 12:35:43.000000 projen-0.72.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    55403 2023-08-04 12:35:59.001876 projen-0.72.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    54524 2023-08-04 12:35:43.000000 projen-0.72.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-04 12:35:43.000000 projen-0.72.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:35:59.001876 projen-0.72.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-04 12:35:43.000000 projen-0.72.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:35:58.985875 projen-0.72.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:35:58.989876 projen-0.72.2/src/projen/
+-rw-r--r--   0 runner    (1001) docker     (123)   601934 2023-08-04 12:35:43.000000 projen-0.72.2/src/projen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:35:58.989876 projen-0.72.2/src/projen/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-04 12:35:43.000000 projen-0.72.2/src/projen/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:35:58.993876 projen-0.72.2/src/projen/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-04 12:35:43.000000 projen-0.72.2/src/projen/_jsii/bin/projen
+-rw-r--r--   0 runner    (1001) docker     (123)  2754034 2023-08-04 12:35:43.000000 projen-0.72.2/src/projen/_jsii/projen@0.72.2.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:35:58.993876 projen-0.72.2/src/projen/awscdk/
+-rw-r--r--   0 runner    (1001) docker     (123)  1040675 2023-08-04 12:35:43.000000 projen-0.72.2/src/projen/awscdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:35:58.993876 projen-0.72.2/src/projen/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    40847 2023-08-04 12:35:43.000000 projen-0.72.2/src/projen/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:35:58.993876 projen-0.72.2/src/projen/cdk/
+-rw-r--r--   0 runner    (1001) docker     (123)   480911 2023-08-04 12:35:43.000000 projen-0.72.2/src/projen/cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:35:58.993876 projen-0.72.2/src/projen/cdk8s/
+-rw-r--r--   0 runner    (1001) docker     (123)   575465 2023-08-04 12:35:43.000000 projen-0.72.2/src/projen/cdk8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:35:58.993876 projen-0.72.2/src/projen/cdktf/
+-rw-r--r--   0 runner    (1001) docker     (123)   213323 2023-08-04 12:35:43.000000 projen-0.72.2/src/projen/cdktf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:35:58.993876 projen-0.72.2/src/projen/circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)    75837 2023-08-04 12:35:43.000000 projen-0.72.2/src/projen/circleci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:35:58.997876 projen-0.72.2/src/projen/github/
+-rw-r--r--   0 runner    (1001) docker     (123)   291142 2023-08-04 12:35:43.000000 projen-0.72.2/src/projen/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:35:58.997876 projen-0.72.2/src/projen/github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)   235582 2023-08-04 12:35:43.000000 projen-0.72.2/src/projen/github/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:35:58.997876 projen-0.72.2/src/projen/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (123)   196190 2023-08-04 12:35:43.000000 projen-0.72.2/src/projen/gitlab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:35:58.997876 projen-0.72.2/src/projen/java/
+-rw-r--r--   0 runner    (1001) docker     (123)   175246 2023-08-04 12:35:43.000000 projen-0.72.2/src/projen/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:35:58.997876 projen-0.72.2/src/projen/javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)   607210 2023-08-04 12:35:43.000000 projen-0.72.2/src/projen/javascript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:35:43.000000 projen-0.72.2/src/projen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:35:58.997876 projen-0.72.2/src/projen/python/
+-rw-r--r--   0 runner    (1001) docker     (123)   190514 2023-08-04 12:35:43.000000 projen-0.72.2/src/projen/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:35:58.997876 projen-0.72.2/src/projen/release/
+-rw-r--r--   0 runner    (1001) docker     (123)   248786 2023-08-04 12:35:43.000000 projen-0.72.2/src/projen/release/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:35:58.997876 projen-0.72.2/src/projen/typescript/
+-rw-r--r--   0 runner    (1001) docker     (123)   430274 2023-08-04 12:35:43.000000 projen-0.72.2/src/projen/typescript/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:35:59.001876 projen-0.72.2/src/projen/vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)    54316 2023-08-04 12:35:43.000000 projen-0.72.2/src/projen/vscode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:35:59.001876 projen-0.72.2/src/projen/web/
+-rw-r--r--   0 runner    (1001) docker     (123)   756498 2023-08-04 12:35:43.000000 projen-0.72.2/src/projen/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:35:58.989876 projen-0.72.2/src/projen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    55403 2023-08-04 12:35:58.000000 projen-0.72.2/src/projen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-04 12:35:58.000000 projen-0.72.2/src/projen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:35:58.000000 projen-0.72.2/src/projen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-04 12:35:58.000000 projen-0.72.2/src/projen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 12:35:58.000000 projen-0.72.2/src/projen.egg-info/top_level.txt
```

### Comparing `projen-0.72.1/LICENSE` & `projen-0.72.2/LICENSE`

 * *Files identical despite different names*

### Comparing `projen-0.72.1/PKG-INFO` & `projen-0.72.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.72.1
+Version: 0.72.2
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.72.1/README.md` & `projen-0.72.2/README.md`

 * *Files identical despite different names*

### Comparing `projen-0.72.1/setup.py` & `projen-0.72.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "projen",
-    "version": "0.72.1",
+    "version": "0.72.2",
     "description": "CDK for software projects",
     "license": "Apache-2.0",
     "url": "https://github.com/projen/projen.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -38,15 +38,15 @@
         "projen.release",
         "projen.typescript",
         "projen.vscode",
         "projen.web"
     ],
     "package_data": {
         "projen._jsii": [
-            "projen@0.72.1.jsii.tgz"
+            "projen@0.72.2.jsii.tgz"
         ],
         "projen": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `projen-0.72.1/src/projen/__init__.py` & `projen-0.72.2/src/projen/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.1/src/projen/awscdk/__init__.py` & `projen-0.72.2/src/projen/awscdk/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.1/src/projen/build/__init__.py` & `projen-0.72.2/src/projen/build/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.1/src/projen/cdk/__init__.py` & `projen-0.72.2/src/projen/cdk/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.1/src/projen/cdk8s/__init__.py` & `projen-0.72.2/src/projen/cdk8s/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.1/src/projen/cdktf/__init__.py` & `projen-0.72.2/src/projen/cdktf/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.1/src/projen/circleci/__init__.py` & `projen-0.72.2/src/projen/circleci/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.1/src/projen/github/__init__.py` & `projen-0.72.2/src/projen/github/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.1/src/projen/github/workflows/__init__.py` & `projen-0.72.2/src/projen/github/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.1/src/projen/gitlab/__init__.py` & `projen-0.72.2/src/projen/gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.1/src/projen/java/__init__.py` & `projen-0.72.2/src/projen/java/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.1/src/projen/javascript/__init__.py` & `projen-0.72.2/src/projen/javascript/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.1/src/projen/python/__init__.py` & `projen-0.72.2/src/projen/python/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.1/src/projen/release/__init__.py` & `projen-0.72.2/src/projen/release/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.1/src/projen/typescript/__init__.py` & `projen-0.72.2/src/projen/typescript/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.1/src/projen/vscode/__init__.py` & `projen-0.72.2/src/projen/vscode/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.1/src/projen/web/__init__.py` & `projen-0.72.2/src/projen/web/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.1/src/projen.egg-info/PKG-INFO` & `projen-0.72.2/src/projen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.72.1
+Version: 0.72.2
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.72.1/src/projen.egg-info/SOURCES.txt` & `projen-0.72.2/src/projen.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/projen/py.typed
 src/projen.egg-info/PKG-INFO
 src/projen.egg-info/SOURCES.txt
 src/projen.egg-info/dependency_links.txt
 src/projen.egg-info/requires.txt
 src/projen.egg-info/top_level.txt
 src/projen/_jsii/__init__.py
-src/projen/_jsii/projen@0.72.1.jsii.tgz
+src/projen/_jsii/projen@0.72.2.jsii.tgz
 src/projen/_jsii/bin/projen
 src/projen/awscdk/__init__.py
 src/projen/build/__init__.py
 src/projen/cdk/__init__.py
 src/projen/cdk8s/__init__.py
 src/projen/cdktf/__init__.py
 src/projen/circleci/__init__.py
```

