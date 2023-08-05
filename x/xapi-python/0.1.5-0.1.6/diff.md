# Comparing `tmp/xapi-python-0.1.5.tar.gz` & `tmp/xapi-python-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xapi-python-0.1.5.tar", last modified: Sat Jul 22 16:45:30 2023, max compression
+gzip compressed data, was "xapi-python-0.1.6.tar", last modified: Sat Aug  5 17:22:16 2023, max compression
```

## Comparing `xapi-python-0.1.5.tar` & `xapi-python-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-07-22 16:45:30.733108 xapi-python-0.1.5/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1071 2023-04-25 04:51:26.000000 xapi-python-0.1.5/LICENSE
--rw-r--r--   0 pawel     (1000) pawel     (1000)     8259 2023-07-22 16:45:30.733108 xapi-python-0.1.5/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)     5954 2023-06-18 12:21:54.000000 xapi-python-0.1.5/README.md
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1131 2023-07-22 16:38:38.000000 xapi-python-0.1.5/pyproject.toml
--rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2023-07-22 16:45:30.733108 xapi-python-0.1.5/setup.cfg
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1027 2023-07-22 16:38:48.000000 xapi-python-0.1.5/setup.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-07-22 16:45:30.733108 xapi-python-0.1.5/tests/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     5768 2023-07-22 16:37:07.000000 xapi-python-0.1.5/tests/test_connection.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     7958 2023-04-26 11:15:10.000000 xapi-python-0.1.5/tests/test_socket.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     4014 2023-04-27 05:35:22.000000 xapi-python-0.1.5/tests/test_stream.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1566 2023-04-29 10:20:03.000000 xapi-python-0.1.5/tests/test_xapi.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-07-22 16:45:30.733108 xapi-python-0.1.5/xapi/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      338 2023-07-22 16:38:27.000000 xapi-python-0.1.5/xapi/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2361 2023-07-22 16:32:36.000000 xapi-python-0.1.5/xapi/connection.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1464 2023-04-24 14:52:49.000000 xapi-python-0.1.5/xapi/enums.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      205 2023-04-29 11:41:41.000000 xapi-python-0.1.5/xapi/exceptions.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     6640 2023-04-29 11:38:37.000000 xapi-python-0.1.5/xapi/socket.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2947 2023-04-29 11:39:31.000000 xapi-python-0.1.5/xapi/stream.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2209 2023-05-03 10:23:56.000000 xapi-python-0.1.5/xapi/xapi.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-07-22 16:45:30.733108 xapi-python-0.1.5/xapi_python.egg-info/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     8259 2023-07-22 16:45:30.000000 xapi-python-0.1.5/xapi_python.egg-info/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)      413 2023-07-22 16:45:30.000000 xapi-python-0.1.5/xapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2023-07-22 16:45:30.000000 xapi-python-0.1.5/xapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       19 2023-07-22 16:45:30.000000 xapi-python-0.1.5/xapi_python.egg-info/requires.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        5 2023-07-22 16:45:30.000000 xapi-python-0.1.5/xapi_python.egg-info/top_level.txt
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-08-05 17:22:16.321906 xapi-python-0.1.6/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1071 2023-04-25 04:51:26.000000 xapi-python-0.1.6/LICENSE
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     8198 2023-08-05 17:22:16.321906 xapi-python-0.1.6/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     5893 2023-08-05 16:11:56.000000 xapi-python-0.1.6/README.md
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1131 2023-08-05 16:11:03.000000 xapi-python-0.1.6/pyproject.toml
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2023-08-05 17:22:16.321906 xapi-python-0.1.6/setup.cfg
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1027 2023-08-05 16:10:44.000000 xapi-python-0.1.6/setup.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-08-05 17:22:16.321906 xapi-python-0.1.6/tests/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     7276 2023-08-05 17:11:36.000000 xapi-python-0.1.6/tests/test_connection.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     7958 2023-04-26 11:15:10.000000 xapi-python-0.1.6/tests/test_socket.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4014 2023-04-27 05:35:22.000000 xapi-python-0.1.6/tests/test_stream.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1566 2023-04-29 10:20:03.000000 xapi-python-0.1.6/tests/test_xapi.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-08-05 17:22:16.321906 xapi-python-0.1.6/xapi/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      338 2023-08-05 16:11:09.000000 xapi-python-0.1.6/xapi/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2657 2023-08-05 17:14:37.000000 xapi-python-0.1.6/xapi/connection.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1464 2023-04-24 14:52:49.000000 xapi-python-0.1.6/xapi/enums.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      205 2023-04-29 11:41:41.000000 xapi-python-0.1.6/xapi/exceptions.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     6640 2023-04-29 11:38:37.000000 xapi-python-0.1.6/xapi/socket.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2947 2023-04-29 11:39:31.000000 xapi-python-0.1.6/xapi/stream.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2209 2023-05-03 10:23:56.000000 xapi-python-0.1.6/xapi/xapi.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-08-05 17:22:16.321906 xapi-python-0.1.6/xapi_python.egg-info/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     8198 2023-08-05 17:22:16.000000 xapi-python-0.1.6/xapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      413 2023-08-05 17:22:16.000000 xapi-python-0.1.6/xapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2023-08-05 17:22:16.000000 xapi-python-0.1.6/xapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       19 2023-08-05 17:22:16.000000 xapi-python-0.1.6/xapi_python.egg-info/requires.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        5 2023-08-05 17:22:16.000000 xapi-python-0.1.6/xapi_python.egg-info/top_level.txt
```

### Comparing `xapi-python-0.1.5/LICENSE` & `xapi-python-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.5/PKG-INFO` & `xapi-python-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xapi-python
-Version: 0.1.5
+Version: 0.1.6
 Summary: The xStation5 API Python library
 Home-page: https://github.com/pawelkn/xapi-python
 Author: Paweł Knioła
 Author-email: Paweł Knioła <pawel.kn@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Paweł Knioła
