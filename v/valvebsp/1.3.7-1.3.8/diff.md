# Comparing `tmp/valvebsp-1.3.7.tar.gz` & `tmp/valvebsp-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valvebsp-1.3.7.tar", last modified: Sat Aug  5 01:00:41 2023, max compression
+gzip compressed data, was "valvebsp-1.3.8.tar", last modified: Sat Aug  5 01:06:04 2023, max compression
```

## Comparing `valvebsp-1.3.7.tar` & `valvebsp-1.3.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:00:41.886959 valvebsp-1.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-05 01:00:32.000000 valvebsp-1.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-08-05 01:00:41.886959 valvebsp-1.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-08-05 01:00:32.000000 valvebsp-1.3.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 01:00:41.886959 valvebsp-1.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-08-05 01:00:41.000000 valvebsp-1.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:00:41.886959 valvebsp-1.3.7/valvebsp/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-05 01:00:32.000000 valvebsp-1.3.7/valvebsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-08-05 01:00:32.000000 valvebsp-1.3.7/valvebsp/bsp.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-05 01:00:32.000000 valvebsp-1.3.7/valvebsp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-05 01:00:32.000000 valvebsp-1.3.7/valvebsp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-08-05 01:00:32.000000 valvebsp-1.3.7/valvebsp/lumps.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-08-05 01:00:32.000000 valvebsp-1.3.7/valvebsp/profiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:00:41.886959 valvebsp-1.3.7/valvebsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-08-05 01:00:41.000000 valvebsp-1.3.7/valvebsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-08-05 01:00:41.000000 valvebsp-1.3.7/valvebsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 01:00:41.000000 valvebsp-1.3.7/valvebsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-05 01:00:41.000000 valvebsp-1.3.7/valvebsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 01:00:41.000000 valvebsp-1.3.7/valvebsp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:06:04.959962 valvebsp-1.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-05 01:05:52.000000 valvebsp-1.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-08-05 01:06:04.959962 valvebsp-1.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-08-05 01:05:52.000000 valvebsp-1.3.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 01:06:04.959962 valvebsp-1.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-08-05 01:06:03.000000 valvebsp-1.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:06:04.959962 valvebsp-1.3.8/valvebsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-05 01:05:52.000000 valvebsp-1.3.8/valvebsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-08-05 01:05:52.000000 valvebsp-1.3.8/valvebsp/bsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-05 01:05:52.000000 valvebsp-1.3.8/valvebsp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-05 01:05:52.000000 valvebsp-1.3.8/valvebsp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-08-05 01:05:52.000000 valvebsp-1.3.8/valvebsp/lumps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-08-05 01:05:52.000000 valvebsp-1.3.8/valvebsp/profiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:06:04.959962 valvebsp-1.3.8/valvebsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-08-05 01:06:04.000000 valvebsp-1.3.8/valvebsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-08-05 01:06:04.000000 valvebsp-1.3.8/valvebsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 01:06:04.000000 valvebsp-1.3.8/valvebsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-05 01:06:04.000000 valvebsp-1.3.8/valvebsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 01:06:04.000000 valvebsp-1.3.8/valvebsp.egg-info/top_level.txt
```

### Comparing `valvebsp-1.3.7/LICENSE` & `valvebsp-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `valvebsp-1.3.7/PKG-INFO` & `valvebsp-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valvebsp
-Version: 1.3.7
+Version: 1.3.8
 Summary: A library to parse .BSP files (level files for the Source engine).
 Home-page: https://pysourcesdk.github.io/ValveBSP/
 Author: Maxime Dupuis
 Author-email: mdupuis@hotmail.ca
 License: gpl-3.0
 Project-URL: Documentation, https://pysourcesdk.github.io/ValveBSP/
 Project-URL: Github, https://github.com/pySourceSDK/ValveBSP
```

### Comparing `valvebsp-1.3.7/README.md` & `valvebsp-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `valvebsp-1.3.7/setup.py` & `valvebsp-1.3.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import re
 
 with open('README.md') as f:
     re_omit = r'<!--- start pypi omit -->.*<!--- end pypi omit -->'
     long_description = re.sub(re_omit, '', f.read(), flags=re.S)
 
-VERSION = 'v1.3.7'
+VERSION = 'v1.3.8'
 if 'VERSION_PLACEHOLDER' in VERSION:
     VERSION = '0.0.0'
 
 setup(
     name='valvebsp',
     packages=['valvebsp'],
     version=VERSION,
```

### Comparing `valvebsp-1.3.7/valvebsp/bsp.py` & `valvebsp-1.3.8/valvebsp/bsp.py`

 * *Files identical despite different names*

### Comparing `valvebsp-1.3.7/valvebsp/constants.py` & `valvebsp-1.3.8/valvebsp/constants.py`

 * *Files identical despite different names*

### Comparing `valvebsp-1.3.7/valvebsp/lumps.py` & `valvebsp-1.3.8/valvebsp/lumps.py`

 * *Files identical despite different names*

### Comparing `valvebsp-1.3.7/valvebsp/profiles.py` & `valvebsp-1.3.8/valvebsp/profiles.py`

 * *Files identical despite different names*

### Comparing `valvebsp-1.3.7/valvebsp.egg-info/PKG-INFO` & `valvebsp-1.3.8/valvebsp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valvebsp
-Version: 1.3.7
+Version: 1.3.8
 Summary: A library to parse .BSP files (level files for the Source engine).
 Home-page: https://pysourcesdk.github.io/ValveBSP/
 Author: Maxime Dupuis
 Author-email: mdupuis@hotmail.ca
 License: gpl-3.0
 Project-URL: Documentation, https://pysourcesdk.github.io/ValveBSP/
 Project-URL: Github, https://github.com/pySourceSDK/ValveBSP
```

