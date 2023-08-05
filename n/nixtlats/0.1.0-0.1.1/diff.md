# Comparing `tmp/nixtlats-0.1.0.tar.gz` & `tmp/nixtlats-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nixtlats-0.1.0.tar", last modified: Sat Aug  5 08:32:24 2023, max compression
+gzip compressed data, was "nixtlats-0.1.1.tar", last modified: Sat Aug  5 08:11:50 2023, max compression
```

## Comparing `nixtlats-0.1.0.tar` & `nixtlats-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 fedex      (501) staff       (20)        0 2023-08-05 08:32:24.552172 nixtlats-0.1.0/
--rw-r--r--   0 fedex      (501) staff       (20)     1155 2023-08-05 06:39:47.000000 nixtlats-0.1.0/LICENSE
--rw-r--r--   0 fedex      (501) staff       (20)     3457 2023-08-05 08:32:24.552020 nixtlats-0.1.0/PKG-INFO
--rw-r--r--   0 fedex      (501) staff       (20)     3108 2023-08-05 06:39:47.000000 nixtlats-0.1.0/README.md
-drwxr-xr-x   0 fedex      (501) staff       (20)        0 2023-08-05 08:32:24.551029 nixtlats-0.1.0/nixtlats/
--rw-r--r--   0 fedex      (501) staff       (20)       73 2023-08-05 08:21:15.000000 nixtlats-0.1.0/nixtlats/__init__.py
--rw-r--r--   0 fedex      (501) staff       (20)     1596 2023-08-05 08:21:15.000000 nixtlats-0.1.0/nixtlats/_modidx.py
--rw-r--r--   0 fedex      (501) staff       (20)     5339 2023-08-05 08:21:15.000000 nixtlats-0.1.0/nixtlats/timegpt.py
-drwxr-xr-x   0 fedex      (501) staff       (20)        0 2023-08-05 08:32:24.551840 nixtlats-0.1.0/nixtlats.egg-info/
--rw-r--r--   0 fedex      (501) staff       (20)     3457 2023-08-05 08:32:24.000000 nixtlats-0.1.0/nixtlats.egg-info/PKG-INFO
--rw-r--r--   0 fedex      (501) staff       (20)      215 2023-08-05 08:32:24.000000 nixtlats-0.1.0/nixtlats.egg-info/SOURCES.txt
--rw-r--r--   0 fedex      (501) staff       (20)        1 2023-08-05 08:32:24.000000 nixtlats-0.1.0/nixtlats.egg-info/dependency_links.txt
--rw-r--r--   0 fedex      (501) staff       (20)        9 2023-08-05 08:32:24.000000 nixtlats-0.1.0/nixtlats.egg-info/top_level.txt
--rw-r--r--   0 fedex      (501) staff       (20)       38 2023-08-05 08:32:24.552216 nixtlats-0.1.0/setup.cfg
--rw-r--r--   0 fedex      (501) staff       (20)      552 2023-08-05 08:32:18.000000 nixtlats-0.1.0/setup.py
+drwxr-xr-x   0 fedex      (501) staff       (20)        0 2023-08-05 08:11:50.537494 nixtlats-0.1.1/
+-rw-r--r--   0 fedex      (501) staff       (20)     1155 2023-08-05 06:39:47.000000 nixtlats-0.1.1/LICENSE
+-rw-r--r--   0 fedex      (501) staff       (20)     3830 2023-08-05 08:11:50.537339 nixtlats-0.1.1/PKG-INFO
+-rw-r--r--   0 fedex      (501) staff       (20)     3108 2023-08-05 06:39:47.000000 nixtlats-0.1.1/README.md
+drwxr-xr-x   0 fedex      (501) staff       (20)        0 2023-08-05 08:11:50.535941 nixtlats-0.1.1/nixtlats/
+-rw-r--r--   0 fedex      (501) staff       (20)       73 2023-08-05 07:57:11.000000 nixtlats-0.1.1/nixtlats/__init__.py
+-rw-r--r--   0 fedex      (501) staff       (20)     1596 2023-08-05 07:35:12.000000 nixtlats-0.1.1/nixtlats/_modidx.py
+-rw-r--r--   0 fedex      (501) staff       (20)     5339 2023-08-05 07:35:12.000000 nixtlats-0.1.1/nixtlats/timegpt.py
+drwxr-xr-x   0 fedex      (501) staff       (20)        0 2023-08-05 08:11:50.537156 nixtlats-0.1.1/nixtlats.egg-info/
+-rw-r--r--   0 fedex      (501) staff       (20)     3830 2023-08-05 08:11:50.000000 nixtlats-0.1.1/nixtlats.egg-info/PKG-INFO
+-rw-r--r--   0 fedex      (501) staff       (20)      312 2023-08-05 08:11:50.000000 nixtlats-0.1.1/nixtlats.egg-info/SOURCES.txt
+-rw-r--r--   0 fedex      (501) staff       (20)        1 2023-08-05 08:11:50.000000 nixtlats-0.1.1/nixtlats.egg-info/dependency_links.txt
+-rw-r--r--   0 fedex      (501) staff       (20)       38 2023-08-05 08:11:50.000000 nixtlats-0.1.1/nixtlats.egg-info/entry_points.txt
+-rw-r--r--   0 fedex      (501) staff       (20)        1 2023-08-05 05:44:38.000000 nixtlats-0.1.1/nixtlats.egg-info/not-zip-safe
+-rw-r--r--   0 fedex      (501) staff       (20)       79 2023-08-05 08:11:50.000000 nixtlats-0.1.1/nixtlats.egg-info/requires.txt
+-rw-r--r--   0 fedex      (501) staff       (20)        9 2023-08-05 08:11:50.000000 nixtlats-0.1.1/nixtlats.egg-info/top_level.txt
+-rw-r--r--   0 fedex      (501) staff       (20)       38 2023-08-05 08:11:50.537537 nixtlats-0.1.1/setup.cfg
+-rw-r--r--   0 fedex      (501) staff       (20)     2549 2023-08-05 08:08:26.000000 nixtlats-0.1.1/setup.py
```

### Comparing `nixtlats-0.1.0/LICENSE` & `nixtlats-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nixtlats-0.1.0/PKG-INFO` & `nixtlats-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: nixtlats
-Version: 0.1.0
-Summary: Nixtla SDK
-Home-page: https://github.com/Nixtla/nixtla
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Nixtla &nbsp; [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Statistical%20Forecasting%20Algorithms%20by%20Nixtla%20&url=https://github.com/Nixtla/statsforecast&via=nixtlainc&hashtags=StatisticalModels,TimeSeries,Forecasting) &nbsp;[![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white)](https://join.slack.com/t/nixtlacommunity/shared_invite/zt-1pmhan9j5-F54XR20edHk0UtYAPcW4KQ)
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/Nixtla/neuralforecast/main/nbs/imgs_indx/logo_mid.png">
 <h1 align="center">NixtlaTS</h1>
 <h3 align="center">Forecast using TimeGPT</h3>
     
@@ -59,8 +47,8 @@
 
 ```python
 from nixtlats import TimeGPT
 timegpt = TimeGPT(token=os.environ['TIMEGPT_TOKEN'], api_url=os.environ['TIMEGPT_API_URL'])
 fcst_df = timegpt.forecast(df, h=24, freq='H', level=[80, 90])
 ```
 
-![](./nbs/img/forecast_readme.png)
+![](./nbs/img/forecast_readme.png)
```

### Comparing `nixtlats-0.1.0/nixtlats/_modidx.py` & `nixtlats-0.1.1/nixtlats/_modidx.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.1.0/nixtlats/timegpt.py` & `nixtlats-0.1.1/nixtlats/timegpt.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.1.0/nixtlats.egg-info/PKG-INFO` & `nixtlats-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 Metadata-Version: 2.1
 Name: nixtlats
-Version: 0.1.0
-Summary: Nixtla SDK
-Home-page: https://github.com/Nixtla/nixtla
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Version: 0.1.1
+Summary: Time series forecasting suite using TimeGPT
+Home-page: https://github.com/Nixtla/nixtla/
+Author: Nixtla
+Author-email: business@nixtla.io
+License: Apache Software License 2.0
+Keywords: time-series forecasting gpt
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Nixtla &nbsp; [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Statistical%20Forecasting%20Algorithms%20by%20Nixtla%20&url=https://github.com/Nixtla/statsforecast&via=nixtlainc&hashtags=StatisticalModels,TimeSeries,Forecasting) &nbsp;[![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white)](https://join.slack.com/t/nixtlacommunity/shared_invite/zt-1pmhan9j5-F54XR20edHk0UtYAPcW4KQ)
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/Nixtla/neuralforecast/main/nbs/imgs_indx/logo_mid.png">
 <h1 align="center">NixtlaTS</h1>
```

