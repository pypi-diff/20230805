# Comparing `tmp/pih-1.48040.tar.gz` & `tmp/pih-1.48041.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.48040.tar", last modified: Sat Aug  5 15:02:06 2023, max compression
+gzip compressed data, was "pih-1.48041.tar", last modified: Sat Aug  5 15:03:58 2023, max compression
```

## Comparing `pih-1.48040.tar` & `pih-1.48041.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 15:02:06.556769 pih-1.48040/
--rw-rw-rw-   0        0        0      261 2023-08-05 15:02:06.556769 pih-1.48040/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-05 15:02:06.289438 pih-1.48040/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.48040/pih/__init__.py
--rw-rw-rw-   0        0        0    20623 2023-08-04 07:31:27.000000 pih-1.48040/pih/collection.py
--rw-rw-rw-   0        0        0    60496 2023-08-05 14:50:54.000000 pih-1.48040/pih/console_api.py
--rw-rw-rw-   0        0        0   109843 2023-08-05 14:58:20.000000 pih-1.48040/pih/const.py
--rw-rw-rw-   0        0        0   321323 2023-08-05 15:01:33.000000 pih-1.48040/pih/pih.py
--rw-rw-rw-   0        0        0    25353 2023-08-05 12:39:59.000000 pih-1.48040/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.48040/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.48040/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2528 2023-08-05 13:46:18.000000 pih-1.48040/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6492 2023-08-03 06:51:54.000000 pih-1.48040/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.48040/pih/service_example.py
--rw-rw-rw-   0        0        0    38354 2023-08-05 14:56:00.000000 pih-1.48040/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.48040/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-08-05 15:02:06.494255 pih-1.48040/pih.egg-info/
--rw-rw-rw-   0        0        0      261 2023-08-05 15:02:04.000000 pih-1.48040/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-08-05 15:02:05.000000 pih-1.48040/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 15:02:04.000000 pih-1.48040/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-08-05 15:02:04.000000 pih-1.48040/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-08-05 15:02:04.000000 pih-1.48040/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2007 2023-08-03 07:28:58.000000 pih-1.48040/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-08-05 15:02:06.556769 pih-1.48040/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-05 15:03:56.635066 pih-1.48041/
+-rw-rw-rw-   0        0        0      261 2023-08-05 15:03:58.361281 pih-1.48041/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-05 15:03:58.064061 pih-1.48041/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.48041/pih/__init__.py
+-rw-rw-rw-   0        0        0    20623 2023-08-04 07:31:27.000000 pih-1.48041/pih/collection.py
+-rw-rw-rw-   0        0        0    60496 2023-08-05 14:50:54.000000 pih-1.48041/pih/console_api.py
+-rw-rw-rw-   0        0        0   109843 2023-08-05 14:58:20.000000 pih-1.48041/pih/const.py
+-rw-rw-rw-   0        0        0   321323 2023-08-05 15:03:45.000000 pih-1.48041/pih/pih.py
+-rw-rw-rw-   0        0        0    25353 2023-08-05 12:39:59.000000 pih-1.48041/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.48041/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.48041/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2528 2023-08-05 13:46:18.000000 pih-1.48041/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6492 2023-08-03 06:51:54.000000 pih-1.48041/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.48041/pih/service_example.py
+-rw-rw-rw-   0        0        0    38354 2023-08-05 14:56:00.000000 pih-1.48041/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.48041/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-08-05 15:03:58.298763 pih-1.48041/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-08-05 15:03:55.000000 pih-1.48041/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-08-05 15:03:56.000000 pih-1.48041/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 15:03:55.000000 pih-1.48041/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-08-05 15:03:56.000000 pih-1.48041/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-05 15:03:56.000000 pih-1.48041/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2007 2023-08-03 07:28:58.000000 pih-1.48041/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-08-05 15:03:58.376978 pih-1.48041/setup.cfg
```

### Comparing `pih-1.48040/pih/collection.py` & `pih-1.48041/pih/collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.48040/pih/console_api.py` & `pih-1.48041/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-1.48040/pih/const.py` & `pih-1.48041/pih/const.py`

 * *Files identical despite different names*

### Comparing `pih-1.48040/pih/pih.py` & `pih-1.48041/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -1648,15 +1648,15 @@
                     handler(message, close_handler)  
             PIH.EVENT.waiting_for_mobile_helper_message_input(
                 recipient, internal_handler)
             return PIH.MIO.ANSWER[recipient][-1] 
 
     class VERSION:
 
-        value: str = "1.48040"
+        value: str = "1.48041"
 
         @staticmethod
         def need_update() -> bool:
             return False
             #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.value < PIH.VERSION.remote()
     
     class INPUT_WAIT:
```

### Comparing `pih-1.48040/pih/rpc.py` & `pih-1.48041/pih/rpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.48040/pih/rpcCommandCall_pb2.py` & `pih-1.48041/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.48040/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.48041/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.48040/pih/rpc_collection.py` & `pih-1.48041/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.48040/pih/rpc_const.py` & `pih-1.48041/pih/rpc_const.py`

 * *Files identical despite different names*

### Comparing `pih-1.48040/pih/service_example.py` & `pih-1.48041/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.48040/pih/tools.py` & `pih-1.48041/pih/tools.py`

 * *Files identical despite different names*

### Comparing `pih-1.48040/pih/widgets.py` & `pih-1.48041/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.48040/pih_setup.py` & `pih-1.48041/pih_setup.py`

 * *Files identical despite different names*

