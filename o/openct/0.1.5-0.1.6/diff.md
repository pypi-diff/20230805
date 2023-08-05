# Comparing `tmp/openct-0.1.5.tar.gz` & `tmp/openct-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openct-0.1.5.tar", max compression
+gzip compressed data, was "openct-0.1.6.tar", max compression
```

## Comparing `openct-0.1.5.tar` & `openct-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-08-05 00:58:12.244308 openct-0.1.5/LICENSE
--rw-r--r--   0        0        0     1693 2023-08-05 00:58:12.244308 openct-0.1.5/README.md
--rw-r--r--   0        0        0      112 2023-08-05 00:58:25.700403 openct-0.1.5/openct/__init__.py
--rw-r--r--   0        0        0      649 2023-08-05 00:58:12.244308 openct-0.1.5/openct/__main__.py
--rw-r--r--   0        0        0       83 2023-08-05 00:58:12.248309 openct-0.1.5/openct/connections/__init__.py
--rw-r--r--   0        0        0     2723 2023-08-05 00:58:12.248309 openct-0.1.5/openct/connections/connections.py
--rw-r--r--   0        0        0       73 2023-08-05 00:58:12.248309 openct-0.1.5/openct/datastore/__init__.py
--rw-r--r--   0        0        0     1359 2023-08-05 00:58:12.248309 openct-0.1.5/openct/datastore/datastore.py
--rw-r--r--   0        0        0       65 2023-08-05 00:58:12.248309 openct-0.1.5/openct/devices/__init__.py
--rw-r--r--   0        0        0      743 2023-08-05 00:58:12.248309 openct-0.1.5/openct/devices/devices.py
--rw-r--r--   0        0        0      201 2023-08-05 00:58:12.248309 openct-0.1.5/openct/setup/__init__.py
--rw-r--r--   0        0        0      556 2023-08-05 00:58:12.248309 openct-0.1.5/openct/setup/__main__.py
--rw-r--r--   0        0        0     1440 2023-08-05 00:58:12.248309 openct-0.1.5/openct/setup/config.py
--rw-r--r--   0        0        0      626 2023-08-05 00:58:12.248309 openct-0.1.5/openct/setup/config_schema.py
--rw-r--r--   0        0        0     1696 2023-08-05 00:58:12.248309 openct-0.1.5/openct/setup/setup.py
--rw-r--r--   0        0        0      645 2023-08-05 00:58:25.696403 openct-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2341 1970-01-01 00:00:00.000000 openct-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-05 01:21:13.529826 openct-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1693 2023-08-05 01:21:13.529826 openct-0.1.6/README.md
+-rw-r--r--   0        0        0      112 2023-08-05 01:21:28.061882 openct-0.1.6/openct/__init__.py
+-rw-r--r--   0        0        0      649 2023-08-05 01:21:13.529826 openct-0.1.6/openct/__main__.py
+-rw-r--r--   0        0        0       83 2023-08-05 01:21:13.529826 openct-0.1.6/openct/connections/__init__.py
+-rw-r--r--   0        0        0     2723 2023-08-05 01:21:13.529826 openct-0.1.6/openct/connections/connections.py
+-rw-r--r--   0        0        0       73 2023-08-05 01:21:13.529826 openct-0.1.6/openct/datastore/__init__.py
+-rw-r--r--   0        0        0     1359 2023-08-05 01:21:13.529826 openct-0.1.6/openct/datastore/datastore.py
+-rw-r--r--   0        0        0       65 2023-08-05 01:21:13.529826 openct-0.1.6/openct/devices/__init__.py
+-rw-r--r--   0        0        0      743 2023-08-05 01:21:13.529826 openct-0.1.6/openct/devices/devices.py
+-rw-r--r--   0        0        0      201 2023-08-05 01:21:13.529826 openct-0.1.6/openct/setup/__init__.py
+-rw-r--r--   0        0        0      888 2023-08-05 01:21:13.529826 openct-0.1.6/openct/setup/__main__.py
+-rw-r--r--   0        0        0     1440 2023-08-05 01:21:13.529826 openct-0.1.6/openct/setup/config.py
+-rw-r--r--   0        0        0      626 2023-08-05 01:21:13.529826 openct-0.1.6/openct/setup/config_schema.py
+-rw-r--r--   0        0        0     1696 2023-08-05 01:21:13.529826 openct-0.1.6/openct/setup/setup.py
+-rw-r--r--   0        0        0      645 2023-08-05 01:21:28.057882 openct-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2341 1970-01-01 00:00:00.000000 openct-0.1.6/PKG-INFO
```

### Comparing `openct-0.1.5/LICENSE` & `openct-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openct-0.1.5/README.md` & `openct-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `openct-0.1.5/openct/__main__.py` & `openct-0.1.6/openct/__main__.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.5/openct/connections/connections.py` & `openct-0.1.6/openct/connections/connections.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.5/openct/datastore/datastore.py` & `openct-0.1.6/openct/datastore/datastore.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.5/openct/devices/devices.py` & `openct-0.1.6/openct/devices/devices.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.5/openct/setup/config.py` & `openct-0.1.6/openct/setup/config.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.5/openct/setup/config_schema.py` & `openct-0.1.6/openct/setup/config_schema.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.5/openct/setup/setup.py` & `openct-0.1.6/openct/setup/setup.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.5/pyproject.toml` & `openct-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openct"
-version = "0.1.5"
+version = "0.1.6"
 description = "Configuration backup and analysis tools for devices running pfSense and RouterOS"
 authors = ["Weehooey <info@weehooey.com>"]
 license = "GNU GPL v3.0"
 readme = "README.md"
 repository = "https://github.com/weehooey/openct"
 
 [tool.poetry.dependencies]
```

### Comparing `openct-0.1.5/PKG-INFO` & `openct-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openct
-Version: 0.1.5
+Version: 0.1.6
 Summary: Configuration backup and analysis tools for devices running pfSense and RouterOS
 Home-page: https://github.com/weehooey/openct
 License: GNU GPL v3.0
 Author: Weehooey
 Author-email: info@weehooey.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
```

