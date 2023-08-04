# Comparing `tmp/aissistant-0.2.tar.gz` & `tmp/aissistant-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissistant-0.2.tar", last modified: Fri Aug  4 23:22:57 2023, max compression
+gzip compressed data, was "aissistant-0.3.tar", last modified: Fri Aug  4 23:47:25 2023, max compression
```

## Comparing `aissistant-0.2.tar` & `aissistant-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 23:22:57.190468 aissistant-0.2/
--rw-rw-rw-   0        0        0     1092 2023-08-03 13:17:02.000000 aissistant-0.2/LICENSE
--rw-rw-rw-   0        0        0       57 2023-08-04 13:30:15.000000 aissistant-0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6597 2023-08-04 23:22:57.190468 aissistant-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-08-04 13:30:20.000000 aissistant-0.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-08-04 23:22:57.182476 aissistant-0.2/aissistant.egg-info/
--rw-rw-rw-   0        0        0     6597 2023-08-04 23:22:57.000000 aissistant-0.2/aissistant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-08-04 23:22:57.000000 aissistant-0.2/aissistant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 23:22:57.000000 aissistant-0.2/aissistant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-08-04 23:22:57.000000 aissistant-0.2/aissistant.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       38 2023-08-04 23:22:57.000000 aissistant-0.2/aissistant.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 23:22:57.000000 aissistant-0.2/aissistant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 23:22:57.190468 aissistant-0.2/setup.cfg
--rw-rw-rw-   0        0        0     7559 2023-08-04 23:22:28.000000 aissistant-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 23:22:57.190468 aissistant-0.2/tests/
--rw-rw-rw-   0        0        0      495 2023-08-04 13:33:39.000000 aissistant-0.2/tests/test_aissistant.py
+drwxrwxrwx   0        0        0        0 2023-08-04 23:47:25.361657 aissistant-0.3/
+-rw-rw-rw-   0        0        0     1092 2023-08-03 13:17:02.000000 aissistant-0.3/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-08-04 13:30:15.000000 aissistant-0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6597 2023-08-04 23:47:25.359664 aissistant-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-08-04 13:30:20.000000 aissistant-0.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-04 23:47:25.354660 aissistant-0.3/aissistant.egg-info/
+-rw-rw-rw-   0        0        0     6597 2023-08-04 23:47:25.000000 aissistant-0.3/aissistant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-08-04 23:47:25.000000 aissistant-0.3/aissistant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 23:47:25.000000 aissistant-0.3/aissistant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-08-04 23:47:25.000000 aissistant-0.3/aissistant.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       38 2023-08-04 23:47:25.000000 aissistant-0.3/aissistant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 23:47:25.000000 aissistant-0.3/aissistant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 23:47:25.362658 aissistant-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     7559 2023-08-04 23:46:59.000000 aissistant-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 23:47:25.357657 aissistant-0.3/tests/
+-rw-rw-rw-   0        0        0      495 2023-08-04 13:33:39.000000 aissistant-0.3/tests/test_aissistant.py
```

### Comparing `aissistant-0.2/LICENSE` & `aissistant-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aissistant-0.2/PKG-INFO` & `aissistant-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: aissistant
-Version: 0.2
-Summary: Aissistant v0.2
+Version: 0.3
+Summary: Aissistant v0.3
 Home-page: https://github.com/markomanninen/aissistant
 Author: Marko Manninen
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# Aissistant v0.2
+# Aissistant v0.3
 
 Initialization prompt for persistent conversation vector database and personal profile in ChatGPT using Noteable plugin and `aissistant` module written by Marko T. Manninen ([https://github.com/markomanninen/aissistant/](https://github.com/markomanninen/aissistant/)) ©
 
 Copyright © 08/2023.
 
 Get creative and productive with this initialization script in ChatGPT that utilizes the Noteable plugin. Natively, you can create, edit, and run code and generate data within notebooks as well as in ChatGPT interchangeably, back and forth. By using this initialization prompt, you can use the combined environment to store data and explore past conversations, as well as manage profile information for a more intelligent chat and coding experience.
```

### Comparing `aissistant-0.2/README.rst` & `aissistant-0.3/README.rst`

 * *Files identical despite different names*

### Comparing `aissistant-0.2/aissistant.egg-info/PKG-INFO` & `aissistant-0.3/aissistant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: aissistant
-Version: 0.2
-Summary: Aissistant v0.2
+Version: 0.3
+Summary: Aissistant v0.3
 Home-page: https://github.com/markomanninen/aissistant
 Author: Marko Manninen
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# Aissistant v0.2
+# Aissistant v0.3
 
 Initialization prompt for persistent conversation vector database and personal profile in ChatGPT using Noteable plugin and `aissistant` module written by Marko T. Manninen ([https://github.com/markomanninen/aissistant/](https://github.com/markomanninen/aissistant/)) ©
 
 Copyright © 08/2023.
 
 Get creative and productive with this initialization script in ChatGPT that utilizes the Noteable plugin. Natively, you can create, edit, and run code and generate data within notebooks as well as in ChatGPT interchangeably, back and forth. By using this initialization prompt, you can use the combined environment to store data and explore past conversations, as well as manage profile information for a more intelligent chat and coding experience.
```

### Comparing `aissistant-0.2/setup.py` & `aissistant-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
-version = 0.2
+version = 0.3
 
 class PostInstallCommand(install):
     def run(self):
         install.run(self)
         print("\n\nWelcome to aissistant!")
         print("For usage tips and help, you can call `help(aissistant)` or access `aissistant.__doc__`, and `dir(aissistant)` to see the functions and `help(any_function)` after importing the module.")
         print("\nEnjoy!\n")
```

