# Comparing `tmp/tremolo-0.0.98.tar.gz` & `tmp/tremolo-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tremolo-0.0.98.tar", last modified: Tue May 23 02:00:57 2023, max compression
+gzip compressed data, was "dist/tremolo-0.0.99.tar", last modified: Thu Jun 29 14:45:54 2023, max compression
```

## Comparing `tremolo-0.0.98.tar` & `tremolo-0.0.99.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-23 02:00:57.000000 tremolo-0.0.98/
--rw-r--r--   0 tux       (1000) users      (100)     1063 2023-05-08 03:43:30.000000 tremolo-0.0.98/LICENSE.txt
--rw-r--r--   0 tux       (1000) users      (100)     4619 2023-05-23 02:00:57.000000 tremolo-0.0.98/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)     4019 2023-05-23 01:20:31.000000 tremolo-0.0.98/README.md
--rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-23 02:00:57.000000 tremolo-0.0.98/setup.cfg
--rwxr-xr-x   0 tux       (1000) users      (100)      975 2023-05-23 01:14:02.000000 tremolo-0.0.98/setup.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-23 02:00:57.000000 tremolo-0.0.98/tremolo/
--rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-05-08 03:43:30.000000 tremolo-0.0.98/tremolo/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)     4465 2023-05-08 03:43:30.000000 tremolo-0.0.98/tremolo/__main__.py
--rw-r--r--   0 tux       (1000) users      (100)     2278 2023-05-08 03:43:30.000000 tremolo-0.0.98/tremolo/asgi_lifespan.py
--rw-r--r--   0 tux       (1000) users      (100)     5666 2023-05-19 13:26:48.000000 tremolo-0.0.98/tremolo/asgi_server.py
--rw-r--r--   0 tux       (1000) users      (100)      542 2023-05-08 03:43:30.000000 tremolo-0.0.98/tremolo/contexts.py
--rw-r--r--   0 tux       (1000) users      (100)      586 2023-05-08 03:43:30.000000 tremolo-0.0.98/tremolo/exceptions.py
--rw-r--r--   0 tux       (1000) users      (100)    10617 2023-05-19 14:03:18.000000 tremolo-0.0.98/tremolo/http_server.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-23 02:00:57.000000 tremolo-0.0.98/tremolo/lib/
--rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-08 03:43:30.000000 tremolo-0.0.98/tremolo/lib/__init__.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-23 02:00:57.000000 tremolo-0.0.98/tremolo/lib/h1parser/
--rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-08 03:43:30.000000 tremolo-0.0.98/tremolo/lib/h1parser/__init__.py
--rwxr-xr-x   0 tux       (1000) users      (100)     4954 2023-05-08 03:43:30.000000 tremolo-0.0.98/tremolo/lib/h1parser/parse_header.py
--rw-r--r--   0 tux       (1000) users      (100)     1798 2023-05-08 03:43:30.000000 tremolo-0.0.98/tremolo/lib/http_exception.py
--rwxr-xr-x   0 tux       (1000) users      (100)    14220 2023-05-23 01:43:26.000000 tremolo-0.0.98/tremolo/lib/http_protocol.py
--rwxr-xr-x   0 tux       (1000) users      (100)     9281 2023-05-19 23:50:26.000000 tremolo-0.0.98/tremolo/lib/http_request.py
--rwxr-xr-x   0 tux       (1000) users      (100)    11322 2023-05-20 00:56:10.000000 tremolo-0.0.98/tremolo/lib/http_response.py
--rw-r--r--   0 tux       (1000) users      (100)      772 2023-05-19 07:52:08.000000 tremolo-0.0.98/tremolo/lib/object_pool.py
--rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-05-19 02:59:43.000000 tremolo-0.0.98/tremolo/lib/request.py
--rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-05-08 03:43:30.000000 tremolo-0.0.98/tremolo/lib/response.py
--rwxr-xr-x   0 tux       (1000) users      (100)    15287 2023-05-23 01:38:51.000000 tremolo-0.0.98/tremolo/tremolo.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-23 02:00:57.000000 tremolo-0.0.98/tremolo.egg-info/
--rw-r--r--   0 tux       (1000) users      (100)     4619 2023-05-23 02:00:57.000000 tremolo-0.0.98/tremolo.egg-info/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)      610 2023-05-23 02:00:57.000000 tremolo-0.0.98/tremolo.egg-info/SOURCES.txt
--rw-r--r--   0 tux       (1000) users      (100)        1 2023-05-23 02:00:57.000000 tremolo-0.0.98/tremolo.egg-info/dependency_links.txt
--rw-r--r--   0 tux       (1000) users      (100)        8 2023-05-23 02:00:57.000000 tremolo-0.0.98/tremolo.egg-info/top_level.txt
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-06-29 14:45:54.000000 tremolo-0.0.99/
+-rw-r--r--   0 tux       (1000) users      (100)     1063 2023-05-08 03:43:30.000000 tremolo-0.0.99/LICENSE.txt
+-rw-r--r--   0 tux       (1000) users      (100)     4803 2023-06-29 14:45:54.000000 tremolo-0.0.99/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)     4203 2023-06-29 14:41:58.000000 tremolo-0.0.99/README.md
+-rw-r--r--   0 tux       (1000) users      (100)       38 2023-06-29 14:45:54.000000 tremolo-0.0.99/setup.cfg
+-rwxr-xr-x   0 tux       (1000) users      (100)      975 2023-06-29 14:42:25.000000 tremolo-0.0.99/setup.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-06-29 14:45:53.000000 tremolo-0.0.99/tremolo/
+-rwxr-xr-x   0 tux       (1000) users      (100)      249 2023-06-09 03:14:53.000000 tremolo-0.0.99/tremolo/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)     4564 2023-06-09 03:14:00.000000 tremolo-0.0.99/tremolo/__main__.py
+-rw-r--r--   0 tux       (1000) users      (100)     2278 2023-05-08 03:43:30.000000 tremolo-0.0.99/tremolo/asgi_lifespan.py
+-rw-r--r--   0 tux       (1000) users      (100)     5719 2023-06-09 01:09:12.000000 tremolo-0.0.99/tremolo/asgi_server.py
+-rw-r--r--   0 tux       (1000) users      (100)      542 2023-05-08 03:43:30.000000 tremolo-0.0.99/tremolo/contexts.py
+-rw-r--r--   0 tux       (1000) users      (100)      586 2023-05-08 03:43:30.000000 tremolo-0.0.99/tremolo/exceptions.py
+-rw-r--r--   0 tux       (1000) users      (100)    10405 2023-06-13 02:52:05.000000 tremolo-0.0.99/tremolo/http_server.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-06-29 14:45:53.000000 tremolo-0.0.99/tremolo/lib/
+-rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-08 03:43:30.000000 tremolo-0.0.99/tremolo/lib/__init__.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-06-29 14:45:53.000000 tremolo-0.0.99/tremolo/lib/h1parser/
+-rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-08 03:43:30.000000 tremolo-0.0.99/tremolo/lib/h1parser/__init__.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     4954 2023-05-08 03:43:30.000000 tremolo-0.0.99/tremolo/lib/h1parser/parse_header.py
+-rw-r--r--   0 tux       (1000) users      (100)     1798 2023-05-08 03:43:30.000000 tremolo-0.0.99/tremolo/lib/http_exception.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    14294 2023-06-13 04:38:29.000000 tremolo-0.0.99/tremolo/lib/http_protocol.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     9281 2023-05-19 23:50:26.000000 tremolo-0.0.99/tremolo/lib/http_request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    11322 2023-05-20 00:56:10.000000 tremolo-0.0.99/tremolo/lib/http_response.py
+-rw-r--r--   0 tux       (1000) users      (100)      772 2023-05-19 07:52:08.000000 tremolo-0.0.99/tremolo/lib/object_pool.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-05-19 02:59:43.000000 tremolo-0.0.99/tremolo/lib/request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-05-08 03:43:30.000000 tremolo-0.0.99/tremolo/lib/response.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    15925 2023-06-09 04:02:32.000000 tremolo-0.0.99/tremolo/tremolo.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-06-29 14:45:53.000000 tremolo-0.0.99/tremolo.egg-info/
+-rw-r--r--   0 tux       (1000) users      (100)     4803 2023-06-29 14:45:53.000000 tremolo-0.0.99/tremolo.egg-info/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)      610 2023-06-29 14:45:53.000000 tremolo-0.0.99/tremolo.egg-info/SOURCES.txt
+-rw-r--r--   0 tux       (1000) users      (100)        1 2023-06-29 14:45:53.000000 tremolo-0.0.99/tremolo.egg-info/dependency_links.txt
+-rw-r--r--   0 tux       (1000) users      (100)        8 2023-06-29 14:45:53.000000 tremolo-0.0.99/tremolo.egg-info/top_level.txt
```

### Comparing `tremolo-0.0.98/LICENSE.txt` & `tremolo-0.0.99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.98/PKG-INFO` & `tremolo-0.0.99/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.98
+Version: 0.0.99
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -101,14 +101,20 @@
 
 To see more available options:
 
 ```
 python3 -m tremolo --help
 ```
 
