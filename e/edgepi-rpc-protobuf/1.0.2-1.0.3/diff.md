# Comparing `tmp/edgepi-rpc-protobuf-1.0.2.tar.gz` & `tmp/edgepi-rpc-protobuf-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgepi-rpc-protobuf-1.0.2.tar", last modified: Mon Jul 31 23:43:03 2023, max compression
+gzip compressed data, was "edgepi-rpc-protobuf-1.0.3.tar", last modified: Fri Aug  4 22:17:57 2023, max compression
```

## Comparing `edgepi-rpc-protobuf-1.0.2.tar` & `edgepi-rpc-protobuf-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:43:03.541235 edgepi-rpc-protobuf-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-31 23:42:41.000000 edgepi-rpc-protobuf-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-31 23:43:03.541235 edgepi-rpc-protobuf-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 23:42:41.000000 edgepi-rpc-protobuf-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-31 23:42:41.000000 edgepi-rpc-protobuf-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-31 23:43:03.541235 edgepi-rpc-protobuf-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:43:03.537235 edgepi-rpc-protobuf-1.0.2/src-python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:43:03.541235 edgepi-rpc-protobuf-1.0.2/src-python/edgepi_rpc_protobuf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-31 23:43:03.000000 edgepi-rpc-protobuf-1.0.2/src-python/edgepi_rpc_protobuf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-31 23:43:03.000000 edgepi-rpc-protobuf-1.0.2/src-python/edgepi_rpc_protobuf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 23:43:03.000000 edgepi-rpc-protobuf-1.0.2/src-python/edgepi_rpc_protobuf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-31 23:43:03.000000 edgepi-rpc-protobuf-1.0.2/src-python/edgepi_rpc_protobuf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:43:03.541235 edgepi-rpc-protobuf-1.0.2/src-python/edgepirpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 23:42:41.000000 edgepi-rpc-protobuf-1.0.2/src-python/edgepirpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:43:03.541235 edgepi-rpc-protobuf-1.0.2/src-python/edgepirpc/protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 23:42:41.000000 edgepi-rpc-protobuf-1.0.2/src-python/edgepirpc/protos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-31 23:42:42.000000 edgepi-rpc-protobuf-1.0.2/src-python/edgepirpc/protos/dout_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-31 23:42:42.000000 edgepi-rpc-protobuf-1.0.2/src-python/edgepirpc/protos/led_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-31 23:42:42.000000 edgepi-rpc-protobuf-1.0.2/src-python/edgepirpc/protos/rpc_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-07-31 23:42:42.000000 edgepi-rpc-protobuf-1.0.2/src-python/edgepirpc/protos/tc_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:17:57.807489 edgepi-rpc-protobuf-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-04 22:17:39.000000 edgepi-rpc-protobuf-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-04 22:17:57.807489 edgepi-rpc-protobuf-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 22:17:39.000000 edgepi-rpc-protobuf-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-04 22:17:39.000000 edgepi-rpc-protobuf-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-04 22:17:57.807489 edgepi-rpc-protobuf-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:17:57.803489 edgepi-rpc-protobuf-1.0.3/src-python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:17:57.803489 edgepi-rpc-protobuf-1.0.3/src-python/edgepi_rpc_protobuf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-04 22:17:57.000000 edgepi-rpc-protobuf-1.0.3/src-python/edgepi_rpc_protobuf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-08-04 22:17:57.000000 edgepi-rpc-protobuf-1.0.3/src-python/edgepi_rpc_protobuf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 22:17:57.000000 edgepi-rpc-protobuf-1.0.3/src-python/edgepi_rpc_protobuf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-04 22:17:57.000000 edgepi-rpc-protobuf-1.0.3/src-python/edgepi_rpc_protobuf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:17:57.803489 edgepi-rpc-protobuf-1.0.3/src-python/edgepirpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 22:17:39.000000 edgepi-rpc-protobuf-1.0.3/src-python/edgepirpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:17:57.807489 edgepi-rpc-protobuf-1.0.3/src-python/edgepirpc/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 22:17:39.000000 edgepi-rpc-protobuf-1.0.3/src-python/edgepirpc/protos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-08-04 22:17:39.000000 edgepi-rpc-protobuf-1.0.3/src-python/edgepirpc/protos/din_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-08-04 22:17:39.000000 edgepi-rpc-protobuf-1.0.3/src-python/edgepirpc/protos/dout_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-08-04 22:17:39.000000 edgepi-rpc-protobuf-1.0.3/src-python/edgepirpc/protos/led_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-04 22:17:39.000000 edgepi-rpc-protobuf-1.0.3/src-python/edgepirpc/protos/rpc_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-08-04 22:17:39.000000 edgepi-rpc-protobuf-1.0.3/src-python/edgepirpc/protos/tc_pb2.py
```

### Comparing `edgepi-rpc-protobuf-1.0.2/LICENSE` & `edgepi-rpc-protobuf-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `edgepi-rpc-protobuf-1.0.2/setup.cfg` & `edgepi-rpc-protobuf-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = edgepi-rpc-protobuf
-version = 1.0.2
+version = 1.0.3
 author = Isaac James
 author_email = ijames@osensa.com
 description = Protobuf generated code for EdgePi RPC
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/EdgePi-Cloud/edgepi-rpc-protobuf
 classifiers =
```

### Comparing `edgepi-rpc-protobuf-1.0.2/src-python/edgepirpc/protos/dout_pb2.py` & `edgepi-rpc-protobuf-1.0.3/src-python/edgepirpc/protos/dout_pb2.py`

 * *Files identical despite different names*

### Comparing `edgepi-rpc-protobuf-1.0.2/src-python/edgepirpc/protos/led_pb2.py` & `edgepi-rpc-protobuf-1.0.3/src-python/edgepirpc/protos/led_pb2.py`

 * *Files identical despite different names*

### Comparing `edgepi-rpc-protobuf-1.0.2/src-python/edgepirpc/protos/rpc_pb2.py` & `edgepi-rpc-protobuf-1.0.3/src-python/edgepirpc/protos/rpc_pb2.py`

 * *Files identical despite different names*

### Comparing `edgepi-rpc-protobuf-1.0.2/src-python/edgepirpc/protos/tc_pb2.py` & `edgepi-rpc-protobuf-1.0.3/src-python/edgepirpc/protos/tc_pb2.py`

 * *Files identical despite different names*

