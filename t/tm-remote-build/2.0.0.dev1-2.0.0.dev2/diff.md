# Comparing `tmp/tm_remote_build-2.0.0.dev1.tar.gz` & `tmp/tm_remote_build-2.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tm_remote_build-2.0.0.dev1.tar", max compression
+gzip compressed data, was "tm_remote_build-2.0.0.dev2.tar", max compression
```

## Comparing `tm_remote_build-2.0.0.dev1.tar` & `tm_remote_build-2.0.0.dev2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-03-12 18:58:59.671309 tm_remote_build-2.0.0.dev1/license
--rw-r--r--   0        0        0      560 2023-08-05 19:40:54.132998 tm_remote_build-2.0.0.dev1/pyproject.toml
--rw-r--r--   0        0        0      602 2023-08-05 14:24:07.034266 tm_remote_build-2.0.0.dev1/readme.md
--rw-r--r--   0        0        0        0 2023-08-05 02:31:58.347902 tm_remote_build-2.0.0.dev1/src/tm_remote_build/__init__.py
--rw-r--r--   0        0        0     4938 2023-08-05 10:46:31.205895 tm_remote_build-2.0.0.dev1/src/tm_remote_build/api.py
--rw-r--r--   0        0        0     3541 2023-08-05 14:05:59.253273 tm_remote_build-2.0.0.dev1/src/tm_remote_build/cli.py
--rw-r--r--   0        0        0     2283 2023-08-05 14:11:30.806732 tm_remote_build-2.0.0.dev1/src/tm_remote_build/log.py
--rw-r--r--   0        0        0     1150 1970-01-01 00:00:00.000000 tm_remote_build-2.0.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-03-12 18:58:59.671309 tm_remote_build-2.0.0.dev2/license
+-rw-r--r--   0        0        0      560 2023-08-05 19:54:48.303092 tm_remote_build-2.0.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0      602 2023-08-05 14:24:07.034266 tm_remote_build-2.0.0.dev2/readme.md
+-rw-r--r--   0        0        0        0 2023-08-05 02:31:58.347902 tm_remote_build-2.0.0.dev2/src/tm_remote_build/__init__.py
+-rw-r--r--   0        0        0     4938 2023-08-05 10:46:31.205895 tm_remote_build-2.0.0.dev2/src/tm_remote_build/api.py
+-rw-r--r--   0        0        0     3440 2023-08-05 20:14:24.962017 tm_remote_build-2.0.0.dev2/src/tm_remote_build/cli.py
+-rw-r--r--   0        0        0     2283 2023-08-05 14:11:30.806732 tm_remote_build-2.0.0.dev2/src/tm_remote_build/log.py
+-rw-r--r--   0        0        0     1150 1970-01-01 00:00:00.000000 tm_remote_build-2.0.0.dev2/PKG-INFO
```

### Comparing `tm_remote_build-2.0.0.dev1/license` & `tm_remote_build-2.0.0.dev2/license`

 * *Files identical despite different names*

### Comparing `tm_remote_build-2.0.0.dev1/pyproject.toml` & `tm_remote_build-2.0.0.dev2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "tm-remote-build"
-version = "2.0.0-dev1"
+version = "2.0.0-dev2"
 description = "Build and deploy openplanet scripts"
 authors = ["skybaks <tmflame@gmail.com>"]
 readme = "readme.md"
 packages = [{include="tm_remote_build", from="src"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `tm_remote_build-2.0.0.dev1/readme.md` & `tm_remote_build-2.0.0.dev2/readme.md`

 * *Files identical despite different names*

### Comparing `tm_remote_build-2.0.0.dev1/src/tm_remote_build/api.py` & `tm_remote_build-2.0.0.dev2/src/tm_remote_build/api.py`

 * *Files identical despite different names*

### Comparing `tm_remote_build-2.0.0.dev1/src/tm_remote_build/cli.py` & `tm_remote_build-2.0.0.dev2/src/tm_remote_build/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,40 +44,41 @@
         )
 
 
 def main() -> None:
     parser = argparse.ArgumentParser(
         prog="tm-remote-build", description="Load or unload Openplanet plugins"
     )
-    subparser = parser.add_subparsers()
+    subparser = parser.add_subparsers(required=True)
 
     def common_args(sub_input) -> None:
         sub_input.add_argument(
             "plugin_id",
             help="The plugin ID to be targeted. For a folder source plugin this would be the folder name. For a zipped source plugin this would be the filename without extension.",
         )
-        sub_input.add_argument(
+        comm_group = sub_input.add_mutually_exclusive_group(required=True)
+        comm_group.add_argument(
             "-p",
             "--port",
             type=int,
             help="The port used to communicate with Openplanet",
         )
-        sub_input.add_argument(
+        comm_group.add_argument(
             "-op",
             "--openplanet",
             choices=DEFAULT_PORTS.keys(),
             help="Alternative to entering port number. Will use the default port for that game.",
         )
         sub_input.add_argument(
             "-v",
             "--verbose",
             action="store_true",
             help="Enable verbose logging for debugging Remote Build to Openplanet communication",
         )
-        sub_input.description = "Specify at least one of [--port, --openplanet] to enable communication with the Remote Build plugin running in the game. If both are specified, --port will take precedence."
+        sub_input.description = "Specify at one of [--port, --openplanet] to enable communication with the Remote Build plugin running in the game."
 
     sub_unload = subparser.add_parser("unload", help="Unload a plugin")
     sub_unload.set_defaults(func=unload)
     common_args(sub_unload)
 
     sub_load = subparser.add_parser("load", help="Load a plugin")
     sub_load.set_defaults(func=load)
@@ -92,12 +93,9 @@
         choices=["user", "app"],
         default="user",
         help='The source location to load plugin from where "user" is the C:/Users/User/OpenplanetX/Plugins folder and "app" is the Openplanet/Plugins folder in the game directory. Default is "user" if unspecified.',
     )
 
     args = parser.parse_args()
 
-    if args.openplanet is None and args.port is None:
-        parser.error("Must specify at least one of [--port, --openplanet]")
-
     logging.basicConfig(level=logging.DEBUG if args.verbose else logging.ERROR)
     args.func(args)
```

### Comparing `tm_remote_build-2.0.0.dev1/src/tm_remote_build/log.py` & `tm_remote_build-2.0.0.dev2/src/tm_remote_build/log.py`

 * *Files identical despite different names*

### Comparing `tm_remote_build-2.0.0.dev1/PKG-INFO` & `tm_remote_build-2.0.0.dev2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tm-remote-build
-Version: 2.0.0.dev1
+Version: 2.0.0.dev2
 Summary: Build and deploy openplanet scripts
 Author: skybaks
 Author-email: tmflame@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