+It's also possible to run the ASGI server programmatically ([example with uvloop](https://github.com/nggit/tremolo/blob/master/example_uvloop.py)):
+
+```
+python3 example_uvloop.py
+```
+
 ## Benchmarking
 The first thing to note is that Tremolo is a pure Python server framework.
 
 As a pure Python server framework, it is hard to find a comparison.
 Because most servers/frameworks today are full of steroids like `httptools`, `uvloop`, Rust, etc.
 
 You can try comparing with [Uvicorn](https://www.uvicorn.org/) with the following option (disabling steroids to be fair):
```

### Comparing `tremolo-0.0.98/README.md` & `tremolo-0.0.99/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -85,14 +85,20 @@
 
 To see more available options:
 
 ```
 python3 -m tremolo --help
 ```
 
+It's also possible to run the ASGI server programmatically ([example with uvloop](https://github.com/nggit/tremolo/blob/master/example_uvloop.py)):
+
+```
+python3 example_uvloop.py
+```
+
 ## Benchmarking
 The first thing to note is that Tremolo is a pure Python server framework.
 
 As a pure Python server framework, it is hard to find a comparison.
 Because most servers/frameworks today are full of steroids like `httptools`, `uvloop`, Rust, etc.
 
 You can try comparing with [Uvicorn](https://www.uvicorn.org/) with the following option (disabling steroids to be fair):
```

### Comparing `tremolo-0.0.98/setup.py` & `tremolo-0.0.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='tremolo',
     packages=['tremolo'],
     package_data={'': ['lib/*', 'lib/h1parser/*']},
-    version='0.0.98',
+    version='0.0.99',
     license='MIT',
     author='nggit',
     author_email='contact@anggit.com',
     description='Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nggit/tremolo',
```

### Comparing `tremolo-0.0.98/tremolo/__main__.py` & `tremolo-0.0.99/tremolo/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,19 +38,20 @@
         print('  --upload-rate             Limits the upload / POST speed')
         print('                            Defaults to 1048576, which means 1MiB/s')
         print('  --buffer-size             Defaults to 16384, or 16KiB')
         print('  --client-max-body-size    Defaults to 2 * 1048576, or 2MiB')
         print('  --request-timeout         Defaults to 30 (seconds)')
         print('  --keepalive-timeout       Defaults to 30 (seconds)')
         print('  --server-name             Set the "Server" field in the response header')
+        print('  --root-path               Set the ASGI root_path. Defaults to ""')
         print('  --help                    Show this help and exit')
         sys.exit()
     elif sys.argv[i - 1] in ('--debug', '--reuse-port'):
         options[sys.argv[i - 1].lstrip('-').replace('-', '_')] = True
-    elif sys.argv[i - 1] in ('--host', '--log-level', '--server-name'):
+    elif sys.argv[i - 1] in ('--host', '--log-level', '--server-name', '--root-path'):
         options[sys.argv[i - 1].lstrip('-').replace('-', '_')] = sys.argv[i]
     elif sys.argv[i - 1] in ('--port',
                              '--worker-num',
                              '--backlog',
                              '--download-rate',
                              '--upload-rate',
                              '--buffer-size',
```

### Comparing `tremolo-0.0.98/tremolo/asgi_lifespan.py` & `tremolo-0.0.99/tremolo/asgi_lifespan.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.98/tremolo/asgi_server.py` & `tremolo-0.0.99/tremolo/asgi_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
             'http_version': self.request.version.decode(encoding='utf-8'),
             'method': self.request.method.decode(encoding='utf-8'),
             'scheme': {True: 'http',
                        False: 'https'}[self.request.transport.get_extra_info('sslcontext') is None],
             'path': unquote(self.request.path.decode(encoding='utf-8'), encoding='utf-8'),
             'raw_path': self.request.path,
             'query_string': self.request.query_string,
+            'root_path': self.options['_root_path'],
             'headers': self.request.header.getheaders(),
             'client': self.request.transport.get_extra_info('peername'),
             'server': self.request.transport.get_extra_info('sockname')
         }
 
         self._read = self.request.read(cache=False)
```

### Comparing `tremolo-0.0.98/tremolo/contexts.py` & `tremolo-0.0.99/tremolo/contexts.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.98/tremolo/exceptions.py` & `tremolo-0.0.99/tremolo/exceptions.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.98/tremolo/http_server.py` & `tremolo-0.0.99/tremolo/http_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,14 @@
         }
 
         super().__init__(self._server['context'], **kwargs)
 
     async def _connection_made(self, func):
         await func(**self._server)
 
-        if self._server['context']._on_connect is not None:
-            self._server['context']._on_connect.set_result(None)
-
     async def _connection_lost(self, func, exc):
         try:
             await func(**self._server)
         finally:
             super().connection_lost(exc)
 
     def connection_made(self, transport):
@@ -39,19 +36,17 @@
 
         func = self._middlewares['connect'][-1][0]
         self._server['context'].set('options', self._middlewares['connect'][-1][1])
 
         if func is None:
             self._server['context']._on_connect = None
         else:
-            self._server['context']._on_connect = self._server['loop'].create_future()
+            self._server['context']._on_connect = self._server['loop'].create_task(self._connection_made(func))
 
-            self._server['context'].tasks.append(
-                self._server['loop'].create_task(self._connection_made(func))
-            )
+            self._server['context'].tasks.append(self._server['context']._on_connect)
 
     def connection_lost(self, exc):
         func = self._middlewares['close'][-1][0]
 
         if func is None:
             super().connection_lost(exc)
             return
@@ -221,15 +216,14 @@
             await self.response.write(b'', throttle=False)
 
         await self.response.send(None)
 
     async def header_received(self):
         if self._server['context']._on_connect is not None:
             await self._server['context']._on_connect
-            self._server['context']._on_connect = None
 
         options = self._server['context'].options
 
         for middleware in self._middlewares['request']:
             options = await self._handle_middleware(middleware[0], {**middleware[1], **options})
 
             if not isinstance(options, dict):
```

### Comparing `tremolo-0.0.98/tremolo/lib/h1parser/parse_header.py` & `tremolo-0.0.99/tremolo/lib/h1parser/parse_header.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.98/tremolo/lib/http_exception.py` & `tremolo-0.0.99/tremolo/lib/http_exception.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.98/tremolo/lib/http_protocol.py` & `tremolo-0.0.99/tremolo/lib/http_protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,16 @@
             if not isinstance(exc, HTTPException):
                 exc = InternalServerError(cause=exc)
 
             await self.handle_exception(exc)
 
     async def _receive_data(self, data, waiter):
         await waiter
-        await self.put_to_queue(data, queue=self._queue[0], transport=self._transport, rate=self._options['upload_rate'])
+        await self.put_to_queue(data, queue=self._queue[0], transport=self._transport,
+                                rate=self._options['upload_rate'], buffer_size=self._options['buffer_size'])
 
     def data_received(self, data):
         if not data:
             return
 
         if self._data is not None:
             self._data.extend(data)
```

### Comparing `tremolo-0.0.98/tremolo/lib/http_request.py` & `tremolo-0.0.99/tremolo/lib/http_request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.98/tremolo/lib/http_response.py` & `tremolo-0.0.99/tremolo/lib/http_response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.98/tremolo/lib/object_pool.py` & `tremolo-0.0.99/tremolo/lib/object_pool.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.98/tremolo/lib/request.py` & `tremolo-0.0.99/tremolo/lib/request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.98/tremolo/lib/response.py` & `tremolo-0.0.99/tremolo/lib/response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.98/tremolo/tremolo.py` & `tremolo-0.0.99/tremolo/tremolo.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,14 +257,15 @@
                             buffer_size=options.get('buffer_size', 16 * 1024),
                             client_max_body_size=options.get('client_max_body_size', 2 * 1048576),
                             request_timeout=options.get('request_timeout', 30),
                             keepalive_timeout=options.get('keepalive_timeout', 30),
                             server_name=server_name,
                             _pool=pool,
                             _app=options['app'],
+                            _root_path=options.get('root_path', ''),
                             _handlers=options['handlers'],
                             _middlewares=options['middlewares']), sock=sock, backlog=backlog, ssl=ssl_context)
 
         print(datetime.now().strftime('[%Y-%m-%d %H:%M:%S]'), end=' ')
         sys.stdout.flush()
         sys.stdout.buffer.write(b'%s (pid %d) is started at %s port %d' % (server_name, os.getpid(), host, port))
 
