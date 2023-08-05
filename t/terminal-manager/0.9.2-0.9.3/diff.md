# Comparing `tmp/terminal_manager-0.9.2.tar.gz` & `tmp/terminal_manager-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal_manager-0.9.2.tar", last modified: Sun Jul 23 07:55:49 2023, max compression
+gzip compressed data, was "terminal_manager-0.9.3.tar", last modified: Sat Aug  5 03:16:54 2023, max compression
```

## Comparing `terminal_manager-0.9.2.tar` & `terminal_manager-0.9.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-23 07:55:49.625497 terminal_manager-0.9.2/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:30.000000 terminal_manager-0.9.2/LICENSE
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      725 2023-07-23 07:55:49.625497 terminal_manager-0.9.2/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      107 2023-07-11 04:42:30.000000 terminal_manager-0.9.2/README.md
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      778 2023-07-23 07:55:12.000000 terminal_manager-0.9.2/pyproject.toml
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-23 07:55:49.625497 terminal_manager-0.9.2/setup.cfg
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-23 07:55:49.617496 terminal_manager-0.9.2/src/
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-23 07:55:49.621497 terminal_manager-0.9.2/src/terminal_manager/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     7023 2023-07-23 04:56:11.000000 terminal_manager-0.9.2/src/terminal_manager/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3352 2023-07-23 04:56:11.000000 terminal_manager-0.9.2/src/terminal_manager/collection.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     6319 2023-07-23 04:56:11.000000 terminal_manager-0.9.2/src/terminal_manager/command.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-23 07:55:49.621497 terminal_manager-0.9.2/src/terminal_manager/default_collections/
--rw-r--r--   0 adrian    (1000) adrian    (1000)      161 2023-07-23 04:56:11.000000 terminal_manager-0.9.2/src/terminal_manager/default_collections/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1084 2023-07-23 04:56:11.000000 terminal_manager-0.9.2/src/terminal_manager/default_collections/const.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     4371 2023-07-23 04:56:11.000000 terminal_manager-0.9.2/src/terminal_manager/default_collections/linux.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5206 2023-07-23 04:56:11.000000 terminal_manager-0.9.2/src/terminal_manager/default_collections/windows_cmd.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5368 2023-07-23 04:56:11.000000 terminal_manager-0.9.2/src/terminal_manager/default_collections/windows_ps.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)       94 2023-07-23 04:56:11.000000 terminal_manager-0.9.2/src/terminal_manager/errors.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      617 2023-07-23 04:56:11.000000 terminal_manager-0.9.2/src/terminal_manager/event.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      222 2023-07-23 04:56:11.000000 terminal_manager-0.9.2/src/terminal_manager/helpers.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8427 2023-07-23 07:53:02.000000 terminal_manager-0.9.2/src/terminal_manager/sensor.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1248 2023-07-23 04:56:11.000000 terminal_manager-0.9.2/src/terminal_manager/synchronizer.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-23 07:55:49.621497 terminal_manager-0.9.2/src/terminal_manager.egg-info/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      725 2023-07-23 07:55:49.000000 terminal_manager-0.9.2/src/terminal_manager.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      776 2023-07-23 07:55:49.000000 terminal_manager-0.9.2/src/terminal_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-23 07:55:49.000000 terminal_manager-0.9.2/src/terminal_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       22 2023-07-23 07:55:49.000000 terminal_manager-0.9.2/src/terminal_manager.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       17 2023-07-23 07:55:49.000000 terminal_manager-0.9.2/src/terminal_manager.egg-info/top_level.txt
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-05 03:16:54.637850 terminal_manager-0.9.3/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:30.000000 terminal_manager-0.9.3/LICENSE
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      725 2023-08-05 03:16:54.637850 terminal_manager-0.9.3/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      107 2023-07-11 04:42:30.000000 terminal_manager-0.9.3/README.md
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      778 2023-08-03 04:57:50.000000 terminal_manager-0.9.3/pyproject.toml
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-08-05 03:16:54.637850 terminal_manager-0.9.3/setup.cfg
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-05 03:16:54.629849 terminal_manager-0.9.3/src/
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-05 03:16:54.633849 terminal_manager-0.9.3/src/terminal_manager/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     7211 2023-08-03 04:25:16.000000 terminal_manager-0.9.3/src/terminal_manager/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     3352 2023-07-23 04:56:11.000000 terminal_manager-0.9.3/src/terminal_manager/collection.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     6319 2023-07-23 04:56:11.000000 terminal_manager-0.9.3/src/terminal_manager/command.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-05 03:16:54.637850 terminal_manager-0.9.3/src/terminal_manager/default_collections/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      161 2023-07-23 04:56:11.000000 terminal_manager-0.9.3/src/terminal_manager/default_collections/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1147 2023-08-03 08:21:01.000000 terminal_manager-0.9.3/src/terminal_manager/default_collections/const.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     4371 2023-07-23 04:56:11.000000 terminal_manager-0.9.3/src/terminal_manager/default_collections/linux.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5206 2023-07-23 04:56:11.000000 terminal_manager-0.9.3/src/terminal_manager/default_collections/windows_cmd.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5368 2023-07-23 04:56:11.000000 terminal_manager-0.9.3/src/terminal_manager/default_collections/windows_ps.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)       94 2023-07-23 04:56:11.000000 terminal_manager-0.9.3/src/terminal_manager/errors.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      617 2023-07-23 04:56:11.000000 terminal_manager-0.9.3/src/terminal_manager/event.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      222 2023-07-23 04:56:11.000000 terminal_manager-0.9.3/src/terminal_manager/helpers.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     8421 2023-08-04 06:41:52.000000 terminal_manager-0.9.3/src/terminal_manager/sensor.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1248 2023-08-03 04:29:54.000000 terminal_manager-0.9.3/src/terminal_manager/synchronizer.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-05 03:16:54.637850 terminal_manager-0.9.3/src/terminal_manager.egg-info/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      725 2023-08-05 03:16:54.000000 terminal_manager-0.9.3/src/terminal_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      776 2023-08-05 03:16:54.000000 terminal_manager-0.9.3/src/terminal_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-08-05 03:16:54.000000 terminal_manager-0.9.3/src/terminal_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       22 2023-08-05 03:16:54.000000 terminal_manager-0.9.3/src/terminal_manager.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       17 2023-08-05 03:16:54.000000 terminal_manager-0.9.3/src/terminal_manager.egg-info/top_level.txt
```

### Comparing `terminal_manager-0.9.2/LICENSE` & `terminal_manager-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.9.2/PKG-INFO` & `terminal_manager-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal_manager
-Version: 0.9.2
+Version: 0.9.3
 Summary: Use terminal commands to control and monitor devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
 Keywords: terminal,console,shell,bash,cmd,power shell,commands,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `terminal_manager-0.9.2/pyproject.toml` & `terminal_manager-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "terminal_manager"
-version = "0.9.2"
+version = "0.9.3"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Use terminal commands to control and monitor devices"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `terminal_manager-0.9.2/src/terminal_manager/__init__.py` & `terminal_manager-0.9.3/src/terminal_manager/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,20 @@
             collection.action_commands if collection else None,
             collection.sensor_commands if collection else None,
         )
         self.command_timeout = command_timeout
         self.allow_turn_off = allow_turn_off
         self.logger = logger
 
