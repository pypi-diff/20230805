# Comparing `tmp/voicemeeter_api-2.4.2.tar.gz` & `tmp/voicemeeter_api-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicemeeter_api-2.4.2.tar", max compression
+gzip compressed data, was "voicemeeter_api-2.4.4.tar", max compression
```

## Comparing `voicemeeter_api-2.4.2.tar` & `voicemeeter_api-2.4.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter_api-2.4.2/LICENSE
--rw-r--r--   0        0        0     1102 2023-08-03 11:07:03.587927 voicemeeter_api-2.4.2/pyproject.toml
--rw-r--r--   0        0        0    18957 2023-08-01 15:15:42.523592 voicemeeter_api-2.4.2/README.md
--rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter_api-2.4.2/voicemeeterlib/__init__.py
--rw-r--r--   0        0        0     8226 2023-07-18 12:50:39.247222 voicemeeter_api-2.4.2/voicemeeterlib/bus.py
--rw-r--r--   0        0        0     4618 2023-08-02 14:26:03.847115 voicemeeter_api-2.4.2/voicemeeterlib/cbindings.py
--rw-r--r--   0        0        0     1194 2023-07-25 17:25:27.080618 voicemeeter_api-2.4.2/voicemeeterlib/command.py
--rw-r--r--   0        0        0     6050 2023-08-01 16:48:00.788867 voicemeeter_api-2.4.2/voicemeeterlib/config.py
--rw-r--r--   0        0        0     1748 2023-07-25 17:25:30.796461 voicemeeter_api-2.4.2/voicemeeterlib/device.py
--rw-r--r--   0        0        0      666 2023-08-02 14:34:34.328692 voicemeeter_api-2.4.2/voicemeeterlib/error.py
--rw-r--r--   0        0        0     2099 2023-06-22 08:38:58.271443 voicemeeter_api-2.4.2/voicemeeterlib/event.py
--rw-r--r--   0        0        0     7778 2023-08-02 16:12:16.446060 voicemeeter_api-2.4.2/voicemeeterlib/factory.py
--rw-r--r--   0        0        0     1091 2023-07-25 17:25:27.080618 voicemeeter_api-2.4.2/voicemeeterlib/inst.py
--rw-r--r--   0        0        0     1800 2023-07-25 17:25:30.842924 voicemeeter_api-2.4.2/voicemeeterlib/iremote.py
--rw-r--r--   0        0        0     2628 2023-07-18 13:00:26.971422 voicemeeter_api-2.4.2/voicemeeterlib/kinds.py
--rw-r--r--   0        0        0     1512 2023-07-25 17:25:30.885025 voicemeeter_api-2.4.2/voicemeeterlib/macrobutton.py
--rw-r--r--   0        0        0     1130 2023-06-21 12:24:03.433043 voicemeeter_api-2.4.2/voicemeeterlib/meta.py
--rw-r--r--   0        0        0     6485 2023-07-28 09:25:54.753959 voicemeeter_api-2.4.2/voicemeeterlib/misc.py
--rw-r--r--   0        0        0     6739 2023-07-01 18:30:01.004734 voicemeeter_api-2.4.2/voicemeeterlib/recorder.py
--rw-r--r--   0        0        0    12303 2023-08-02 16:11:06.719892 voicemeeter_api-2.4.2/voicemeeterlib/remote.py
--rw-r--r--   0        0        0    15352 2023-07-22 11:42:06.374784 voicemeeter_api-2.4.2/voicemeeterlib/strip.py
--rw-r--r--   0        0        0     2277 2023-08-01 15:15:42.525096 voicemeeter_api-2.4.2/voicemeeterlib/subject.py
--rw-r--r--   0        0        0     2930 2023-07-18 13:06:02.678934 voicemeeter_api-2.4.2/voicemeeterlib/updater.py
--rw-r--r--   0        0        0     2436 2023-07-21 11:41:24.422287 voicemeeter_api-2.4.2/voicemeeterlib/util.py
--rw-r--r--   0        0        0     5945 2023-08-03 11:07:31.205227 voicemeeter_api-2.4.2/voicemeeterlib/vban.py
--rw-r--r--   0        0        0    18745 1970-01-01 00:00:00.000000 voicemeeter_api-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter_api-2.4.4/LICENSE
+-rw-r--r--   0        0        0     1102 2023-08-05 12:08:15.182775 voicemeeter_api-2.4.4/pyproject.toml
+-rw-r--r--   0        0        0    18957 2023-08-01 15:15:42.523592 voicemeeter_api-2.4.4/README.md
+-rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter_api-2.4.4/voicemeeterlib/__init__.py
+-rw-r--r--   0        0        0     8238 2023-08-05 12:08:15.184385 voicemeeter_api-2.4.4/voicemeeterlib/bus.py
+-rw-r--r--   0        0        0     4618 2023-08-02 14:26:03.847115 voicemeeter_api-2.4.4/voicemeeterlib/cbindings.py
+-rw-r--r--   0        0        0     1194 2023-07-25 17:25:27.080618 voicemeeter_api-2.4.4/voicemeeterlib/command.py
+-rw-r--r--   0        0        0     6050 2023-08-01 16:48:00.788867 voicemeeter_api-2.4.4/voicemeeterlib/config.py
+-rw-r--r--   0        0        0     1748 2023-07-25 17:25:30.796461 voicemeeter_api-2.4.4/voicemeeterlib/device.py
+-rw-r--r--   0        0        0      666 2023-08-02 14:34:34.328692 voicemeeter_api-2.4.4/voicemeeterlib/error.py
+-rw-r--r--   0        0        0     2099 2023-06-22 08:38:58.271443 voicemeeter_api-2.4.4/voicemeeterlib/event.py
+-rw-r--r--   0        0        0     7778 2023-08-02 16:12:16.446060 voicemeeter_api-2.4.4/voicemeeterlib/factory.py
+-rw-r--r--   0        0        0     1091 2023-07-25 17:25:27.080618 voicemeeter_api-2.4.4/voicemeeterlib/inst.py
+-rw-r--r--   0        0        0     1800 2023-07-25 17:25:30.842924 voicemeeter_api-2.4.4/voicemeeterlib/iremote.py
+-rw-r--r--   0        0        0     2628 2023-07-18 13:00:26.971422 voicemeeter_api-2.4.4/voicemeeterlib/kinds.py
+-rw-r--r--   0        0        0     1512 2023-07-25 17:25:30.885025 voicemeeter_api-2.4.4/voicemeeterlib/macrobutton.py
+-rw-r--r--   0        0        0     1130 2023-06-21 12:24:03.433043 voicemeeter_api-2.4.4/voicemeeterlib/meta.py
+-rw-r--r--   0        0        0     6485 2023-07-28 09:25:54.753959 voicemeeter_api-2.4.4/voicemeeterlib/misc.py
+-rw-r--r--   0        0        0     6739 2023-07-01 18:30:01.004734 voicemeeter_api-2.4.4/voicemeeterlib/recorder.py
+-rw-r--r--   0        0        0    12604 2023-08-05 12:08:15.184385 voicemeeter_api-2.4.4/voicemeeterlib/remote.py
+-rw-r--r--   0        0        0    15364 2023-08-05 12:08:15.185313 voicemeeter_api-2.4.4/voicemeeterlib/strip.py
+-rw-r--r--   0        0        0     2277 2023-08-01 15:15:42.525096 voicemeeter_api-2.4.4/voicemeeterlib/subject.py
+-rw-r--r--   0        0        0     2965 2023-08-05 12:08:15.200090 voicemeeter_api-2.4.4/voicemeeterlib/updater.py
+-rw-r--r--   0        0        0     2436 2023-07-21 11:41:24.422287 voicemeeter_api-2.4.4/voicemeeterlib/util.py
+-rw-r--r--   0        0        0     5945 2023-08-03 11:07:31.205227 voicemeeter_api-2.4.4/voicemeeterlib/vban.py
+-rw-r--r--   0        0        0    18745 1970-01-01 00:00:00.000000 voicemeeter_api-2.4.4/PKG-INFO
```

### Comparing `voicemeeter_api-2.4.2/LICENSE` & `voicemeeter_api-2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.2/pyproject.toml` & `voicemeeter_api-2.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voicemeeter-api"
-version = "2.4.2"
+version = "2.4.4"
 description = "A Python wrapper for the Voiceemeter API"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/voicemeeter-api-python"
 
 packages = [{ include = "voicemeeterlib" }]