@@ -328,14 +329,30 @@
                                             }[reuse_port], 1)
         sock.bind((host, port))
         sock.set_inheritable(True)
 
         return sock
 
     def run(self, host=None, port=80, reuse_port=True, worker_num=1, **kwargs):
+        if 'app' in kwargs and not isinstance(kwargs['app'], str):
+            import __main__
+
+            if hasattr(__main__, '__file__'):
+                for attr_name in dir(__main__):
+                    if attr_name.startswith('__'):
+                        continue
+
+                    if getattr(__main__, attr_name) == kwargs['app']:
+                        break
+                else:
+                    attr_name = 'app'
+
+                kwargs['app'] = '{:s}:{:s}'.format(__main__.__file__,
+                                                   attr_name)
+
         if host is None:
             default_host = ''
         else:
             default_host = host
             self.listen(port, host=host, **kwargs)
 
         try:
```

### Comparing `tremolo-0.0.98/tremolo.egg-info/PKG-INFO` & `tremolo-0.0.99/tremolo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.98
+Version: 0.0.99
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -101,14 +101,20 @@
 
 To see more available options:
 
 ```
 python3 -m tremolo --help
 ```
 
+It's also possible to run the ASGI server programmatically ([example with uvloop](https://github.com/nggit/tremolo/blob/master/example_uvloop.py)):
+
+```
+python3 example_uvloop.py
+```
+
 ## Benchmarking
 The first thing to note is that Tremolo is a pure Python server framework.
 
 As a pure Python server framework, it is hard to find a comparison.
 Because most servers/frameworks today are full of steroids like `httptools`, `uvloop`, Rust, etc.
 
 You can try comparing with [Uvicorn](https://www.uvicorn.org/) with the following option (disabling steroids to be fair):
```

### Comparing `tremolo-0.0.98/tremolo.egg-info/SOURCES.txt` & `tremolo-0.0.99/tremolo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

