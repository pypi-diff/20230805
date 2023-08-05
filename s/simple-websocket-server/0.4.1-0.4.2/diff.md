# Comparing `tmp/simple-websocket-server-0.4.1.tar.gz` & `tmp/simple-websocket-server-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simple-websocket-server-0.4.1.tar", last modified: Fri Jan  8 13:39:11 2021, max compression
+gzip compressed data, was "simple-websocket-server-0.4.2.tar", last modified: Wed May 25 20:28:22 2022, max compression
```

## Comparing `simple-websocket-server-0.4.1.tar` & `simple-websocket-server-0.4.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2021-01-08 13:39:11.000000 simple-websocket-server-0.4.1/
--rw-rw-r--   0 jk        (1000) jk        (1000)     6248 2021-01-08 13:39:11.000000 simple-websocket-server-0.4.1/PKG-INFO
--rw-rw-r--   0 jk        (1000) jk        (1000)       34 2018-08-05 12:52:07.000000 simple-websocket-server-0.4.1/MANIFEST.in
-drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2021-01-08 13:39:11.000000 simple-websocket-server-0.4.1/simple_websocket_server.egg-info/
--rw-rw-r--   0 jk        (1000) jk        (1000)     6248 2021-01-08 13:39:11.000000 simple-websocket-server-0.4.1/simple_websocket_server.egg-info/PKG-INFO
--rw-rw-r--   0 jk        (1000) jk        (1000)      262 2021-01-08 13:39:11.000000 simple-websocket-server-0.4.1/simple_websocket_server.egg-info/SOURCES.txt
--rw-rw-r--   0 jk        (1000) jk        (1000)       24 2021-01-08 13:39:11.000000 simple-websocket-server-0.4.1/simple_websocket_server.egg-info/top_level.txt
--rw-rw-r--   0 jk        (1000) jk        (1000)        1 2021-01-08 13:39:11.000000 simple-websocket-server-0.4.1/simple_websocket_server.egg-info/dependency_links.txt
--rw-rw-r--   0 jk        (1000) jk        (1000)       38 2021-01-08 13:39:11.000000 simple-websocket-server-0.4.1/setup.cfg
--rw-rw-r--   0 jk        (1000) jk        (1000)     4192 2018-10-28 20:24:03.000000 simple-websocket-server-0.4.1/README.md
-drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2021-01-08 13:39:11.000000 simple-websocket-server-0.4.1/simple_websocket_server/
--rw-rw-r--   0 jk        (1000) jk        (1000)    23029 2021-01-08 13:31:58.000000 simple-websocket-server-0.4.1/simple_websocket_server/__init__.py
--rw-rw-r--   0 jk        (1000) jk        (1000)     1073 2018-10-09 16:21:05.000000 simple-websocket-server-0.4.1/LICENSE
--rw-rw-r--   0 jk        (1000) jk        (1000)     1167 2021-01-08 13:09:55.000000 simple-websocket-server-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 20:28:22.839316 simple-websocket-server-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-05-25 20:28:12.000000 simple-websocket-server-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-05-25 20:28:12.000000 simple-websocket-server-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5212 2022-05-25 20:28:22.839316 simple-websocket-server-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4193 2022-05-25 20:28:12.000000 simple-websocket-server-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-25 20:28:22.839316 simple-websocket-server-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-05-25 20:28:12.000000 simple-websocket-server-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 20:28:22.839316 simple-websocket-server-0.4.2/simple_websocket_server/
+-rw-r--r--   0 runner    (1001) docker     (121)    23047 2022-05-25 20:28:12.000000 simple-websocket-server-0.4.2/simple_websocket_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 20:28:22.839316 simple-websocket-server-0.4.2/simple_websocket_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5212 2022-05-25 20:28:22.000000 simple-websocket-server-0.4.2/simple_websocket_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      262 2022-05-25 20:28:22.000000 simple-websocket-server-0.4.2/simple_websocket_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-25 20:28:22.000000 simple-websocket-server-0.4.2/simple_websocket_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-05-25 20:28:22.000000 simple-websocket-server-0.4.2/simple_websocket_server.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `simple-websocket-server-0.4.1/PKG-INFO` & `simple-websocket-server-0.4.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,147 +1,15 @@
 Metadata-Version: 2.1
 Name: simple-websocket-server
-Version: 0.4.1
+Version: 0.4.2
 Summary: A simple WebSocket server
 Home-page: https://github.com/pikhovkin/simple-websocket-server
 Author: Sergei Pikhovkin
 Author-email: s@pikhovkin.ru
 License: MIT
-Description: # A simple WebSocket server
-        
-        [![CircleCI](https://img.shields.io/circleci/project/github/pikhovkin/simple-websocket-server.svg)](https://circleci.com/gh/pikhovkin/simple-websocket-server)
-        [![PyPI](https://img.shields.io/pypi/v/simple-websocket-server.svg)](https://pypi.org/project/simple-websocket-server/)
-        ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/simple-websocket-server.svg)
-        [![PyPI - License](https://img.shields.io/pypi/l/simple-websocket-server.svg)](./LICENSE)
-        
-        Based on [simple-websocket-server](https://github.com/dpallot/simple-websocket-server).
-        
-        - RFC 6455 (All latest browsers)
-        - TLS/SSL out of the box
-        - Passes Autobahns Websocket Testsuite
-        - Support for Python 2 and 3
-        
-        #### Installation
-        
-            pip install simple-websocket-server
-        
-        #### Echo Server Example
-        
-        `````python
-        from simple_websocket_server import WebSocketServer, WebSocket
-        
-        
-        class SimpleEcho(WebSocket):
-            def handle(self):
-                # echo message back to client
-                self.send_message(self.data)
-        
-            def connected(self):
-                print(self.address, 'connected')
-        
-            def handle_close(self):
-                print(self.address, 'closed')
-        
-        
-        server = WebSocketServer('', 8000, SimpleEcho)
-        server.serve_forever()
-        `````
-        
-        Open *tests/websocket.html* and connect to the server.
-        
-        #### Chat Server Example
-        
-        `````python
-        from simple_websocket_server import WebSocketServer, WebSocket
-        
-        
-        class SimpleChat(WebSocket):
-            def handle(self):
-                for client in clients:
-                    if client != self:
-                        client.send_message(self.address[0] + u' - ' + self.data)
-        
-            def connected(self):
-                print(self.address, 'connected')
-                for client in clients:
-                    client.send_message(self.address[0] + u' - connected')
-                clients.append(self)
-        
-            def handle_close(self):
-                clients.remove(self)
-                print(self.address, 'closed')
-                for client in clients:
-                    client.send_message(self.address[0] + u' - disconnected')
-        
-        
-        clients = []
-        
-        server = WebSocketServer('', 8000, SimpleChat)
-        server.serve_forever()
-        `````
-        Open multiple *tests/websocket.html* and connect to the server.
-        
-        #### Want to get up and running faster?
-        
-        There is an example which provides a simple echo and chat server
-        
-        Echo Server
-        
-            python tests/example_server.py --example echo
-        
-        Chat Server (open up multiple *tests/websocket.html* files)
-        
-            python tests/example_server.py --example chat
-        
-        #### TLS/SSL Example
-        
-        1) Generate a certificate with key
-        
-                openssl req -new -x509 -days 365 -nodes -out cert.pem -keyout key.pem
-        
-        2) Run the secure TSL/SSL server (in this case the cert.pem file is in the same directory)
-        
-                python tests/example_server.py --example chat --ssl 1
-        
-        3) Offer the certificate to the browser by serving *tests/websocket.html* through https.
-        The HTTPS server will look for cert.pem in the local directory.
-        Ensure the *tests/websocket.html* is also in the same directory to where the server is run.
-        
-                python tests/simple_https_server.py
-        
-        4) Open a web browser to: *https://localhost:443/tests/websocket.html*
-        
-        5) Change *ws://localhost:8000/* to *wss://localhost:8000* and click connect.
-        
-        Note: if you are having problems connecting, ensure that the certificate is added in your browser against the exception *https://localhost:8000* or whatever host:port pair you want to connect to.
-        
-        #### For the Programmers
-        
-        connected: called when handshake is complete
-         - self.address: TCP address port tuple of the endpoint
-        
-        handle_close: called when the endpoint is closed or there is an error
-         - self.address: TCP address port tuple of the endpoint
-        
-        handle: gets called when there is an incoming message from the client endpoint
-         - self.address: TCP address port tuple of the endpoint
-         - self.opcode: the WebSocket frame type (STREAM, TEXT, BINARY)
-         - self.data: bytearray (BINARY frame) or unicode string payload (TEXT frame)  
-         - self.request: HTTP details from the WebSocket handshake (refer to BaseHTTPRequestHandler)
-        
-        send_message: send some text or binary data to the client endpoint
-         - sending data as a unicode object will send a TEXT frame
-         - sending data as a bytearray object will send a BINARY frame
-        
-        close: send close frame to endpoint
-        
-        ### Licensing
-        
-        MIT
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Healthcare Industry
@@ -150,7 +18,142 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# A simple WebSocket server
+
+[![GitHub Actions](https://github.com/pikhovkin/simple-websocket-server/workflows/build/badge.svg)](https://github.com/pikhovkin/simple-websocket-server/actions)
+[![PyPI](https://img.shields.io/pypi/v/simple-websocket-server.svg)](https://pypi.org/project/simple-websocket-server/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/simple-websocket-server.svg)
+[![PyPI - License](https://img.shields.io/pypi/l/simple-websocket-server.svg)](./LICENSE)
+
+Based on [simple-websocket-server](https://github.com/dpallot/simple-websocket-server).
+
+- RFC 6455 (All latest browsers)
+- TLS/SSL out of the box
+- Passes Autobahns Websocket Testsuite
+- Support for Python 2 and 3
+
+#### Installation
+
+    pip install simple-websocket-server
+
+#### Echo Server Example
+
+`````python
+from simple_websocket_server import WebSocketServer, WebSocket
+
+
+class SimpleEcho(WebSocket):
+    def handle(self):
+        # echo message back to client
+        self.send_message(self.data)
+
+    def connected(self):
+        print(self.address, 'connected')
+
+    def handle_close(self):
+        print(self.address, 'closed')
+
+
+server = WebSocketServer('', 8000, SimpleEcho)
+server.serve_forever()
+`````
+
+Open *tests/websocket.html* and connect to the server.
+
+#### Chat Server Example
+
+`````python
+from simple_websocket_server import WebSocketServer, WebSocket
+
+
+class SimpleChat(WebSocket):
+    def handle(self):
+        for client in clients:
+            if client != self:
+                client.send_message(self.address[0] + u' - ' + self.data)
+
+    def connected(self):
+        print(self.address, 'connected')
+        for client in clients:
+            client.send_message(self.address[0] + u' - connected')
+        clients.append(self)
+
+    def handle_close(self):
+        clients.remove(self)
+        print(self.address, 'closed')
+        for client in clients:
+            client.send_message(self.address[0] + u' - disconnected')
+
+
+clients = []
+
+server = WebSocketServer('', 8000, SimpleChat)
+server.serve_forever()
+`````
+Open multiple *tests/websocket.html* and connect to the server.
+
+#### Want to get up and running faster?
+
+There is an example which provides a simple echo and chat server
+
+Echo Server
+
+    python tests/example_server.py --example echo
+
+Chat Server (open up multiple *tests/websocket.html* files)
+
+    python tests/example_server.py --example chat
+
+#### TLS/SSL Example
+
+1) Generate a certificate with key
+
+        openssl req -new -x509 -days 365 -nodes -out cert.pem -keyout key.pem
+
+2) Run the secure TSL/SSL server (in this case the cert.pem file is in the same directory)
+
+        python tests/example_server.py --example chat --ssl 1
+
+3) Offer the certificate to the browser by serving *tests/websocket.html* through https.
+The HTTPS server will look for cert.pem in the local directory.
+Ensure the *tests/websocket.html* is also in the same directory to where the server is run.
+
+        python tests/simple_https_server.py
+
+4) Open a web browser to: *https://localhost:443/tests/websocket.html*
+
+5) Change *ws://localhost:8000/* to *wss://localhost:8000* and click connect.
+
+Note: if you are having problems connecting, ensure that the certificate is added in your browser against the exception *https://localhost:8000* or whatever host:port pair you want to connect to.
+
+#### For the Programmers
+
+connected: called when handshake is complete
+ - self.address: TCP address port tuple of the endpoint
+
+handle_close: called when the endpoint is closed or there is an error
+ - self.address: TCP address port tuple of the endpoint
+
+handle: gets called when there is an incoming message from the client endpoint
+ - self.address: TCP address port tuple of the endpoint
+ - self.opcode: the WebSocket frame type (STREAM, TEXT, BINARY)
+ - self.data: bytearray (BINARY frame) or unicode string payload (TEXT frame)
+ - self.request: HTTP details from the WebSocket handshake (refer to BaseHTTPRequestHandler)
+
+send_message: send some text or binary data to the client endpoint
+ - sending data as a unicode object will send a TEXT frame
+ - sending data as a bytearray object will send a BINARY frame
+
+close: send close frame to endpoint
+
+### Licensing
+
+MIT
+
+
```

