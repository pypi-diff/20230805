# Comparing `tmp/pyiplocation-0.2.tar.gz` & `tmp/pyiplocation-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiplocation-0.2.tar", last modified: Sat Aug  5 13:34:41 2023, max compression
+gzip compressed data, was "pyiplocation-0.3.tar", last modified: Sat Aug  5 13:46:46 2023, max compression
```

## Comparing `pyiplocation-0.2.tar` & `pyiplocation-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 13:34:41.629064 pyiplocation-0.2/
--rw-rw-rw-   0        0        0     1107 2023-08-04 10:34:13.000000 pyiplocation-0.2/LICENSE
--rw-rw-rw-   0        0        0     1431 2023-08-05 13:34:41.628061 pyiplocation-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      840 2023-08-05 13:30:20.000000 pyiplocation-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-05 13:34:41.613143 pyiplocation-0.2/pyiplocation/
--rw-rw-rw-   0        0        0     2760 2023-08-04 21:22:43.000000 pyiplocation-0.2/pyiplocation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-05 13:34:41.625066 pyiplocation-0.2/pyiplocation.egg-info/
--rw-rw-rw-   0        0        0     1431 2023-08-05 13:34:41.000000 pyiplocation-0.2/pyiplocation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-08-05 13:34:41.000000 pyiplocation-0.2/pyiplocation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 13:34:41.000000 pyiplocation-0.2/pyiplocation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-05 13:34:41.000000 pyiplocation-0.2/pyiplocation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-08-05 13:34:41.000000 pyiplocation-0.2/pyiplocation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-05 13:34:41.629064 pyiplocation-0.2/setup.cfg
--rw-rw-rw-   0        0        0      776 2023-08-05 13:33:56.000000 pyiplocation-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:46:46.584478 pyiplocation-0.3/
+-rw-rw-rw-   0        0        0     1107 2023-08-04 10:34:13.000000 pyiplocation-0.3/LICENSE
+-rw-rw-rw-   0        0        0     1495 2023-08-05 13:46:46.583475 pyiplocation-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      840 2023-08-05 13:30:20.000000 pyiplocation-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 13:46:46.563865 pyiplocation-0.3/pyiplocation/
+-rw-rw-rw-   0        0        0     2760 2023-08-04 21:22:43.000000 pyiplocation-0.3/pyiplocation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:46:46.582464 pyiplocation-0.3/pyiplocation.egg-info/
+-rw-rw-rw-   0        0        0     1495 2023-08-05 13:46:46.000000 pyiplocation-0.3/pyiplocation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-08-05 13:46:46.000000 pyiplocation-0.3/pyiplocation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 13:46:46.000000 pyiplocation-0.3/pyiplocation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-05 13:46:46.000000 pyiplocation-0.3/pyiplocation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-05 13:46:46.000000 pyiplocation-0.3/pyiplocation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 13:46:46.585500 pyiplocation-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      851 2023-08-05 13:46:39.000000 pyiplocation-0.3/setup.py
```

### Comparing `pyiplocation-0.2/LICENSE` & `pyiplocation-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiplocation-0.2/PKG-INFO` & `pyiplocation-0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pyiplocation
-Version: 0.2
+Version: 0.3
 Summary: A package for geolocating IPs
 Home-page: https://github.com/gugu256/gugu256
 Author: gugu256
 Author-email: gugu256@mail.com
 License: MIT
+Project-URL: Homepage, https://github.com/gugu256/pyiplocation
 Keywords: ip location
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pyiplocation-0.2/README.md` & `pyiplocation-0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyiplocation-0.2/pyiplocation/__init__.py` & `pyiplocation-0.3/pyiplocation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiplocation-0.2/pyiplocation.egg-info/PKG-INFO` & `pyiplocation-0.3/pyiplocation.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pyiplocation
-Version: 0.2
+Version: 0.3
 Summary: A package for geolocating IPs
 Home-page: https://github.com/gugu256/gugu256
 Author: gugu256
 Author-email: gugu256@mail.com
 License: MIT
+Project-URL: Homepage, https://github.com/gugu256/pyiplocation
 Keywords: ip location
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pyiplocation-0.2/setup.py` & `pyiplocation-0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from setuptools import setup
 
 
 setup(
     name='pyiplocation',
-    version='0.2',
+    version='0.3',
     license='MIT',
     description= "A package for geolocating IPs",
     long_description= open("README.md").read(),
     long_description_content_type= "text/markdown",
+    project_urls={"Homepage": "https://github.com/gugu256/pyiplocation"},
     author="gugu256",
     author_email='gugu256@mail.com',
     url='https://github.com/gugu256/gugu256',
     keywords='ip location',
     install_requires=[
           'requests',
       ],
```

