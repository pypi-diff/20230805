# Comparing `tmp/rivian_python_client-1.0.0.tar.gz` & `tmp/rivian_python_client-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rivian_python_client-1.0.0.tar", max compression
+gzip compressed data, was "rivian_python_client-1.0.1.tar", max compression
```

## Comparing `rivian_python_client-1.0.0.tar` & `rivian_python_client-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      325 2023-08-04 16:01:43.321081 rivian_python_client-1.0.0/README.md
--rw-r--r--   0        0        0      775 2023-08-04 16:02:00.061496 rivian_python_client-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      155 2023-08-04 16:01:43.321081 rivian_python_client-1.0.0/src/rivian/__init__.py
--rw-r--r--   0        0        0     5766 2023-08-04 16:01:43.321081 rivian_python_client-1.0.0/src/rivian/const.py
--rw-r--r--   0        0        0      969 2023-08-04 16:01:43.321081 rivian_python_client-1.0.0/src/rivian/exceptions.py
--rw-r--r--   0        0        0        0 2023-08-04 16:01:43.321081 rivian_python_client-1.0.0/src/rivian/py.typed
--rw-r--r--   0        0        0    26126 2023-08-04 16:01:43.321081 rivian_python_client-1.0.0/src/rivian/rivian.py
--rw-r--r--   0        0        0     3031 2023-08-04 16:01:43.321081 rivian_python_client-1.0.0/src/rivian/utils.py
--rw-r--r--   0        0        0     7509 2023-08-04 16:01:43.321081 rivian_python_client-1.0.0/src/rivian/ws_monitor.py
--rw-r--r--   0        0        0      976 1970-01-01 00:00:00.000000 rivian_python_client-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      325 2023-08-05 18:02:19.088641 rivian_python_client-1.0.1/README.md
+-rw-r--r--   0        0        0      775 2023-08-05 18:02:40.152866 rivian_python_client-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      155 2023-08-05 18:02:19.096641 rivian_python_client-1.0.1/src/rivian/__init__.py
+-rw-r--r--   0        0        0     5766 2023-08-05 18:02:19.096641 rivian_python_client-1.0.1/src/rivian/const.py
+-rw-r--r--   0        0        0      969 2023-08-05 18:02:19.096641 rivian_python_client-1.0.1/src/rivian/exceptions.py
+-rw-r--r--   0        0        0        0 2023-08-05 18:02:19.096641 rivian_python_client-1.0.1/src/rivian/py.typed
+-rw-r--r--   0        0        0    26156 2023-08-05 18:02:19.096641 rivian_python_client-1.0.1/src/rivian/rivian.py
+-rw-r--r--   0        0        0     3031 2023-08-05 18:02:19.096641 rivian_python_client-1.0.1/src/rivian/utils.py
+-rw-r--r--   0        0        0     7509 2023-08-05 18:02:19.096641 rivian_python_client-1.0.1/src/rivian/ws_monitor.py
+-rw-r--r--   0        0        0      976 1970-01-01 00:00:00.000000 rivian_python_client-1.0.1/PKG-INFO
```

### Comparing `rivian_python_client-1.0.0/pyproject.toml` & `rivian_python_client-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rivian-python-client"
-version = "1.0.0"
+version = "1.0.1"
 description = "Rivian API Client (Unofficial)"
 readme = "README.md"
 authors = ["Brian Retterer <bretterer@gmail.com>"]
 license = "MIT"
 packages = [
     { include = "rivian", from = "src" },
 ]
```

### Comparing `rivian_python_client-1.0.0/src/rivian/const.py` & `rivian_python_client-1.0.1/src/rivian/const.py`

 * *Files identical despite different names*

### Comparing `rivian_python_client-1.0.0/src/rivian/exceptions.py` & `rivian_python_client-1.0.1/src/rivian/exceptions.py`

 * *Files identical despite different names*

### Comparing `rivian_python_client-1.0.0/src/rivian/rivian.py` & `rivian_python_client-1.0.1/src/rivian/rivian.py`

 * *Files 2% similar despite different names*

```diff
@@ -446,18 +446,18 @@
             VehicleCommand.CABIN_HVAC_RIGHT_SEAT_HEAT,
             VehicleCommand.CABIN_HVAC_RIGHT_SEAT_VENT,
             VehicleCommand.CABIN_HVAC_STEERING_HEAT,
         ):
             if not (
                 params
                 and isinstance((level := params.get("level")), int)
-                and 0 <= level <= 3
+                and 0 <= level <= 4
             ):
                 raise RivianBadRequestError(
-                    "HVAC setting must include parameter `level` with a valid value between 0 and 3"
+                    "HVAC setting must include parameter `level` with a valid value between 0 and 4"
                 )
         if command == VehicleCommand.CABIN_PRECONDITIONING_SET_TEMP:
             if not (
                 params
                 and isinstance((temp := params.get("HVAC_set_temp")), (float, int))
                 and (16 <= temp <= 29 or temp in (0, 63.5))
             ):
@@ -480,15 +480,15 @@
         """Send a command to the vehicle.
 
         To generate a public/private key for commands, use the `utils.generate_key_pair` function.
         The public key will first need to be enrolled via the `enroll_phone` method, otherwise commands will fail.
 
         Certain commands may require additional details via the `params` mapping.
         Some known examples include:
-          - `CABIN_HVAC_*`: params = {"level": 0..3} where 0 is off, 1 is low/on, 2 is medium and 3 is high
+          - `CABIN_HVAC_*`: params = {"level": 0..4} where 0 is off, 1 is on, 2 is low/level_1, 3 is medium/level_2 and 4 is high/level_3
           - `CABIN_PRECONDITIONING_SET_TEMP`: params = {"HVAC_set_temp": "deg_C"} where `deg_C` is a string value between 16 and 29 or 0/63.5 for LO/HI, respectively
           - `CHARGING_LIMITS`: params = {"SOC_limit": 50..100}
         """
         self._validate_vehicle_command(command, params)
 
         command = str(command)
         timestamp = str(int(time.time()))
```

### Comparing `rivian_python_client-1.0.0/src/rivian/utils.py` & `rivian_python_client-1.0.1/src/rivian/utils.py`

 * *Files identical despite different names*

### Comparing `rivian_python_client-1.0.0/src/rivian/ws_monitor.py` & `rivian_python_client-1.0.1/src/rivian/ws_monitor.py`

 * *Files identical despite different names*

### Comparing `rivian_python_client-1.0.0/PKG-INFO` & `rivian_python_client-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rivian-python-client
-Version: 1.0.0
+Version: 1.0.1
 Summary: Rivian API Client (Unofficial)
 License: MIT
 Author: Brian Retterer
 Author-email: bretterer@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

