# Comparing `tmp/ssh_terminal_manager-0.9.3.tar.gz` & `tmp/ssh_terminal_manager-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_terminal_manager-0.9.3.tar", last modified: Sat Jul 29 10:49:55 2023, max compression
+gzip compressed data, was "ssh_terminal_manager-0.9.4.tar", last modified: Sat Aug  5 03:11:01 2023, max compression
```

## Comparing `ssh_terminal_manager-0.9.3.tar` & `ssh_terminal_manager-0.9.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-29 10:49:55.442410 ssh_terminal_manager-0.9.3/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.9.3/LICENSE
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      864 2023-07-29 10:49:55.442410 ssh_terminal_manager-0.9.3/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      223 2023-07-25 07:37:47.000000 ssh_terminal_manager-0.9.3/README.md
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      901 2023-07-29 10:49:12.000000 ssh_terminal_manager-0.9.3/pyproject.toml
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-29 10:49:55.442410 ssh_terminal_manager-0.9.3/setup.cfg
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-29 10:49:55.438410 ssh_terminal_manager-0.9.3/src/
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-29 10:49:55.442410 ssh_terminal_manager-0.9.3/src/ssh_terminal_manager/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8824 2023-07-29 10:40:33.000000 ssh_terminal_manager-0.9.3/src/ssh_terminal_manager/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      393 2023-07-23 04:56:11.000000 ssh_terminal_manager-0.9.3/src/ssh_terminal_manager/errors.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1797 2023-07-29 10:39:37.000000 ssh_terminal_manager-0.9.3/src/ssh_terminal_manager/ping_client.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-29 10:49:55.442410 ssh_terminal_manager-0.9.3/src/ssh_terminal_manager.egg-info/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      864 2023-07-29 10:49:55.000000 ssh_terminal_manager-0.9.3/src/ssh_terminal_manager.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      383 2023-07-29 10:49:55.000000 ssh_terminal_manager-0.9.3/src/ssh_terminal_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-29 10:49:55.000000 ssh_terminal_manager-0.9.3/src/ssh_terminal_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       91 2023-07-29 10:49:55.000000 ssh_terminal_manager-0.9.3/src/ssh_terminal_manager.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       21 2023-07-29 10:49:55.000000 ssh_terminal_manager-0.9.3/src/ssh_terminal_manager.egg-info/top_level.txt
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-05 03:11:01.879338 ssh_terminal_manager-0.9.4/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.9.4/LICENSE
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      864 2023-08-05 03:11:01.879338 ssh_terminal_manager-0.9.4/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      223 2023-07-25 07:37:47.000000 ssh_terminal_manager-0.9.4/README.md
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      901 2023-08-03 05:01:35.000000 ssh_terminal_manager-0.9.4/pyproject.toml
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-08-05 03:11:01.879338 ssh_terminal_manager-0.9.4/setup.cfg
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-05 03:11:01.875338 ssh_terminal_manager-0.9.4/src/
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-05 03:11:01.879338 ssh_terminal_manager-0.9.4/src/ssh_terminal_manager/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8910 2023-08-03 05:41:41.000000 ssh_terminal_manager-0.9.4/src/ssh_terminal_manager/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      393 2023-07-23 04:56:11.000000 ssh_terminal_manager-0.9.4/src/ssh_terminal_manager/errors.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1797 2023-07-30 02:33:58.000000 ssh_terminal_manager-0.9.4/src/ssh_terminal_manager/ping_client.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-05 03:11:01.879338 ssh_terminal_manager-0.9.4/src/ssh_terminal_manager.egg-info/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      864 2023-08-05 03:11:01.000000 ssh_terminal_manager-0.9.4/src/ssh_terminal_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      383 2023-08-05 03:11:01.000000 ssh_terminal_manager-0.9.4/src/ssh_terminal_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-08-05 03:11:01.000000 ssh_terminal_manager-0.9.4/src/ssh_terminal_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       91 2023-08-05 03:11:01.000000 ssh_terminal_manager-0.9.4/src/ssh_terminal_manager.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       21 2023-08-05 03:11:01.000000 ssh_terminal_manager-0.9.4/src/ssh_terminal_manager.egg-info/top_level.txt
```

### Comparing `ssh_terminal_manager-0.9.3/LICENSE` & `ssh_terminal_manager-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ssh_terminal_manager-0.9.3/PKG-INFO` & `ssh_terminal_manager-0.9.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh_terminal_manager
-Version: 0.9.3
+Version: 0.9.4
 Summary: Use terminal commands to control and monitor remote devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-terminal-manager/issues
 Keywords: ssh,terminal,console,shell,bash,cmd,power shell,commands,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ssh_terminal_manager-0.9.3/pyproject.toml` & `ssh_terminal_manager-0.9.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ssh_terminal_manager"
-version = "0.9.3"
+version = "0.9.4"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Use terminal commands to control and monitor remote devices"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -27,14 +27,14 @@
   "commands",
   "command line"
 ]
 dependencies = [
   "async-timeout >= 4.0.2",
   "icmplib >= 3.0",
   "paramiko >= 3.2.0",
-  "terminal-manager >= 0.9.2",
+  "terminal-manager >= 0.9.3",
   "wakeonlan >= 3.0.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/zhbjsh/ssh-terminal-manager"
 "Bug Tracker" = "https://github.com/zhbjsh/ssh-terminal-manager/issues"
```

### Comparing `ssh_terminal_manager-0.9.3/src/ssh_terminal_manager/__init__.py` & `ssh_terminal_manager-0.9.4/src/ssh_terminal_manager/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """SSH terminal manager."""
 from __future__ import annotations
 
 import asyncio
 import logging
 from time import time
 
-import icmplib
 import paramiko
 import wakeonlan
 from terminal_manager import (
     DEFAULT_ALLOW_TURN_OFF,
     DEFAULT_COMMAND_TIMEOUT,
     PLACEHOLDER_KEY,
     ActionCommand,
@@ -187,23 +186,25 @@
         except Exception as exc:
             self._disconnect()
             raise SSHConnectError(f"SSH connection failed ({exc})") from exc
 
         self.state.update(CONNECTED, True)
 
     def _disconnect(self) -> None:
-        if not self.state.connected:
-            return
-
         self.client.close()
         self.state.update(CONNECTED, False)
 
         for command in self.sensor_commands:
             command.update_sensors(self, None)
 
+    async def async_close(self) -> None:
+        await super().async_close()
+        await self.async_disconnect()
+        self.state.update(ONLINE, False)
+
     async def async_execute_command_string(
         self, string: str, command_timeout: int | None = None
     ) -> CommandOutput:
         loop = asyncio.get_running_loop()
         timeout = command_timeout or self.command_timeout
         return await loop.run_in_executor(
             None, self._execute_command_string, string, timeout
```

### Comparing `ssh_terminal_manager-0.9.3/src/ssh_terminal_manager/ping_client.py` & `ssh_terminal_manager-0.9.4/src/ssh_terminal_manager/ping_client.py`

 * *Files identical despite different names*

### Comparing `ssh_terminal_manager-0.9.3/src/ssh_terminal_manager.egg-info/PKG-INFO` & `ssh_terminal_manager-0.9.4/src/ssh_terminal_manager.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh-terminal-manager
-Version: 0.9.3
+Version: 0.9.4
 Summary: Use terminal commands to control and monitor remote devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-terminal-manager/issues
 Keywords: ssh,terminal,console,shell,bash,cmd,power shell,commands,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

