# Comparing `tmp/Nutter-Tools-0.0.3.tar.gz` & `tmp/Nutter-Tools-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Nutter-Tools-0.0.3.tar", last modified: Sat Aug  5 14:25:54 2023, max compression
+gzip compressed data, was "Nutter-Tools-0.0.31.tar", last modified: Sat Aug  5 14:38:39 2023, max compression
```

## Comparing `Nutter-Tools-0.0.3.tar` & `Nutter-Tools-0.0.31.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 14:25:54.167523 Nutter-Tools-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-08-05 13:55:36.000000 Nutter-Tools-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      514 2023-08-05 14:25:54.166045 Nutter-Tools-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1478 2023-08-05 13:55:36.000000 Nutter-Tools-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-08-05 14:25:54.167523 Nutter-Tools-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      833 2023-08-05 14:25:48.000000 Nutter-Tools-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-05 14:25:54.139764 Nutter-Tools-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-08-05 14:25:54.165053 Nutter-Tools-0.0.3/src/Nutter_Tools.egg-info/
--rw-rw-rw-   0        0        0      514 2023-08-05 14:25:54.000000 Nutter-Tools-0.0.3/src/Nutter_Tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-08-05 14:25:54.000000 Nutter-Tools-0.0.3/src/Nutter_Tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 14:25:54.000000 Nutter-Tools-0.0.3/src/Nutter_Tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-08-05 14:25:54.000000 Nutter-Tools-0.0.3/src/Nutter_Tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-05 14:25:54.000000 Nutter-Tools-0.0.3/src/Nutter_Tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 14:38:39.726369 Nutter-Tools-0.0.31/
+-rw-rw-rw-   0        0        0     1091 2023-08-05 13:55:36.000000 Nutter-Tools-0.0.31/LICENSE.txt
+-rw-rw-rw-   0        0        0      515 2023-08-05 14:38:39.725371 Nutter-Tools-0.0.31/PKG-INFO
+-rw-rw-rw-   0        0        0     1478 2023-08-05 13:55:36.000000 Nutter-Tools-0.0.31/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-05 14:38:39.726369 Nutter-Tools-0.0.31/setup.cfg
+-rw-rw-rw-   0        0        0      834 2023-08-05 14:38:29.000000 Nutter-Tools-0.0.31/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 14:38:39.688186 Nutter-Tools-0.0.31/src/
+drwxrwxrwx   0        0        0        0 2023-08-05 14:38:39.724451 Nutter-Tools-0.0.31/src/Nutter_Tools.egg-info/
+-rw-rw-rw-   0        0        0      515 2023-08-05 14:38:39.000000 Nutter-Tools-0.0.31/src/Nutter_Tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-08-05 14:38:39.000000 Nutter-Tools-0.0.31/src/Nutter_Tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 14:38:39.000000 Nutter-Tools-0.0.31/src/Nutter_Tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-08-05 14:38:39.000000 Nutter-Tools-0.0.31/src/Nutter_Tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-05 14:38:39.000000 Nutter-Tools-0.0.31/src/Nutter_Tools.egg-info/top_level.txt
```

### Comparing `Nutter-Tools-0.0.3/LICENSE.txt` & `Nutter-Tools-0.0.31/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nutter-Tools-0.0.3/PKG-INFO` & `Nutter-Tools-0.0.31/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nutter-Tools
-Version: 0.0.3
+Version: 0.0.31
 Summary: A simple program to find files easily with similar type of extension and to organize them.
 Home-page: https://github.com/Spidy20/PyMusic_Player
 Author: Ram Nikhilesh
 Keywords: nuttertools,tools,ntools
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Nutter-Tools-0.0.3/README.md` & `Nutter-Tools-0.0.31/README.md`

 * *Files identical despite different names*

### Comparing `Nutter-Tools-0.0.3/setup.py` & `Nutter-Tools-0.0.31/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='Nutter-Tools',
-    version='0.0.3',
+    version='0.0.31',
     description='A simple program to find files easily with similar type of extension and to organize them.',
     author= 'Ram Nikhilesh',
     url = 'https://github.com/Spidy20/PyMusic_Player',
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     keywords=['nuttertools', 'tools', 'ntools'],
     classifiers=[
```

### Comparing `Nutter-Tools-0.0.3/src/Nutter_Tools.egg-info/PKG-INFO` & `Nutter-Tools-0.0.31/src/Nutter_Tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nutter-Tools
-Version: 0.0.3
+Version: 0.0.31
 Summary: A simple program to find files easily with similar type of extension and to organize them.
 Home-page: https://github.com/Spidy20/PyMusic_Player
 Author: Ram Nikhilesh
 Keywords: nuttertools,tools,ntools
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

