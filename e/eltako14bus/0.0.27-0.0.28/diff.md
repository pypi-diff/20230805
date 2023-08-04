# Comparing `tmp/eltako14bus-0.0.27.tar.gz` & `tmp/eltako14bus-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eltako14bus-0.0.27.tar", last modified: Fri Jun  2 20:16:45 2023, max compression
+gzip compressed data, was "eltako14bus-0.0.28.tar", last modified: Fri Aug  4 22:24:36 2023, max compression
```

## Comparing `eltako14bus-0.0.27.tar` & `eltako14bus-0.0.28.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-06-02 20:16:45.947741 eltako14bus-0.0.27/
--rw-rw-r--   0 philipp   (1000) philipp   (1000)    35149 2023-05-30 12:57:46.000000 eltako14bus-0.0.27/LICENSE
--rw-rw-r--   0 philipp   (1000) philipp   (1000)     2939 2023-06-02 20:16:45.943741 eltako14bus-0.0.27/PKG-INFO
--rw-rw-r--   0 philipp   (1000) philipp   (1000)     2412 2023-05-30 12:57:46.000000 eltako14bus-0.0.27/README.md
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-06-02 20:16:45.939741 eltako14bus-0.0.27/eltako14bus.egg-info/
--rw-rw-r--   0 philipp   (1000) philipp   (1000)     2939 2023-06-02 20:16:45.000000 eltako14bus-0.0.27/eltako14bus.egg-info/PKG-INFO
--rw-rw-r--   0 philipp   (1000) philipp   (1000)      393 2023-06-02 20:16:45.000000 eltako14bus-0.0.27/eltako14bus.egg-info/SOURCES.txt
--rw-rw-r--   0 philipp   (1000) philipp   (1000)        1 2023-06-02 20:16:45.000000 eltako14bus-0.0.27/eltako14bus.egg-info/dependency_links.txt
--rw-rw-r--   0 philipp   (1000) philipp   (1000)       91 2023-06-02 20:16:45.000000 eltako14bus-0.0.27/eltako14bus.egg-info/requires.txt
--rw-rw-r--   0 philipp   (1000) philipp   (1000)       10 2023-06-02 20:16:45.000000 eltako14bus-0.0.27/eltako14bus.egg-info/top_level.txt
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-06-02 20:16:45.943741 eltako14bus-0.0.27/eltakobus/
--rw-rw-r--   0 philipp   (1000) philipp   (1000)      468 2023-05-16 21:47:48.000000 eltako14bus-0.0.27/eltakobus/__init__.py
--rw-rw-r--   0 philipp   (1000) philipp   (1000)     8533 2023-05-09 21:38:00.000000 eltako14bus-0.0.27/eltakobus/bus.py
--rw-rw-r--   0 philipp   (1000) philipp   (1000)     1100 2023-05-16 21:47:48.000000 eltako14bus-0.0.27/eltakobus/coap.py
--rw-rw-r--   0 philipp   (1000) philipp   (1000)    30434 2023-05-17 07:23:07.000000 eltako14bus-0.0.27/eltakobus/device.py
--rw-rw-r--   0 philipp   (1000) philipp   (1000)    20918 2023-05-17 07:23:07.000000 eltako14bus-0.0.27/eltakobus/eep.py
--rw-rw-r--   0 philipp   (1000) philipp   (1000)      955 2023-05-17 07:23:07.000000 eltako14bus-0.0.27/eltakobus/error.py
--rw-rw-r--   0 philipp   (1000) philipp   (1000)     2521 2023-05-17 07:23:07.000000 eltako14bus-0.0.27/eltakobus/locking.py
--rw-rw-r--   0 philipp   (1000) philipp   (1000)    19187 2023-05-18 21:29:37.000000 eltako14bus-0.0.27/eltakobus/message.py
--rw-rw-r--   0 philipp   (1000) philipp   (1000)     8825 2023-05-09 21:38:00.000000 eltako14bus-0.0.27/eltakobus/serial.py
--rw-rw-r--   0 philipp   (1000) philipp   (1000)     1628 2023-05-17 07:23:07.000000 eltako14bus-0.0.27/eltakobus/util.py
--rw-rw-r--   0 philipp   (1000) philipp   (1000)       38 2023-06-02 20:16:45.947741 eltako14bus-0.0.27/setup.cfg
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     1108 2023-06-02 20:16:19.000000 eltako14bus-0.0.27/setup.py
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-08-04 22:24:36.299651 eltako14bus-0.0.28/
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)    35149 2023-05-30 12:57:46.000000 eltako14bus-0.0.28/LICENSE
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)     2939 2023-08-04 22:24:36.299651 eltako14bus-0.0.28/PKG-INFO
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)     2412 2023-05-30 12:57:46.000000 eltako14bus-0.0.28/README.md
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-08-04 22:24:36.259652 eltako14bus-0.0.28/eltako14bus.egg-info/
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)     2939 2023-08-04 22:24:35.000000 eltako14bus-0.0.28/eltako14bus.egg-info/PKG-INFO
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)      393 2023-08-04 22:24:35.000000 eltako14bus-0.0.28/eltako14bus.egg-info/SOURCES.txt
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)        1 2023-08-04 22:24:35.000000 eltako14bus-0.0.28/eltako14bus.egg-info/dependency_links.txt
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)       91 2023-08-04 22:24:35.000000 eltako14bus-0.0.28/eltako14bus.egg-info/requires.txt
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)       10 2023-08-04 22:24:35.000000 eltako14bus-0.0.28/eltako14bus.egg-info/top_level.txt
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-08-04 22:24:36.299651 eltako14bus-0.0.28/eltakobus/
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)      468 2023-05-16 21:47:48.000000 eltako14bus-0.0.28/eltakobus/__init__.py
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)     8533 2023-05-09 21:38:00.000000 eltako14bus-0.0.28/eltakobus/bus.py
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)     1100 2023-05-16 21:47:48.000000 eltako14bus-0.0.28/eltakobus/coap.py
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)    30434 2023-05-17 07:23:07.000000 eltako14bus-0.0.28/eltakobus/device.py
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)    22111 2023-08-04 21:43:35.000000 eltako14bus-0.0.28/eltakobus/eep.py
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)      955 2023-05-17 07:23:07.000000 eltako14bus-0.0.28/eltakobus/error.py
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)     2521 2023-05-17 07:23:07.000000 eltako14bus-0.0.28/eltakobus/locking.py
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)    19187 2023-05-18 21:29:37.000000 eltako14bus-0.0.28/eltakobus/message.py
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)     8825 2023-05-09 21:38:00.000000 eltako14bus-0.0.28/eltakobus/serial.py
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)     1628 2023-05-17 07:23:07.000000 eltako14bus-0.0.28/eltakobus/util.py
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)       38 2023-08-04 22:24:36.299651 eltako14bus-0.0.28/setup.cfg
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     1108 2023-08-04 22:22:39.000000 eltako14bus-0.0.28/setup.py
```

### Comparing `eltako14bus-0.0.27/LICENSE` & `eltako14bus-0.0.28/LICENSE`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.27/PKG-INFO` & `eltako14bus-0.0.28/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eltako14bus
-Version: 0.0.27
+Version: 0.0.28
 Summary: Library for participating in the Eltako Series 14 RS485 bus
 Home-page: https://github.com/grimmpp/eltako14bus
 Author: chrysn, grimmpp
 Author-email: chrysn@fsfe.org, grimmpp14@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Description-Content-Type: text/markdown
```

