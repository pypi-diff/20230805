# Comparing `tmp/weathermap-1.0.2.tar.gz` & `tmp/weathermap-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weathermap-1.0.2.tar", last modified: Fri Aug  4 00:42:21 2023, max compression
+gzip compressed data, was "weathermap-1.0.3.tar", last modified: Sat Aug  5 01:08:13 2023, max compression
```

## Comparing `weathermap-1.0.2.tar` & `weathermap-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 00:42:21.145645 weathermap-1.0.2/
--rw-rw-rw-   0        0        0     3273 2023-08-04 00:42:21.145645 weathermap-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-04 00:42:21.145645 weathermap-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1046 2023-08-04 00:42:17.000000 weathermap-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 00:42:21.131682 weathermap-1.0.2/weathermap/
--rw-rw-rw-   0        0        0       41 2023-08-03 23:11:08.000000 weathermap-1.0.2/weathermap/_init_.py
--rw-rw-rw-   0        0        0     2960 2023-08-03 23:54:04.000000 weathermap-1.0.2/weathermap/weathermap.py
-drwxrwxrwx   0        0        0        0 2023-08-04 00:42:21.144649 weathermap-1.0.2/weathermap.egg-info/
--rw-rw-rw-   0        0        0     3273 2023-08-04 00:42:21.000000 weathermap-1.0.2/weathermap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-08-04 00:42:21.000000 weathermap-1.0.2/weathermap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 00:42:21.000000 weathermap-1.0.2/weathermap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-04 00:42:21.000000 weathermap-1.0.2/weathermap.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 00:42:21.000000 weathermap-1.0.2/weathermap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 01:08:13.884554 weathermap-1.0.3/
+-rw-rw-rw-   0        0        0     3377 2023-08-05 01:08:13.883556 weathermap-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2570 2023-08-05 00:01:47.000000 weathermap-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-05 01:08:13.884554 weathermap-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1148 2023-08-05 01:08:06.000000 weathermap-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 01:08:13.875578 weathermap-1.0.3/weathermap/
+-rw-rw-rw-   0        0        0       26 2023-08-04 17:36:57.000000 weathermap-1.0.3/weathermap/_init_.py
+-rw-rw-rw-   0        0        0     6130 2023-08-04 23:52:42.000000 weathermap-1.0.3/weathermap/weathermap.py
+drwxrwxrwx   0        0        0        0 2023-08-05 01:08:13.882559 weathermap-1.0.3/weathermap.egg-info/
+-rw-rw-rw-   0        0        0     3377 2023-08-05 01:08:13.000000 weathermap-1.0.3/weathermap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-08-05 01:08:13.000000 weathermap-1.0.3/weathermap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 01:08:13.000000 weathermap-1.0.3/weathermap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-05 01:08:13.000000 weathermap-1.0.3/weathermap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 01:08:13.000000 weathermap-1.0.3/weathermap.egg-info/top_level.txt
```

### Comparing `weathermap-1.0.2/PKG-INFO` & `weathermap-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: weathermap
-Version: 1.0.2
+Version: 1.0.3
 Summary: Openweathermap api simplified
 Home-page: https://github.com/savan2508/WeatherApp
 Author: Savan Patel
 Author-email: sawanpatel2508@gmail.com
 Keywords: weather,forecast,openweathermap,openweather
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # weathermap
 
 The weathermap package aims to aid users in getting necessary weather information in a simplified way, making it easy to integrate into various development projects where weather data is needed. The project can be accessed on PyPI [here](https://pypi.org/project/weathermap/), and the GitHub repository is available [here](https://github.com/savan2508/WeatherApp).
 
 ## Project Overview
```

### Comparing `weathermap-1.0.2/setup.py` & `weathermap-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='weathermap',
-    version='1.0.2',
+    version='1.0.3',
     description='Openweathermap api simplified',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Savan Patel',
     author_email='sawanpatel2508@gmail.com',
     url='https://github.com/savan2508/WeatherApp',
     packages=find_packages(exclude=['tests']),
@@ -22,9 +22,11 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 )
```

### Comparing `weathermap-1.0.2/weathermap.egg-info/PKG-INFO` & `weathermap-1.0.3/weathermap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: weathermap
-Version: 1.0.2
+Version: 1.0.3
 Summary: Openweathermap api simplified
 Home-page: https://github.com/savan2508/WeatherApp
 Author: Savan Patel
 Author-email: sawanpatel2508@gmail.com
 Keywords: weather,forecast,openweathermap,openweather
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # weathermap
 
 The weathermap package aims to aid users in getting necessary weather information in a simplified way, making it easy to integrate into various development projects where weather data is needed. The project can be accessed on PyPI [here](https://pypi.org/project/weathermap/), and the GitHub repository is available [here](https://github.com/savan2508/WeatherApp).
 
 ## Project Overview
```

