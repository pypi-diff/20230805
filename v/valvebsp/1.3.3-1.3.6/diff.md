# Comparing `tmp/valvebsp-1.3.3.tar.gz` & `tmp/valvebsp-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valvebsp-1.3.3.tar", last modified: Sat Aug  5 00:17:52 2023, max compression
+gzip compressed data, was "valvebsp-1.3.6.tar", last modified: Sat Aug  5 00:54:39 2023, max compression
```

## Comparing `valvebsp-1.3.3.tar` & `valvebsp-1.3.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:17:52.641466 valvebsp-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-05 00:17:43.000000 valvebsp-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-08-05 00:17:52.641466 valvebsp-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-08-05 00:17:43.000000 valvebsp-1.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 00:17:52.641466 valvebsp-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-08-05 00:17:50.000000 valvebsp-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:17:52.641466 valvebsp-1.3.3/valvebsp/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-05 00:17:43.000000 valvebsp-1.3.3/valvebsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-08-05 00:17:43.000000 valvebsp-1.3.3/valvebsp/bsp.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-05 00:17:43.000000 valvebsp-1.3.3/valvebsp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-05 00:17:43.000000 valvebsp-1.3.3/valvebsp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-08-05 00:17:43.000000 valvebsp-1.3.3/valvebsp/lumps.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-08-05 00:17:43.000000 valvebsp-1.3.3/valvebsp/profiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:17:52.641466 valvebsp-1.3.3/valvebsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-08-05 00:17:52.000000 valvebsp-1.3.3/valvebsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-08-05 00:17:52.000000 valvebsp-1.3.3/valvebsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 00:17:52.000000 valvebsp-1.3.3/valvebsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-05 00:17:52.000000 valvebsp-1.3.3/valvebsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 00:17:52.000000 valvebsp-1.3.3/valvebsp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:54:39.903559 valvebsp-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-05 00:54:31.000000 valvebsp-1.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-08-05 00:54:39.903559 valvebsp-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-08-05 00:54:31.000000 valvebsp-1.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 00:54:39.903559 valvebsp-1.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-08-05 00:54:39.000000 valvebsp-1.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:54:39.903559 valvebsp-1.3.6/valvebsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-05 00:54:31.000000 valvebsp-1.3.6/valvebsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-08-05 00:54:31.000000 valvebsp-1.3.6/valvebsp/bsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-05 00:54:31.000000 valvebsp-1.3.6/valvebsp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-05 00:54:31.000000 valvebsp-1.3.6/valvebsp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-08-05 00:54:31.000000 valvebsp-1.3.6/valvebsp/lumps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-08-05 00:54:31.000000 valvebsp-1.3.6/valvebsp/profiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:54:39.903559 valvebsp-1.3.6/valvebsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-08-05 00:54:39.000000 valvebsp-1.3.6/valvebsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-08-05 00:54:39.000000 valvebsp-1.3.6/valvebsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 00:54:39.000000 valvebsp-1.3.6/valvebsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-05 00:54:39.000000 valvebsp-1.3.6/valvebsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 00:54:39.000000 valvebsp-1.3.6/valvebsp.egg-info/top_level.txt
```

### Comparing `valvebsp-1.3.3/LICENSE` & `valvebsp-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `valvebsp-1.3.3/PKG-INFO` & `valvebsp-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valvebsp
-Version: 1.3.3
+Version: 1.3.6
 Summary: A library to parse .BSP files (level files for the Source engine).
 Home-page: https://pysourcesdk.github.io/ValveBSP/
 Author: Maxime Dupuis
 Author-email: mdupuis@hotmail.ca
 License: gpl-3.0
 Project-URL: Documentation, https://pysourcesdk.github.io/ValveBSP/
 Project-URL: Github, https://github.com/pySourceSDK/ValveBSP
```

### Comparing `valvebsp-1.3.3/README.md` & `valvebsp-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `valvebsp-1.3.3/setup.py` & `valvebsp-1.3.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import re
 
 with open('README.md') as f:
     re_omit = r'<!--- start pypi omit -->.*<!--- end pypi omit -->'
     long_description = re.sub(re_omit, '', f.read(), flags=re.S)
 
-VERSION = 'v1.3.3'
+VERSION = 'v1.3.6'
 if 'VERSION_PLACEHOLDER' in VERSION:
     VERSION = '0.0.0'
 
 setup(
     name='valvebsp',
     packages=['valvebsp'],
     version=VERSION,
```

### Comparing `valvebsp-1.3.3/valvebsp/bsp.py` & `valvebsp-1.3.6/valvebsp/bsp.py`

 * *Files identical despite different names*

### Comparing `valvebsp-1.3.3/valvebsp/constants.py` & `valvebsp-1.3.6/valvebsp/constants.py`

 * *Files identical despite different names*

### Comparing `valvebsp-1.3.3/valvebsp/lumps.py` & `valvebsp-1.3.6/valvebsp/lumps.py`

 * *Files identical despite different names*

### Comparing `valvebsp-1.3.3/valvebsp/profiles.py` & `valvebsp-1.3.6/valvebsp/profiles.py`

 * *Files identical despite different names*

### Comparing `valvebsp-1.3.3/valvebsp.egg-info/PKG-INFO` & `valvebsp-1.3.6/valvebsp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valvebsp
-Version: 1.3.3
+Version: 1.3.6
 Summary: A library to parse .BSP files (level files for the Source engine).
 Home-page: https://pysourcesdk.github.io/ValveBSP/
 Author: Maxime Dupuis
 Author-email: mdupuis@hotmail.ca
 License: gpl-3.0
 Project-URL: Documentation, https://pysourcesdk.github.io/ValveBSP/
 Project-URL: Github, https://github.com/pySourceSDK/ValveBSP
```

