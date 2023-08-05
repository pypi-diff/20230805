# Comparing `tmp/aissistant-0.3.tar.gz` & `tmp/aissistant-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissistant-0.3.tar", last modified: Fri Aug  4 23:47:25 2023, max compression
+gzip compressed data, was "aissistant-0.4.tar", last modified: Sat Aug  5 00:08:15 2023, max compression
```

## Comparing `aissistant-0.3.tar` & `aissistant-0.4.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 23:47:25.361657 aissistant-0.3/
--rw-rw-rw-   0        0        0     1092 2023-08-03 13:17:02.000000 aissistant-0.3/LICENSE
--rw-rw-rw-   0        0        0       57 2023-08-04 13:30:15.000000 aissistant-0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6597 2023-08-04 23:47:25.359664 aissistant-0.3/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-08-04 13:30:20.000000 aissistant-0.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-08-04 23:47:25.354660 aissistant-0.3/aissistant.egg-info/
--rw-rw-rw-   0        0        0     6597 2023-08-04 23:47:25.000000 aissistant-0.3/aissistant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-08-04 23:47:25.000000 aissistant-0.3/aissistant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 23:47:25.000000 aissistant-0.3/aissistant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-08-04 23:47:25.000000 aissistant-0.3/aissistant.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       38 2023-08-04 23:47:25.000000 aissistant-0.3/aissistant.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 23:47:25.000000 aissistant-0.3/aissistant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 23:47:25.362658 aissistant-0.3/setup.cfg
--rw-rw-rw-   0        0        0     7559 2023-08-04 23:46:59.000000 aissistant-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 23:47:25.357657 aissistant-0.3/tests/
--rw-rw-rw-   0        0        0      495 2023-08-04 13:33:39.000000 aissistant-0.3/tests/test_aissistant.py
+drwxrwxrwx   0        0        0        0 2023-08-05 00:08:15.746001 aissistant-0.4/
+-rw-rw-rw-   0        0        0     1092 2023-08-03 13:17:02.000000 aissistant-0.4/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-08-04 13:30:15.000000 aissistant-0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6639 2023-08-05 00:08:15.746001 aissistant-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-08-04 13:30:20.000000 aissistant-0.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-05 00:08:15.732000 aissistant-0.4/aissistant/
+-rw-rw-rw-   0        0        0        0 2023-08-05 00:03:48.000000 aissistant-0.4/aissistant/__init__.py
+-rw-rw-rw-   0        0        0    23706 2023-08-04 23:35:34.000000 aissistant-0.4/aissistant/aissistant.py
+drwxrwxrwx   0        0        0        0 2023-08-05 00:08:15.741999 aissistant-0.4/aissistant.egg-info/
+-rw-rw-rw-   0        0        0     6639 2023-08-05 00:08:15.000000 aissistant-0.4/aissistant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-08-05 00:08:15.000000 aissistant-0.4/aissistant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 00:08:15.000000 aissistant-0.4/aissistant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-08-05 00:08:15.000000 aissistant-0.4/aissistant.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       62 2023-08-05 00:08:15.000000 aissistant-0.4/aissistant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-05 00:08:15.000000 aissistant-0.4/aissistant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 00:08:15.747000 aissistant-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     7642 2023-08-05 00:07:06.000000 aissistant-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 00:08:15.743999 aissistant-0.4/tests/
+-rw-rw-rw-   0        0        0      495 2023-08-04 13:33:39.000000 aissistant-0.4/tests/test_aissistant.py
```

### Comparing `aissistant-0.3/LICENSE` & `aissistant-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aissistant-0.3/PKG-INFO` & `aissistant-0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: aissistant
-Version: 0.3
-Summary: Aissistant v0.3
+Version: 0.4
+Summary: Aissistant v0.4
 Home-page: https://github.com/markomanninen/aissistant
 Author: Marko Manninen
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+Provides-Extra: gpu
+Provides-Extra: cpu
 License-File: LICENSE
 
 
-# Aissistant v0.3
+# Aissistant v0.4
 
 Initialization prompt for persistent conversation vector database and personal profile in ChatGPT using Noteable plugin and `aissistant` module written by Marko T. Manninen ([https://github.com/markomanninen/aissistant/](https://github.com/markomanninen/aissistant/)) ©
 
 Copyright © 08/2023.
 
 Get creative and productive with this initialization script in ChatGPT that utilizes the Noteable plugin. Natively, you can create, edit, and run code and generate data within notebooks as well as in ChatGPT interchangeably, back and forth. By using this initialization prompt, you can use the combined environment to store data and explore past conversations, as well as manage profile information for a more intelligent chat and coding experience.
```

### Comparing `aissistant-0.3/README.rst` & `aissistant-0.4/README.rst`

 * *Files identical despite different names*

### Comparing `aissistant-0.3/aissistant.egg-info/PKG-INFO` & `aissistant-0.4/aissistant.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: aissistant
-Version: 0.3
-Summary: Aissistant v0.3
+Version: 0.4
+Summary: Aissistant v0.4
 Home-page: https://github.com/markomanninen/aissistant
 Author: Marko Manninen
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+Provides-Extra: gpu
+Provides-Extra: cpu
 License-File: LICENSE
 
 
-# Aissistant v0.3
+# Aissistant v0.4
 
 Initialization prompt for persistent conversation vector database and personal profile in ChatGPT using Noteable plugin and `aissistant` module written by Marko T. Manninen ([https://github.com/markomanninen/aissistant/](https://github.com/markomanninen/aissistant/)) ©
 
 Copyright © 08/2023.
 
 Get creative and productive with this initialization script in ChatGPT that utilizes the Noteable plugin. Natively, you can create, edit, and run code and generate data within notebooks as well as in ChatGPT interchangeably, back and forth. By using this initialization prompt, you can use the combined environment to store data and explore past conversations, as well as manage profile information for a more intelligent chat and coding experience.
```

### Comparing `aissistant-0.3/setup.py` & `aissistant-0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
-version = 0.3
+version = 0.4
 
 class PostInstallCommand(install):
     def run(self):
         install.run(self)
         print("\n\nWelcome to aissistant!")
         print("For usage tips and help, you can call `help(aissistant)` or access `aissistant.__doc__`, and `dir(aissistant)` to see the functions and `help(any_function)` after importing the module.")
         print("\nEnjoy!\n")
@@ -117,24 +117,27 @@
 
 Along the way interacting with the user, ChatGPT, and Noteable notebook document, write headings and descriptions of the operations in markdown format to the notebook above each executed cell in a human-readable way.
 """
 
 setup(
     name='aissistant',
     version=version,
-	cmdclass={'install': PostInstallCommand},
+    cmdclass={'install': PostInstallCommand},
     packages=find_packages(),
     install_requires=[
-        'faiss-gpu',
         'sentence-transformers',
         'numpy',
     ],
+    extras_require={
+        'gpu': ['faiss-gpu'],
+        'cpu': ['faiss-cpu'],
+    },
     entry_points={
         'console_scripts': [
-            'aissistant=aissistant.cli:main',
+            'aissistant=issistant.aissistant.cli:main',
         ],
     },
     author='Marko Manninen',
     url='https://github.com/markomanninen/aissistant',
     license='MIT',
     classifiers=[
         'Development Status :: 3 - Alpha',
```

