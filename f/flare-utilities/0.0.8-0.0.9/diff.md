# Comparing `tmp/Flare_Utilities-0.0.8.tar.gz` & `tmp/Flare_Utilities-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Flare_Utilities-0.0.8.tar", last modified: Mon Mar  6 15:03:33 2023, max compression
+gzip compressed data, was "dist\Flare_Utilities-0.0.9.tar", last modified: Mon Mar  6 15:18:57 2023, max compression
```

## Comparing `Flare_Utilities-0.0.8.tar` & `Flare_Utilities-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-06 15:03:33.000000 Flare_Utilities-0.0.8/
--rw-rw-rw-   0        0        0     2180 2023-03-06 15:03:33.000000 Flare_Utilities-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1411 2023-02-02 12:29:17.000000 Flare_Utilities-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-06 15:03:33.000000 Flare_Utilities-0.0.8/Reporting/
-drwxrwxrwx   0        0        0        0 2023-03-06 15:03:33.000000 Flare_Utilities-0.0.8/Reporting/Flare_Utilities.egg-info/
--rw-rw-rw-   0        0        0     2180 2023-03-06 15:03:32.000000 Flare_Utilities-0.0.8/Reporting/Flare_Utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-03-06 15:03:32.000000 Flare_Utilities-0.0.8/Reporting/Flare_Utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-06 15:03:32.000000 Flare_Utilities-0.0.8/Reporting/Flare_Utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-03-06 15:03:32.000000 Flare_Utilities-0.0.8/Reporting/Flare_Utilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-06 15:03:32.000000 Flare_Utilities-0.0.8/Reporting/Flare_Utilities.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-06 15:03:33.000000 Flare_Utilities-0.0.8/Reporting/pytransform/
--rw-rw-rw-   0        0        0    13587 2023-01-30 16:12:42.000000 Flare_Utilities-0.0.8/Reporting/pytransform/__init__.py
--rw-rw-rw-   0        0        0       42 2023-03-06 15:03:33.000000 Flare_Utilities-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1462 2023-03-06 15:03:26.000000 Flare_Utilities-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-06 15:18:57.000000 Flare_Utilities-0.0.9/
+-rw-rw-rw-   0        0        0     2180 2023-03-06 15:18:57.000000 Flare_Utilities-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1411 2023-02-02 12:29:17.000000 Flare_Utilities-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-06 15:18:56.000000 Flare_Utilities-0.0.9/Reporting/
+drwxrwxrwx   0        0        0        0 2023-03-06 15:18:57.000000 Flare_Utilities-0.0.9/Reporting/Flare_Utilities.egg-info/
+-rw-rw-rw-   0        0        0     2180 2023-03-06 15:18:56.000000 Flare_Utilities-0.0.9/Reporting/Flare_Utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-03-06 15:18:56.000000 Flare_Utilities-0.0.9/Reporting/Flare_Utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-06 15:18:56.000000 Flare_Utilities-0.0.9/Reporting/Flare_Utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-03-06 15:18:56.000000 Flare_Utilities-0.0.9/Reporting/Flare_Utilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-03-06 15:18:56.000000 Flare_Utilities-0.0.9/Reporting/Flare_Utilities.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-06 15:18:57.000000 Flare_Utilities-0.0.9/Reporting/pytransform/
+-rw-rw-rw-   0        0        0    13587 2023-01-30 16:12:42.000000 Flare_Utilities-0.0.9/Reporting/pytransform/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-03-06 15:18:57.000000 Flare_Utilities-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1462 2023-03-06 15:18:27.000000 Flare_Utilities-0.0.9/setup.py
```

### Comparing `Flare_Utilities-0.0.8/PKG-INFO` & `Flare_Utilities-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flare_Utilities
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
         Flare Utilities having support libraries for Flare-BDD framework for reporting purposes.
     
 Home-page: UNKNOWN
 Author: Aravinth Alliraj
 License: UNKNOWN
 Description: # Flare Utilities
```

### Comparing `Flare_Utilities-0.0.8/README.md` & `Flare_Utilities-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `Flare_Utilities-0.0.8/Reporting/Flare_Utilities.egg-info/PKG-INFO` & `Flare_Utilities-0.0.9/Reporting/Flare_Utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flare-Utilities
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
         Flare Utilities having support libraries for Flare-BDD framework for reporting purposes.
     
 Home-page: UNKNOWN
 Author: Aravinth Alliraj
 License: UNKNOWN
 Description: # Flare Utilities
```

### Comparing `Flare_Utilities-0.0.8/Reporting/pytransform/__init__.py` & `Flare_Utilities-0.0.9/Reporting/pytransform/__init__.py`

 * *Files identical despite different names*

### Comparing `Flare_Utilities-0.0.8/setup.py` & `Flare_Utilities-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 # def clean_project_directory():
 #     return os.system('rm -vrf ./build ./dist ./*.pyc ./*.tgz ./*.egg-info')
 
 
 setup(
     name="Flare_Utilities",
-    version="0.0.8",
+    version="0.0.9",
     description="""
         Flare Utilities having support libraries for Flare-BDD framework for reporting purposes.
     """,
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     author="Aravinth Alliraj",
     packages=find_packages('Reporting'),
```