@@ -220,8 +220,8 @@
 git clone https://github.com/pawelkn/xapi-python.git
 cd xapi-python
 python3 -m unittest discover tests
 ```
 
 ## Buy Me A Coffee! ☕
 
-If you find the project beneficial and would like to support me, please consider showing your appreciation by buying me a coffee on [Buy Me A Coffee](https://www.buymeacoffee.com/pawelkn) or [Buy Coffee Poland](https://buycoffee.to/pawelkn)
+If you find the project beneficial and would like to support me, please consider showing your appreciation by buying me a coffee on [Buy Me A Coffee](https://buycoffee.to/pawelkn)
```

### Comparing `xapi-python-0.1.5/README.md` & `xapi-python-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -176,8 +176,8 @@
 git clone https://github.com/pawelkn/xapi-python.git
 cd xapi-python
 python3 -m unittest discover tests
 ```
 
 ## Buy Me A Coffee! ☕
 
-If you find the project beneficial and would like to support me, please consider showing your appreciation by buying me a coffee on [Buy Me A Coffee](https://www.buymeacoffee.com/pawelkn) or [Buy Coffee Poland](https://buycoffee.to/pawelkn)
+If you find the project beneficial and would like to support me, please consider showing your appreciation by buying me a coffee on [Buy Me A Coffee](https://buycoffee.to/pawelkn)
```

### Comparing `xapi-python-0.1.5/pyproject.toml` & `xapi-python-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xapi-python"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Paweł Knioła", email="pawel.kn@gmail.com" },
 ]
 description = "The xStation5 API Python library"
 keywords = [
   "python", "python3", "bitcoin", "trading", "websocket", "trading-api", "forex", "xapi", "forex-trading",
   "exchange-api", "forex-data", "xstation", "xstation5", "xtb", "xopenhub", "forex-api", "xopenhub-api",
```

### Comparing `xapi-python-0.1.5/setup.py` & `xapi-python-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,10 +16,10 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12"
     ],
     python_requires='>=3.7',
-    version="0.1.5",
+    version="0.1.6",
     packages=['xapi'],
 )
```

### Comparing `xapi-python-0.1.5/tests/test_socket.py` & `xapi-python-0.1.6/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.5/tests/test_stream.py` & `xapi-python-0.1.6/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.5/tests/test_xapi.py` & `xapi-python-0.1.6/tests/test_xapi.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.5/xapi/connection.py` & `xapi-python-0.1.6/xapi/connection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from .exceptions import ConnectionClosed
 
 import websockets.client
 import websockets.exceptions
 import socket
 import asyncio
 import json
+import time
 
 class Connection():
     def __init__(self):
         self.safe = False
         self._conn = None
         self._lock = asyncio.Lock()
+        self._last_request_time = None
 
     async def connect(self, url):
         try:
             self._conn = await websockets.client.connect(url, close_timeout=0, max_size=None)
 
         except websockets.exceptions.WebSocketException as e:
             raise ConnectionClosed(f"WebSocket exception: {e}")
@@ -47,29 +49,35 @@
                 raise ConnectionClosed("Not connected")
 
         except websockets.exceptions.WebSocketException as e:
             self._conn = None
             raise ConnectionClosed(f"WebSocket exception: {e}")
 
     async def _request(self, command):
+        if self._last_request_time is not None:
+            elapsed_time = time.time() - self._last_request_time
+            if elapsed_time < 0.2:
+                await asyncio.sleep(0.2 - elapsed_time)
+
         try:
             if self._conn:
                 await self._conn.send(json.dumps(command))
+                self._last_request_time = time.time()
             else:
                 raise ConnectionClosed("Not connected")
 
         except websockets.exceptions.WebSocketException as e:
             self._conn = None
             raise ConnectionClosed(f"WebSocket exception: {e}")
 
     async def _transaction(self, command):
         async with self._lock:
             try:
                 if self._conn:
-                    await self._conn.send(json.dumps(command))
+                    await self._request(command)
                     response = await self._conn.recv()
                     return json.loads(response)
                 else:
                     raise ConnectionClosed("Not connected")
 
             except websockets.exceptions.WebSocketException as e:
                 self._conn = None
```

### Comparing `xapi-python-0.1.5/xapi/enums.py` & `xapi-python-0.1.6/xapi/enums.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.5/xapi/socket.py` & `xapi-python-0.1.6/xapi/socket.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.5/xapi/stream.py` & `xapi-python-0.1.6/xapi/stream.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.5/xapi/xapi.py` & `xapi-python-0.1.6/xapi/xapi.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.5/xapi_python.egg-info/PKG-INFO` & `xapi-python-0.1.6/xapi_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xapi-python
-Version: 0.1.5
+Version: 0.1.6
 Summary: The xStation5 API Python library
 Home-page: https://github.com/pawelkn/xapi-python
 Author: Paweł Knioła
 Author-email: Paweł Knioła <pawel.kn@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Paweł Knioła
@@ -220,8 +220,8 @@
 git clone https://github.com/pawelkn/xapi-python.git
 cd xapi-python
 python3 -m unittest discover tests
 ```
 
 ## Buy Me A Coffee! ☕
 
-If you find the project beneficial and would like to support me, please consider showing your appreciation by buying me a coffee on [Buy Me A Coffee](https://www.buymeacoffee.com/pawelkn) or [Buy Coffee Poland](https://buycoffee.to/pawelkn)
+If you find the project beneficial and would like to support me, please consider showing your appreciation by buying me a coffee on [Buy Me A Coffee](https://buycoffee.to/pawelkn)
```

