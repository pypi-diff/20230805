# Comparing `tmp/amniotic-0.5.7.tar.gz` & `tmp/amniotic-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amniotic-0.5.7.tar", last modified: Sat Jun 17 17:43:03 2023, max compression
+gzip compressed data, was "amniotic-0.5.8.tar", last modified: Sat Jun 24 14:35:41 2023, max compression
```

## Comparing `amniotic-0.5.7.tar` & `amniotic-0.5.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:43:03.873954 amniotic-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-17 17:43:03.873954 amniotic-0.5.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:43:03.869954 amniotic-0.5.7/amniotic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 17:42:54.000000 amniotic-0.5.7/amniotic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20097 2023-06-17 17:42:54.000000 amniotic-0.5.7/amniotic/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-17 17:42:54.000000 amniotic-0.5.7/amniotic/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:43:03.873954 amniotic-0.5.7/amniotic/mqtt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 17:42:54.000000 amniotic-0.5.7/amniotic/mqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20347 2023-06-17 17:42:54.000000 amniotic-0.5.7/amniotic/mqtt/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-17 17:42:54.000000 amniotic-0.5.7/amniotic/mqtt/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-06-17 17:42:54.000000 amniotic-0.5.7/amniotic/mqtt/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-17 17:42:54.000000 amniotic-0.5.7/amniotic/mqtt/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-17 17:42:54.000000 amniotic-0.5.7/amniotic/mqtt/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-17 17:43:00.000000 amniotic-0.5.7/amniotic/version
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-17 17:42:54.000000 amniotic-0.5.7/amniotic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:43:03.869954 amniotic-0.5.7/amniotic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-17 17:43:03.000000 amniotic-0.5.7/amniotic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-17 17:43:03.000000 amniotic-0.5.7/amniotic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 17:43:03.000000 amniotic-0.5.7/amniotic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-17 17:43:03.000000 amniotic-0.5.7/amniotic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-17 17:43:03.000000 amniotic-0.5.7/amniotic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-17 17:43:03.000000 amniotic-0.5.7/amniotic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 17:43:03.873954 amniotic-0.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-17 17:42:54.000000 amniotic-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:35:41.024410 amniotic-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-24 14:35:41.024410 amniotic-0.5.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:35:41.020410 amniotic-0.5.8/amniotic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 14:35:33.000000 amniotic-0.5.8/amniotic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20097 2023-06-24 14:35:33.000000 amniotic-0.5.8/amniotic/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-24 14:35:33.000000 amniotic-0.5.8/amniotic/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:35:41.024410 amniotic-0.5.8/amniotic/mqtt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 14:35:33.000000 amniotic-0.5.8/amniotic/mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20347 2023-06-24 14:35:33.000000 amniotic-0.5.8/amniotic/mqtt/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-24 14:35:33.000000 amniotic-0.5.8/amniotic/mqtt/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-06-24 14:35:33.000000 amniotic-0.5.8/amniotic/mqtt/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-24 14:35:33.000000 amniotic-0.5.8/amniotic/mqtt/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-24 14:35:33.000000 amniotic-0.5.8/amniotic/mqtt/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-24 14:35:38.000000 amniotic-0.5.8/amniotic/version
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-24 14:35:33.000000 amniotic-0.5.8/amniotic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:35:41.020410 amniotic-0.5.8/amniotic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-24 14:35:40.000000 amniotic-0.5.8/amniotic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-24 14:35:41.000000 amniotic-0.5.8/amniotic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 14:35:40.000000 amniotic-0.5.8/amniotic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-24 14:35:40.000000 amniotic-0.5.8/amniotic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-24 14:35:40.000000 amniotic-0.5.8/amniotic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-24 14:35:40.000000 amniotic-0.5.8/amniotic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 14:35:41.024410 amniotic-0.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-24 14:35:33.000000 amniotic-0.5.8/setup.py
```

### Comparing `amniotic-0.5.7/PKG-INFO` & `amniotic-0.5.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: amniotic
-Version: 0.5.7
+Version: 0.5.8
 Summary: A multi-output ambient sound mixer for Home Assistant
 Home-page: https://link.frontmatter.ai/amniotic
 Author: Frontmatter
 License: Copyright © 2022 Frontmatter. All rights reserved.
 Keywords: ambient sound audio white noise masking sleep
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Provides-Extra: debug
 
 # Amniotic
 
 A multi-output ambient sound mixer for Home Assistant.
 
 Amniotic lets you use a single device to create on-the-fly, custom ambient audio mixes - e.g. mixing Waterfall sounds
 with Birdsong on one set of speakers, while playing Fireplace sounds from a second audio device - to suit your tastes
