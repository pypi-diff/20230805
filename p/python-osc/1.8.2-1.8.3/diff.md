# Comparing `tmp/python-osc-1.8.2.tar.gz` & `tmp/python-osc-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-osc-1.8.2.tar", last modified: Sat Aug  5 18:06:16 2023, max compression
+gzip compressed data, was "python-osc-1.8.3.tar", last modified: Sat Aug  5 18:19:30 2023, max compression
```

## Comparing `python-osc-1.8.2.tar` & `python-osc-1.8.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 18:06:16.257336 python-osc-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-08-05 18:06:07.000000 python-osc-1.8.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-05 18:06:07.000000 python-osc-1.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-08-05 18:06:16.257336 python-osc-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-08-05 18:06:07.000000 python-osc-1.8.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-05 18:06:07.000000 python-osc-1.8.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 18:06:16.253337 python-osc-1.8.2/python_osc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-08-05 18:06:16.000000 python-osc-1.8.2/python_osc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-05 18:06:16.000000 python-osc-1.8.2/python_osc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 18:06:16.000000 python-osc-1.8.2/python_osc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-05 18:06:16.000000 python-osc-1.8.2/python_osc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 18:06:16.253337 python-osc-1.8.2/pythonosc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/osc_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/osc_bundle_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/osc_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/osc_message_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/osc_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/osc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 18:06:16.253337 python-osc-1.8.2/pythonosc/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/parsing/ntp.py
--rw-r--r--   0 runner    (1001) docker     (123)    15243 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/parsing/osc_types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 18:06:16.257336 python-osc-1.8.2/pythonosc/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 18:06:16.257336 python-osc-1.8.2/pythonosc/test/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/test/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/test/parsing/test_ntp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/test/parsing/test_osc_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/test/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/test/test_osc_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/test/test_osc_bundle_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/test/test_osc_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/test/test_osc_message_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/test/test_osc_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/test/test_osc_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/test/test_udp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-08-05 18:06:07.000000 python-osc-1.8.2/pythonosc/udp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-05 18:06:16.257336 python-osc-1.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 18:19:30.658362 python-osc-1.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-08-05 18:19:19.000000 python-osc-1.8.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-05 18:19:19.000000 python-osc-1.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-08-05 18:19:30.658362 python-osc-1.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-08-05 18:19:19.000000 python-osc-1.8.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-05 18:19:19.000000 python-osc-1.8.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 18:19:30.658362 python-osc-1.8.3/python_osc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-08-05 18:19:30.000000 python-osc-1.8.3/python_osc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-05 18:19:30.000000 python-osc-1.8.3/python_osc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 18:19:30.000000 python-osc-1.8.3/python_osc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-05 18:19:30.000000 python-osc-1.8.3/python_osc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 18:19:30.658362 python-osc-1.8.3/pythonosc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 18:19:19.000000 python-osc-1.8.3/pythonosc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-08-05 18:19:19.000000 python-osc-1.8.3/pythonosc/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-08-05 18:19:19.000000 python-osc-1.8.3/pythonosc/osc_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-08-05 18:19:19.000000 python-osc-1.8.3/pythonosc/osc_bundle_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-08-05 18:19:19.000000 python-osc-1.8.3/pythonosc/osc_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-08-05 18:19:19.000000 python-osc-1.8.3/pythonosc/osc_message_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-08-05 18:19:19.000000 python-osc-1.8.3/pythonosc/osc_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-08-05 18:19:19.000000 python-osc-1.8.3/pythonosc/osc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 18:19:30.658362 python-osc-1.8.3/pythonosc/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 18:19:19.000000 python-osc-1.8.3/pythonosc/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-08-05 18:19:19.000000 python-osc-1.8.3/pythonosc/parsing/ntp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15243 2023-08-05 18:19:19.000000 python-osc-1.8.3/pythonosc/parsing/osc_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 18:19:19.000000 python-osc-1.8.3/pythonosc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 18:19:30.658362 python-osc-1.8.3/pythonosc/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 18:19:19.000000 python-osc-1.8.3/pythonosc/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 18:19:30.658362 python-osc-1.8.3/pythonosc/test/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 18:19:19.000000 python-osc-1.8.3/pythonosc/test/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-05 18:19:19.000000 python-osc-1.8.3/pythonosc/test/parsing/test_ntp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-08-05 18:19:19.000000 python-osc-1.8.3/pythonosc/test/parsing/test_osc_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-08-05 18:19:19.000000 python-osc-1.8.3/pythonosc/test/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-08-05 18:19:19.000000 python-osc-1.8.3/pythonosc/test/test_osc_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-08-05 18:19:19.000000 python-osc-1.8.3/pythonosc/test/test_osc_bundle_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-08-05 18:19:19.000000 python-osc-1.8.3/pythonosc/test/test_osc_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-08-05 18:19:19.000000 python-osc-1.8.3/pythonosc/test/test_osc_message_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-08-05 18:19:19.000000 python-osc-1.8.3/pythonosc/test/test_osc_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-08-05 18:19:19.000000 python-osc-1.8.3/pythonosc/test/test_osc_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-08-05 18:19:19.000000 python-osc-1.8.3/pythonosc/test/test_udp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-08-05 18:19:19.000000 python-osc-1.8.3/pythonosc/udp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-05 18:19:30.662362 python-osc-1.8.3/setup.cfg
```

### Comparing `python-osc-1.8.2/LICENSE.txt` & `python-osc-1.8.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.2/PKG-INFO` & `python-osc-1.8.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-osc
-Version: 1.8.2
+Version: 1.8.3
 Summary: Open Sound Control server and client implementations in pure Python
 Author-email: attwad <tmusoft@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -81,21 +81,14 @@
 .. image:: https://img.shields.io/pypi/v/python-osc.svg
     :target: https://pypi.python.org/pypi/python-osc
 
 .. code-block:: bash
 
     $ pip install python-osc
 
