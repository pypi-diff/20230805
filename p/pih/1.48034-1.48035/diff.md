# Comparing `tmp/pih-1.48034.tar.gz` & `tmp/pih-1.48035.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.48034.tar", last modified: Fri Aug  4 01:33:29 2023, max compression
+gzip compressed data, was "pih-1.48035.tar", last modified: Fri Aug  4 02:07:09 2023, max compression
```

## Comparing `pih-1.48034.tar` & `pih-1.48035.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 01:33:17.897314 pih-1.48034/
--rw-rw-rw-   0        0        0      261 2023-08-04 01:33:29.763343 pih-1.48034/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-04 01:33:27.368146 pih-1.48034/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.48034/pih/__init__.py
--rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.48034/pih/collection.py
--rw-rw-rw-   0        0        0    60753 2023-08-04 00:59:36.000000 pih-1.48034/pih/console_api.py
--rw-rw-rw-   0        0        0   109574 2023-08-04 01:03:56.000000 pih-1.48034/pih/const.py
--rw-rw-rw-   0        0        0   320963 2023-08-04 01:32:24.000000 pih-1.48034/pih/pih.py
--rw-rw-rw-   0        0        0    25242 2023-08-03 08:55:57.000000 pih-1.48034/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.48034/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.48034/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2528 2023-08-03 23:30:35.000000 pih-1.48034/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6492 2023-08-03 06:51:54.000000 pih-1.48034/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.48034/pih/service_example.py
--rw-rw-rw-   0        0        0    38338 2023-08-04 01:31:31.000000 pih-1.48034/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.48034/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-08-04 01:33:29.482095 pih-1.48034/pih.egg-info/
--rw-rw-rw-   0        0        0      261 2023-08-04 01:33:16.000000 pih-1.48034/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-08-04 01:33:17.000000 pih-1.48034/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 01:33:16.000000 pih-1.48034/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-08-04 01:33:16.000000 pih-1.48034/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-08-04 01:33:16.000000 pih-1.48034/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2007 2023-08-03 07:28:58.000000 pih-1.48034/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-08-04 01:33:29.810218 pih-1.48034/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 02:07:10.152557 pih-1.48035/
+-rw-rw-rw-   0        0        0      261 2023-08-04 02:07:10.168187 pih-1.48035/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-04 02:07:09.869509 pih-1.48035/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.48035/pih/__init__.py
+-rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.48035/pih/collection.py
+-rw-rw-rw-   0        0        0    60753 2023-08-04 00:59:36.000000 pih-1.48035/pih/console_api.py
+-rw-rw-rw-   0        0        0   109574 2023-08-04 01:03:56.000000 pih-1.48035/pih/const.py
+-rw-rw-rw-   0        0        0   320958 2023-08-04 02:06:50.000000 pih-1.48035/pih/pih.py
+-rw-rw-rw-   0        0        0    25372 2023-08-04 02:02:54.000000 pih-1.48035/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.48035/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.48035/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2528 2023-08-03 23:30:35.000000 pih-1.48035/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6492 2023-08-03 06:51:54.000000 pih-1.48035/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.48035/pih/service_example.py
+-rw-rw-rw-   0        0        0    38338 2023-08-04 01:31:31.000000 pih-1.48035/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.48035/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-08-04 02:07:10.121832 pih-1.48035/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-08-04 02:07:07.000000 pih-1.48035/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-08-04 02:07:08.000000 pih-1.48035/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 02:07:07.000000 pih-1.48035/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-08-04 02:07:08.000000 pih-1.48035/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-04 02:07:08.000000 pih-1.48035/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2007 2023-08-03 07:28:58.000000 pih-1.48035/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-08-04 02:07:10.168187 pih-1.48035/setup.cfg
```

### Comparing `pih-1.48034/pih/collection.py` & `pih-1.48035/pih/collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.48034/pih/console_api.py` & `pih-1.48035/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-1.48034/pih/const.py` & `pih-1.48035/pih/const.py`

 * *Files identical despite different names*

### Comparing `pih-1.48034/pih/pih.py` & `pih-1.48035/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -624,15 +624,15 @@
     @property
     def arg_namespace(self) -> Namespace:
         return self.arg_parser.parse_args()
 
     def named_arg(self, name: str) -> str | None:
         return self.arg_parser.parse_args().__getattribute__(name)
     
-    def add_argument(self, *args, **kwargs) -> None:
+    def add_arg(self, *args, **kwargs) -> None:
         if DataTool.is_none(self.arg_parser):
             self.arg_parser = ArgumentParser(description="Service help")
         self.arg_parser.add_argument(*args, **kwargs)
     
     @property
     def file_path(self) -> str:
         return sys.argv[0]
@@ -1648,15 +1648,15 @@
                     handler(message, close_handler)  
             PIH.EVENT.waiting_for_mobile_helper_message_input(
                 recipient, internal_handler)
             return PIH.MIO.ANSWER[recipient][-1] 
 
     class VERSION:
 
-        value: str = "1.48034"
+        value: str = "1.48035"
 
         @staticmethod
         def need_update() -> bool:
             return False
             #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.value < PIH.VERSION.remote()
     
     class INPUT_WAIT:
```

### Comparing `pih-1.48034/pih/rpc.py` & `pih-1.48035/pih/rpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,19 +270,21 @@
                 A = sys.modules["pih.pih"].A
 
             max_workers = max_workers or RPC.Service.MAX_WORKERS
             service_description: ServiceDescription = role_or_information if isinstance(
                 role_or_information, ServiceInformationBase) else A.CT_SR.description(role_or_information)
             self.description = service_description
             arg_name: str = "isolated"
-            A.SE.add_argument(j(("--", arg_name)),
+            A.SE.add_arg(j(("--", arg_name)),
                             help="Service isolated flag", nargs="?", const=1, type=str, default=None)
             isolate_arg: str | None = None
             try:
-                isolate_arg = A.SE.named_arg(arg_name).lower()
+                isolated_arg_value: str | None = A.SE.named_arg(arg_name)
+                if A.D.is_not_none(isolated_arg_value):
+                    isolate_arg = str(isolated_arg_value).lower()
             except AttributeError as error:
                 pass
             if A.D.is_not_none(isolate_arg):
                 if A.D.is_none(self.description.isolated):
                     self.description.isolated = isolate_arg not in ["0", "no", "false"]
                 elif self.description.isolated:
                     self.description.isolated = isolate_arg not in [
```

### Comparing `pih-1.48034/pih/rpcCommandCall_pb2.py` & `pih-1.48035/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.48034/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.48035/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.48034/pih/rpc_collection.py` & `pih-1.48035/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.48034/pih/rpc_const.py` & `pih-1.48035/pih/rpc_const.py`

 * *Files identical despite different names*

### Comparing `pih-1.48034/pih/service_example.py` & `pih-1.48035/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.48034/pih/tools.py` & `pih-1.48035/pih/tools.py`

 * *Files identical despite different names*

### Comparing `pih-1.48034/pih/widgets.py` & `pih-1.48035/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.48034/pih_setup.py` & `pih-1.48035/pih_setup.py`

 * *Files identical despite different names*

