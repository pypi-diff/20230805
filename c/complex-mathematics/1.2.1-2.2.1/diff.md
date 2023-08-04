# Comparing `tmp/complex_mathematics-1.2.1.tar.gz` & `tmp/complex_mathematics-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "complex_mathematics-1.2.1.tar", last modified: Fri Aug  4 18:19:44 2023, max compression
+gzip compressed data, was "complex_mathematics-2.2.1.tar", last modified: Fri Aug  4 22:33:42 2023, max compression
```

## Comparing `complex_mathematics-1.2.1.tar` & `complex_mathematics-2.2.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 18:19:44.031150 complex_mathematics-1.2.1/
--rw-rw-rw-   0        0        0     1092 2023-08-04 16:05:05.000000 complex_mathematics-1.2.1/LICENSE
--rw-rw-rw-   0        0        0      398 2023-08-04 18:19:44.030153 complex_mathematics-1.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-04 18:19:44.013201 complex_mathematics-1.2.1/complex_mathematics/
--rw-rw-rw-   0        0        0     1622 2023-08-04 16:21:52.000000 complex_mathematics-1.2.1/complex_mathematics/__init__.py
--rw-rw-rw-   0        0        0     1354 2023-08-04 15:12:51.000000 complex_mathematics-1.2.1/complex_mathematics/linalg.py
--rw-rw-rw-   0        0        0     1586 2023-08-04 18:10:13.000000 complex_mathematics-1.2.1/complex_mathematics/ml.py
-drwxrwxrwx   0        0        0        0 2023-08-04 18:19:44.027161 complex_mathematics-1.2.1/complex_mathematics.egg-info/
--rw-rw-rw-   0        0        0      398 2023-08-04 18:19:43.000000 complex_mathematics-1.2.1/complex_mathematics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-08-04 18:19:43.000000 complex_mathematics-1.2.1/complex_mathematics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 18:19:43.000000 complex_mathematics-1.2.1/complex_mathematics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-08-04 18:19:43.000000 complex_mathematics-1.2.1/complex_mathematics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-08-04 18:19:43.000000 complex_mathematics-1.2.1/complex_mathematics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 18:19:44.032149 complex_mathematics-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-08-04 18:18:18.000000 complex_mathematics-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 22:33:42.176585 complex_mathematics-2.2.1/
+-rw-rw-rw-   0        0        0     1092 2023-08-04 16:05:05.000000 complex_mathematics-2.2.1/LICENSE
+-rw-rw-rw-   0        0        0      398 2023-08-04 22:33:42.174592 complex_mathematics-2.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-04 22:33:42.122732 complex_mathematics-2.2.1/complex_mathematics/
+-rw-rw-rw-   0        0        0     1622 2023-08-04 16:21:52.000000 complex_mathematics-2.2.1/complex_mathematics/__init__.py
+-rw-rw-rw-   0        0        0      692 2023-08-04 22:33:07.000000 complex_mathematics-2.2.1/complex_mathematics/algebra.py
+-rw-rw-rw-   0        0        0     1354 2023-08-04 15:12:51.000000 complex_mathematics-2.2.1/complex_mathematics/linalg.py
+-rw-rw-rw-   0        0        0     1586 2023-08-04 18:10:13.000000 complex_mathematics-2.2.1/complex_mathematics/ml.py
+drwxrwxrwx   0        0        0        0 2023-08-04 22:33:42.170600 complex_mathematics-2.2.1/complex_mathematics.egg-info/
+-rw-rw-rw-   0        0        0      398 2023-08-04 22:33:41.000000 complex_mathematics-2.2.1/complex_mathematics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2023-08-04 22:33:42.000000 complex_mathematics-2.2.1/complex_mathematics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 22:33:41.000000 complex_mathematics-2.2.1/complex_mathematics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-04 22:33:41.000000 complex_mathematics-2.2.1/complex_mathematics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-08-04 22:33:41.000000 complex_mathematics-2.2.1/complex_mathematics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 22:33:42.177583 complex_mathematics-2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-08-04 22:33:00.000000 complex_mathematics-2.2.1/setup.py
```

### Comparing `complex_mathematics-1.2.1/LICENSE` & `complex_mathematics-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `complex_mathematics-1.2.1/complex_mathematics/__init__.py` & `complex_mathematics-2.2.1/complex_mathematics/__init__.py`

 * *Files identical despite different names*

### Comparing `complex_mathematics-1.2.1/complex_mathematics/linalg.py` & `complex_mathematics-2.2.1/complex_mathematics/linalg.py`

 * *Files identical despite different names*

### Comparing `complex_mathematics-1.2.1/complex_mathematics/ml.py` & `complex_mathematics-2.2.1/complex_mathematics/ml.py`

 * *Files identical despite different names*

### Comparing `complex_mathematics-1.2.1/setup.py` & `complex_mathematics-2.2.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='complex_mathematics',
-    version='1.2.1',
+    version='2.2.1',
     packages=find_packages(),
     install_requires=[
         'numpy', 'scipy'
     ],
     license='MIT',
     author="Arnav Malhotra",
     author_email="emumalhotra@gmail.com",
```

