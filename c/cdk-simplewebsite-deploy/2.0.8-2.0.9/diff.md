# Comparing `tmp/cdk-simplewebsite-deploy-2.0.8.tar.gz` & `tmp/cdk-simplewebsite-deploy-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-simplewebsite-deploy-2.0.8.tar", last modified: Fri Feb  4 00:47:50 2022, max compression
+gzip compressed data, was "cdk-simplewebsite-deploy-2.0.9.tar", last modified: Sun Feb 13 00:42:55 2022, max compression
```

## Comparing `cdk-simplewebsite-deploy-2.0.8.tar` & `cdk-simplewebsite-deploy-2.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 00:47:50.696991 cdk-simplewebsite-deploy-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-02-04 00:47:36.000000 cdk-simplewebsite-deploy-2.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-02-04 00:47:36.000000 cdk-simplewebsite-deploy-2.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7269 2022-02-04 00:47:50.696991 cdk-simplewebsite-deploy-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6263 2022-02-04 00:47:36.000000 cdk-simplewebsite-deploy-2.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-02-04 00:47:36.000000 cdk-simplewebsite-deploy-2.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-04 00:47:50.696991 cdk-simplewebsite-deploy-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-02-04 00:47:36.000000 cdk-simplewebsite-deploy-2.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 00:47:50.692991 cdk-simplewebsite-deploy-2.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 00:47:50.696991 cdk-simplewebsite-deploy-2.0.8/src/cdk_simplewebsite_deploy/
--rw-r--r--   0 runner    (1001) docker     (121)    17904 2022-02-04 00:47:36.000000 cdk-simplewebsite-deploy-2.0.8/src/cdk_simplewebsite_deploy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 00:47:50.696991 cdk-simplewebsite-deploy-2.0.8/src/cdk_simplewebsite_deploy/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-02-04 00:47:36.000000 cdk-simplewebsite-deploy-2.0.8/src/cdk_simplewebsite_deploy/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23151 2022-02-04 00:47:36.000000 cdk-simplewebsite-deploy-2.0.8/src/cdk_simplewebsite_deploy/_jsii/cdk-simplewebsite-deploy@2.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 00:47:36.000000 cdk-simplewebsite-deploy-2.0.8/src/cdk_simplewebsite_deploy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 00:47:50.696991 cdk-simplewebsite-deploy-2.0.8/src/cdk_simplewebsite_deploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7269 2022-02-04 00:47:50.000000 cdk-simplewebsite-deploy-2.0.8/src/cdk_simplewebsite_deploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      513 2022-02-04 00:47:50.000000 cdk-simplewebsite-deploy-2.0.8/src/cdk_simplewebsite_deploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 00:47:50.000000 cdk-simplewebsite-deploy-2.0.8/src/cdk_simplewebsite_deploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 00:47:50.000000 cdk-simplewebsite-deploy-2.0.8/src/cdk_simplewebsite_deploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-02-04 00:47:50.000000 cdk-simplewebsite-deploy-2.0.8/src/cdk_simplewebsite_deploy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 00:42:55.218831 cdk-simplewebsite-deploy-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-02-13 00:42:37.000000 cdk-simplewebsite-deploy-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-02-13 00:42:37.000000 cdk-simplewebsite-deploy-2.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     7269 2022-02-13 00:42:55.218831 cdk-simplewebsite-deploy-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6263 2022-02-13 00:42:37.000000 cdk-simplewebsite-deploy-2.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-02-13 00:42:37.000000 cdk-simplewebsite-deploy-2.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-13 00:42:55.218831 cdk-simplewebsite-deploy-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-02-13 00:42:37.000000 cdk-simplewebsite-deploy-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 00:42:55.214831 cdk-simplewebsite-deploy-2.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 00:42:55.214831 cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy/
+-rw-r--r--   0 runner    (1001) docker     (121)    17904 2022-02-13 00:42:37.000000 cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 00:42:55.218831 cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      394 2022-02-13 00:42:37.000000 cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23921 2022-02-13 00:42:37.000000 cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy/_jsii/cdk-simplewebsite-deploy@2.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-13 00:42:37.000000 cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 00:42:55.218831 cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7269 2022-02-13 00:42:54.000000 cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      513 2022-02-13 00:42:55.000000 cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-13 00:42:54.000000 cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-13 00:42:54.000000 cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-02-13 00:42:54.000000 cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy.egg-info/top_level.txt
```

### Comparing `cdk-simplewebsite-deploy-2.0.8/LICENSE` & `cdk-simplewebsite-deploy-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-simplewebsite-deploy-2.0.8/PKG-INFO` & `cdk-simplewebsite-deploy-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-simplewebsite-deploy
-Version: 2.0.8
+Version: 2.0.9
 Summary: This is an AWS CDK v2 Construct to simplify deploying a single-page website use CloudFront distributions.
 Home-page: https://github.com/SnapPetal/cdk-simplewebsite-deploy
 Author: Thon Becker<thon.becker@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/SnapPetal/cdk-simplewebsite-deploy
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk-simplewebsite-deploy-2.0.8/README.md` & `cdk-simplewebsite-deploy-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cdk-simplewebsite-deploy-2.0.8/setup.py` & `cdk-simplewebsite-deploy-2.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-simplewebsite-deploy",
-    "version": "2.0.8",
+    "version": "2.0.9",
     "description": "This is an AWS CDK v2 Construct to simplify deploying a single-page website use CloudFront distributions.",
     "license": "Apache-2.0",
     "url": "https://github.com/SnapPetal/cdk-simplewebsite-deploy",
     "long_description_content_type": "text/markdown",
     "author": "Thon Becker<thon.becker@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdk_simplewebsite_deploy",
         "cdk_simplewebsite_deploy._jsii"
     ],
     "package_data": {
         "cdk_simplewebsite_deploy._jsii": [
-            "cdk-simplewebsite-deploy@2.0.8.jsii.tgz"
+            "cdk-simplewebsite-deploy@2.0.9.jsii.tgz"
         ],
         "cdk_simplewebsite_deploy": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
-        "aws-cdk-lib>=2.10.0, <3.0.0",
-        "constructs>=10.0.52, <11.0.0",
-        "jsii>=1.52.1, <2.0.0",
+        "aws-cdk-lib>=2.12.0, <3.0.0",
+        "constructs>=10.0.61, <11.0.0",
+        "jsii>=1.53.0, <2.0.0",
         "publication>=0.0.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `cdk-simplewebsite-deploy-2.0.8/src/cdk_simplewebsite_deploy/__init__.py` & `cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-simplewebsite-deploy-2.0.8/src/cdk_simplewebsite_deploy.egg-info/PKG-INFO` & `cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-simplewebsite-deploy
-Version: 2.0.8
+Version: 2.0.9
 Summary: This is an AWS CDK v2 Construct to simplify deploying a single-page website use CloudFront distributions.
 Home-page: https://github.com/SnapPetal/cdk-simplewebsite-deploy
 Author: Thon Becker<thon.becker@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/SnapPetal/cdk-simplewebsite-deploy
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk-simplewebsite-deploy-2.0.8/src/cdk_simplewebsite_deploy.egg-info/SOURCES.txt` & `cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cdk_simplewebsite_deploy/py.typed
 src/cdk_simplewebsite_deploy.egg-info/PKG-INFO
 src/cdk_simplewebsite_deploy.egg-info/SOURCES.txt
 src/cdk_simplewebsite_deploy.egg-info/dependency_links.txt
 src/cdk_simplewebsite_deploy.egg-info/requires.txt
 src/cdk_simplewebsite_deploy.egg-info/top_level.txt
 src/cdk_simplewebsite_deploy/_jsii/__init__.py
-src/cdk_simplewebsite_deploy/_jsii/cdk-simplewebsite-deploy@2.0.8.jsii.tgz
+src/cdk_simplewebsite_deploy/_jsii/cdk-simplewebsite-deploy@2.0.9.jsii.tgz
```

