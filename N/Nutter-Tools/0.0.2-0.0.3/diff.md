# Comparing `tmp/Nutter-Tools-0.0.2.tar.gz` & `tmp/Nutter-Tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Nutter-Tools-0.0.2.tar", last modified: Sat Aug  5 14:24:04 2023, max compression
+gzip compressed data, was "Nutter-Tools-0.0.3.tar", last modified: Sat Aug  5 14:25:54 2023, max compression
```

## Comparing `Nutter-Tools-0.0.2.tar` & `Nutter-Tools-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 14:24:04.205118 Nutter-Tools-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-08-05 13:55:36.000000 Nutter-Tools-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      514 2023-08-05 14:24:04.203782 Nutter-Tools-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1478 2023-08-05 13:55:36.000000 Nutter-Tools-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-08-05 14:24:04.205118 Nutter-Tools-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      864 2023-08-05 14:23:54.000000 Nutter-Tools-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-05 14:24:04.181655 Nutter-Tools-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-08-05 14:24:04.202785 Nutter-Tools-0.0.2/src/Nutter_Tools.egg-info/
--rw-rw-rw-   0        0        0      514 2023-08-05 14:24:04.000000 Nutter-Tools-0.0.2/src/Nutter_Tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-08-05 14:24:04.000000 Nutter-Tools-0.0.2/src/Nutter_Tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 14:24:04.000000 Nutter-Tools-0.0.2/src/Nutter_Tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-08-05 14:24:04.000000 Nutter-Tools-0.0.2/src/Nutter_Tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-05 14:24:04.000000 Nutter-Tools-0.0.2/src/Nutter_Tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 14:25:54.167523 Nutter-Tools-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-08-05 13:55:36.000000 Nutter-Tools-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      514 2023-08-05 14:25:54.166045 Nutter-Tools-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1478 2023-08-05 13:55:36.000000 Nutter-Tools-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-05 14:25:54.167523 Nutter-Tools-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      833 2023-08-05 14:25:48.000000 Nutter-Tools-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 14:25:54.139764 Nutter-Tools-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-08-05 14:25:54.165053 Nutter-Tools-0.0.3/src/Nutter_Tools.egg-info/
+-rw-rw-rw-   0        0        0      514 2023-08-05 14:25:54.000000 Nutter-Tools-0.0.3/src/Nutter_Tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-08-05 14:25:54.000000 Nutter-Tools-0.0.3/src/Nutter_Tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 14:25:54.000000 Nutter-Tools-0.0.3/src/Nutter_Tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-08-05 14:25:54.000000 Nutter-Tools-0.0.3/src/Nutter_Tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-05 14:25:54.000000 Nutter-Tools-0.0.3/src/Nutter_Tools.egg-info/top_level.txt
```

### Comparing `Nutter-Tools-0.0.2/LICENSE.txt` & `Nutter-Tools-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nutter-Tools-0.0.2/PKG-INFO` & `Nutter-Tools-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nutter-Tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple program to find files easily with similar type of extension and to organize them.
 Home-page: https://github.com/Spidy20/PyMusic_Player
 Author: Ram Nikhilesh
 Keywords: nuttertools,tools,ntools
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Nutter-Tools-0.0.2/README.md` & `Nutter-Tools-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `Nutter-Tools-0.0.2/setup.py` & `Nutter-Tools-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='Nutter-Tools',
-    version='0.0.2',
+    version='0.0.3',
     description='A simple program to find files easily with similar type of extension and to organize them.',
     author= 'Ram Nikhilesh',
     url = 'https://github.com/Spidy20/PyMusic_Player',
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     keywords=['nuttertools', 'tools', 'ntools'],
     classifiers=[
@@ -18,12 +18,10 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     py_modules=['NTools'],
     package_dir={'':'src'},
     install_requires = [
-        'OS',
         'shutil',
-        'time'
     ]
 )
```

### Comparing `Nutter-Tools-0.0.2/src/Nutter_Tools.egg-info/PKG-INFO` & `Nutter-Tools-0.0.3/src/Nutter_Tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nutter-Tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple program to find files easily with similar type of extension and to organize them.
 Home-page: https://github.com/Spidy20/PyMusic_Player
 Author: Ram Nikhilesh
 Keywords: nuttertools,tools,ntools
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