```

### Comparing `voicemeeter_api-2.4.2/README.md` & `voicemeeter_api-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.2/voicemeeterlib/bus.py` & `voicemeeter_api-2.4.4/voicemeeterlib/bus.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
 
         Otherwise call CAPI func.
         """
 
         def fget(x):
             return round(20 * log(x, 10), 1) if x > 0 else -200.0
 
-        if self._remote.running and self._remote.event.ldirty:
+        if not self._remote.stopped() and self._remote.event.ldirty:
             vals = self._remote.cache["bus_level"][self.range[0] : self.range[-1]]
         else:
             vals = [self._remote.get_level(mode, i) for i in range(*self.range)]
 
         return tuple(fget(val) for val in vals)
 
     @property
@@ -228,15 +228,15 @@
     @property
     def isdirty(self) -> bool:
         """
         Returns dirty status for this specific channel.
 
         Expected to be used in a callback only.
         """
-        if self._remote.running:
+        if not self._remote.stopped():
             return any(self._remote._bus_comp[self.range[0] : self.range[-1]])
 
     is_updated = isdirty
 
 
 def make_bus_level_map(kind):
     return tuple((i, i + 8) for i in range(0, (kind.phys_out + kind.virt_out) * 8, 8))
```

### Comparing `voicemeeter_api-2.4.2/voicemeeterlib/cbindings.py` & `voicemeeter_api-2.4.4/voicemeeterlib/cbindings.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.2/voicemeeterlib/command.py` & `voicemeeter_api-2.4.4/voicemeeterlib/command.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.2/voicemeeterlib/config.py` & `voicemeeter_api-2.4.4/voicemeeterlib/config.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.2/voicemeeterlib/device.py` & `voicemeeter_api-2.4.4/voicemeeterlib/device.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.2/voicemeeterlib/error.py` & `voicemeeter_api-2.4.4/voicemeeterlib/error.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.2/voicemeeterlib/event.py` & `voicemeeter_api-2.4.4/voicemeeterlib/event.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.2/voicemeeterlib/factory.py` & `voicemeeter_api-2.4.4/voicemeeterlib/factory.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.2/voicemeeterlib/inst.py` & `voicemeeter_api-2.4.4/voicemeeterlib/inst.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.2/voicemeeterlib/iremote.py` & `voicemeeter_api-2.4.4/voicemeeterlib/iremote.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.2/voicemeeterlib/kinds.py` & `voicemeeter_api-2.4.4/voicemeeterlib/kinds.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.2/voicemeeterlib/macrobutton.py` & `voicemeeter_api-2.4.4/voicemeeterlib/macrobutton.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.2/voicemeeterlib/meta.py` & `voicemeeter_api-2.4.4/voicemeeterlib/meta.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.2/voicemeeterlib/misc.py` & `voicemeeter_api-2.4.4/voicemeeterlib/misc.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.2/voicemeeterlib/recorder.py` & `voicemeeter_api-2.4.4/voicemeeterlib/recorder.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.2/voicemeeterlib/remote.py` & `voicemeeter_api-2.4.4/voicemeeterlib/remote.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import ctypes as ct
 import logging
+import threading
 import time
 from abc import abstractmethod
 from queue import Queue
 from typing import Iterable, Optional, Union
 
 from .cbindings import CBindings
 from .error import CAPIError, VMError
@@ -24,19 +25,19 @@
     DELAY = 0.001
 
     def __init__(self, **kwargs):
         self.strip_mode = 0
         self.cache = {}
         self.midi = Midi()
         self.subject = self.observer = Subject()
-        self.running = False
         self.event = Event(
             {k: kwargs.pop(k) for k in ("pdirty", "mdirty", "midi", "ldirty")}
         )
         self.gui = VmGui()
+        self.stop_event = None
         self.logger = logger.getChild(self.__class__.__name__)
 
         for attr, val in kwargs.items():
             setattr(self, attr, val)
 
     def __enter__(self):
         """setup procedures"""
@@ -48,24 +49,28 @@
     @abstractmethod
     def __str__(self):
         """Ensure subclasses override str magic method"""
         pass
 
     def init_thread(self):
         """Starts updates thread."""
-        self.running = True
         self.event.info()
 
         self.logger.debug("initiating events thread")
+        self.stop_event = threading.Event()
+        self.stop_event.clear()
         queue = Queue()
         self.updater = Updater(self, queue)
         self.updater.start()
-        self.producer = Producer(self, queue)
+        self.producer = Producer(self, queue, self.stop_event)
         self.producer.start()
 
+    def stopped(self):
+        return self.stop_event is None or self.stop_event.is_set()
+
     def login(self) -> None:
         """Login to the API, initialize dirty parameters"""
         self.gui.launched = self.call(self.bind_login, ok=(0, 1)) == 0
         if not self.gui.launched:
             self.logger.info(
                 "Voicemeeter engine running but GUI not launched. Launching the GUI now."
             )
@@ -327,16 +332,18 @@
             self.logger.debug(
                 f"profile '{name}' extends '{extended}', profiles merged.."
             )
         self.apply(config)
         self.logger.info(f"Profile '{name}' applied!")
 
     def end_thread(self):
-        self.logger.debug("events thread shutdown started")
-        self.running = False
+        if not self.stopped():
+            self.logger.debug("events thread shutdown started")
+            self.stop_event.set()
+            self.producer.join()  # wait for producer thread to complete cycle
 
     def logout(self) -> None:
         """Logout of the API"""
         time.sleep(0.1)
         self.call(self.bind_logout)
         self.logger.info(f"{type(self).__name__}: Successfully logged out of {self}")
```

### Comparing `voicemeeter_api-2.4.2/voicemeeterlib/strip.py` & `voicemeeter_api-2.4.4/voicemeeterlib/strip.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,15 +411,15 @@
 
         Otherwise call CAPI func.
         """
 
         def fget(x):
             return round(20 * log(x, 10), 1) if x > 0 else -200.0
 
