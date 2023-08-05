# Comparing `tmp/weathermap-1.0.3.tar.gz` & `tmp/weathermap-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weathermap-1.0.3.tar", last modified: Sat Aug  5 01:08:13 2023, max compression
+gzip compressed data, was "weathermap-1.0.4.tar", last modified: Sat Aug  5 01:39:57 2023, max compression
```

## Comparing `weathermap-1.0.3.tar` & `weathermap-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 01:08:13.884554 weathermap-1.0.3/
--rw-rw-rw-   0        0        0     3377 2023-08-05 01:08:13.883556 weathermap-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2570 2023-08-05 00:01:47.000000 weathermap-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-08-05 01:08:13.884554 weathermap-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1148 2023-08-05 01:08:06.000000 weathermap-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-05 01:08:13.875578 weathermap-1.0.3/weathermap/
--rw-rw-rw-   0        0        0       26 2023-08-04 17:36:57.000000 weathermap-1.0.3/weathermap/_init_.py
--rw-rw-rw-   0        0        0     6130 2023-08-04 23:52:42.000000 weathermap-1.0.3/weathermap/weathermap.py
-drwxrwxrwx   0        0        0        0 2023-08-05 01:08:13.882559 weathermap-1.0.3/weathermap.egg-info/
--rw-rw-rw-   0        0        0     3377 2023-08-05 01:08:13.000000 weathermap-1.0.3/weathermap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-08-05 01:08:13.000000 weathermap-1.0.3/weathermap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 01:08:13.000000 weathermap-1.0.3/weathermap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-05 01:08:13.000000 weathermap-1.0.3/weathermap.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 01:08:13.000000 weathermap-1.0.3/weathermap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 01:39:57.235799 weathermap-1.0.4/
+-rw-rw-rw-   0        0        0     3377 2023-08-05 01:39:57.235799 weathermap-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2570 2023-08-05 00:01:47.000000 weathermap-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-05 01:39:57.236796 weathermap-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1148 2023-08-05 01:39:52.000000 weathermap-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 01:39:57.221838 weathermap-1.0.4/weathermap/
+-rw-rw-rw-   0        0        0       57 2023-08-05 01:39:01.000000 weathermap-1.0.4/weathermap/_init_.py
+-rw-rw-rw-   0        0        0     6130 2023-08-04 23:52:42.000000 weathermap-1.0.4/weathermap/weathermap.py
+drwxrwxrwx   0        0        0        0 2023-08-05 01:39:57.233804 weathermap-1.0.4/weathermap.egg-info/
+-rw-rw-rw-   0        0        0     3377 2023-08-05 01:39:57.000000 weathermap-1.0.4/weathermap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-08-05 01:39:57.000000 weathermap-1.0.4/weathermap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 01:39:57.000000 weathermap-1.0.4/weathermap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-05 01:39:57.000000 weathermap-1.0.4/weathermap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 01:39:57.000000 weathermap-1.0.4/weathermap.egg-info/top_level.txt
```

### Comparing `weathermap-1.0.3/PKG-INFO` & `weathermap-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weathermap
-Version: 1.0.3
+Version: 1.0.4
 Summary: Openweathermap api simplified
 Home-page: https://github.com/savan2508/WeatherApp
 Author: Savan Patel
 Author-email: sawanpatel2508@gmail.com
 Keywords: weather,forecast,openweathermap,openweather
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `weathermap-1.0.3/README.md` & `weathermap-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `weathermap-1.0.3/setup.py` & `weathermap-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='weathermap',
-    version='1.0.3',
+    version='1.0.4',
     description='Openweathermap api simplified',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Savan Patel',
     author_email='sawanpatel2508@gmail.com',
     url='https://github.com/savan2508/WeatherApp',
     packages=find_packages(exclude=['tests']),
```

### Comparing `weathermap-1.0.3/weathermap/weathermap.py` & `weathermap-1.0.4/weathermap/weathermap.py`

 * *Files identical despite different names*

### Comparing `weathermap-1.0.3/weathermap.egg-info/PKG-INFO` & `weathermap-1.0.4/weathermap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weathermap
-Version: 1.0.3
+Version: 1.0.4
 Summary: Openweathermap api simplified
 Home-page: https://github.com/savan2508/WeatherApp
 Author: Savan Patel
 Author-email: sawanpatel2508@gmail.com
 Keywords: weather,forecast,openweathermap,openweather
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

