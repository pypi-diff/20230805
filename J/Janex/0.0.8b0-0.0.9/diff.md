# Comparing `tmp/Janex-0.0.8b0.tar.gz` & `tmp/Janex-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Janex-0.0.8b0.tar", last modified: Tue Jul 18 02:08:44 2023, max compression
+gzip compressed data, was "Janex-0.0.9.tar", last modified: Tue Jul 18 02:13:50 2023, max compression
```

## Comparing `Janex-0.0.8b0.tar` & `Janex-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-07-18 02:08:44.497804 Janex-0.0.8b0/
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-07-18 02:08:44.497804 Janex-0.0.8b0/Janex/
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-07-18 02:08:44.497804 Janex-0.0.8b0/Janex/JanexSub/
--rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-07-09 22:55:43.000000 Janex-0.0.8b0/Janex/JanexSub/JanexSub.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-07-09 22:55:43.000000 Janex-0.0.8b0/Janex/JanexSub/__init__.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-07-17 23:57:36.000000 Janex-0.0.8b0/Janex/__init__.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)      260 2023-07-09 22:55:43.000000 Janex-0.0.8b0/Janex/chat.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)     5408 2023-07-18 01:59:26.000000 Janex-0.0.8b0/Janex/main.py
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-07-18 02:08:44.497804 Janex-0.0.8b0/Janex.egg-info/
--rw-r--r--   0 cipher    (1000) cipher    (1000)     3429 2023-07-18 02:08:44.000000 Janex-0.0.8b0/Janex.egg-info/PKG-INFO
--rw-r--r--   0 cipher    (1000) cipher    (1000)      270 2023-07-18 02:08:44.000000 Janex-0.0.8b0/Janex.egg-info/SOURCES.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)        1 2023-07-18 02:08:44.000000 Janex-0.0.8b0/Janex.egg-info/dependency_links.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)       12 2023-07-18 02:08:44.000000 Janex-0.0.8b0/Janex.egg-info/requires.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)        6 2023-07-18 02:08:44.000000 Janex-0.0.8b0/Janex.egg-info/top_level.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)     2950 2023-06-30 13:17:04.000000 Janex-0.0.8b0/LICENSE
--rw-r--r--   0 cipher    (1000) cipher    (1000)     3429 2023-07-18 02:08:44.497804 Janex-0.0.8b0/PKG-INFO
--rw-r--r--   0 cipher    (1000) cipher    (1000)     3022 2023-07-18 00:12:10.000000 Janex-0.0.8b0/README.md
--rw-r--r--   0 cipher    (1000) cipher    (1000)       38 2023-07-18 02:08:44.497804 Janex-0.0.8b0/setup.cfg
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1321 2023-07-18 02:08:42.000000 Janex-0.0.8b0/setup.py
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-07-18 02:13:50.047318 Janex-0.0.9/
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-07-18 02:13:50.047318 Janex-0.0.9/Janex/
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-07-18 02:13:50.047318 Janex-0.0.9/Janex/JanexSub/
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-07-09 22:55:43.000000 Janex-0.0.9/Janex/JanexSub/JanexSub.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-07-09 22:55:43.000000 Janex-0.0.9/Janex/JanexSub/__init__.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-07-17 23:57:36.000000 Janex-0.0.9/Janex/__init__.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      260 2023-07-09 22:55:43.000000 Janex-0.0.9/Janex/chat.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     5408 2023-07-18 01:59:26.000000 Janex-0.0.9/Janex/main.py
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-07-18 02:13:50.047318 Janex-0.0.9/Janex.egg-info/
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     3427 2023-07-18 02:13:49.000000 Janex-0.0.9/Janex.egg-info/PKG-INFO
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      270 2023-07-18 02:13:50.000000 Janex-0.0.9/Janex.egg-info/SOURCES.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        1 2023-07-18 02:13:49.000000 Janex-0.0.9/Janex.egg-info/dependency_links.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       12 2023-07-18 02:13:49.000000 Janex-0.0.9/Janex.egg-info/requires.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        6 2023-07-18 02:13:49.000000 Janex-0.0.9/Janex.egg-info/top_level.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     2950 2023-06-30 13:17:04.000000 Janex-0.0.9/LICENSE
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     3427 2023-07-18 02:13:50.047318 Janex-0.0.9/PKG-INFO
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     3022 2023-07-18 00:12:10.000000 Janex-0.0.9/README.md
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       38 2023-07-18 02:13:50.047318 Janex-0.0.9/setup.cfg
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1319 2023-07-18 02:13:11.000000 Janex-0.0.9/setup.py
```

### Comparing `Janex-0.0.8b0/Janex/main.py` & `Janex-0.0.9/Janex/main.py`

 * *Files identical despite different names*

### Comparing `Janex-0.0.8b0/Janex.egg-info/PKG-INFO` & `Janex-0.0.9/Janex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Janex
-Version: 0.0.8b0
+Version: 0.0.9
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Janex/archive/refs/tags/v0.0.2-beta.tar.gz
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `Janex-0.0.8b0/LICENSE` & `Janex-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Janex-0.0.8b0/PKG-INFO` & `Janex-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Janex
-Version: 0.0.8b0
+Version: 0.0.9
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Janex/archive/refs/tags/v0.0.2-beta.tar.gz
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `Janex-0.0.8b0/README.md` & `Janex-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `Janex-0.0.8b0/setup.py` & `Janex-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="Janex",
 
     # version of the module
-    version="0.0.8b0",
+    version="0.0.9",
 
     # Name of Author
     author="Cipher58",
 
     download_url = 'https://github.com/Cipher58/Janex/archive/refs/tags/v0.0.2-beta.tar.gz',
 
     # your Email address
```

