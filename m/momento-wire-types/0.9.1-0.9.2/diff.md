# Comparing `tmp/momento-wire-types-0.9.1.tar.gz` & `tmp/momento-wire-types-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momento-wire-types-0.9.1.tar", last modified: Thu Mar 24 16:43:21 2022, max compression
+gzip compressed data, was "momento-wire-types-0.9.2.tar", last modified: Fri Mar 25 00:02:31 2022, max compression
```

## Comparing `momento-wire-types-0.9.1.tar` & `momento-wire-types-0.9.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 16:43:21.750877 momento-wire-types-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-03-24 16:43:21.750877 momento-wire-types-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-03-24 16:43:09.000000 momento-wire-types-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-03-24 16:43:21.750877 momento-wire-types-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-03-24 16:43:09.000000 momento-wire-types-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 16:43:21.746877 momento-wire-types-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 16:43:21.750877 momento-wire-types-0.9.1/src/momento_wire_types/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-24 16:43:09.000000 momento-wire-types-0.9.1/src/momento_wire_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3741 2022-03-24 16:43:21.000000 momento-wire-types-0.9.1/src/momento_wire_types/cacheclient_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     3811 2022-03-24 16:43:21.000000 momento-wire-types-0.9.1/src/momento_wire_types/cacheclient_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     5054 2022-03-24 16:43:21.000000 momento-wire-types-0.9.1/src/momento_wire_types/controlclient_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     5693 2022-03-24 16:43:21.000000 momento-wire-types-0.9.1/src/momento_wire_types/controlclient_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 16:43:21.750877 momento-wire-types-0.9.1/src/momento_wire_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-03-24 16:43:21.000000 momento-wire-types-0.9.1/src/momento_wire_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-03-24 16:43:21.000000 momento-wire-types-0.9.1/src/momento_wire_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-24 16:43:21.000000 momento-wire-types-0.9.1/src/momento_wire_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-03-24 16:43:21.000000 momento-wire-types-0.9.1/src/momento_wire_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-03-24 16:43:21.000000 momento-wire-types-0.9.1/src/momento_wire_types.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-25 00:02:31.968652 momento-wire-types-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)      507 2022-03-25 00:02:31.968652 momento-wire-types-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-03-25 00:02:18.000000 momento-wire-types-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      322 2022-03-25 00:02:31.972652 momento-wire-types-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      443 2022-03-25 00:02:18.000000 momento-wire-types-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-25 00:02:31.968652 momento-wire-types-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-25 00:02:31.968652 momento-wire-types-0.9.2/src/momento_wire_types/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-25 00:02:18.000000 momento-wire-types-0.9.2/src/momento_wire_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3741 2022-03-25 00:02:31.000000 momento-wire-types-0.9.2/src/momento_wire_types/cacheclient_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3811 2022-03-25 00:02:31.000000 momento-wire-types-0.9.2/src/momento_wire_types/cacheclient_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5054 2022-03-25 00:02:31.000000 momento-wire-types-0.9.2/src/momento_wire_types/controlclient_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5693 2022-03-25 00:02:31.000000 momento-wire-types-0.9.2/src/momento_wire_types/controlclient_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-25 00:02:31.968652 momento-wire-types-0.9.2/src/momento_wire_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      507 2022-03-25 00:02:31.000000 momento-wire-types-0.9.2/src/momento_wire_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2022-03-25 00:02:31.000000 momento-wire-types-0.9.2/src/momento_wire_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-25 00:02:31.000000 momento-wire-types-0.9.2/src/momento_wire_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-03-25 00:02:31.000000 momento-wire-types-0.9.2/src/momento_wire_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-03-25 00:02:31.000000 momento-wire-types-0.9.2/src/momento_wire_types.egg-info/top_level.txt
```

### Comparing `momento-wire-types-0.9.1/src/momento_wire_types/cacheclient_pb2.py` & `momento-wire-types-0.9.2/src/momento_wire_types/cacheclient_pb2.py`

 * *Files identical despite different names*

### Comparing `momento-wire-types-0.9.1/src/momento_wire_types/cacheclient_pb2_grpc.py` & `momento-wire-types-0.9.2/src/momento_wire_types/cacheclient_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `momento-wire-types-0.9.1/src/momento_wire_types/controlclient_pb2.py` & `momento-wire-types-0.9.2/src/momento_wire_types/controlclient_pb2.py`

 * *Files identical despite different names*

### Comparing `momento-wire-types-0.9.1/src/momento_wire_types/controlclient_pb2_grpc.py` & `momento-wire-types-0.9.2/src/momento_wire_types/controlclient_pb2_grpc.py`

 * *Files identical despite different names*

