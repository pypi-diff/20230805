# Comparing `tmp/openct-0.1.2.tar.gz` & `tmp/openct-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openct-0.1.2.tar", max compression
+gzip compressed data, was "openct-0.1.3.tar", max compression
```

## Comparing `openct-0.1.2.tar` & `openct-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-08-04 19:50:41.006445 openct-0.1.2/LICENSE
--rw-r--r--   0        0        0      996 2023-08-04 19:50:41.006445 openct-0.1.2/README.md
--rw-r--r--   0        0        0       89 2023-08-04 19:50:41.006445 openct-0.1.2/openct/__init__.py
--rw-r--r--   0        0        0      895 2023-08-04 19:50:41.006445 openct-0.1.2/openct/__main__.py
--rw-r--r--   0        0        0       83 2023-08-04 19:50:41.006445 openct-0.1.2/openct/connections/__init__.py
--rw-r--r--   0        0        0     1776 2023-08-04 19:50:41.006445 openct-0.1.2/openct/connections/connections.py
--rw-r--r--   0        0        0       73 2023-08-04 19:50:41.006445 openct-0.1.2/openct/datastore/__init__.py
--rw-r--r--   0        0        0     1359 2023-08-04 19:50:41.006445 openct-0.1.2/openct/datastore/datastore.py
--rw-r--r--   0        0        0       65 2023-08-04 19:50:41.006445 openct-0.1.2/openct/devices/__init__.py
--rw-r--r--   0        0        0      918 2023-08-04 19:50:41.006445 openct-0.1.2/openct/devices/devices.py
--rw-r--r--   0        0        0      201 2023-08-04 19:50:41.006445 openct-0.1.2/openct/setup/__init__.py
--rw-r--r--   0        0        0      556 2023-08-04 19:50:41.006445 openct-0.1.2/openct/setup/__main__.py
--rw-r--r--   0        0        0     1440 2023-08-04 19:50:41.006445 openct-0.1.2/openct/setup/config.py
--rw-r--r--   0        0        0      626 2023-08-04 19:50:41.006445 openct-0.1.2/openct/setup/config_schema.py
--rw-r--r--   0        0        0     1354 2023-08-04 19:50:41.006445 openct-0.1.2/openct/setup/setup.py
--rw-r--r--   0        0        0      592 2023-08-04 19:50:41.010445 openct-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 openct-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-04 21:33:44.669420 openct-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1693 2023-08-04 21:33:44.669420 openct-0.1.3/README.md
+-rw-r--r--   0        0        0       89 2023-08-04 21:33:44.673420 openct-0.1.3/openct/__init__.py
+-rw-r--r--   0        0        0      904 2023-08-04 21:33:44.673420 openct-0.1.3/openct/__main__.py
+-rw-r--r--   0        0        0       83 2023-08-04 21:33:44.673420 openct-0.1.3/openct/connections/__init__.py
+-rw-r--r--   0        0        0     2159 2023-08-04 21:33:44.673420 openct-0.1.3/openct/connections/connections.py
+-rw-r--r--   0        0        0       73 2023-08-04 21:33:44.673420 openct-0.1.3/openct/datastore/__init__.py
+-rw-r--r--   0        0        0     1359 2023-08-04 21:33:44.673420 openct-0.1.3/openct/datastore/datastore.py
+-rw-r--r--   0        0        0       65 2023-08-04 21:33:44.673420 openct-0.1.3/openct/devices/__init__.py
+-rw-r--r--   0        0        0      918 2023-08-04 21:33:44.673420 openct-0.1.3/openct/devices/devices.py
+-rw-r--r--   0        0        0      201 2023-08-04 21:33:44.673420 openct-0.1.3/openct/setup/__init__.py
+-rw-r--r--   0        0        0      556 2023-08-04 21:33:44.673420 openct-0.1.3/openct/setup/__main__.py
+-rw-r--r--   0        0        0     1440 2023-08-04 21:33:44.673420 openct-0.1.3/openct/setup/config.py
+-rw-r--r--   0        0        0      626 2023-08-04 21:33:44.673420 openct-0.1.3/openct/setup/config_schema.py
+-rw-r--r--   0        0        0     1354 2023-08-04 21:33:44.673420 openct-0.1.3/openct/setup/setup.py
+-rw-r--r--   0        0        0      592 2023-08-04 21:33:44.673420 openct-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2341 1970-01-01 00:00:00.000000 openct-0.1.3/PKG-INFO
```

### Comparing `openct-0.1.2/LICENSE` & `openct-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openct-0.1.2/openct/__main__.py` & `openct-0.1.3/openct/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,8 +27,8 @@
             config.identity.key_file,
             config.dirs.backup_dir,
         )
 
         if device.is_available():
             device.fetch_backup()
         else:
-            logging.error("Could not connect to device")
+            logging.error("Could not connect to device %s", host)
```

### Comparing `openct-0.1.2/openct/connections/connections.py` & `openct-0.1.3/openct/connections/connections.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Module for connection protocols"""
 
 from typing import Protocol
+import logging
 
 from fabric import Connection as FabricConnection
-from paramiko.ssh_exception import SSHException
+from paramiko.ssh_exception import SSHException, NoValidConnectionsError
+from invoke import UnexpectedExit
 
 
 class DeviceConnection(Protocol):
     """DeviceConnection abstract base class"""
 
     def test_connection(self) -> bool:
         ...
@@ -39,22 +41,28 @@
             user=self.username,
             connect_timeout=self.connection_timeout,
             connect_kwargs={"key_filename": self.key_file},
         ) as connection:
             try:
                 connection.open()
                 return True
-            except (TimeoutError, SSHException):
+            except (TimeoutError, SSHException, NoValidConnectionsError):
+                logging.error("Could not connect to device %s", self.ip_address)
                 return False
 
     def fetch_backup(self) -> None:
         with FabricConnection(
             host=self.ip_address,
             user=self.username,
             connect_timeout=self.connection_timeout,
             connect_kwargs={"key_filename": self.key_file},
         ) as connection:
-            connection.run("/export file=backup", hide=True, warn=False)
-            connection.get(
-                "backup.rsc", f"{self.backup_dir}/backup_{self.ip_address}.rsc"
-            )
-            connection.run("file/remove backup.rsc", hide=True, warn=False)
+            try:
+                connection.run("/export file=backup", hide=True, warn=False)
+                connection.get(
+                    "backup.rsc", f"{self.backup_dir}/backup_{self.ip_address}.rsc"
+                )
+                connection.run("file/remove backup.rsc", hide=True, warn=False)
+            except UnexpectedExit:
+                logging.error(
+                    "Error while fetching backup from device %s", self.ip_address
+                )
```

### Comparing `openct-0.1.2/openct/datastore/datastore.py` & `openct-0.1.3/openct/datastore/datastore.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.2/openct/devices/devices.py` & `openct-0.1.3/openct/devices/devices.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.2/openct/setup/__main__.py` & `openct-0.1.3/openct/setup/__main__.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.2/openct/setup/config.py` & `openct-0.1.3/openct/setup/config.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.2/openct/setup/config_schema.py` & `openct-0.1.3/openct/setup/config_schema.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.2/openct/setup/setup.py` & `openct-0.1.3/openct/setup/setup.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.2/pyproject.toml` & `openct-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openct"
-version = "0.1.2"
+version = "0.1.3"
 description = "Configuration backup and analysis tools for devices running pfSense and RouterOS"
 authors = ["Weehooey <info@weehooey.com>"]
 license = "GNU GPL v3.0"
 readme = "README.md"
 repository = "https://github.com/weehooey/openct"
 
 [tool.poetry.dependencies]
```