-        if self._remote.running and self._remote.event.ldirty:
+        if not self._remote.stopped() and self._remote.event.ldirty:
             vals = self._remote.cache["strip_level"][self.range[0] : self.range[-1]]
         else:
             vals = [self._remote.get_level(mode, i) for i in range(*self.range)]
 
         return tuple(fget(val) for val in vals)
 
     @property
@@ -444,15 +444,15 @@
     @property
     def isdirty(self) -> bool:
         """
         Returns dirty status for this specific channel.
 
         Expected to be used in a callback only.
         """
-        if self._remote.running:
+        if not self._remote.stopped():
             return any(self._remote._strip_comp[self.range[0] : self.range[-1]])
 
     is_updated = isdirty
 
 
 def make_strip_level_map(kind):
     phys_map = tuple((i, i + 2) for i in range(0, kind.phys_in * 2, 2))
```

### Comparing `voicemeeter_api-2.4.2/voicemeeterlib/subject.py` & `voicemeeter_api-2.4.4/voicemeeterlib/subject.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.2/voicemeeterlib/updater.py` & `voicemeeter_api-2.4.4/voicemeeterlib/updater.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,26 @@
 
 logger = logging.getLogger(__name__)
 
 
 class Producer(threading.Thread):
     """Continously send job queue to the Updater thread at a rate of self._remote.ratelimit."""
 
