# Comparing `tmp/python-osc-1.8.1.tar.gz` & `tmp/python-osc-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-osc-1.8.1.tar", last modified: Sun Jan 15 16:42:23 2023, max compression
+gzip compressed data, was "python-osc-1.8.2.tar", last modified: Sat Aug  5 18:06:16 2023, max compression
```

## Comparing `python-osc-1.8.1.tar` & `python-osc-1.8.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 tmu        (501) staff       (20)        0 2023-01-15 16:42:23.772180 python-osc-1.8.1/
--rw-r--r--   0 tmu        (501) staff       (20)     1211 2017-12-19 02:21:53.000000 python-osc-1.8.1/LICENSE.txt
--rw-r--r--   0 tmu        (501) staff       (20)       66 2023-01-15 16:35:26.000000 python-osc-1.8.1/MANIFEST.in
--rw-r--r--   0 tmu        (501) staff       (20)     6162 2023-01-15 16:42:23.772386 python-osc-1.8.1/PKG-INFO
--rw-r--r--   0 tmu        (501) staff       (20)     4262 2023-01-15 16:35:26.000000 python-osc-1.8.1/README.rst
-drwxr-xr-x   0 tmu        (501) staff       (20)        0 2023-01-15 16:42:23.755637 python-osc-1.8.1/python_osc.egg-info/
--rw-r--r--   0 tmu        (501) staff       (20)     6162 2023-01-15 16:42:23.000000 python-osc-1.8.1/python_osc.egg-info/PKG-INFO
--rw-r--r--   0 tmu        (501) staff       (20)      954 2023-01-15 16:42:23.000000 python-osc-1.8.1/python_osc.egg-info/SOURCES.txt
--rw-r--r--   0 tmu        (501) staff       (20)        1 2023-01-15 16:42:23.000000 python-osc-1.8.1/python_osc.egg-info/dependency_links.txt
--rw-r--r--   0 tmu        (501) staff       (20)       10 2023-01-15 16:42:23.000000 python-osc-1.8.1/python_osc.egg-info/top_level.txt
-drwxr-xr-x   0 tmu        (501) staff       (20)        0 2023-01-15 16:42:23.761410 python-osc-1.8.1/pythonosc/
--rw-r--r--   0 tmu        (501) staff       (20)        0 2017-12-19 02:21:53.000000 python-osc-1.8.1/pythonosc/__init__.py
--rw-r--r--   0 tmu        (501) staff       (20)     8654 2023-01-15 16:35:26.000000 python-osc-1.8.1/pythonosc/dispatcher.py
--rw-r--r--   0 tmu        (501) staff       (20)     3778 2023-01-15 16:35:26.000000 python-osc-1.8.1/pythonosc/osc_bundle.py
--rw-r--r--   0 tmu        (501) staff       (20)     2057 2023-01-15 16:35:26.000000 python-osc-1.8.1/pythonosc/osc_bundle_builder.py
--rw-r--r--   0 tmu        (501) staff       (20)     4536 2023-01-15 16:35:26.000000 python-osc-1.8.1/pythonosc/osc_message.py
--rw-r--r--   0 tmu        (501) staff       (20)     7218 2023-01-15 16:35:26.000000 python-osc-1.8.1/pythonosc/osc_message_builder.py
--rw-r--r--   0 tmu        (501) staff       (20)     2748 2023-01-15 16:35:26.000000 python-osc-1.8.1/pythonosc/osc_packet.py
--rw-r--r--   0 tmu        (501) staff       (20)     5572 2023-01-15 16:35:26.000000 python-osc-1.8.1/pythonosc/osc_server.py
-drwxr-xr-x   0 tmu        (501) staff       (20)        0 2023-01-15 16:42:23.762704 python-osc-1.8.1/pythonosc/parsing/
--rw-r--r--   0 tmu        (501) staff       (20)        0 2017-12-19 02:21:53.000000 python-osc-1.8.1/pythonosc/parsing/__init__.py
--rw-r--r--   0 tmu        (501) staff       (20)     1886 2023-01-15 16:35:26.000000 python-osc-1.8.1/pythonosc/parsing/ntp.py
--rw-r--r--   0 tmu        (501) staff       (20)    15243 2023-01-15 16:35:26.000000 python-osc-1.8.1/pythonosc/parsing/osc_types.py
--rw-r--r--   0 tmu        (501) staff       (20)        0 2023-01-15 16:35:26.000000 python-osc-1.8.1/pythonosc/py.typed
-drwxr-xr-x   0 tmu        (501) staff       (20)        0 2023-01-15 16:42:23.769504 python-osc-1.8.1/pythonosc/test/
--rw-r--r--   0 tmu        (501) staff       (20)        0 2017-12-19 02:21:53.000000 python-osc-1.8.1/pythonosc/test/__init__.py
-drwxr-xr-x   0 tmu        (501) staff       (20)        0 2023-01-15 16:42:23.771426 python-osc-1.8.1/pythonosc/test/parsing/
--rw-r--r--   0 tmu        (501) staff       (20)        0 2017-12-19 02:21:53.000000 python-osc-1.8.1/pythonosc/test/parsing/__init__.py
--rw-r--r--   0 tmu        (501) staff       (20)      606 2021-05-23 18:08:21.000000 python-osc-1.8.1/pythonosc/test/parsing/test_ntp.py
--rw-r--r--   0 tmu        (501) staff       (20)    12457 2019-10-10 07:30:09.000000 python-osc-1.8.1/pythonosc/test/parsing/test_osc_types.py
--rw-r--r--   0 tmu        (501) staff       (20)     6136 2019-01-10 19:06:13.000000 python-osc-1.8.1/pythonosc/test/test_dispatcher.py
--rw-r--r--   0 tmu        (501) staff       (20)     4020 2019-01-10 19:06:13.000000 python-osc-1.8.1/pythonosc/test/test_osc_bundle.py
--rw-r--r--   0 tmu        (501) staff       (20)     1538 2019-01-10 19:06:13.000000 python-osc-1.8.1/pythonosc/test/test_osc_bundle_builder.py
--rw-r--r--   0 tmu        (501) staff       (20)    13236 2023-01-15 16:35:26.000000 python-osc-1.8.1/pythonosc/test/test_osc_message.py
--rw-r--r--   0 tmu        (501) staff       (20)     3800 2023-01-15 16:35:26.000000 python-osc-1.8.1/pythonosc/test/test_osc_message_builder.py
--rw-r--r--   0 tmu        (501) staff       (20)     2176 2019-01-10 19:06:13.000000 python-osc-1.8.1/pythonosc/test/test_osc_packet.py
--rw-r--r--   0 tmu        (501) staff       (20)     2796 2023-01-15 16:35:26.000000 python-osc-1.8.1/pythonosc/test/test_osc_server.py
--rw-r--r--   0 tmu        (501) staff       (20)     1864 2019-01-10 19:06:13.000000 python-osc-1.8.1/pythonosc/test/test_udp_client.py
--rw-r--r--   0 tmu        (501) staff       (20)     2606 2023-01-15 16:35:26.000000 python-osc-1.8.1/pythonosc/udp_client.py
--rw-r--r--   0 tmu        (501) staff       (20)      358 2023-01-15 16:42:23.773067 python-osc-1.8.1/setup.cfg
--rwxr-xr-x   0 tmu        (501) staff       (20)     1070 2023-01-15 16:37:21.000000 python-osc-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 18:06:16.257336 python-osc-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-08-05 18:06:07.000000 python-osc-1.8.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-05 18:06:07.000000 python-osc-1.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-08-05 18:06:16.257336 python-osc-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-08-05 18:06:07.000000 python-osc-1.8.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-05 18:06:07.000000 python-osc-1.8.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 18:06:16.253337 python-osc-1.8.2/python_osc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-08-05 18:06:16.000000 python-osc-1.8.2/python_osc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-05 18:06:16.000000 python-osc-1.8.2/python_osc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 18:06:16.000000 python-osc-1.8.2/python_osc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-05 18:06:16.000000 python-osc-1.8.2/python_osc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 18:06:16.253337 python-osc-1.8.2/pythonosc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/osc_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/osc_bundle_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/osc_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/osc_message_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/osc_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/osc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 18:06:16.253337 python-osc-1.8.2/pythonosc/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/parsing/ntp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15243 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/parsing/osc_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 18:06:16.257336 python-osc-1.8.2/pythonosc/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 18:06:16.257336 python-osc-1.8.2/pythonosc/test/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/test/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/test/parsing/test_ntp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/test/parsing/test_osc_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/test/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/test/test_osc_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/test/test_osc_bundle_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/test/test_osc_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/test/test_osc_message_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/test/test_osc_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/test/test_osc_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/test/test_udp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/udp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-05 18:06:16.257336 python-osc-1.8.2/setup.cfg
```

### Comparing `python-osc-1.8.1/LICENSE.txt` & `python-osc-1.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.1/PKG-INFO` & `python-osc-1.8.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,178 +1,202 @@
 Metadata-Version: 2.1
 Name: python-osc
