# Comparing `tmp/openct-0.1.3.tar.gz` & `tmp/openct-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openct-0.1.3.tar", max compression
+gzip compressed data, was "openct-0.1.4.tar", max compression
```

## Comparing `openct-0.1.3.tar` & `openct-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-08-04 21:33:44.669420 openct-0.1.3/LICENSE
--rw-r--r--   0        0        0     1693 2023-08-04 21:33:44.669420 openct-0.1.3/README.md
--rw-r--r--   0        0        0       89 2023-08-04 21:33:44.673420 openct-0.1.3/openct/__init__.py
--rw-r--r--   0        0        0      904 2023-08-04 21:33:44.673420 openct-0.1.3/openct/__main__.py
--rw-r--r--   0        0        0       83 2023-08-04 21:33:44.673420 openct-0.1.3/openct/connections/__init__.py
--rw-r--r--   0        0        0     2159 2023-08-04 21:33:44.673420 openct-0.1.3/openct/connections/connections.py
--rw-r--r--   0        0        0       73 2023-08-04 21:33:44.673420 openct-0.1.3/openct/datastore/__init__.py
--rw-r--r--   0        0        0     1359 2023-08-04 21:33:44.673420 openct-0.1.3/openct/datastore/datastore.py
--rw-r--r--   0        0        0       65 2023-08-04 21:33:44.673420 openct-0.1.3/openct/devices/__init__.py
--rw-r--r--   0        0        0      918 2023-08-04 21:33:44.673420 openct-0.1.3/openct/devices/devices.py
--rw-r--r--   0        0        0      201 2023-08-04 21:33:44.673420 openct-0.1.3/openct/setup/__init__.py
--rw-r--r--   0        0        0      556 2023-08-04 21:33:44.673420 openct-0.1.3/openct/setup/__main__.py
--rw-r--r--   0        0        0     1440 2023-08-04 21:33:44.673420 openct-0.1.3/openct/setup/config.py
--rw-r--r--   0        0        0      626 2023-08-04 21:33:44.673420 openct-0.1.3/openct/setup/config_schema.py
--rw-r--r--   0        0        0     1354 2023-08-04 21:33:44.673420 openct-0.1.3/openct/setup/setup.py
--rw-r--r--   0        0        0      592 2023-08-04 21:33:44.673420 openct-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2341 1970-01-01 00:00:00.000000 openct-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-04 23:26:09.325491 openct-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1693 2023-08-04 23:26:09.325491 openct-0.1.4/README.md
+-rw-r--r--   0        0        0       89 2023-08-04 23:26:09.325491 openct-0.1.4/openct/__init__.py
+-rw-r--r--   0        0        0      649 2023-08-04 23:26:09.325491 openct-0.1.4/openct/__main__.py
+-rw-r--r--   0        0        0       83 2023-08-04 23:26:09.325491 openct-0.1.4/openct/connections/__init__.py
+-rw-r--r--   0        0        0     2723 2023-08-04 23:26:09.329491 openct-0.1.4/openct/connections/connections.py
+-rw-r--r--   0        0        0       73 2023-08-04 23:26:09.329491 openct-0.1.4/openct/datastore/__init__.py
+-rw-r--r--   0        0        0     1359 2023-08-04 23:26:09.329491 openct-0.1.4/openct/datastore/datastore.py
+-rw-r--r--   0        0        0       65 2023-08-04 23:26:09.329491 openct-0.1.4/openct/devices/__init__.py
+-rw-r--r--   0        0        0      743 2023-08-04 23:26:09.329491 openct-0.1.4/openct/devices/devices.py
+-rw-r--r--   0        0        0      201 2023-08-04 23:26:09.329491 openct-0.1.4/openct/setup/__init__.py
+-rw-r--r--   0        0        0      556 2023-08-04 23:26:09.329491 openct-0.1.4/openct/setup/__main__.py
+-rw-r--r--   0        0        0     1440 2023-08-04 23:26:09.329491 openct-0.1.4/openct/setup/config.py
+-rw-r--r--   0        0        0      626 2023-08-04 23:26:09.329491 openct-0.1.4/openct/setup/config_schema.py
+-rw-r--r--   0        0        0     1354 2023-08-04 23:26:09.329491 openct-0.1.4/openct/setup/setup.py
+-rw-r--r--   0        0        0      592 2023-08-04 23:26:09.329491 openct-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2341 1970-01-01 00:00:00.000000 openct-0.1.4/PKG-INFO
```

### Comparing `openct-0.1.3/LICENSE` & `openct-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openct-0.1.3/README.md` & `openct-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `openct-0.1.3/openct/connections/connections.py` & `openct-0.1.4/openct/connections/connections.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 """Module for connection protocols"""
 
 from typing import Protocol
 import logging
 
 from fabric import Connection as FabricConnection
-from paramiko.ssh_exception import SSHException, NoValidConnectionsError
-from invoke import UnexpectedExit
+from paramiko.ssh_exception import (
+    SSHException,
+    NoValidConnectionsError,
+    BadHostKeyException,
+    AuthenticationException,
+)
+from invoke import UnexpectedExit, Failure
+
+from openct.setup import Config
 
 
 class DeviceConnection(Protocol):
     """DeviceConnection abstract base class"""
 
     def test_connection(self) -> bool:
         ...
@@ -17,52 +24,63 @@
     def fetch_backup(self) -> None:
         ...
 
 
 class SshConnection(DeviceConnection):
     """DeviceConnection using Fabric"""
 
-    def __init__(
-        self,
-        ip_address: str,
-        username: str,
-        connection_timeout: int,
-        key_file: str,
-        backup_dir: str,
-    ) -> None:
+    def __init__(self, ip_address: str, config: Config) -> None:
         self.ip_address = ip_address
-        self.username = username
-        self.connection_timeout = connection_timeout
-        self.key_file = key_file
-        self.backup_dir = backup_dir
+        self.username = config.identity.username
+        self.connection_timeout = config.settings.connection_timeout
+        self.key_file = config.identity.key_file
+        self.backup_dir = config.dirs.backup_dir
 
     def test_connection(self) -> bool:
         with FabricConnection(
             host=self.ip_address,
             user=self.username,
             connect_timeout=self.connection_timeout,
             connect_kwargs={"key_filename": self.key_file},
         ) as connection:
             try:
                 connection.open()
                 return True
-            except (TimeoutError, SSHException, NoValidConnectionsError):
+            except (
+                TimeoutError,
+                BadHostKeyException,
+                AuthenticationException,
+                SSHException,
+                NoValidConnectionsError,
+            ) as error:
                 logging.error("Could not connect to device %s", self.ip_address)
+                logging.info(error)
                 return False
 
     def fetch_backup(self) -> None:
         with FabricConnection(
             host=self.ip_address,
             user=self.username,
             connect_timeout=self.connection_timeout,
             connect_kwargs={"key_filename": self.key_file},
         ) as connection:
             try:
-                connection.run("/export file=backup", hide=True, warn=False)
+                connection.run(
+                    "/export file=backup",
+                    hide=True,
+                    warn=False,
+                    timeout=self.connection_timeout,
+                )
                 connection.get(
                     "backup.rsc", f"{self.backup_dir}/backup_{self.ip_address}.rsc"
                 )
-                connection.run("file/remove backup.rsc", hide=True, warn=False)
-            except UnexpectedExit:
+                connection.run(
+                    "file/remove backup.rsc",
+                    hide=True,
+                    warn=False,
+                    timeout=self.connection_timeout,
+                )
+            except (UnexpectedExit, Failure) as error:
                 logging.error(
                     "Error while fetching backup from device %s", self.ip_address
                 )
+                logging.info(error)
```