+    async def __aenter__(self):
+        return self
+
+    async def __aexit__(self, *args):
+        await self.async_close()
+
     @property
     def hostname(self) -> str | None:
         if sensor := self.sensors_by_key.get(SensorKey.HOSTNAME):
             return sensor.last_known_value
 
     @property
     def os_name(self) -> str | None:
@@ -87,14 +93,17 @@
             return sensor.last_known_value
 
     @property
     def wake_on_lan(self) -> bool | None:
         if sensor := self.sensors_by_key.get(SensorKey.WAKE_ON_LAN):
             return sensor.last_known_value
 
+    async def async_close(self) -> None:
+        """Close."""
+
     async def async_update_sensor_commands(self, force: bool = False) -> None:
         """Update the sensor commands.
 
         Execute sensor commands that passed their `interval` or
         all sensor commands with `force=True`.
 
         """
```

### Comparing `terminal_manager-0.9.2/src/terminal_manager/collection.py` & `terminal_manager-0.9.3/src/terminal_manager/collection.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.9.2/src/terminal_manager/command.py` & `terminal_manager-0.9.3/src/terminal_manager/command.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.9.2/src/terminal_manager/default_collections/const.py` & `terminal_manager-0.9.3/src/terminal_manager/default_collections/const.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-class ActionKey:
+from enum import StrEnum
+
+
+class ActionKey(StrEnum):
     TURN_OFF = "turn_off"
     RESTART = "restart"
 
 