-Version: 1.8.1
+Version: 1.8.2
 Summary: Open Sound Control server and client implementations in pure Python
-Home-page: https://github.com/attwad/python-osc
-Author: attwad
-Author-email: tmusoft@gmail.com
-License: UNKNOWN
-Description: ==========
-        python-osc
-        ==========
+Author-email: attwad <tmusoft@gmail.com>
+License: This is free and unencumbered software released into the public domain.
         
-        Open Sound Control server and client implementations in **pure python** (3.5+).
+        Anyone is free to copy, modify, publish, use, compile, sell, or
+        distribute this software, either in source code form or as a compiled
+        binary, for any purpose, commercial or non-commercial, and by any
+        means.
+        
+        In jurisdictions that recognize copyright laws, the author or authors
+        of this software dedicate any and all copyright interest in the
+        software to the public domain. We make this dedication for the benefit
+        of the public at large and to the detriment of our heirs and
+        successors. We intend this dedication to be an overt act of
+        relinquishment in perpetuity of all present and future rights to this
+        software under copyright law.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+        EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+        MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+        IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
+        OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+        ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+        OTHER DEALINGS IN THE SOFTWARE.
         
-        .. image:: https://github.com/attwad/python-osc/actions/workflows/python-test.yml/badge.svg
-            :target: https://github.com/attwad/python-osc/actions/workflows/python-test.yml
+        For more information, please refer to <http://unlicense.org/>
         
