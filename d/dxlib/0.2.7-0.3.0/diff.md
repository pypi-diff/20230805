# Comparing `tmp/dxlib-0.2.7.tar.gz` & `tmp/dxlib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxlib-0.2.7.tar", last modified: Sat Jul 29 07:59:45 2023, max compression
+gzip compressed data, was "dxlib-0.3.0.tar", last modified: Sat Aug  5 05:03:00 2023, max compression
```

## Comparing `dxlib-0.2.7.tar` & `dxlib-0.3.0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:59:45.003340 dxlib-0.2.7/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)    10948 2023-07-16 21:40:36.000000 dxlib-0.2.7/LICENSE
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     3244 2023-07-29 07:59:44.999342 dxlib-0.2.7/PKG-INFO
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     2487 2023-07-16 21:40:36.000000 dxlib-0.2.7/README.md
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:59:43.940454 dxlib-0.2.7/dxlib/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       95 2023-07-15 07:58:04.000000 dxlib-0.2.7/dxlib/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:59:44.304341 dxlib-0.2.7/dxlib/api/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      117 2023-07-29 07:41:11.000000 dxlib-0.2.7/dxlib/api/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      777 2023-07-29 07:56:12.000000 dxlib-0.2.7/dxlib/api/alpaca_markets.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1304 2023-07-15 07:58:04.000000 dxlib-0.2.7/dxlib/api/alphavantage.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     3117 2023-07-29 07:33:09.000000 dxlib-0.2.7/dxlib/api/core.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:49:44.000000 dxlib-0.2.7/dxlib/api/logger.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:49:34.000000 dxlib-0.2.7/dxlib/api/terminal.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:59:44.452341 dxlib-0.2.7/dxlib/core/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:09.000000 dxlib-0.2.7/dxlib/core/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      387 2023-07-15 07:58:04.000000 dxlib-0.2.7/dxlib/core/euler_method.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      262 2023-07-15 07:58:04.000000 dxlib-0.2.7/dxlib/core/finite_differences.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     9503 2023-07-25 00:10:53.000000 dxlib-0.2.7/dxlib/core/options.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:59:44.528341 dxlib-0.2.7/dxlib/data/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       21 2023-07-15 07:58:04.000000 dxlib-0.2.7/dxlib/data/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     2150 2023-07-15 09:26:56.000000 dxlib-0.2.7/dxlib/data/utils.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:59:44.603340 dxlib-0.2.7/dxlib/db/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      603 2023-07-17 19:47:05.000000 dxlib-0.2.7/dxlib/db/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:59:44.741341 dxlib-0.2.7/dxlib/db/sql/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-06-30 10:14:59.000000 dxlib-0.2.7/dxlib/db/sql/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      148 2023-07-15 07:58:04.000000 dxlib-0.2.7/dxlib/db/sql/create.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      730 2023-07-15 07:58:04.000000 dxlib-0.2.7/dxlib/db/sql/queries.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     4241 2023-07-15 07:58:05.000000 dxlib-0.2.7/dxlib/db/utils.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:59:44.818341 dxlib-0.2.7/dxlib/models/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:31.000000 dxlib-0.2.7/dxlib/models/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:26:00.000000 dxlib-0.2.7/dxlib/models/systematic_trading.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     5388 2023-07-29 07:35:54.000000 dxlib-0.2.7/dxlib/portfolio_theory_module.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:59:44.854341 dxlib-0.2.7/dxlib/research/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:50:59.000000 dxlib-0.2.7/dxlib/research/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:59:44.928341 dxlib-0.2.7/dxlib/simulation/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:15.000000 dxlib-0.2.7/dxlib/simulation/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     7903 2023-07-15 07:58:05.000000 dxlib-0.2.7/dxlib/simulation/backtesting.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       80 2023-07-29 07:56:48.000000 dxlib-0.2.7/dxlib/test.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:59:44.965340 dxlib-0.2.7/dxlib/visualization/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:06:43.000000 dxlib-0.2.7/dxlib/visualization/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:59:44.081452 dxlib-0.2.7/dxlib.egg-info/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     3244 2023-07-29 07:59:43.000000 dxlib-0.2.7/dxlib.egg-info/PKG-INFO
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      810 2023-07-29 07:59:43.000000 dxlib-0.2.7/dxlib.egg-info/SOURCES.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        1 2023-07-29 07:59:43.000000 dxlib-0.2.7/dxlib.egg-info/dependency_links.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       96 2023-07-29 07:59:43.000000 dxlib-0.2.7/dxlib.egg-info/requires.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        6 2023-07-29 07:59:43.000000 dxlib-0.2.7/dxlib.egg-info/top_level.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       38 2023-07-29 07:59:45.004341 dxlib-0.2.7/setup.cfg
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1328 2023-07-15 07:44:19.000000 dxlib-0.2.7/setup.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-08-05 05:03:00.154438 dxlib-0.3.0/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)    10948 2023-07-16 21:40:36.000000 dxlib-0.3.0/LICENSE
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     3244 2023-08-05 05:03:00.149923 dxlib-0.3.0/PKG-INFO
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     2487 2023-07-16 21:40:36.000000 dxlib-0.3.0/README.md
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-08-05 05:02:58.901285 dxlib-0.3.0/dxlib/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       87 2023-08-04 04:26:27.000000 dxlib-0.3.0/dxlib/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-08-05 05:02:59.205266 dxlib-0.3.0/dxlib/api/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      120 2023-08-04 00:44:05.000000 dxlib-0.3.0/dxlib/api/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     4003 2023-08-05 04:43:46.000000 dxlib-0.3.0/dxlib/api/alpaca_markets.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1304 2023-07-15 07:58:04.000000 dxlib-0.3.0/dxlib/api/alphavantage.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     3117 2023-07-29 07:33:09.000000 dxlib-0.3.0/dxlib/api/request.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-08-05 05:02:59.448022 dxlib-0.3.0/dxlib/core/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      250 2023-08-04 01:55:13.000000 dxlib-0.3.0/dxlib/core/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      939 2023-08-04 03:56:18.000000 dxlib-0.3.0/dxlib/core/history.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1209 2023-08-03 21:53:12.000000 dxlib-0.3.0/dxlib/core/logger.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     9503 2023-07-25 00:10:53.000000 dxlib-0.3.0/dxlib/core/options.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     9279 2023-08-04 07:09:09.000000 dxlib-0.3.0/dxlib/core/portfolio.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1168 2023-08-04 06:45:00.000000 dxlib-0.3.0/dxlib/core/security.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-08-05 05:02:59.529254 dxlib-0.3.0/dxlib/data/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       21 2023-07-15 07:58:04.000000 dxlib-0.3.0/dxlib/data/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     2150 2023-07-15 09:26:56.000000 dxlib-0.3.0/dxlib/data/utils.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-08-05 05:02:59.610062 dxlib-0.3.0/dxlib/db/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      603 2023-07-17 19:47:05.000000 dxlib-0.3.0/dxlib/db/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-08-05 05:02:59.756154 dxlib-0.3.0/dxlib/db/sql/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-06-30 10:14:59.000000 dxlib-0.3.0/dxlib/db/sql/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      148 2023-07-15 07:58:04.000000 dxlib-0.3.0/dxlib/db/sql/create.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      730 2023-07-15 07:58:04.000000 dxlib-0.3.0/dxlib/db/sql/queries.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     4241 2023-07-15 07:58:05.000000 dxlib-0.3.0/dxlib/db/utils.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     5388 2023-07-29 07:35:54.000000 dxlib-0.3.0/dxlib/portfolio_theory_module.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-08-05 05:02:59.799039 dxlib-0.3.0/dxlib/research/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:50:59.000000 dxlib-0.3.0/dxlib/research/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-08-05 05:02:59.918524 dxlib-0.3.0/dxlib/simulation/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       51 2023-08-04 04:16:50.000000 dxlib-0.3.0/dxlib/simulation/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     7903 2023-07-15 07:58:05.000000 dxlib-0.3.0/dxlib/simulation/backtesting.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     3824 2023-08-04 07:07:54.000000 dxlib-0.3.0/dxlib/simulation/simulate.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-08-05 05:03:00.076406 dxlib-0.3.0/dxlib/strategies/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:31.000000 dxlib-0.3.0/dxlib/strategies/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      387 2023-07-15 07:58:04.000000 dxlib-0.3.0/dxlib/strategies/euler_method.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      262 2023-07-15 07:58:04.000000 dxlib-0.3.0/dxlib/strategies/finite_differences.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      464 2023-08-04 04:18:56.000000 dxlib-0.3.0/dxlib/strategies/systematic_trading.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-08-05 05:03:00.115480 dxlib-0.3.0/dxlib/visualization/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:06:43.000000 dxlib-0.3.0/dxlib/visualization/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-08-05 05:02:59.048996 dxlib-0.3.0/dxlib.egg-info/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     3244 2023-08-05 05:02:58.000000 dxlib-0.3.0/dxlib.egg-info/PKG-INFO
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      896 2023-08-05 05:02:58.000000 dxlib-0.3.0/dxlib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        1 2023-08-05 05:02:58.000000 dxlib-0.3.0/dxlib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      172 2023-08-05 05:02:58.000000 dxlib-0.3.0/dxlib.egg-info/requires.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        6 2023-08-05 05:02:58.000000 dxlib-0.3.0/dxlib.egg-info/top_level.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       38 2023-08-05 05:03:00.155438 dxlib-0.3.0/setup.cfg
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1328 2023-07-15 07:44:19.000000 dxlib-0.3.0/setup.py
```

### Comparing `dxlib-0.2.7/LICENSE` & `dxlib-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.7/PKG-INFO` & `dxlib-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxlib
-Version: 0.2.7
+Version: 0.3.0
 Summary: Quantitative Methods for Finance
 Home-page: https://github.com/delphos-quant/dxlib
 Author: Rafael Zimmer
 Author-email: rzimmerde@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dxlib-0.2.7/README.md` & `dxlib-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.7/dxlib/api/alphavantage.py` & `dxlib-0.3.0/dxlib/api/alphavantage.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.7/dxlib/api/core.py` & `dxlib-0.3.0/dxlib/api/request.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.7/dxlib/core/options.py` & `dxlib-0.3.0/dxlib/core/options.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.7/dxlib/data/utils.py` & `dxlib-0.3.0/dxlib/data/utils.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.7/dxlib/db/__init__.py` & `dxlib-0.3.0/dxlib/db/__init__.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.7/dxlib/db/sql/queries.py` & `dxlib-0.3.0/dxlib/db/sql/queries.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.7/dxlib/db/utils.py` & `dxlib-0.3.0/dxlib/db/utils.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.7/dxlib/portfolio_theory_module.py` & `dxlib-0.3.0/dxlib/portfolio_theory_module.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.7/dxlib/simulation/backtesting.py` & `dxlib-0.3.0/dxlib/simulation/backtesting.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.7/dxlib.egg-info/PKG-INFO` & `dxlib-0.3.0/dxlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxlib
-Version: 0.2.7
+Version: 0.3.0
 Summary: Quantitative Methods for Finance
 Home-page: https://github.com/delphos-quant/dxlib
 Author: Rafael Zimmer
 Author-email: rzimmerde@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dxlib-0.2.7/dxlib.egg-info/SOURCES.txt` & `dxlib-0.3.0/dxlib.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 LICENSE
 README.md
 setup.py
 dxlib/__init__.py
 dxlib/portfolio_theory_module.py
-dxlib/test.py
 dxlib.egg-info/PKG-INFO
 dxlib.egg-info/SOURCES.txt
 dxlib.egg-info/dependency_links.txt
 dxlib.egg-info/requires.txt
 dxlib.egg-info/top_level.txt
 dxlib/api/__init__.py
 dxlib/api/alpaca_markets.py
 dxlib/api/alphavantage.py
-dxlib/api/core.py
-dxlib/api/logger.py
-dxlib/api/terminal.py
+dxlib/api/request.py
 dxlib/core/__init__.py
-dxlib/core/euler_method.py
-dxlib/core/finite_differences.py
+dxlib/core/history.py
+dxlib/core/logger.py
 dxlib/core/options.py
+dxlib/core/portfolio.py
+dxlib/core/security.py
 dxlib/data/__init__.py
 dxlib/data/utils.py
 dxlib/db/__init__.py
 dxlib/db/utils.py
 dxlib/db/sql/__init__.py
 dxlib/db/sql/create.py
 dxlib/db/sql/queries.py
-dxlib/models/__init__.py
-dxlib/models/systematic_trading.py
 dxlib/research/__init__.py
 dxlib/simulation/__init__.py
 dxlib/simulation/backtesting.py
+dxlib/simulation/simulate.py
+dxlib/strategies/__init__.py
+dxlib/strategies/euler_method.py
+dxlib/strategies/finite_differences.py
+dxlib/strategies/systematic_trading.py
 dxlib/visualization/__init__.py
```

### Comparing `dxlib-0.2.7/setup.py` & `dxlib-0.3.0/setup.py`

 * *Files identical despite different names*