-    def __init__(self, remote, queue):
-        super().__init__(name="producer", daemon=True)
+    def __init__(self, remote, queue, stop_event):
+        super().__init__(name="producer", daemon=False)
         self._remote = remote
         self.queue = queue
+        self.stop_event = stop_event
         self.logger = logger.getChild(self.__class__.__name__)
 
+    def stopped(self):
+        return self.stop_event.is_set()
+
     def run(self):
-        while self._remote.running:
+        while not self.stopped():
             if self._remote.event.pdirty:
                 self.queue.put("pdirty")
             if self._remote.event.mdirty:
                 self.queue.put("mdirty")
             if self._remote.event.midi:
                 self.queue.put("midi")
             if self._remote.event.ldirty:
@@ -52,24 +56,20 @@
 
     def run(self):
         """
         Continously update observers of dirty states.
 
         Generate _strip_comp, _bus_comp and update level cache if ldirty.
         """
-        while True:
-            event = self.queue.get()
-            if event is None:
-                self.logger.debug(f"terminating {self.name} thread")
-                break
-
+        while event := self.queue.get():
             if event == "pdirty" and self._remote.pdirty:
                 self._remote.subject.notify(event)
             elif event == "mdirty" and self._remote.mdirty:
                 self._remote.subject.notify(event)
             elif event == "midi" and self._remote.get_midi_message():
                 self._remote.subject.notify(event)
             elif event == "ldirty" and self._remote.ldirty:
                 self._update_comps(self._remote._strip_buf, self._remote._bus_buf)
                 self._remote.cache["strip_level"] = self._remote._strip_buf
                 self._remote.cache["bus_level"] = self._remote._bus_buf
                 self._remote.subject.notify(event)
+        self.logger.debug(f"terminating {self.name} thread")
```

### Comparing `voicemeeter_api-2.4.2/voicemeeterlib/util.py` & `voicemeeter_api-2.4.4/voicemeeterlib/util.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.2/voicemeeterlib/vban.py` & `voicemeeter_api-2.4.4/voicemeeterlib/vban.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.4.2/PKG-INFO` & `voicemeeter_api-2.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicemeeter-api
-Version: 2.4.2
+Version: 2.4.4
 Summary: A Python wrapper for the Voiceemeter API
 Home-page: https://github.com/onyx-and-iris/voicemeeter-api-python
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