-        
-        Current status
-        ==============
-        
-        This library was developed following the
-        `OpenSoundControl Specification 1.0 <https://opensoundcontrol.stanford.edu/spec-1_0.html>`_
-        and is currently in a stable state.
-        
-        Features
-        ========
-        
-        * UDP blocking/threading/forking/asyncio server implementations
-        * UDP client
-        * int, int64, float, string, double, MIDI, timestamps, blob OSC arguments
-        * simple OSC address<->callback matching system
-        * extensive unit test coverage
-        * basic client and server examples
-        
-        Documentation
-        =============
-        
-        Available at https://python-osc.readthedocs.io/.
-        
-        Installation
-        ============
-        
-        python-osc is a pure python library that has no external dependencies,
-        to install it just use pip (prefered):
-        
-        .. image:: https://img.shields.io/pypi/v/python-osc.svg
-            :target: https://pypi.python.org/pypi/python-osc
-        
-        .. code-block:: bash
-        
-            $ pip install python-osc
-        
-        or from the raw sources for the development version:
-        
-        .. code-block:: bash
-        
-            $ python setup.py test
-            $ python setup.py install
-        
-        Examples
-        ========
-        
-        Simple client
-        -------------
-        
-        .. code-block:: python
-        
-          """Small example OSC client
-        
-          This program sends 10 random values between 0.0 and 1.0 to the /filter address,
-          waiting for 1 seconds between each value.
-          """
-          import argparse
-          import random
-          import time
-        
-          from pythonosc import udp_client
-        
-        
-          if __name__ == "__main__":
-            parser = argparse.ArgumentParser()
-            parser.add_argument("--ip", default="127.0.0.1",
-                help="The ip of the OSC server")
-            parser.add_argument("--port", type=int, default=5005,
-                help="The port the OSC server is listening on")
-            args = parser.parse_args()
-        
-            client = udp_client.SimpleUDPClient(args.ip, args.port)
-        
-            for x in range(10):
-              client.send_message("/filter", random.random())
-              time.sleep(1)
-        
-        Simple server
-        -------------
-        
-        .. code-block:: python
-        
-          """Small example OSC server
-        
-          This program listens to several addresses, and prints some information about
-          received packets.
-          """
-          import argparse
-          import math
-        
-          from pythonosc.dispatcher import Dispatcher
-          from pythonosc import osc_server
-        
-          def print_volume_handler(unused_addr, args, volume):
-            print("[{0}] ~ {1}".format(args[0], volume))
-        
-          def print_compute_handler(unused_addr, args, volume):
-            try:
-              print("[{0}] ~ {1}".format(args[0], args[1](volume)))
-            except ValueError: pass
-        
-          if __name__ == "__main__":
-            parser = argparse.ArgumentParser()
-            parser.add_argument("--ip",
-                default="127.0.0.1", help="The ip to listen on")
-            parser.add_argument("--port",
-                type=int, default=5005, help="The port to listen on")
-            args = parser.parse_args()
-        
-            dispatcher = Dispatcher()
-            dispatcher.map("/filter", print)
-            dispatcher.map("/volume", print_volume_handler, "Volume")
-            dispatcher.map("/logvolume", print_compute_handler, "Log volume", math.log)
-        
-            server = osc_server.ThreadingOSCUDPServer(
-                (args.ip, args.port), dispatcher)
-            print("Serving on {}".format(server.server_address))
-            server.serve_forever()
-        
-        Building bundles
-        ----------------
-        
-        .. code-block:: python
-        
-            from pythonosc import osc_bundle_builder
-            from pythonosc import osc_message_builder
-        
-            bundle = osc_bundle_builder.OscBundleBuilder(
-                osc_bundle_builder.IMMEDIATELY)
-            msg = osc_message_builder.OscMessageBuilder(address="/SYNC")
-            msg.add_arg(4.0)
-            # Add 4 messages in the bundle, each with more arguments.
-            bundle.add_content(msg.build())
-            msg.add_arg(2)
-            bundle.add_content(msg.build())
-            msg.add_arg("value")
-            bundle.add_content(msg.build())
-            msg.add_arg(b"\x01\x02\x03")
-            bundle.add_content(msg.build())
-        
-            sub_bundle = bundle.build()
-            # Now add the same bundle inside itself.
-            bundle.add_content(sub_bundle)
-            # The bundle has 5 elements in total now.
-        
-            bundle = bundle.build()
-            # You can now send it via a client as described in other examples.
-        
-        License?
-        ========
-        Unlicensed, do what you want with it. (http://unlicense.org)
-        
-Keywords: osc sound midi music
-Platform: any
+Project-URL: Repository, https://github.com/attwad/python-osc
+Keywords: osc,sound,midi,music
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: Freely Distributable
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: System :: Networking
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
+==========
+python-osc
+==========
+
+Open Sound Control server and client implementations in **pure python**.
+
+.. image:: https://github.com/attwad/python-osc/actions/workflows/python-test.yml/badge.svg
+    :target: https://github.com/attwad/python-osc/actions/workflows/python-test.yml
+
+
+Current status
+==============
+
+This library was developed following the
+`OpenSoundControl Specification 1.0 <https://opensoundcontrol.stanford.edu/spec-1_0.html>`_
+and is currently in a stable state.
+
+Features
+========
+
+* UDP blocking/threading/forking/asyncio server implementations
+* UDP client
+* int, int64, float, string, double, MIDI, timestamps, blob, nil OSC arguments
+* simple OSC address<->callback matching system
+* extensive unit test coverage
+* basic client and server examples
+
+Documentation
+=============
+
+Available at https://python-osc.readthedocs.io/.
+
+Installation
+============
+
+python-osc is a pure python library that has no external dependencies,
+to install it just use pip (prefered):
+
+.. image:: https://img.shields.io/pypi/v/python-osc.svg
+    :target: https://pypi.python.org/pypi/python-osc
+
+.. code-block:: bash
+
+    $ pip install python-osc
+
+or from the raw sources for the development version:
+
+.. code-block:: bash
+
+    $ python setup.py test
+    $ python setup.py install
+
+Examples
+========
+
+Simple client
+-------------
+
+.. code-block:: python
+
+  """Small example OSC client
+
+  This program sends 10 random values between 0.0 and 1.0 to the /filter address,
+  waiting for 1 seconds between each value.
+  """
+  import argparse
+  import random
+  import time
+
+  from pythonosc import udp_client
+
+
+  if __name__ == "__main__":
+    parser = argparse.ArgumentParser()
+    parser.add_argument("--ip", default="127.0.0.1",
+        help="The ip of the OSC server")
+    parser.add_argument("--port", type=int, default=5005,
+        help="The port the OSC server is listening on")
+    args = parser.parse_args()
+
+    client = udp_client.SimpleUDPClient(args.ip, args.port)
+
+    for x in range(10):
+      client.send_message("/filter", random.random())
+      time.sleep(1)
+
+Simple server
+-------------
+
+.. code-block:: python
+
+  """Small example OSC server
+
+  This program listens to several addresses, and prints some information about
+  received packets.
+  """
+  import argparse
+  import math
+
+  from pythonosc.dispatcher import Dispatcher
+  from pythonosc import osc_server
+
+  def print_volume_handler(unused_addr, args, volume):
+    print("[{0}] ~ {1}".format(args[0], volume))
+
+  def print_compute_handler(unused_addr, args, volume):
+    try:
+      print("[{0}] ~ {1}".format(args[0], args[1](volume)))
+    except ValueError: pass
+
+  if __name__ == "__main__":
+    parser = argparse.ArgumentParser()
+    parser.add_argument("--ip",
+        default="127.0.0.1", help="The ip to listen on")
+    parser.add_argument("--port",
+        type=int, default=5005, help="The port to listen on")
+    args = parser.parse_args()
+
+    dispatcher = Dispatcher()
+    dispatcher.map("/filter", print)
+    dispatcher.map("/volume", print_volume_handler, "Volume")
+    dispatcher.map("/logvolume", print_compute_handler, "Log volume", math.log)
+
+    server = osc_server.ThreadingOSCUDPServer(
+        (args.ip, args.port), dispatcher)
+    print("Serving on {}".format(server.server_address))
+    server.serve_forever()
+
+Building bundles
+----------------
+
+.. code-block:: python
+
+    from pythonosc import osc_bundle_builder
+    from pythonosc import osc_message_builder
+
+    bundle = osc_bundle_builder.OscBundleBuilder(
+        osc_bundle_builder.IMMEDIATELY)
+    msg = osc_message_builder.OscMessageBuilder(address="/SYNC")
+    msg.add_arg(4.0)
+    # Add 4 messages in the bundle, each with more arguments.
+    bundle.add_content(msg.build())
+    msg.add_arg(2)
+    bundle.add_content(msg.build())
+    msg.add_arg("value")
+    bundle.add_content(msg.build())
+    msg.add_arg(b"\x01\x02\x03")
+    bundle.add_content(msg.build())
+
+    sub_bundle = bundle.build()
+    # Now add the same bundle inside itself.
+    bundle.add_content(sub_bundle)
+    # The bundle has 5 elements in total now.
+
+    bundle = bundle.build()
+    # You can now send it via a client as described in other examples.
+
+License?
+========
+Unlicensed, do what you want with it. (http://unlicense.org)
```

### Comparing `python-osc-1.8.1/README.rst` & `python-osc-1.8.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ==========
 python-osc
 ==========
 
-Open Sound Control server and client implementations in **pure python** (3.5+).
+Open Sound Control server and client implementations in **pure python**.
 
 .. image:: https://github.com/attwad/python-osc/actions/workflows/python-test.yml/badge.svg
     :target: https://github.com/attwad/python-osc/actions/workflows/python-test.yml
 
 
 Current status
 ==============
@@ -16,15 +16,15 @@
 and is currently in a stable state.
 
 Features
 ========
 
 * UDP blocking/threading/forking/asyncio server implementations
 * UDP client
-* int, int64, float, string, double, MIDI, timestamps, blob OSC arguments
+* int, int64, float, string, double, MIDI, timestamps, blob, nil OSC arguments
 * simple OSC address<->callback matching system
 * extensive unit test coverage
 * basic client and server examples
 
 Documentation
 =============
```

### Comparing `python-osc-1.8.1/python_osc.egg-info/PKG-INFO` & `python-osc-1.8.2/python_osc.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,178 +1,202 @@
 Metadata-Version: 2.1
 Name: python-osc
-Version: 1.8.1
+Version: 1.8.2
 Summary: Open Sound Control server and client implementations in pure Python
-Home-page: https://github.com/attwad/python-osc
-Author: attwad
-Author-email: tmusoft@gmail.com
-License: UNKNOWN
-Description: ==========
-        python-osc
-        ==========
+Author-email: attwad <tmusoft@gmail.com>
+License: This is free and unencumbered software released into the public domain.
         
-        Open Sound Control server and client implementations in **pure python** (3.5+).
+        Anyone is free to copy, modify, publish, use, compile, sell, or
+        distribute this software, either in source code form or as a compiled
+        binary, for any purpose, commercial or non-commercial, and by any
+        means.
+        
+        In jurisdictions that recognize copyright laws, the author or authors
+        of this software dedicate any and all copyright interest in the
+        software to the public domain. We make this dedication for the benefit
+        of the public at large and to the detriment of our heirs and
+        successors. We intend this dedication to be an overt act of
+        relinquishment in perpetuity of all present and future rights to this
+        software under copyright law.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+        EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+        MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+        IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
+        OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+        ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+        OTHER DEALINGS IN THE SOFTWARE.
         
-        .. image:: https://github.com/attwad/python-osc/actions/workflows/python-test.yml/badge.svg
-            :target: https://github.com/attwad/python-osc/actions/workflows/python-test.yml
+        For more information, please refer to <http://unlicense.org/>
         
-        
-        Current status
-        ==============
-        
-        This library was developed following the
-        `OpenSoundControl Specification 1.0 <https://opensoundcontrol.stanford.edu/spec-1_0.html>`_
-        and is currently in a stable state.
-        
-        Features
-        ========
-        
-        * UDP blocking/threading/forking/asyncio server implementations
-        * UDP client
-        * int, int64, float, string, double, MIDI, timestamps, blob OSC arguments
-        * simple OSC address<->callback matching system
-        * extensive unit test coverage
-        * basic client and server examples
-        
-        Documentation
-        =============
-        
-        Available at https://python-osc.readthedocs.io/.
-        
-        Installation
-        ============
-        
-        python-osc is a pure python library that has no external dependencies,
-        to install it just use pip (prefered):
-        
-        .. image:: https://img.shields.io/pypi/v/python-osc.svg
-            :target: https://pypi.python.org/pypi/python-osc
-        
-        .. code-block:: bash
-        
-            $ pip install python-osc
-        
-        or from the raw sources for the development version:
-        
-        .. code-block:: bash
-        
-            $ python setup.py test
-            $ python setup.py install
-        
-        Examples
-        ========
-        
-        Simple client
-        -------------
-        
-        .. code-block:: python
-        
-          """Small example OSC client
-        
-          This program sends 10 random values between 0.0 and 1.0 to the /filter address,
-          waiting for 1 seconds between each value.
-          """
-          import argparse
-          import random
-          import time
-        
-          from pythonosc import udp_client
-        
-        
-          if __name__ == "__main__":
-            parser = argparse.ArgumentParser()
-            parser.add_argument("--ip", default="127.0.0.1",
-                help="The ip of the OSC server")
-            parser.add_argument("--port", type=int, default=5005,
-                help="The port the OSC server is listening on")
-            args = parser.parse_args()
-        
-            client = udp_client.SimpleUDPClient(args.ip, args.port)
-        
-            for x in range(10):
-              client.send_message("/filter", random.random())
-              time.sleep(1)
-        
-        Simple server
-        -------------
-        
-        .. code-block:: python
-        
-          """Small example OSC server
-        
-          This program listens to several addresses, and prints some information about
-          received packets.
-          """
-          import argparse
-          import math
-        
-          from pythonosc.dispatcher import Dispatcher
-          from pythonosc import osc_server
-        
-          def print_volume_handler(unused_addr, args, volume):
-            print("[{0}] ~ {1}".format(args[0], volume))
-        
-          def print_compute_handler(unused_addr, args, volume):
-            try:
-              print("[{0}] ~ {1}".format(args[0], args[1](volume)))
-            except ValueError: pass
-        
-          if __name__ == "__main__":
-            parser = argparse.ArgumentParser()
-            parser.add_argument("--ip",
-                default="127.0.0.1", help="The ip to listen on")
-            parser.add_argument("--port",
-                type=int, default=5005, help="The port to listen on")
-            args = parser.parse_args()
-        
-            dispatcher = Dispatcher()
-            dispatcher.map("/filter", print)
-            dispatcher.map("/volume", print_volume_handler, "Volume")
-            dispatcher.map("/logvolume", print_compute_handler, "Log volume", math.log)
-        
-            server = osc_server.ThreadingOSCUDPServer(
-                (args.ip, args.port), dispatcher)
-            print("Serving on {}".format(server.server_address))
-            server.serve_forever()
-        
-        Building bundles
-        ----------------
-        
-        .. code-block:: python
-        
-            from pythonosc import osc_bundle_builder
-            from pythonosc import osc_message_builder
-        
-            bundle = osc_bundle_builder.OscBundleBuilder(
-                osc_bundle_builder.IMMEDIATELY)
-            msg = osc_message_builder.OscMessageBuilder(address="/SYNC")
-            msg.add_arg(4.0)
-            # Add 4 messages in the bundle, each with more arguments.
-            bundle.add_content(msg.build())
-            msg.add_arg(2)
-            bundle.add_content(msg.build())
-            msg.add_arg("value")
-            bundle.add_content(msg.build())
-            msg.add_arg(b"\x01\x02\x03")
-            bundle.add_content(msg.build())
-        
-            sub_bundle = bundle.build()
-            # Now add the same bundle inside itself.
-            bundle.add_content(sub_bundle)
-            # The bundle has 5 elements in total now.
-        
-            bundle = bundle.build()
-            # You can now send it via a client as described in other examples.
-        
-        License?
-        ========
-        Unlicensed, do what you want with it. (http://unlicense.org)
-        
-Keywords: osc sound midi music
-Platform: any
+Project-URL: Repository, https://github.com/attwad/python-osc
+Keywords: osc,sound,midi,music
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: Freely Distributable
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: System :: Networking
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
+==========
+python-osc
+==========
+
+Open Sound Control server and client implementations in **pure python**.
+
+.. image:: https://github.com/attwad/python-osc/actions/workflows/python-test.yml/badge.svg
+    :target: https://github.com/attwad/python-osc/actions/workflows/python-test.yml
+
+
+Current status
+==============
+
+This library was developed following the
+`OpenSoundControl Specification 1.0 <https://opensoundcontrol.stanford.edu/spec-1_0.html>`_
+and is currently in a stable state.
+
+Features
+========
+
+* UDP blocking/threading/forking/asyncio server implementations
+* UDP client
+* int, int64, float, string, double, MIDI, timestamps, blob, nil OSC arguments
+* simple OSC address<->callback matching system
+* extensive unit test coverage
+* basic client and server examples
+
+Documentation
+=============
+
+Available at https://python-osc.readthedocs.io/.
+
+Installation
+============
+
+python-osc is a pure python library that has no external dependencies,
+to install it just use pip (prefered):
+
+.. image:: https://img.shields.io/pypi/v/python-osc.svg
+    :target: https://pypi.python.org/pypi/python-osc
+
+.. code-block:: bash
+
+    $ pip install python-osc
+
+or from the raw sources for the development version:
+
+.. code-block:: bash
+
+    $ python setup.py test
+    $ python setup.py install
+
+Examples
+========
+
+Simple client
+-------------
+
+.. code-block:: python
+
+  """Small example OSC client
+
+  This program sends 10 random values between 0.0 and 1.0 to the /filter address,
+  waiting for 1 seconds between each value.
+  """
+  import argparse
+  import random
+  import time
+
+  from pythonosc import udp_client
+
+
+  if __name__ == "__main__":
+    parser = argparse.ArgumentParser()
+    parser.add_argument("--ip", default="127.0.0.1",
+        help="The ip of the OSC server")
+    parser.add_argument("--port", type=int, default=5005,
+        help="The port the OSC server is listening on")
+    args = parser.parse_args()
+
+    client = udp_client.SimpleUDPClient(args.ip, args.port)
+
+    for x in range(10):
+      client.send_message("/filter", random.random())
+      time.sleep(1)
+
+Simple server
+-------------
+
+.. code-block:: python
+
+  """Small example OSC server
+
+  This program listens to several addresses, and prints some information about
+  received packets.
+  """
+  import argparse
+  import math
+
+  from pythonosc.dispatcher import Dispatcher
+  from pythonosc import osc_server
+
+  def print_volume_handler(unused_addr, args, volume):
+    print("[{0}] ~ {1}".format(args[0], volume))
+
+  def print_compute_handler(unused_addr, args, volume):
+    try:
+      print("[{0}] ~ {1}".format(args[0], args[1](volume)))
+    except ValueError: pass
+
+  if __name__ == "__main__":
+    parser = argparse.ArgumentParser()
+    parser.add_argument("--ip",
+        default="127.0.0.1", help="The ip to listen on")
+    parser.add_argument("--port",
+        type=int, default=5005, help="The port to listen on")
+    args = parser.parse_args()
+
+    dispatcher = Dispatcher()
+    dispatcher.map("/filter", print)
+    dispatcher.map("/volume", print_volume_handler, "Volume")
+    dispatcher.map("/logvolume", print_compute_handler, "Log volume", math.log)
+
+    server = osc_server.ThreadingOSCUDPServer(
+        (args.ip, args.port), dispatcher)
+    print("Serving on {}".format(server.server_address))
+    server.serve_forever()
+
+Building bundles
+----------------
+
+.. code-block:: python
+
+    from pythonosc import osc_bundle_builder
+    from pythonosc import osc_message_builder
+
+    bundle = osc_bundle_builder.OscBundleBuilder(
+        osc_bundle_builder.IMMEDIATELY)
+    msg = osc_message_builder.OscMessageBuilder(address="/SYNC")
+    msg.add_arg(4.0)
+    # Add 4 messages in the bundle, each with more arguments.
+    bundle.add_content(msg.build())
+    msg.add_arg(2)
+    bundle.add_content(msg.build())
+    msg.add_arg("value")
+    bundle.add_content(msg.build())
+    msg.add_arg(b"\x01\x02\x03")
+    bundle.add_content(msg.build())
+
+    sub_bundle = bundle.build()
+    # Now add the same bundle inside itself.
+    bundle.add_content(sub_bundle)
+    # The bundle has 5 elements in total now.
+
+    bundle = bundle.build()
+    # You can now send it via a client as described in other examples.
+
+License?
+========
+Unlicensed, do what you want with it. (http://unlicense.org)
```

### Comparing `python-osc-1.8.1/python_osc.egg-info/SOURCES.txt` & `python-osc-1.8.2/python_osc.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
-setup.py
 python_osc.egg-info/PKG-INFO
 python_osc.egg-info/SOURCES.txt
 python_osc.egg-info/dependency_links.txt
 python_osc.egg-info/top_level.txt
 pythonosc/__init__.py
 pythonosc/dispatcher.py
 pythonosc/osc_bundle.py
```

### Comparing `python-osc-1.8.1/pythonosc/dispatcher.py` & `python-osc-1.8.2/pythonosc/dispatcher.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.1/pythonosc/osc_bundle.py` & `python-osc-1.8.2/pythonosc/osc_bundle.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.1/pythonosc/osc_bundle_builder.py` & `python-osc-1.8.2/pythonosc/osc_bundle_builder.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.1/pythonosc/osc_message.py` & `python-osc-1.8.2/pythonosc/osc_message.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.1/pythonosc/osc_message_builder.py` & `python-osc-1.8.2/pythonosc/osc_message_builder.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.1/pythonosc/osc_packet.py` & `python-osc-1.8.2/pythonosc/osc_packet.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.1/pythonosc/osc_server.py` & `python-osc-1.8.2/pythonosc/osc_server.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.1/pythonosc/parsing/ntp.py` & `python-osc-1.8.2/pythonosc/parsing/ntp.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.1/pythonosc/parsing/osc_types.py` & `python-osc-1.8.2/pythonosc/parsing/osc_types.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.1/pythonosc/test/parsing/test_ntp.py` & `python-osc-1.8.2/pythonosc/test/parsing/test_ntp.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.1/pythonosc/test/parsing/test_osc_types.py` & `python-osc-1.8.2/pythonosc/test/parsing/test_osc_types.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.1/pythonosc/test/test_dispatcher.py` & `python-osc-1.8.2/pythonosc/test/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.1/pythonosc/test/test_osc_bundle.py` & `python-osc-1.8.2/pythonosc/test/test_osc_bundle.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.1/pythonosc/test/test_osc_bundle_builder.py` & `python-osc-1.8.2/pythonosc/test/test_osc_bundle_builder.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.1/pythonosc/test/test_osc_message.py` & `python-osc-1.8.2/pythonosc/test/test_osc_message.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.1/pythonosc/test/test_osc_message_builder.py` & `python-osc-1.8.2/pythonosc/test/test_osc_message_builder.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.1/pythonosc/test/test_osc_packet.py` & `python-osc-1.8.2/pythonosc/test/test_osc_packet.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.1/pythonosc/test/test_osc_server.py` & `python-osc-1.8.2/pythonosc/test/test_osc_server.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.1/pythonosc/test/test_udp_client.py` & `python-osc-1.8.2/pythonosc/test/test_udp_client.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.1/pythonosc/udp_client.py` & `python-osc-1.8.2/pythonosc/udp_client.py`

 * *Files identical despite different names*