-or from the raw sources for the development version:
-
-.. code-block:: bash
-
-    $ python setup.py test
-    $ python setup.py install
-
 Examples
 ========
 
 Simple client
 -------------
 
 .. code-block:: python
```

### Comparing `python-osc-1.8.2/README.rst` & `python-osc-1.8.3/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -39,21 +39,14 @@
 .. image:: https://img.shields.io/pypi/v/python-osc.svg
     :target: https://pypi.python.org/pypi/python-osc
 
 .. code-block:: bash
 
     $ pip install python-osc
 
-or from the raw sources for the development version:
-
-.. code-block:: bash
-
-    $ python setup.py test
-    $ python setup.py install
-
 Examples
 ========
 
 Simple client
 -------------
 
 .. code-block:: python
```

### Comparing `python-osc-1.8.2/pyproject.toml` & `python-osc-1.8.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python-osc"
-version="1.8.2"
+version="1.8.3"
 description="Open Sound Control server and client implementations in pure Python"
 readme="README.rst"
 requires-python=">=3.7"
 license = {file = "LICENSE.txt"}
 authors = [
   {name = "attwad", email = "tmusoft@gmail.com"},
 ]
```

### Comparing `python-osc-1.8.2/python_osc.egg-info/PKG-INFO` & `python-osc-1.8.3/python_osc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-osc
-Version: 1.8.2
+Version: 1.8.3
 Summary: Open Sound Control server and client implementations in pure Python
 Author-email: attwad <tmusoft@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -81,21 +81,14 @@
 .. image:: https://img.shields.io/pypi/v/python-osc.svg
     :target: https://pypi.python.org/pypi/python-osc
 
 .. code-block:: bash
 
     $ pip install python-osc
 
-or from the raw sources for the development version:
-
-.. code-block:: bash
-
-    $ python setup.py test
-    $ python setup.py install
-
 Examples
 ========
 
 Simple client
 -------------
 
 .. code-block:: python
```

### Comparing `python-osc-1.8.2/python_osc.egg-info/SOURCES.txt` & `python-osc-1.8.3/python_osc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.2/pythonosc/dispatcher.py` & `python-osc-1.8.3/pythonosc/dispatcher.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.2/pythonosc/osc_bundle.py` & `python-osc-1.8.3/pythonosc/osc_bundle.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.2/pythonosc/osc_bundle_builder.py` & `python-osc-1.8.3/pythonosc/osc_bundle_builder.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.2/pythonosc/osc_message.py` & `python-osc-1.8.3/pythonosc/osc_message.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.2/pythonosc/osc_message_builder.py` & `python-osc-1.8.3/pythonosc/osc_message_builder.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.2/pythonosc/osc_packet.py` & `python-osc-1.8.3/pythonosc/osc_packet.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.2/pythonosc/osc_server.py` & `python-osc-1.8.3/pythonosc/osc_server.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.2/pythonosc/parsing/ntp.py` & `python-osc-1.8.3/pythonosc/parsing/ntp.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.2/pythonosc/parsing/osc_types.py` & `python-osc-1.8.3/pythonosc/parsing/osc_types.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.2/pythonosc/test/parsing/test_ntp.py` & `python-osc-1.8.3/pythonosc/test/parsing/test_ntp.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.2/pythonosc/test/parsing/test_osc_types.py` & `python-osc-1.8.3/pythonosc/test/parsing/test_osc_types.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.2/pythonosc/test/test_dispatcher.py` & `python-osc-1.8.3/pythonosc/test/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.2/pythonosc/test/test_osc_bundle.py` & `python-osc-1.8.3/pythonosc/test/test_osc_bundle.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.2/pythonosc/test/test_osc_bundle_builder.py` & `python-osc-1.8.3/pythonosc/test/test_osc_bundle_builder.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.2/pythonosc/test/test_osc_message.py` & `python-osc-1.8.3/pythonosc/test/test_osc_message.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.2/pythonosc/test/test_osc_message_builder.py` & `python-osc-1.8.3/pythonosc/test/test_osc_message_builder.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.2/pythonosc/test/test_osc_packet.py` & `python-osc-1.8.3/pythonosc/test/test_osc_packet.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.2/pythonosc/test/test_osc_server.py` & `python-osc-1.8.3/pythonosc/test/test_osc_server.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.2/pythonosc/test/test_udp_client.py` & `python-osc-1.8.3/pythonosc/test/test_udp_client.py`

 * *Files identical despite different names*

### Comparing `python-osc-1.8.2/pythonosc/udp_client.py` & `python-osc-1.8.3/pythonosc/udp_client.py`

 * *Files identical despite different names*

