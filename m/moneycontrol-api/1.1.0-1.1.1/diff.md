# Comparing `tmp/moneycontrol_api-1.1.0.tar.gz` & `tmp/moneycontrol_api-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneycontrol_api-1.1.0.tar", last modified: Sat Aug  5 14:22:26 2023, max compression
+gzip compressed data, was "moneycontrol_api-1.1.1.tar", last modified: Sat Aug  5 14:39:21 2023, max compression
```

## Comparing `moneycontrol_api-1.1.0.tar` & `moneycontrol_api-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:22:26.933150 moneycontrol_api-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-08-05 14:22:15.000000 moneycontrol_api-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-05 14:22:26.933150 moneycontrol_api-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-05 14:22:15.000000 moneycontrol_api-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-05 14:22:15.000000 moneycontrol_api-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 14:22:26.933150 moneycontrol_api-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:22:26.933150 moneycontrol_api-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:22:26.933150 moneycontrol_api-1.1.0/src/moneycontrol/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-05 14:22:15.000000 moneycontrol_api-1.1.0/src/moneycontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-08-05 14:22:15.000000 moneycontrol_api-1.1.0/src/moneycontrol/moneycontrol_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:22:26.933150 moneycontrol_api-1.1.0/src/moneycontrol_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-05 14:22:26.000000 moneycontrol_api-1.1.0/src/moneycontrol_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-05 14:22:26.000000 moneycontrol_api-1.1.0/src/moneycontrol_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 14:22:26.000000 moneycontrol_api-1.1.0/src/moneycontrol_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-05 14:22:26.000000 moneycontrol_api-1.1.0/src/moneycontrol_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:39:21.552104 moneycontrol_api-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-08-05 14:39:05.000000 moneycontrol_api-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-05 14:39:21.552104 moneycontrol_api-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-05 14:39:05.000000 moneycontrol_api-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-05 14:39:05.000000 moneycontrol_api-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 14:39:21.552104 moneycontrol_api-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:39:21.548103 moneycontrol_api-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:39:21.552104 moneycontrol_api-1.1.1/src/moneycontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-05 14:39:05.000000 moneycontrol_api-1.1.1/src/moneycontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-08-05 14:39:05.000000 moneycontrol_api-1.1.1/src/moneycontrol/moneycontrol_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:39:21.552104 moneycontrol_api-1.1.1/src/moneycontrol_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-05 14:39:21.000000 moneycontrol_api-1.1.1/src/moneycontrol_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-05 14:39:21.000000 moneycontrol_api-1.1.1/src/moneycontrol_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 14:39:21.000000 moneycontrol_api-1.1.1/src/moneycontrol_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-05 14:39:21.000000 moneycontrol_api-1.1.1/src/moneycontrol_api.egg-info/top_level.txt
```

### Comparing `moneycontrol_api-1.1.0/LICENSE` & `moneycontrol_api-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `moneycontrol_api-1.1.0/PKG-INFO` & `moneycontrol_api-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneycontrol_api
-Version: 1.1.0
+Version: 1.1.1
 Summary: Moneycontrol API is a python library to get news data from moneycontrol.com in JSON format.
 Author-email: Arabian Coconut <x48cl9zm@duck.com>
 Project-URL: Homepage, https://github.com/ArabianCoconut/Moneycontrol-api
 Project-URL: Live Demo, https://mc-api-j0rn.onrender.com
 Keywords: moneycontrol api,moneycontrol
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # MoneyControl Api
 ### Status of project: **Complete**
 #### Author: Arabian Coconut
-#### Version: 1.0.0
+#### Version: 1.1.1
 
 ---
 ## Description
 
 This is a python API for moneycontrol.com, which provides you with the news, latest news, and 
 business news from moneycontrol.com in JSON format for your server's integration.
```

### Comparing `moneycontrol_api-1.1.0/README.md` & `moneycontrol_api-1.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 # MoneyControl Api
 ### Status of project: **Complete**
 #### Author: Arabian Coconut
-#### Version: 1.0.0
+#### Version: 1.1.1
 
 ---
 ## Description
 
 This is a python API for moneycontrol.com, which provides you with the news, latest news, and 
 business news from moneycontrol.com in JSON format for your server's integration.
```

### Comparing `moneycontrol_api-1.1.0/pyproject.toml` & `moneycontrol_api-1.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moneycontrol_api"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Arabian Coconut", email="x48cl9zm@duck.com" },
 ]
 description = "Moneycontrol API is a python library to get news data from moneycontrol.com in JSON format."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `moneycontrol_api-1.1.0/src/moneycontrol/moneycontrol_api.py` & `moneycontrol_api-1.1.1/src/moneycontrol/moneycontrol_api.py`

 * *Files identical despite different names*

### Comparing `moneycontrol_api-1.1.0/src/moneycontrol_api.egg-info/PKG-INFO` & `moneycontrol_api-1.1.1/src/moneycontrol_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneycontrol-api
-Version: 1.1.0
+Version: 1.1.1
 Summary: Moneycontrol API is a python library to get news data from moneycontrol.com in JSON format.
 Author-email: Arabian Coconut <x48cl9zm@duck.com>
 Project-URL: Homepage, https://github.com/ArabianCoconut/Moneycontrol-api
 Project-URL: Live Demo, https://mc-api-j0rn.onrender.com
 Keywords: moneycontrol api,moneycontrol
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # MoneyControl Api
 ### Status of project: **Complete**
 #### Author: Arabian Coconut
-#### Version: 1.0.0
+#### Version: 1.1.1
 
 ---
 ## Description
 
 This is a python API for moneycontrol.com, which provides you with the news, latest news, and 
 business news from moneycontrol.com in JSON format for your server's integration.
```

