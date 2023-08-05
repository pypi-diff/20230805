# Comparing `tmp/Nutter-Tools-0.0.1.tar.gz` & `tmp/Nutter-Tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Nutter-Tools-0.0.1.tar", last modified: Sat Aug  5 14:06:53 2023, max compression
+gzip compressed data, was "Nutter-Tools-0.0.2.tar", last modified: Sat Aug  5 14:24:04 2023, max compression
```

## Comparing `Nutter-Tools-0.0.1.tar` & `Nutter-Tools-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 14:06:53.905797 Nutter-Tools-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-08-05 13:55:36.000000 Nutter-Tools-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      547 2023-08-05 14:06:53.903731 Nutter-Tools-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1478 2023-08-05 13:55:36.000000 Nutter-Tools-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-08-05 14:06:53.906739 Nutter-Tools-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-08-05 14:06:47.000000 Nutter-Tools-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-05 14:06:53.871533 Nutter-Tools-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-08-05 14:06:53.902726 Nutter-Tools-0.0.1/src/Nutter_Tools.egg-info/
--rw-rw-rw-   0        0        0      547 2023-08-05 14:06:53.000000 Nutter-Tools-0.0.1/src/Nutter_Tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-08-05 14:06:53.000000 Nutter-Tools-0.0.1/src/Nutter_Tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 14:06:53.000000 Nutter-Tools-0.0.1/src/Nutter_Tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-08-05 14:06:53.000000 Nutter-Tools-0.0.1/src/Nutter_Tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-05 14:06:53.000000 Nutter-Tools-0.0.1/src/Nutter_Tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 14:24:04.205118 Nutter-Tools-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-08-05 13:55:36.000000 Nutter-Tools-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      514 2023-08-05 14:24:04.203782 Nutter-Tools-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1478 2023-08-05 13:55:36.000000 Nutter-Tools-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-05 14:24:04.205118 Nutter-Tools-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      864 2023-08-05 14:23:54.000000 Nutter-Tools-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 14:24:04.181655 Nutter-Tools-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-08-05 14:24:04.202785 Nutter-Tools-0.0.2/src/Nutter_Tools.egg-info/
+-rw-rw-rw-   0        0        0      514 2023-08-05 14:24:04.000000 Nutter-Tools-0.0.2/src/Nutter_Tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-08-05 14:24:04.000000 Nutter-Tools-0.0.2/src/Nutter_Tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 14:24:04.000000 Nutter-Tools-0.0.2/src/Nutter_Tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-08-05 14:24:04.000000 Nutter-Tools-0.0.2/src/Nutter_Tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-05 14:24:04.000000 Nutter-Tools-0.0.2/src/Nutter_Tools.egg-info/top_level.txt
```

### Comparing `Nutter-Tools-0.0.1/LICENSE.txt` & `Nutter-Tools-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nutter-Tools-0.0.1/README.md` & `Nutter-Tools-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `Nutter-Tools-0.0.1/setup.py` & `Nutter-Tools-0.0.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='Nutter-Tools',
-    version='0.0.1',
+    version='0.0.2',
     description='A simple program to find files easily with similar type of extension and to organize them.',
     author= 'Ram Nikhilesh',
     url = 'https://github.com/Spidy20/PyMusic_Player',
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
-    keywords=['music player python', 'music player tkinter', 'music player gui'],
+    keywords=['nuttertools', 'tools', 'ntools'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     py_modules=['NTools'],
```

