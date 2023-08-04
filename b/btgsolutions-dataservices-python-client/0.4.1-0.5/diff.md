# Comparing `tmp/btgsolutions-dataservices-python-client-0.4.1.tar.gz` & `tmp/btgsolutions-dataservices-python-client-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/btgsolutions-dataservices-python-client-0.4.1.tar", last modified: Mon Jul 31 14:00:24 2023, max compression
+gzip compressed data, was "dist/btgsolutions-dataservices-python-client-0.5.tar", last modified: Fri Aug  4 22:05:43 2023, max compression
```

## Comparing `btgsolutions-dataservices-python-client-0.4.1.tar` & `btgsolutions-dataservices-python-client-0.5.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-31 14:00:24.000000 btgsolutions-dataservices-python-client-0.4.1/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       24 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.4.1/MANIFEST.in
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2110 2023-07-31 14:00:24.000000 btgsolutions-dataservices-python-client-0.4.1/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1385 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.4.1/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-31 14:00:24.000000 btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       93 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1575 2023-07-31 13:58:23.000000 btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices/config.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      599 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices/exceptions.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-31 14:00:24.000000 btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices/rest/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      136 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices/rest/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1363 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices/rest/authenticator.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3001 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices/rest/historical_candles.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5752 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices/rest/intraday_candles.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-31 14:00:24.000000 btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices/websocket/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       45 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices/websocket/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7985 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices/websocket/websocket_client.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      270 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices/websocket/websocket_default_functions.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-31 14:00:24.000000 btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices_python_client.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2110 2023-07-31 14:00:24.000000 btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices_python_client.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      841 2023-07-31 14:00:24.000000 btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices_python_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-31 14:00:24.000000 btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices_python_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       68 2023-07-31 14:00:24.000000 btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices_python_client.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       26 2023-07-31 14:00:24.000000 btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices_python_client.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       67 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.4.1/requirements.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-07-31 14:00:24.000000 btgsolutions-dataservices-python-client-0.4.1/setup.cfg
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     1272 2023-07-31 13:58:25.000000 btgsolutions-dataservices-python-client-0.4.1/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-04 22:05:43.000000 btgsolutions-dataservices-python-client-0.5/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       24 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5/MANIFEST.in
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2108 2023-08-04 22:05:43.000000 btgsolutions-dataservices-python-client-0.5/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1385 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5/README.md
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-04 22:05:43.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       93 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1642 2023-08-04 21:57:33.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/config.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      599 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/exceptions.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-04 22:05:43.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/rest/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      168 2023-08-04 19:36:26.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/rest/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1363 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/rest/authenticator.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2646 2023-08-04 22:05:02.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/rest/bulk_data.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3001 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/rest/historical_candles.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5752 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/rest/intraday_candles.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-04 22:05:43.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/websocket/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       45 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/websocket/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7985 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/websocket/websocket_client.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      270 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/websocket/websocket_default_functions.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-04 22:05:43.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices_python_client.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2108 2023-08-04 22:05:43.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices_python_client.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      885 2023-08-04 22:05:43.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices_python_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-08-04 22:05:43.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices_python_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       68 2023-08-04 22:05:43.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices_python_client.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       26 2023-08-04 22:05:43.000000 btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices_python_client.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       67 2023-07-27 17:34:22.000000 btgsolutions-dataservices-python-client-0.5/requirements.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-08-04 22:05:43.000000 btgsolutions-dataservices-python-client-0.5/setup.cfg
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     1270 2023-08-04 22:05:30.000000 btgsolutions-dataservices-python-client-0.5/setup.py
```

### Comparing `btgsolutions-dataservices-python-client-0.4.1/PKG-INFO` & `btgsolutions-dataservices-python-client-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btgsolutions-dataservices-python-client
-Version: 0.4.1
+Version: 0.5
 Summary: Python package containing several classes and data for extracting and manipulating market and trading data.
 Home-page: https://github.com/BTG-Pactual-Solutions/btgsolutions-dataservices-python-client
 Author: BTG Solutions Data Services powered by BTG Pactual Solutions
 License: UNKNOWN
 Description: # BTG Solutions - Data Service
         
         It's a Python library to get Brazilian Financial Market Data.
```

### Comparing `btgsolutions-dataservices-python-client-0.4.1/README.md` & `btgsolutions-dataservices-python-client-0.5/README.md`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices/config.py` & `btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,8 +29,9 @@
     return list(set(socket_urls[f'{feed}_{target}']))
 
 
 
 MAX_WS_RECONNECT_RETRIES = 5
 
 ### Rest
-url_apis = "https://dataservices.btgpactualsolutions.com/api/v2"
+url_apis = "https://dataservices.btgpactualsolutions.com/api/v2"
+url_api_v1 = "https://dataservices.btgpactualsolutions.com/api/v1"
```

### Comparing `btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices/exceptions.py` & `btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/exceptions.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices/rest/authenticator.py` & `btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/rest/authenticator.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices/rest/historical_candles.py` & `btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/rest/historical_candles.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices/rest/intraday_candles.py` & `btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/rest/intraday_candles.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices/websocket/websocket_client.py` & `btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices/websocket/websocket_client.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices_python_client.egg-info/PKG-INFO` & `btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices_python_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btgsolutions-dataservices-python-client
-Version: 0.4.1
+Version: 0.5
 Summary: Python package containing several classes and data for extracting and manipulating market and trading data.
 Home-page: https://github.com/BTG-Pactual-Solutions/btgsolutions-dataservices-python-client
 Author: BTG Solutions Data Services powered by BTG Pactual Solutions
 License: UNKNOWN
 Description: # BTG Solutions - Data Service
         
         It's a Python library to get Brazilian Financial Market Data.
```

### Comparing `btgsolutions-dataservices-python-client-0.4.1/btgsolutions_dataservices_python_client.egg-info/SOURCES.txt` & `btgsolutions-dataservices-python-client-0.5/btgsolutions_dataservices_python_client.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 requirements.txt
 setup.py
 btgsolutions_dataservices/__init__.py
 btgsolutions_dataservices/config.py
 btgsolutions_dataservices/exceptions.py
 btgsolutions_dataservices/rest/__init__.py
 btgsolutions_dataservices/rest/authenticator.py
+btgsolutions_dataservices/rest/bulk_data.py
 btgsolutions_dataservices/rest/historical_candles.py
 btgsolutions_dataservices/rest/intraday_candles.py
 btgsolutions_dataservices/websocket/__init__.py
 btgsolutions_dataservices/websocket/websocket_client.py
 btgsolutions_dataservices/websocket/websocket_default_functions.py
 btgsolutions_dataservices_python_client.egg-info/PKG-INFO
 btgsolutions_dataservices_python_client.egg-info/SOURCES.txt
```

### Comparing `btgsolutions-dataservices-python-client-0.4.1/setup.py` & `btgsolutions-dataservices-python-client-0.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         with open(requirementPath) as f:
             install_requires = f.read().splitlines()
 
 description = "Python package containing several classes and data for extracting and manipulating market and trading data."
 
 setup(
     name='btgsolutions-dataservices-python-client',
-    version='0.4.1',
+    version='0.5',
     description=description,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="BTG Solutions Data Services powered by BTG Pactual Solutions",
     packages=find_packages(),
     url="https://github.com/BTG-Pactual-Solutions/btgsolutions-dataservices-python-client",
     install_requires=install_requires,
```