### Comparing `openct-0.1.3/openct/datastore/datastore.py` & `openct-0.1.4/openct/datastore/datastore.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.3/openct/devices/devices.py` & `openct-0.1.4/openct/devices/devices.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Module for device classes"""
 
 from abc import ABC, abstractmethod
 
 from openct.connections import DeviceConnection, SshConnection
+from openct.setup import Config
 
 
 class Device(ABC):
     """Device abstract base class"""
 
     def __init__(self, connection: DeviceConnection) -> None:
         self.connection = connection
@@ -18,23 +19,12 @@
     def is_available(self) -> bool:
         return self.connection.test_connection()
 
 
 class RouterOSDevice(Device):
     """RouterOS device"""
 
-    def __init__(
-        self,
-        ip_address: str,
-        username: str,
-        connection_timeout: int,
-        key_file: str,
-        backup_dir: str,
-    ) -> None:
-        super().__init__(
-            SshConnection(
-                ip_address, username, connection_timeout, key_file, backup_dir
-            )
-        )
+    def __init__(self, ip_address: str, config: Config) -> None:
+        super().__init__(SshConnection(ip_address, config))
 
     def fetch_backup(self) -> str:
         return self.connection.fetch_backup()
```

### Comparing `openct-0.1.3/openct/setup/__main__.py` & `openct-0.1.4/openct/setup/__main__.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.3/openct/setup/config.py` & `openct-0.1.4/openct/setup/config.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.3/openct/setup/config_schema.py` & `openct-0.1.4/openct/setup/config_schema.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.3/openct/setup/setup.py` & `openct-0.1.4/openct/setup/setup.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.3/pyproject.toml` & `openct-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openct"
-version = "0.1.3"
+version = "0.1.4"
 description = "Configuration backup and analysis tools for devices running pfSense and RouterOS"
 authors = ["Weehooey <info@weehooey.com>"]
 license = "GNU GPL v3.0"
 readme = "README.md"
 repository = "https://github.com/weehooey/openct"
 
 [tool.poetry.dependencies]
```

### Comparing `openct-0.1.3/PKG-INFO` & `openct-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openct
-Version: 0.1.3
+Version: 0.1.4
 Summary: Configuration backup and analysis tools for devices running pfSense and RouterOS
 Home-page: https://github.com/weehooey/openct
 License: GNU GPL v3.0
 Author: Weehooey
 Author-email: info@weehooey.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
```