### Comparing `eltako14bus-0.0.27/README.md` & `eltako14bus-0.0.28/README.md`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.27/eltako14bus.egg-info/PKG-INFO` & `eltako14bus-0.0.28/eltako14bus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eltako14bus
-Version: 0.0.27
+Version: 0.0.28
 Summary: Library for participating in the Eltako Series 14 RS485 bus
 Home-page: https://github.com/grimmpp/eltako14bus
 Author: chrysn, grimmpp
 Author-email: chrysn@fsfe.org, grimmpp14@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Description-Content-Type: text/markdown
```

### Comparing `eltako14bus-0.0.27/eltakobus/bus.py` & `eltako14bus-0.0.28/eltakobus/bus.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.27/eltakobus/coap.py` & `eltako14bus-0.0.28/eltakobus/coap.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.27/eltakobus/device.py` & `eltako14bus-0.0.28/eltakobus/device.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.27/eltakobus/eep.py` & `eltako14bus-0.0.28/eltakobus/eep.py`

 * *Files 4% similar despite different names*

```diff
@@ -524,14 +524,57 @@
         self._sun_east = sun_east
         self._hemisphere = hemisphere
 
 class A5_13_01(_WeatherStation):
     """Weather station"""
 
 # ======================================
+# MARK: -  temperature + humidity sensor
+# ======================================
+class _TemperatureAndHumiditySensor(EEP):
+    @classmethod
+    def decode_message(cls, msg):
+        if msg.org != 0x07:
+            raise WrongOrgError
+        
+        # 0 .. 100%
+        humidity = (msg.data[1] /255.0) * 100
+        # -20°C .. +60°C
+        temperature = (msg.data[2] / 255.0 ) * 80.0 - 20.0
+        
+
+        return cls(temperature,humidity)
+
+    def encode_message(self, address):
+        data = bytearray([0, 0, 0, 0])
+        data[0] = 0x00
+        data[1] = int((self.humidity / 100.0) * 255.0)
+        data[2] = int(((self.temperature + 20.0) / 80.0) * 255.0)
+        data[3] = 0x00
+        
+        status = 0x00
+
+        return Regular4BSMessage(address, status, data, True)
+
+    @property
+    def temperature(self):
+        return self._temperature
+    
+    @property
+    def humidity(self):
+        return self._humidity
+    
+    def __init__(self, temperature, humidity):
+        self._temperature = temperature
+        self._humidity = humidity
+
+class A5_04_02(_TemperatureAndHumiditySensor):
+    """Temperature and Humidity Sensor"""
+
+# ======================================
 # MARK: - Automated Meter Reading
 # ======================================
 
 class _AutomatedMeterReading(EEP):
     @classmethod
     def decode_message(cls, msg):
         if msg.org != 0x07:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `eltako14bus-0.0.27/eltakobus/error.py` & `eltako14bus-0.0.28/eltakobus/error.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.27/eltakobus/locking.py` & `eltako14bus-0.0.28/eltakobus/locking.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.27/eltakobus/message.py` & `eltako14bus-0.0.28/eltakobus/message.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.27/eltakobus/serial.py` & `eltako14bus-0.0.28/eltakobus/serial.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.27/eltakobus/util.py` & `eltako14bus-0.0.28/eltakobus/util.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.27/setup.py` & `eltako14bus-0.0.28/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 }
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="eltako14bus",
-    version="0.0.27",
+    version="0.0.28",
     author="chrysn, grimmpp",
     author_email="chrysn@fsfe.org, grimmpp14@gmail.com",
     description="Library for participating in the Eltako Series 14 RS485 bus",
     url="https://github.com/grimmpp/eltako14bus",
     packages=setuptools.find_packages(),
     extras_require=extras_require,
     # Not that there'd be tests, but at least it fetches the right dependencies and syntax checks everything
```

