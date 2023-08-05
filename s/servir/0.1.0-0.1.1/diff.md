# Comparing `tmp/servir-0.1.0.tar.gz` & `tmp/servir-0.1.1.tar.gz`

## Comparing `servir-0.1.0.tar` & `servir-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 servir-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 servir-0.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 servir-0.1.0/src/servir/__init__.py
--rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 servir-0.1.0/src/servir/_background_server.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 servir-0.1.0/src/servir/_protocols.py
--rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 servir-0.1.0/src/servir/_provide.py
--rw-r--r--   0        0        0     5936 2020-02-02 00:00:00.000000 servir-0.1.0/src/servir/_resources.py
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 servir-0.1.0/src/servir/_tilesets.py
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 servir-0.1.0/src/servir/_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 servir-0.1.0/src/servir/py.typed
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 servir-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 servir-0.1.0/tests/test_provider.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 servir-0.1.0/tests/test_servir.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 servir-0.1.0/tests/test_tilesets.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 servir-0.1.0/tests/test_util.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 servir-0.1.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 servir-0.1.0/LICENSE
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 servir-0.1.0/README.md
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 servir-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 servir-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 servir-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 servir-0.1.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 servir-0.1.1/src/servir/__init__.py
+-rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 servir-0.1.1/src/servir/_background_server.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 servir-0.1.1/src/servir/_protocols.py
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 servir-0.1.1/src/servir/_provide.py
+-rw-r--r--   0        0        0     5936 2020-02-02 00:00:00.000000 servir-0.1.1/src/servir/_resources.py
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 servir-0.1.1/src/servir/_tilesets.py
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 servir-0.1.1/src/servir/_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 servir-0.1.1/src/servir/py.typed
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 servir-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 servir-0.1.1/tests/test_provider.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 servir-0.1.1/tests/test_servir.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 servir-0.1.1/tests/test_tilesets.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 servir-0.1.1/tests/test_util.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 servir-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 servir-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 servir-0.1.1/README.md
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 servir-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 servir-0.1.1/PKG-INFO
```

### Comparing `servir-0.1.0/.github/workflows/ci.yml` & `servir-0.1.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `servir-0.1.0/.github/workflows/release.yml` & `servir-0.1.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `servir-0.1.0/src/servir/_background_server.py` & `servir-0.1.1/src/servir/_background_server.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,37 +14,46 @@
     from typing_extensions import Self
 
 
 class BackgroundServer:
     """A threading-based background server for Starlette apps."""
 
     _app: ASGIApp
+    _host: str | None
     _port: int | None
     _server_thread: threading.Thread | None
     _server: uvicorn.Server | None
 
     def __init__(self, app: ASGIApp) -> None:
         """Initialize a background server for the given Starlette app.
 
         Parameters
         ----------
         app : ASGIApp
             The Starlette app to run in the background.
         """
         self._app = app
+        self._host = None
         self._port = None
         self._server_thread = None
         self._server = None
 
     @property
     def app(self) -> ASGIApp:
         """The Starlette app being run in the background."""
         return self._app
 
     @property
+    def host(self) -> str:
+        """The host to which the server is bound."""
+        if self._server_thread is None or self._host is None:
+            raise RuntimeError("Server not running")
+        return self._host
+
+    @property
     def port(self) -> int:
         """The port on which the server is running."""
         if self._server_thread is None or self._port is None:
             raise RuntimeError("Server not running.")
         return self._port
 
     def stop(self) -> Self:
@@ -61,23 +70,29 @@
             self._server = None
             self._server_thread = None
 
         return self
 
     def start(
         self,
+        *,
+        host: str = "localhost",
         port: int | None = None,
         timeout: int = 1,
         daemon: bool = True,
         log_level: str = "warning",
     ) -> Self:
         """Start app in a background thread.
 
         Parameters
         ----------
+        host : str, optional
+            The host on which to bind the server. If not provided, the server will bind
+            to localhost. You can use "0.0.0.0" to expose the server to the local network
+            or use a hostname. IPv6 addresses are supported.
         port : int, optional
             The port on which to run the server. If not provided, a random port will be
             selected.
         timeout : int, optional
             The timeout for keep-alive connections, by default 1.
         daemon : bool, optional
             Whether to run the server thread as a daemon thread, by default True.
@@ -90,19 +105,21 @@
             The background server instance.
         """
         if self._server_thread is not None:
             return self
 
         config = uvicorn.Config(
             app=self.app,
+            host=host,
             port=port or portpicker.pick_unused_port(),
             timeout_keep_alive=timeout,
             log_level=log_level,
         )
 
+        self._host = config.host
         self._port = config.port
         self._server = uvicorn.Server(config=config)
         self._server_thread = threading.Thread(target=self._server.run, daemon=daemon)
         self._server_thread.start()
 
         # wait for the server to start
         while not self._server.started:
```

### Comparing `servir-0.1.0/src/servir/_protocols.py` & `servir-0.1.1/src/servir/_protocols.py`

 * *Files identical despite different names*

### Comparing `servir-0.1.0/src/servir/_provide.py` & `servir-0.1.1/src/servir/_provide.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             return f"/proxy/{self.port}"
 
         # https://github.com/yuvipanda/altair_data_server/blob/4d6ffcb19f864218c8d825ff2c95a1c8180585d0/altair_data_server/_altair_server.py#L73-L93
         if "JUPYTERHUB_SERVICE_PREFIX" in os.environ:
             urlprefix = os.environ["JUPYTERHUB_SERVICE_PREFIX"]
             return f"{urlprefix}/proxy/{self.port}"
 
-        return f"http://localhost:{self.port}"
+        return f"http://{self.host}:{self.port}"
 
     @typing.overload
     def create(self, path: pathlib.Path | str, /, **kwargs: typing.Any) -> Resource:
         ...
 
     @typing.overload
     def create(
```

### Comparing `servir-0.1.0/src/servir/_resources.py` & `servir-0.1.1/src/servir/_resources.py`

 * *Files identical despite different names*

### Comparing `servir-0.1.0/src/servir/_tilesets.py` & `servir-0.1.1/src/servir/_tilesets.py`

 * *Files identical despite different names*

### Comparing `servir-0.1.0/src/servir/_util.py` & `servir-0.1.1/src/servir/_util.py`

 * *Files identical despite different names*

### Comparing `servir-0.1.0/tests/test_provider.py` & `servir-0.1.1/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `servir-0.1.0/tests/test_util.py` & `servir-0.1.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `servir-0.1.0/LICENSE` & `servir-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `servir-0.1.0/README.md` & `servir-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `servir-0.1.0/pyproject.toml` & `servir-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `servir-0.1.0/PKG-INFO` & `servir-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servir
-Version: 0.1.0
+Version: 0.1.1
 Summary: an extensible async background server
 Project-URL: Documentation, https://github.com/unknown/servir#readme
 Project-URL: Issues, https://github.com/unknown/servir/issues
 Project-URL: Source, https://github.com/unknown/servir
 Author-email: Trevor Manz <trevor.j.manz@gmail.com>
 License: MIT
 License-File: LICENSE
```

