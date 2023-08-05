# Comparing `tmp/tm_remote_build-1.3.0.tar.gz` & `tmp/tm_remote_build-2.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tm_remote_build-1.3.0.tar", max compression
+gzip compressed data, was "tm_remote_build-2.0.0.dev1.tar", max compression
```

## Comparing `tm_remote_build-1.3.0.tar` & `tm_remote_build-2.0.0.dev1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-03-12 18:58:59.671309 tm_remote_build-1.3.0/license
--rw-r--r--   0        0        0      555 2023-03-13 22:21:54.651281 tm_remote_build-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     1398 2023-03-13 22:21:54.651281 tm_remote_build-1.3.0/readme.md
--rw-r--r--   0        0        0     1654 2023-03-13 22:21:54.652283 tm_remote_build-1.3.0/src/tm_remote_build/__init__.py
--rw-r--r--   0        0        0     5811 2023-03-12 23:57:03.483493 tm_remote_build-1.3.0/src/tm_remote_build/api.py
--rw-r--r--   0        0        0     2561 2023-03-13 22:21:54.653281 tm_remote_build-1.3.0/src/tm_remote_build/cli.py
--rw-r--r--   0        0        0     1803 2023-03-12 21:18:15.263792 tm_remote_build-1.3.0/src/tm_remote_build/log.py
--rw-r--r--   0        0        0     1915 1970-01-01 00:00:00.000000 tm_remote_build-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-03-12 18:58:59.671309 tm_remote_build-2.0.0.dev1/license
+-rw-r--r--   0        0        0      560 2023-08-05 19:40:54.132998 tm_remote_build-2.0.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0      602 2023-08-05 14:24:07.034266 tm_remote_build-2.0.0.dev1/readme.md
+-rw-r--r--   0        0        0        0 2023-08-05 02:31:58.347902 tm_remote_build-2.0.0.dev1/src/tm_remote_build/__init__.py
+-rw-r--r--   0        0        0     4938 2023-08-05 10:46:31.205895 tm_remote_build-2.0.0.dev1/src/tm_remote_build/api.py
+-rw-r--r--   0        0        0     3541 2023-08-05 14:05:59.253273 tm_remote_build-2.0.0.dev1/src/tm_remote_build/cli.py
+-rw-r--r--   0        0        0     2283 2023-08-05 14:11:30.806732 tm_remote_build-2.0.0.dev1/src/tm_remote_build/log.py
+-rw-r--r--   0        0        0     1150 1970-01-01 00:00:00.000000 tm_remote_build-2.0.0.dev1/PKG-INFO
```

### Comparing `tm_remote_build-1.3.0/license` & `tm_remote_build-2.0.0.dev1/license`

 * *Files identical despite different names*

### Comparing `tm_remote_build-1.3.0/pyproject.toml` & `tm_remote_build-2.0.0.dev1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "tm-remote-build"
-version = "1.3.0"
+version = "2.0.0-dev1"
 description = "Build and deploy openplanet scripts"
 authors = ["skybaks <tmflame@gmail.com>"]
 readme = "readme.md"
 packages = [{include="tm_remote_build", from="src"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `tm_remote_build-1.3.0/src/tm_remote_build/api.py` & `tm_remote_build-2.0.0.dev1/src/tm_remote_build/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -72,32 +72,29 @@
         if len(data_bytes) > data_length:
             logger.debug("Trimming data")
             data_bytes = data_bytes[0:data_length]
         return data_bytes.decode()
 
 
 class RemoteBuildAPI:
-    def __init__(self, game: str, port: int) -> None:
-        self.game = game
+    def __init__(self, port: int) -> None:
         self.openplanet = OpenplanetTcpSocket(port)
         self.data_folder = ""
-        self.app_folder = ""
         self.op_log = OpenplanetLog()
-        self.logger = logging.getLogger(__name__ + self.game)
-        self.logger.init_game_name(self.game)
+        self.get_data_folder()
 
     def send_route(self, route: str, data: dict) -> dict:
         response = {}
         if self.openplanet.try_connect():
             self.openplanet.send({"route": route, "data": data})
             response_text = self.openplanet.receive()
             try:
                 response = json.loads(response_text)
             except Exception as e:
-                self.logger.exception(e)
+                logger.exception(e)
         return response
 
     def get_status(self) -> bool:
         response = self.send_route("get_status", {})
         status = response.get("data", "")
         return status == "Alive"
 
@@ -108,59 +105,39 @@
         response = self.send_route("get_data_folder", {})
         response_data_folder = response.get("data", "")
         if os.path.isdir(response_data_folder):
             self.data_folder = response_data_folder
             self.op_log.set_path(os.path.join(self.data_folder, "Openplanet.log"))
         return self.data_folder != ""
 
-    def get_app_folder(self) -> bool:
-        if not self.get_status():
-            return False
-
-        response = self.send_route("get_app_folder", {})
-        response_app_folder = response.get("data", "")
-        if os.path.isdir(response_app_folder):
-            self.app_folder = response_app_folder
-        return self.app_folder != ""
-
-    def load_plugin(self, plugin_id, plugin_src="user", plugin_type="zip") -> bool:
+    def load_plugin(
+        self, plugin_id: str, plugin_src: str = "user", plugin_type: str = "zip"
+    ) -> bool:
         if not self.get_status():
             return False
 
         self.op_log.start_monitor()
         response = self.send_route(
             "load_plugin",
             {
                 "id": plugin_id,
                 "source": plugin_src,
                 "type": plugin_type,
             },
         )
-        log_msgs = self.op_log.end_monitor()
-        for msg in log_msgs:
-            if msg.source == "ScriptEngine":
-                if ":  ERR :" in msg.text:
-                    self.logger.error(msg.text)
-                elif ": WARN :" in msg.text:
-                    self.logger.warning(msg.text)
-                else:
-                    self.logger.info(msg.text)
+        self.op_log.end_monitor()
         if response:
             if response.get("error", ""):
-                [
-                    self.logger.error(err)
-                    for err in response["error"].strip().split("\n")
-                ]
+                [logger.error(err) for err in response["error"].strip().split("\n")]
         return response.get("error", "") == ""
 
-    def unload_plugin(self, plugin_id) -> bool:
+    def unload_plugin(self, plugin_id: str) -> bool:
         if not self.get_status():
             return False
 
+        self.op_log.start_monitor()
         response = self.send_route("unload_plugin", {"id": plugin_id})
+        self.op_log.end_monitor()
         if response:
             if response.get("error", ""):
-                [
-                    self.logger.error(err)
-                    for err in response["error"].strip().split("\n")
-                ]
+                [logger.error(err) for err in response["error"].strip().split("\n")]
         return response.get("error", "") == ""
```

### Comparing `tm_remote_build-1.3.0/src/tm_remote_build/log.py` & `tm_remote_build-2.0.0.dev1/src/tm_remote_build/log.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import logging
+from colorama import Fore
 
 logger = logging.getLogger(__name__)
 
 
 def _get_next_brackets(log_line, start_offset) -> "tuple[int, str]":
     start_index = log_line.index("[", start_offset)
     end_index = log_line.index("]", start_index)
@@ -34,19 +35,30 @@
         if os.path.isfile(file_path):
             self.file_path = file_path
 
     def start_monitor(self) -> None:
         if not os.path.isfile(self.file_path):
             self.last_len = 0
             return
-        with open(self.file_path, "r") as log_file:
-            self.last_len = len(log_file.read())
-            logger.debug(str(self.last_len))
+        self.last_len = os.stat(self.file_path).st_size
+        logger.debug(str(self.last_len))
 
-    def end_monitor(self) -> "list[OpenplanetLogMessage]":
+    def end_monitor(self, print_msgs: bool = True) -> None:
         if not os.path.isfile(self.file_path):
             return []
         new_lines = []
         with open(self.file_path, "r") as log_file:
-            new_lines = log_file.read()[self.last_len :].splitlines()
+            log_file.seek(self.last_len)
+            new_lines = log_file.read().splitlines()
             logger.debug(str(len(new_lines)) + " new lines found")
-        return [OpenplanetLogMessage(line) for line in new_lines]
+        if print_msgs:
+            log_msgs: "list[OpenplanetLogMessage]" = [
+                OpenplanetLogMessage(line) for line in new_lines
+            ]
+            for msg in log_msgs:
+                if msg.source == "ScriptEngine":
+                    if ":  ERR :" in msg.text:
+                        print(Fore.RED + msg.text + Fore.RESET)
+                    elif ": WARN :" in msg.text:
+                        print(Fore.YELLOW + msg.text + Fore.RESET)
+                    else:
+                        print(msg.text)
```