### Comparing `simple-websocket-server-0.4.1/simple_websocket_server.egg-info/PKG-INFO` & `simple-websocket-server-0.4.2/simple_websocket_server.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,147 +1,15 @@
 Metadata-Version: 2.1
 Name: simple-websocket-server
-Version: 0.4.1
+Version: 0.4.2
 Summary: A simple WebSocket server
 Home-page: https://github.com/pikhovkin/simple-websocket-server
 Author: Sergei Pikhovkin
 Author-email: s@pikhovkin.ru
 License: MIT
-Description: # A simple WebSocket server
-        
-        [![CircleCI](https://img.shields.io/circleci/project/github/pikhovkin/simple-websocket-server.svg)](https://circleci.com/gh/pikhovkin/simple-websocket-server)
-        [![PyPI](https://img.shields.io/pypi/v/simple-websocket-server.svg)](https://pypi.org/project/simple-websocket-server/)
-        ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/simple-websocket-server.svg)
-        [![PyPI - License](https://img.shields.io/pypi/l/simple-websocket-server.svg)](./LICENSE)
-        
-        Based on [simple-websocket-server](https://github.com/dpallot/simple-websocket-server).
-        
-        - RFC 6455 (All latest browsers)
-        - TLS/SSL out of the box
-        - Passes Autobahns Websocket Testsuite
-        - Support for Python 2 and 3
-        
-        #### Installation
-        
-            pip install simple-websocket-server
-        
-        #### Echo Server Example
-        
-        `````python
-        from simple_websocket_server import WebSocketServer, WebSocket
-        
-        
-        class SimpleEcho(WebSocket):
-            def handle(self):
-                # echo message back to client
-                self.send_message(self.data)
-        
-            def connected(self):
-                print(self.address, 'connected')
-        
-            def handle_close(self):
-                print(self.address, 'closed')
-        
-        
-        server = WebSocketServer('', 8000, SimpleEcho)
-        server.serve_forever()
-        `````
-        
-        Open *tests/websocket.html* and connect to the server.
-        
-        #### Chat Server Example
-        
-        `````python
-        from simple_websocket_server import WebSocketServer, WebSocket
-        
-        
-        class SimpleChat(WebSocket):
-            def handle(self):
-                for client in clients:
-                    if client != self:
-                        client.send_message(self.address[0] + u' - ' + self.data)
-        
-            def connected(self):
-                print(self.address, 'connected')
-                for client in clients:
-                    client.send_message(self.address[0] + u' - connected')
-                clients.append(self)
-        
-            def handle_close(self):
-                clients.remove(self)
-                print(self.address, 'closed')
-                for client in clients:
-                    client.send_message(self.address[0] + u' - disconnected')
-        
-        
-        clients = []
-        
-        server = WebSocketServer('', 8000, SimpleChat)
-        server.serve_forever()
-        `````
-        Open multiple *tests/websocket.html* and connect to the server.
-        
-        #### Want to get up and running faster?
-        
-        There is an example which provides a simple echo and chat server
-        
-        Echo Server
-        
-            python tests/example_server.py --example echo
-        
-        Chat Server (open up multiple *tests/websocket.html* files)
-        
-            python tests/example_server.py --example chat
-        
-        #### TLS/SSL Example
-        
-        1) Generate a certificate with key
-        
-                openssl req -new -x509 -days 365 -nodes -out cert.pem -keyout key.pem
-        
-        2) Run the secure TSL/SSL server (in this case the cert.pem file is in the same directory)
-        
-                python tests/example_server.py --example chat --ssl 1
-        
-        3) Offer the certificate to the browser by serving *tests/websocket.html* through https.
-        The HTTPS server will look for cert.pem in the local directory.
-        Ensure the *tests/websocket.html* is also in the same directory to where the server is run.
-        
-                python tests/simple_https_server.py
-        
-        4) Open a web browser to: *https://localhost:443/tests/websocket.html*
-        
-        5) Change *ws://localhost:8000/* to *wss://localhost:8000* and click connect.
-        
-        Note: if you are having problems connecting, ensure that the certificate is added in your browser against the exception *https://localhost:8000* or whatever host:port pair you want to connect to.
-        
-        #### For the Programmers
-        
-        connected: called when handshake is complete
-         - self.address: TCP address port tuple of the endpoint
-        
-        handle_close: called when the endpoint is closed or there is an error
-         - self.address: TCP address port tuple of the endpoint
-        
-        handle: gets called when there is an incoming message from the client endpoint
-         - self.address: TCP address port tuple of the endpoint
-         - self.opcode: the WebSocket frame type (STREAM, TEXT, BINARY)
-         - self.data: bytearray (BINARY frame) or unicode string payload (TEXT frame)  
-         - self.request: HTTP details from the WebSocket handshake (refer to BaseHTTPRequestHandler)
-        
-        send_message: send some text or binary data to the client endpoint
-         - sending data as a unicode object will send a TEXT frame
-         - sending data as a bytearray object will send a BINARY frame
-        
-        close: send close frame to endpoint
-        
-        ### Licensing
-        
-        MIT
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Healthcare Industry
@@ -150,7 +18,142 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# A simple WebSocket server
+
+[![GitHub Actions](https://github.com/pikhovkin/simple-websocket-server/workflows/build/badge.svg)](https://github.com/pikhovkin/simple-websocket-server/actions)
+[![PyPI](https://img.shields.io/pypi/v/simple-websocket-server.svg)](https://pypi.org/project/simple-websocket-server/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/simple-websocket-server.svg)
+[![PyPI - License](https://img.shields.io/pypi/l/simple-websocket-server.svg)](./LICENSE)
+
+Based on [simple-websocket-server](https://github.com/dpallot/simple-websocket-server).
+
+- RFC 6455 (All latest browsers)
+- TLS/SSL out of the box
+- Passes Autobahns Websocket Testsuite
+- Support for Python 2 and 3
+
+#### Installation
+
+    pip install simple-websocket-server
+
+#### Echo Server Example
+
+`````python
+from simple_websocket_server import WebSocketServer, WebSocket
+
+
+class SimpleEcho(WebSocket):
+    def handle(self):
+        # echo message back to client
+        self.send_message(self.data)
+
+    def connected(self):
+        print(self.address, 'connected')
+
+    def handle_close(self):
+        print(self.address, 'closed')
+
+
+server = WebSocketServer('', 8000, SimpleEcho)
+server.serve_forever()
+`````
+
+Open *tests/websocket.html* and connect to the server.
+
+#### Chat Server Example
+
+`````python
+from simple_websocket_server import WebSocketServer, WebSocket
+
+
+class SimpleChat(WebSocket):
+    def handle(self):
+        for client in clients:
+            if client != self:
+                client.send_message(self.address[0] + u' - ' + self.data)
+
+    def connected(self):
+        print(self.address, 'connected')
+        for client in clients:
+            client.send_message(self.address[0] + u' - connected')
+        clients.append(self)
+
+    def handle_close(self):
+        clients.remove(self)
+        print(self.address, 'closed')
+        for client in clients:
+            client.send_message(self.address[0] + u' - disconnected')
+
+
+clients = []
+
+server = WebSocketServer('', 8000, SimpleChat)
+server.serve_forever()
+`````
+Open multiple *tests/websocket.html* and connect to the server.
+
+#### Want to get up and running faster?
+
+There is an example which provides a simple echo and chat server
+
+Echo Server
+
+    python tests/example_server.py --example echo
+
+Chat Server (open up multiple *tests/websocket.html* files)
+
+    python tests/example_server.py --example chat
+
+#### TLS/SSL Example
+
+1) Generate a certificate with key
+
+        openssl req -new -x509 -days 365 -nodes -out cert.pem -keyout key.pem
+
+2) Run the secure TSL/SSL server (in this case the cert.pem file is in the same directory)
+
+        python tests/example_server.py --example chat --ssl 1
+
+3) Offer the certificate to the browser by serving *tests/websocket.html* through https.
+The HTTPS server will look for cert.pem in the local directory.
+Ensure the *tests/websocket.html* is also in the same directory to where the server is run.
+
+        python tests/simple_https_server.py
+
+4) Open a web browser to: *https://localhost:443/tests/websocket.html*
+
+5) Change *ws://localhost:8000/* to *wss://localhost:8000* and click connect.
+
+Note: if you are having problems connecting, ensure that the certificate is added in your browser against the exception *https://localhost:8000* or whatever host:port pair you want to connect to.
+
+#### For the Programmers
+
+connected: called when handshake is complete
+ - self.address: TCP address port tuple of the endpoint
+
+handle_close: called when the endpoint is closed or there is an error
+ - self.address: TCP address port tuple of the endpoint
+
+handle: gets called when there is an incoming message from the client endpoint
+ - self.address: TCP address port tuple of the endpoint
+ - self.opcode: the WebSocket frame type (STREAM, TEXT, BINARY)
+ - self.data: bytearray (BINARY frame) or unicode string payload (TEXT frame)
+ - self.request: HTTP details from the WebSocket handshake (refer to BaseHTTPRequestHandler)
+
+send_message: send some text or binary data to the client endpoint
+ - sending data as a unicode object will send a TEXT frame
+ - sending data as a bytearray object will send a BINARY frame
+
+close: send close frame to endpoint
+
+### Licensing
+
+MIT
+
+
```

### Comparing `simple-websocket-server-0.4.1/README.md` & `simple-websocket-server-0.4.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # A simple WebSocket server
 
-[![CircleCI](https://img.shields.io/circleci/project/github/pikhovkin/simple-websocket-server.svg)](https://circleci.com/gh/pikhovkin/simple-websocket-server)
+[![GitHub Actions](https://github.com/pikhovkin/simple-websocket-server/workflows/build/badge.svg)](https://github.com/pikhovkin/simple-websocket-server/actions)
 [![PyPI](https://img.shields.io/pypi/v/simple-websocket-server.svg)](https://pypi.org/project/simple-websocket-server/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/simple-websocket-server.svg)
 [![PyPI - License](https://img.shields.io/pypi/l/simple-websocket-server.svg)](./LICENSE)
 
 Based on [simple-websocket-server](https://github.com/dpallot/simple-websocket-server).
 
 - RFC 6455 (All latest browsers)
@@ -113,15 +113,15 @@
 
 handle_close: called when the endpoint is closed or there is an error
  - self.address: TCP address port tuple of the endpoint
 
 handle: gets called when there is an incoming message from the client endpoint
  - self.address: TCP address port tuple of the endpoint
  - self.opcode: the WebSocket frame type (STREAM, TEXT, BINARY)
- - self.data: bytearray (BINARY frame) or unicode string payload (TEXT frame)  
+ - self.data: bytearray (BINARY frame) or unicode string payload (TEXT frame)
  - self.request: HTTP details from the WebSocket handshake (refer to BaseHTTPRequestHandler)
 
 send_message: send some text or binary data to the client endpoint
  - sending data as a unicode object will send a TEXT frame
  - sending data as a bytearray object will send a BINARY frame
 
 close: send close frame to endpoint
```

### Comparing `simple-websocket-server-0.4.1/simple_websocket_server/__init__.py` & `simple-websocket-server-0.4.2/simple_websocket_server/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
             pass
         elif self.opcode == STREAM:
             pass
         elif self.opcode == TEXT:
             pass
         elif self.opcode == BINARY:
             pass
-        elif self.opcode == PONG or self.opcode == PING:
+        elif self.opcode in (PONG, PING):
             if len(self.data) > 125:
                 raise Exception('control frame length can not be > 125')
         else:
             # unknown or reserved opcode so just close
             raise Exception('unknown opcode')
 
         if self.opcode == CLOSE:
@@ -175,15 +175,15 @@
                         status = 1002
             else:
                 status = 1002
 
             self.close(status, reason)
         elif self.fin == 0:
             if self.opcode != STREAM:
-                if self.opcode == PING or self.opcode == PONG:
+                if self.opcode in (PING, PONG):
                     raise Exception('control messages can not be fragmented')
 
                 self.frag_type = self.opcode
                 self.frag_start = True
                 self.frag_decoder.reset()
 
                 if self.frag_type == TEXT:
@@ -265,15 +265,15 @@
                     self.sendq.append((BINARY, hs.encode('ascii')))
                     self.handshaked = True
                     self.connected()
                 except Exception as e:
                     hs = FAILED_HANDSHAKE_STR
                     self._send_buffer(hs.encode('ascii'), True)
                     self.client.close()
-                    raise Exception('handshake failed: {}'.format(e))
+                    raise Exception('handshake failed: {}'.format(e))  # pylint: disable=consider-using-f-string
         else:
             data = self.client.recv(16384)
             if not data:
                 raise Exception("remote socket closed")
 
             if VER >= 3:
                 for d in data:
@@ -560,16 +560,16 @@
 class WebSocketServer(object):
     request_queue_size = 5
 
     # pylint: disable=too-many-arguments
     def __init__(self, host, port, websocketclass, certfile=None, keyfile=None,
                  ssl_version=ssl.PROTOCOL_TLSv1, select_interval=0.1):
         self.websocketclass = websocketclass
-        if host == '':
-            host = None
+        if not host:
+            host = '127.0.0.1'
         fam = socket.AF_INET6 if host is None else 0
         host_info = socket.getaddrinfo(host, port, fam, socket.SOCK_STREAM, socket.IPPROTO_TCP, socket.AI_PASSIVE)
         self.serversocket = socket.socket(host_info[0][0], host_info[0][1], host_info[0][2])
         self.serversocket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self.serversocket.bind(host_info[0][4])
         self.serversocket.listen(self.request_queue_size)
         self.select_interval = select_interval
```

### Comparing `simple-websocket-server-0.4.1/LICENSE` & `simple-websocket-server-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-websocket-server-0.4.1/setup.py` & `simple-websocket-server-0.4.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='simple-websocket-server',
-    version='0.4.1',
+    version='0.4.2',
     author='Sergei Pikhovkin',
     author_email='s@pikhovkin.ru',
     packages=find_packages(exclude=['tests*']),
     license='MIT',
     description=('A simple WebSocket server'),
-    long_description=open('README.md').read(),
+    long_description=open('README.md').read(),  # pylint: disable=consider-using-with, unspecified-encoding
     long_description_content_type='text/markdown',
     url='https://github.com/pikhovkin/simple-websocket-server',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
```