```

### Comparing `amniotic-0.5.7/amniotic/audio.py` & `amniotic-0.5.8/amniotic/audio.py`

 * *Files identical despite different names*

### Comparing `amniotic-0.5.7/amniotic/config.py` & `amniotic-0.5.8/amniotic/config.py`

 * *Files identical despite different names*

### Comparing `amniotic-0.5.7/amniotic/mqtt/control.py` & `amniotic-0.5.8/amniotic/mqtt/control.py`

 * *Files identical despite different names*

### Comparing `amniotic-0.5.7/amniotic/mqtt/device.py` & `amniotic-0.5.8/amniotic/mqtt/device.py`

 * *Files identical despite different names*

### Comparing `amniotic-0.5.7/amniotic/mqtt/loop.py` & `amniotic-0.5.8/amniotic/mqtt/loop.py`

 * *Files identical despite different names*

### Comparing `amniotic-0.5.7/amniotic/mqtt/sensor.py` & `amniotic-0.5.8/amniotic/mqtt/sensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import psutil as psutil
 from datetime import timedelta
 from typing import Optional, Union, Any
 
 from amniotic.mqtt import control
 from amniotic.version import __version__
 
 
@@ -242,14 +241,15 @@
 
     def get_value(self, key: Optional[str] = None):
         """
 
         Get CPU usage.
 
         """
+        import psutil as psutil
         return psutil.cpu_percent(interval=1)
 
 
 class Memory(Sensor):
     """
 
     Home Assistant sensor showing overview of which Themes are enabled, etc.
@@ -265,8 +265,9 @@
 
     def get_value(self, key: Optional[str] = None):
         """
 
         Get memory usage.
 
         """
+        import psutil as psutil
         return psutil.virtual_memory().percent
```

### Comparing `amniotic-0.5.7/amniotic/mqtt/tools.py` & `amniotic-0.5.8/amniotic/mqtt/tools.py`

 * *Files identical despite different names*

### Comparing `amniotic-0.5.7/amniotic.egg-info/PKG-INFO` & `amniotic-0.5.8/amniotic.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: amniotic
-Version: 0.5.7
+Version: 0.5.8
 Summary: A multi-output ambient sound mixer for Home Assistant
 Home-page: https://link.frontmatter.ai/amniotic
 Author: Frontmatter
 License: Copyright © 2022 Frontmatter. All rights reserved.
 Keywords: ambient sound audio white noise masking sleep
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Provides-Extra: debug
 
 # Amniotic
 
 A multi-output ambient sound mixer for Home Assistant.
 
 Amniotic lets you use a single device to create on-the-fly, custom ambient audio mixes - e.g. mixing Waterfall sounds
 with Birdsong on one set of speakers, while playing Fireplace sounds from a second audio device - to suit your tastes
```

### Comparing `amniotic-0.5.7/setup.py` & `amniotic-0.5.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,17 +26,20 @@
         'paho-mqtt',
         'python-vlc',
         'getmac',
         'pyyaml',
         'appdirs',
         'johnnydep',
         'pytube',
-        'cachetools',
-        'psutil'
+        'cachetools'
     ],
-    extras_require={},
+    extras_require={
+        'debug': [
+            'psutil'
+        ]
+    },
     entry_points={
         'console_scripts': [
             'amniotic = amniotic.mqtt.loop:start',
         ],
     }
 )
```