-class ActionName:
+class ActionName(StrEnum):
     TURN_OFF = "Turn off"
     RESTART = "Restart"
 
 
-class SensorKey:
+class SensorKey(StrEnum):
     NETWORK_INTERFACE = "network_interface"
     MAC_ADDRESS = "mac_address"
     WAKE_ON_LAN = "wake_on_lan"
     MACHINE_TYPE = "machine_type"
     HOSTNAME = "hostname"
     OS_NAME = "os_name"
     OS_VERSION = "os_version"
@@ -21,15 +24,15 @@
     FREE_MEMORY = "free_memory"
     CPU_LOAD = "cpu_load"
     FREE_DISK_SPACE = "free_disk_space"
     TEMPERATURE = "temperature"
     PROCESSES = "processes"
 
 
-class SensorName:
+class SensorName(StrEnum):
     NETWORK_INTERFACE = "Network Interface"
     MAC_ADDRESS = "MAC Address"
     WAKE_ON_LAN = "Wake on LAN"
     MACHINE_TYPE = "Machine Type"
     HOSTNAME = "Hostname"
     OS_NAME = "OS Name"
     OS_VERSION = "OS Version"
```

### Comparing `terminal_manager-0.9.2/src/terminal_manager/default_collections/linux.py` & `terminal_manager-0.9.3/src/terminal_manager/default_collections/linux.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.9.2/src/terminal_manager/default_collections/windows_cmd.py` & `terminal_manager-0.9.3/src/terminal_manager/default_collections/windows_cmd.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.9.2/src/terminal_manager/default_collections/windows_ps.py` & `terminal_manager-0.9.3/src/terminal_manager/default_collections/windows_ps.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.9.2/src/terminal_manager/event.py` & `terminal_manager-0.9.3/src/terminal_manager/event.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.9.2/src/terminal_manager/sensor.py` & `terminal_manager-0.9.3/src/terminal_manager/sensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,35 +31,35 @@
     def __post_init__(self):
         self.id = None
         self.key = self.key or name_to_key(self.name)
         self.value: Any | None = None
         self.last_known_value: Any | None = None
         self.child_sensors: list[Sensor] = []
         self.on_update = Event()
-        self.on_child_added = Event()
-        self.on_child_removed = Event()
+        self.on_child_add = Event()
+        self.on_child_remove = Event()
 
     @property
     def controllable(self) -> bool:
         return self.command_set is not None
 
     @property
     def child_sensors_by_key(self) -> dict[str, Sensor]:
         return {child.key: child for child in self.child_sensors}
 
     def _get_control_command(self, _: Any) -> Command | None:
         return self.command_set
 
     def _add_child(self, child: Sensor) -> None:
         self.child_sensors.append(child)
-        self.on_child_added.notify(self, child)
+        self.on_child_add.notify(self, child)
 
     def _remove_child(self, child: Sensor) -> None:
         self.child_sensors.remove(child)
-        self.on_child_removed.notify(self, child)
+        self.on_child_remove.notify(self, child)
 
     def _render(self, data: str) -> str:
         if self.renderer:
             data = self.renderer(data)
 
         return data.strip()
```

### Comparing `terminal_manager-0.9.2/src/terminal_manager/synchronizer.py` & `terminal_manager-0.9.3/src/terminal_manager/synchronizer.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.9.2/src/terminal_manager.egg-info/PKG-INFO` & `terminal_manager-0.9.3/src/terminal_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal-manager
-Version: 0.9.2
+Version: 0.9.3
 Summary: Use terminal commands to control and monitor devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
 Keywords: terminal,console,shell,bash,cmd,power shell,commands,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `terminal_manager-0.9.2/src/terminal_manager.egg-info/SOURCES.txt` & `terminal_manager-0.9.3/src/terminal_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

