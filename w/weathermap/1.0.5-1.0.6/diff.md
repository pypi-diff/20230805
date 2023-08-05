# Comparing `tmp/weathermap-1.0.5.tar.gz` & `tmp/weathermap-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weathermap-1.0.5.tar", last modified: Sat Aug  5 02:33:02 2023, max compression
+gzip compressed data, was "weathermap-1.0.6.tar", last modified: Sat Aug  5 03:09:08 2023, max compression
```

## Comparing `weathermap-1.0.5.tar` & `weathermap-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 02:33:02.842379 weathermap-1.0.5/
--rw-rw-rw-   0        0        0     3377 2023-08-05 02:33:02.841382 weathermap-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2570 2023-08-05 00:01:47.000000 weathermap-1.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-08-05 02:33:02.842379 weathermap-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1115 2023-08-05 02:31:17.000000 weathermap-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-05 02:33:02.835396 weathermap-1.0.5/weathermap/
--rw-rw-rw-   0        0        0       57 2023-08-05 01:39:01.000000 weathermap-1.0.5/weathermap/_init_.py
--rw-rw-rw-   0        0        0     6130 2023-08-04 23:52:42.000000 weathermap-1.0.5/weathermap/weathermap.py
-drwxrwxrwx   0        0        0        0 2023-08-05 02:33:02.840384 weathermap-1.0.5/weathermap.egg-info/
--rw-rw-rw-   0        0        0     3377 2023-08-05 02:33:02.000000 weathermap-1.0.5/weathermap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-08-05 02:33:02.000000 weathermap-1.0.5/weathermap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 02:33:02.000000 weathermap-1.0.5/weathermap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-05 02:33:02.000000 weathermap-1.0.5/weathermap.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-05 02:33:02.000000 weathermap-1.0.5/weathermap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 03:09:08.952228 weathermap-1.0.6/
+-rw-rw-rw-   0        0        0     3377 2023-08-05 03:09:08.951229 weathermap-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2570 2023-08-05 00:01:47.000000 weathermap-1.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-05 03:09:08.952228 weathermap-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1115 2023-08-05 03:02:39.000000 weathermap-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 03:09:08.945248 weathermap-1.0.6/weathermap/
+-rw-rw-rw-   0        0        0       68 2023-08-05 03:01:11.000000 weathermap-1.0.6/weathermap/_init_.py
+-rw-rw-rw-   0        0        0     6130 2023-08-04 23:52:42.000000 weathermap-1.0.6/weathermap/weathermap.py
+drwxrwxrwx   0        0        0        0 2023-08-05 03:09:08.950233 weathermap-1.0.6/weathermap.egg-info/
+-rw-rw-rw-   0        0        0     3377 2023-08-05 03:09:08.000000 weathermap-1.0.6/weathermap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-08-05 03:09:08.000000 weathermap-1.0.6/weathermap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 03:09:08.000000 weathermap-1.0.6/weathermap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-05 03:09:08.000000 weathermap-1.0.6/weathermap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-05 03:09:08.000000 weathermap-1.0.6/weathermap.egg-info/top_level.txt
```

### Comparing `weathermap-1.0.5/PKG-INFO` & `weathermap-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weathermap
-Version: 1.0.5
+Version: 1.0.6
 Summary: Openweathermap api simplified
 Home-page: https://github.com/savan2508/WeatherApp
 Author: Savan Patel
 Author-email: sawanpatel2508@gmail.com
 Keywords: weather,forecast,openweathermap,openweather
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `weathermap-1.0.5/README.md` & `weathermap-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `weathermap-1.0.5/setup.py` & `weathermap-1.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='weathermap',
-    version='1.0.5',
+    version='1.0.6',
     packages=['weathermap'],
     description='Openweathermap api simplified',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Savan Patel',
     author_email='sawanpatel2508@gmail.com',
     url='https://github.com/savan2508/WeatherApp',
```

### Comparing `weathermap-1.0.5/weathermap/weathermap.py` & `weathermap-1.0.6/weathermap/weathermap.py`

 * *Files identical despite different names*

### Comparing `weathermap-1.0.5/weathermap.egg-info/PKG-INFO` & `weathermap-1.0.6/weathermap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weathermap
-Version: 1.0.5
+Version: 1.0.6
 Summary: Openweathermap api simplified
 Home-page: https://github.com/savan2508/WeatherApp
 Author: Savan Patel
 Author-email: sawanpatel2508@gmail.com
 Keywords: weather,forecast,openweathermap,openweather
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

