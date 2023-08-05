# Comparing `tmp/vban_cmd-2.4.1.tar.gz` & `tmp/vban_cmd-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vban_cmd-2.4.1.tar", max compression
+gzip compressed data, was "vban_cmd-2.4.3.tar", max compression
```

## Comparing `vban_cmd-2.4.1.tar` & `vban_cmd-2.4.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1091 2022-03-24 12:30:28.474287 vban_cmd-2.4.1/LICENSE
--rw-r--r--   0        0        0      951 2023-08-02 16:17:42.142733 vban_cmd-2.4.1/pyproject.toml
--rw-r--r--   0        0        0    12875 2023-07-15 07:15:00.451610 vban_cmd-2.4.1/README.md
--rw-r--r--   0        0        0       70 2022-07-12 16:30:51.963399 vban_cmd-2.4.1/vban_cmd/__init__.py
--rw-r--r--   0        0        0     5276 2023-06-25 10:36:16.654167 vban_cmd-2.4.1/vban_cmd/bus.py
--rw-r--r--   0        0        0     1127 2023-06-25 10:36:19.263212 vban_cmd-2.4.1/vban_cmd/command.py
--rw-r--r--   0        0        0     5855 2023-07-11 17:23:11.340063 vban_cmd-2.4.1/vban_cmd/config.py
--rw-r--r--   0        0        0      220 2023-08-02 14:36:24.956502 vban_cmd-2.4.1/vban_cmd/error.py
--rw-r--r--   0        0        0     1621 2023-06-22 09:26:30.424951 vban_cmd-2.4.1/vban_cmd/event.py
--rw-r--r--   0        0        0     6888 2023-08-02 16:14:19.633476 vban_cmd-2.4.1/vban_cmd/factory.py
--rw-r--r--   0        0        0     4130 2023-07-25 14:58:38.295129 vban_cmd-2.4.1/vban_cmd/iremote.py
--rw-r--r--   0        0        0     2418 2023-07-25 14:54:48.277200 vban_cmd-2.4.1/vban_cmd/kinds.py
--rw-r--r--   0        0        0     1158 2023-07-25 15:00:05.263943 vban_cmd-2.4.1/vban_cmd/macrobutton.py
--rw-r--r--   0        0        0     2992 2023-06-25 10:36:33.230612 vban_cmd-2.4.1/vban_cmd/meta.py
--rw-r--r--   0        0        0     9625 2023-07-25 14:57:29.669770 vban_cmd-2.4.1/vban_cmd/packet.py
--rw-r--r--   0        0        0    10137 2023-06-25 12:32:36.307607 vban_cmd-2.4.1/vban_cmd/strip.py
--rw-r--r--   0        0        0     2277 2023-06-25 10:36:40.287522 vban_cmd-2.4.1/vban_cmd/subject.py
--rw-r--r--   0        0        0     2525 2023-07-12 03:46:12.026345 vban_cmd-2.4.1/vban_cmd/util.py
--rw-r--r--   0        0        0     5735 2023-07-26 10:30:31.333522 vban_cmd-2.4.1/vban_cmd/vban.py
--rw-r--r--   0        0        0     7423 2023-08-02 16:15:23.555395 vban_cmd-2.4.1/vban_cmd/vbancmd.py
--rw-r--r--   0        0        0     6879 2023-07-25 14:56:03.314782 vban_cmd-2.4.1/vban_cmd/worker.py
--rw-r--r--   0        0        0    12994 1970-01-01 00:00:00.000000 vban_cmd-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-03-24 12:30:28.474287 vban_cmd-2.4.3/LICENSE
+-rw-r--r--   0        0        0      951 2023-08-05 12:38:42.114435 vban_cmd-2.4.3/pyproject.toml
+-rw-r--r--   0        0        0    12875 2023-07-15 07:15:00.451610 vban_cmd-2.4.3/README.md
+-rw-r--r--   0        0        0       70 2022-07-12 16:30:51.963399 vban_cmd-2.4.3/vban_cmd/__init__.py
+-rw-r--r--   0        0        0     5282 2023-08-05 12:38:42.131764 vban_cmd-2.4.3/vban_cmd/bus.py
+-rw-r--r--   0        0        0     1127 2023-06-25 10:36:19.263212 vban_cmd-2.4.3/vban_cmd/command.py
+-rw-r--r--   0        0        0     5855 2023-07-11 17:23:11.340063 vban_cmd-2.4.3/vban_cmd/config.py
+-rw-r--r--   0        0        0      220 2023-08-02 14:36:24.956502 vban_cmd-2.4.3/vban_cmd/error.py
+-rw-r--r--   0        0        0     1621 2023-06-22 09:26:30.424951 vban_cmd-2.4.3/vban_cmd/event.py
+-rw-r--r--   0        0        0     6888 2023-08-02 16:14:19.633476 vban_cmd-2.4.3/vban_cmd/factory.py
+-rw-r--r--   0        0        0     4130 2023-07-25 14:58:38.295129 vban_cmd-2.4.3/vban_cmd/iremote.py
+-rw-r--r--   0        0        0     2418 2023-07-25 14:54:48.277200 vban_cmd-2.4.3/vban_cmd/kinds.py
+-rw-r--r--   0        0        0     1158 2023-07-25 15:00:05.263943 vban_cmd-2.4.3/vban_cmd/macrobutton.py
+-rw-r--r--   0        0        0     2992 2023-06-25 10:36:33.230612 vban_cmd-2.4.3/vban_cmd/meta.py
+-rw-r--r--   0        0        0    10281 2023-08-04 19:17:58.269466 vban_cmd-2.4.3/vban_cmd/packet.py
+-rw-r--r--   0        0        0    10143 2023-08-05 12:38:42.132905 vban_cmd-2.4.3/vban_cmd/strip.py
+-rw-r--r--   0        0        0     2277 2023-06-25 10:36:40.287522 vban_cmd-2.4.3/vban_cmd/subject.py
+-rw-r--r--   0        0        0     2525 2023-07-12 03:46:12.026345 vban_cmd-2.4.3/vban_cmd/util.py
+-rw-r--r--   0        0        0     5735 2023-07-26 10:30:31.333522 vban_cmd-2.4.3/vban_cmd/vban.py
+-rw-r--r--   0        0        0     7756 2023-08-05 12:38:42.133906 vban_cmd-2.4.3/vban_cmd/vbancmd.py
+-rw-r--r--   0        0        0     7274 2023-08-05 12:38:42.133906 vban_cmd-2.4.3/vban_cmd/worker.py
+-rw-r--r--   0        0        0    12994 1970-01-01 00:00:00.000000 vban_cmd-2.4.3/PKG-INFO
```

### Comparing `vban_cmd-2.4.1/LICENSE` & `vban_cmd-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.1/pyproject.toml` & `vban_cmd-2.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vban-cmd"
-version = "2.4.1"
+version = "2.4.3"
 description = "Python interface for the VBAN RT Packet Service (Sendtext)"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/vban-cmd-python"
 
 [tool.poetry.dependencies]
```

### Comparing `vban_cmd-2.4.1/README.md` & `vban_cmd-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.1/vban_cmd/bus.py` & `vban_cmd-2.4.3/vban_cmd/bus.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
     def getter(self):
         """Returns a tuple of level values for the channel."""
 
         def fget(i):
             return round((((1 << 16) - 1) - i) * -0.01, 1)
 
-        if self._remote.running and self._remote.event.ldirty:
+        if not self._remote.stopped() and self._remote.event.ldirty:
             return tuple(
                 fget(i)
                 for i in self._remote.cache["bus_level"][self.range[0] : self.range[-1]]
             )
         return tuple(
             fget(i)
             for i in self._remote._get_levels(self.public_packet)[1][
```

### Comparing `vban_cmd-2.4.1/vban_cmd/command.py` & `vban_cmd-2.4.3/vban_cmd/command.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.1/vban_cmd/config.py` & `vban_cmd-2.4.3/vban_cmd/config.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.1/vban_cmd/event.py` & `vban_cmd-2.4.3/vban_cmd/event.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.1/vban_cmd/factory.py` & `vban_cmd-2.4.3/vban_cmd/factory.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.1/vban_cmd/iremote.py` & `vban_cmd-2.4.3/vban_cmd/iremote.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.1/vban_cmd/kinds.py` & `vban_cmd-2.4.3/vban_cmd/kinds.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.1/vban_cmd/macrobutton.py` & `vban_cmd-2.4.3/vban_cmd/macrobutton.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.1/vban_cmd/meta.py` & `vban_cmd-2.4.3/vban_cmd/meta.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.1/vban_cmd/packet.py` & `vban_cmd-2.4.3/vban_cmd/packet.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 from dataclasses import dataclass
 
 from .kinds import KindMapClass
 from .util import comp
 
+VBAN_PROTOCOL_TXT = 0x40
+VBAN_PROTOCOL_SERVICE = 0x60
+
 VBAN_SERVICE_RTPACKETREGISTER = 32
 VBAN_SERVICE_RTPACKET = 33
+
 MAX_PACKET_SIZE = 1436
-HEADER_SIZE = 4 + 1 + 1 + 1 + 1 + 16 + 4
+HEADER_SIZE = 4 + 1 + 1 + 1 + 1 + 16
 
 
 @dataclass
 class VbanRtPacket:
     """Represents the body of a VBAN RT data packet"""
 
     _kind: KindMapClass
-    _voicemeeterType: bytes
-    _reserved: bytes
-    _buffersize: bytes
-    _voicemeeterVersion: bytes
-    _optionBits: bytes
-    _samplerate: bytes
-    _inputLeveldB100: bytes
-    _outputLeveldB100: bytes
-    _TransportBit: bytes
-    _stripState: bytes
-    _busState: bytes
-    _stripGaindB100Layer1: bytes
-    _stripGaindB100Layer2: bytes
-    _stripGaindB100Layer3: bytes
-    _stripGaindB100Layer4: bytes
-    _stripGaindB100Layer5: bytes
-    _stripGaindB100Layer6: bytes
-    _stripGaindB100Layer7: bytes
-    _stripGaindB100Layer8: bytes
-    _busGaindB100: bytes
-    _stripLabelUTF8c60: bytes
-    _busLabelUTF8c60: bytes
+    _voicemeeterType: bytes  # data[28:29]
+    _reserved: bytes  # data[29:30]
+    _buffersize: bytes  # data[30:32]
+    _voicemeeterVersion: bytes  # data[32:36]
+    _optionBits: bytes  # data[36:40]
+    _samplerate: bytes  # data[40:44]
+    _inputLeveldB100: bytes  # data[44:112]
+    _outputLeveldB100: bytes  # data[112:240]
+    _TransportBit: bytes  # data[240:244]
+    _stripState: bytes  # data[244:276]
+    _busState: bytes  # data[276:308]
+    _stripGaindB100Layer1: bytes  # data[308:324]
+    _stripGaindB100Layer2: bytes  # data[324:340]
+    _stripGaindB100Layer3: bytes  # data[340:356]
+    _stripGaindB100Layer4: bytes  # data[356:372]
+    _stripGaindB100Layer5: bytes  # data[372:388]
+    _stripGaindB100Layer6: bytes  # data[388:404]
+    _stripGaindB100Layer7: bytes  # data[404:420]
+    _stripGaindB100Layer8: bytes  # data[420:436]
+    _busGaindB100: bytes  # data[436:452]
+    _stripLabelUTF8c60: bytes  # data[452:932]
+    _busLabelUTF8c60: bytes  # data[932:1412]
 
     def _generate_levels(self, levelarray) -> tuple:
         return tuple(
             int.from_bytes(levelarray[i : i + 2], "little")
             for i in range(0, len(levelarray), 2)
         )
 
@@ -203,52 +207,81 @@
         return tuple(
             self._busLabelUTF8c60[i : i + 60].decode().split("\x00")[0]
             for i in range(0, 480, 60)
         )
 
 
 @dataclass
+class SubscribeHeader:
+    """Represents the header an RT Packet Service subscription packet"""
+
+    name = "Register RTP"
+    timeout = 15
+    vban: bytes = "VBAN".encode()
+    format_sr: bytes = (VBAN_PROTOCOL_SERVICE).to_bytes(1, "little")
+    format_nbs: bytes = (0).to_bytes(1, "little")
+    format_nbc: bytes = (VBAN_SERVICE_RTPACKETREGISTER).to_bytes(1, "little")
+    format_bit: bytes = (timeout & 0x000000FF).to_bytes(1, "little")  # timeout
+    streamname: bytes = name.encode("ascii") + bytes(16 - len(name))
+    framecounter: bytes = (0).to_bytes(4, "little")
+
+    @property
+    def header(self):
+        header = self.vban
+        header += self.format_sr
+        header += self.format_nbs
+        header += self.format_nbc
+        header += self.format_bit
+        header += self.streamname
+        header += self.framecounter
+        assert (
+            len(header) == HEADER_SIZE + 4
+        ), f"expected header size {HEADER_SIZE} bytes + 4 bytes framecounter ({HEADER_SIZE +4} bytes total)"
+        return header
+
+
+@dataclass
 class VbanRtPacketHeader:
-    """Represents the header of VBAN RT data packet"""
+    """Represents the header of a VBAN RT response packet"""
 
     name = "Voicemeeter-RTP"
     vban: bytes = "VBAN".encode()
-    format_sr: bytes = (0x60).to_bytes(1, "little")
+    format_sr: bytes = (VBAN_PROTOCOL_SERVICE).to_bytes(1, "little")
     format_nbs: bytes = (0).to_bytes(1, "little")
     format_nbc: bytes = (VBAN_SERVICE_RTPACKET).to_bytes(1, "little")
     format_bit: bytes = (0).to_bytes(1, "little")
     streamname: bytes = name.encode("ascii") + bytes(16 - len(name))
 
     @property
     def header(self):
         header = self.vban
         header += self.format_sr
         header += self.format_nbs
         header += self.format_nbc
         header += self.format_bit
         header += self.streamname
-        assert len(header) == HEADER_SIZE - 4, f"Header expected {HEADER_SIZE-4} bytes"
+        assert len(header) == HEADER_SIZE, f"expected header size {HEADER_SIZE} bytes"
         return header
 
 
 @dataclass
 class RequestHeader:
-    """Represents a REQUEST RT PACKET header"""
+    """Represents the header of an REQUEST RT PACKET"""
 
     name: str
     bps_index: int
     channel: int
     vban: bytes = "VBAN".encode()
     nbs: bytes = (0).to_bytes(1, "little")
     bit: bytes = (0x10).to_bytes(1, "little")
     framecounter: bytes = (0).to_bytes(4, "little")
 
     @property
     def sr(self):
-        return (0x40 + self.bps_index).to_bytes(1, "little")
+        return (VBAN_PROTOCOL_TXT + self.bps_index).to_bytes(1, "little")
 
     @property
     def nbc(self):
         return (self.channel).to_bytes(1, "little")
 
     @property
     def streamname(self):
@@ -259,36 +292,11 @@
         header = self.vban
         header += self.sr
         header += self.nbs
         header += self.nbc
         header += self.bit
         header += self.streamname
         header += self.framecounter
-        assert len(header) == HEADER_SIZE, f"Header expected {HEADER_SIZE} bytes"
-        return header
-
-
-@dataclass
-class SubscribeHeader:
-    """Represents a packet used to subscribe to the RT Packet Service"""
-
-    name = "Register RTP"
-    timeout = 15
-    vban: bytes = "VBAN".encode()
-    format_sr: bytes = (0x60).to_bytes(1, "little")
-    format_nbs: bytes = (0).to_bytes(1, "little")
-    format_nbc: bytes = (VBAN_SERVICE_RTPACKETREGISTER).to_bytes(1, "little")
-    format_bit: bytes = (timeout & 0x000000FF).to_bytes(1, "little")  # timeout
-    streamname: bytes = name.encode("ascii") + bytes(16 - len(name))
-    framecounter: bytes = (0).to_bytes(4, "little")
-
-    @property
-    def header(self):
-        header = self.vban
-        header += self.format_sr
-        header += self.format_nbs
-        header += self.format_nbc
-        header += self.format_bit
-        header += self.streamname
-        header += self.framecounter
-        assert len(header) == HEADER_SIZE, f"Header expected {HEADER_SIZE} bytes"
+        assert (
+            len(header) == HEADER_SIZE + 4
+        ), f"expected header size {HEADER_SIZE} bytes + 4 bytes framecounter ({HEADER_SIZE +4} bytes total)"
         return header
```

### Comparing `vban_cmd-2.4.1/vban_cmd/strip.py` & `vban_cmd-2.4.3/vban_cmd/strip.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,15 +292,15 @@
 
     def getter(self):
         """Returns a tuple of level values for the channel."""
 
         def fget(i):
             return round((((1 << 16) - 1) - i) * -0.01, 1)
 
-        if self._remote.running and self._remote.event.ldirty:
+        if not self._remote.stopped() and self._remote.event.ldirty:
             return tuple(
                 fget(i)
                 for i in self._remote.cache["strip_level"][
                     self.range[0] : self.range[-1]
                 ]
             )
         return tuple(
```

### Comparing `vban_cmd-2.4.1/vban_cmd/subject.py` & `vban_cmd-2.4.3/vban_cmd/subject.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.1/vban_cmd/util.py` & `vban_cmd-2.4.3/vban_cmd/util.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.1/vban_cmd/vban.py` & `vban_cmd-2.4.3/vban_cmd/vban.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.1/vban_cmd/vbancmd.py` & `vban_cmd-2.4.3/vban_cmd/vbancmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import socket
+import threading
 import time
 from abc import ABCMeta, abstractmethod
 from pathlib import Path
 from queue import Queue
 from typing import Iterable, Union
 
 from .error import VBANCMDError
@@ -84,32 +85,36 @@
     def __enter__(self):
         self.login()
         return self
 
     def login(self) -> None:
         """Starts the subscriber and updater threads (unless in outbound mode)"""
         if not self.outbound:
-            self.running = True
             self.event.info()
 
-            self.subscriber = Subscriber(self)
+            self.stop_event = threading.Event()
+            self.stop_event.clear()
+            self.subscriber = Subscriber(self, self.stop_event)
             self.subscriber.start()
 
             queue = Queue()
             self.updater = Updater(self, queue)
             self.updater.start()
-            self.producer = Producer(self, queue)
+            self.producer = Producer(self, queue, self.stop_event)
             self.producer.start()
 
         self.logger.info(
             "Successfully logged into VBANCMD {kind} with ip='{ip}', port={port}, streamname='{streamname}'".format(
                 **self.__dict__
             )
         )
 
+    def stopped(self):
+        return self.stop_event.is_set()
+
     def _set_rt(self, cmd: str, val: Union[str, float]):
         """Sends a string request command over a network."""
         self.socks[Socket.request].sendto(
             self.packet_request.header + f"{cmd}={val};".encode(),
             (socket.gethostbyname(self.ip), self.port),
         )
         self.packet_request.framecounter = (
@@ -209,14 +214,16 @@
             self.logger.debug(
                 f"profile '{name}' extends '{extended}', profiles merged.."
             )
         self.apply(config)
         self.logger.info(f"Profile '{name}' applied!")
 
     def logout(self) -> None:
-        self.running = False
-        time.sleep(0.2)
+        if not self.stopped():
+            self.logger.debug("events thread shutdown started")
+            self.stop_event.set()
+            self.subscriber.join()  # wait for subscriber thread to complete cycle
         [sock.close() for sock in self.socks]
         self.logger.info(f"{type(self).__name__}: Successfully logged out of {self}")
 
     def __exit__(self, exc_type, exc_value, exc_traceback) -> None:
         self.logout()
```

### Comparing `vban_cmd-2.4.1/vban_cmd/worker.py` & `vban_cmd-2.4.3/vban_cmd/worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,72 +10,88 @@
 
 logger = logging.getLogger(__name__)
 
 
 class Subscriber(threading.Thread):
     """fire a subscription packet every 10 seconds"""
 
-    def __init__(self, remote):
-        super().__init__(name="subscriber", daemon=True)
+    def __init__(self, remote, stop_event):
+        super().__init__(name="subscriber", daemon=False)
         self._remote = remote
+        self.stop_event = stop_event
         self.logger = logger.getChild(self.__class__.__name__)
         self.packet = SubscribeHeader()
 
     def run(self):
-        while self._remote.running:
+        while not self.stopped():
             try:
                 self._remote.socks[Socket.register].sendto(
                     self.packet.header,
                     (socket.gethostbyname(self._remote.ip), self._remote.port),
                 )
                 self.packet.framecounter = (
                     int.from_bytes(self.packet.framecounter, "little") + 1
                 ).to_bytes(4, "little")
-                time.sleep(10)
+                self.wait_until_stopped(10)
             except socket.gaierror as e:
                 self.logger.exception(f"{type(e).__name__}: {e}")
                 raise VBANCMDConnectionError(
                     f"unable to resolve hostname {self._remote.ip}"
                 ) from e
+        self.logger.debug(f"terminating {self.name} thread")
+
+    def stopped(self):
+        return self.stop_event.is_set()
+
+    def wait_until_stopped(self, timeout, period=0.2):
+        must_end = time.time() + timeout
+        while time.time() < must_end:
+            if self.stopped():
+                break
+            time.sleep(period)
 
 
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
         self.packet_expected = VbanRtPacketHeader()
+        self._remote.socks[Socket.response].settimeout(self._remote.timeout)
+        self._remote.socks[Socket.response].bind(
+            (socket.gethostbyname(socket.gethostname()), self._remote.port)
+        )
         self._remote._public_packet = self._get_rt()
         (
             self._remote.cache["strip_level"],
             self._remote.cache["bus_level"],
         ) = self._remote._get_levels(self._remote.public_packet)
 
     def _get_rt(self) -> VbanRtPacket:
         """Attempt to fetch data packet until a valid one found"""
 
         def fget():
             data = None
             while not data:
                 data = self._fetch_rt_packet()
-                time.sleep(self._remote.DELAY)
             return data
 
         return fget()
 
     def _fetch_rt_packet(self) -> Optional[VbanRtPacket]:
         try:
             data, _ = self._remote.socks[Socket.response].recvfrom(2048)
-            # check for packet data
+            # do we have packet data?
             if len(data) > HEADER_SIZE:
-                # check if packet is of type rt packet response
-                if self.packet_expected.header == data[: HEADER_SIZE - 4]:
+                # is the packet of type VBAN RT response?
+                if self.packet_expected.header == data[:HEADER_SIZE]:
                     return VbanRtPacket(
                         _kind=self._remote.kind,
                         _voicemeeterType=data[28:29],
                         _reserved=data[29:30],
                         _buffersize=data[30:32],
                         _voicemeeterVersion=data[32:36],
                         _optionBits=data[36:40],
@@ -99,16 +115,19 @@
                     )
         except TimeoutError as e:
             self.logger.exception(f"{type(e).__name__}: {e}")
             raise VBANCMDConnectionError(
                 f"timeout waiting for RtPacket from {self._remote.ip}"
             ) from e
 
+    def stopped(self):
+        return self.stop_event.is_set()
+
     def run(self):
-        while self._remote.running:
+        while not self.stopped():
             _pp = self._get_rt()
             pdirty = _pp.pdirty(self._remote.public_packet)
             ldirty = _pp.ldirty(
                 self._remote.cache["strip_level"], self._remote.cache["bus_level"]
             )
 
             if pdirty or ldirty:
@@ -133,33 +152,24 @@
     """
 
     def __init__(self, remote, queue):
         super().__init__(name="updater", daemon=True)
         self._remote = remote
         self.queue = queue
         self.logger = logger.getChild(self.__class__.__name__)
-        self._remote.socks[Socket.response].settimeout(self._remote.timeout)
-        self._remote.socks[Socket.response].bind(
-            (socket.gethostbyname(socket.gethostname()), self._remote.port)
-        )
         self._remote._strip_comp = [False] * (self._remote.kind.num_strip_levels)
         self._remote._bus_comp = [False] * (self._remote.kind.num_bus_levels)
 
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
             elif event == "ldirty" and self._remote.ldirty:
                 self._remote._strip_comp, self._remote._bus_comp = (
                     self._remote._public_packet._strip_comp,
                     self._remote._public_packet._bus_comp,
                 )
@@ -167,7 +177,8 @@
                     self._remote.cache["strip_level"],
                     self._remote.cache["bus_level"],
                 ) = (
                     self._remote._public_packet.inputlevels,
                     self._remote._public_packet.outputlevels,
                 )
                 self._remote.subject.notify(event)
+        self.logger.debug(f"terminating {self.name} thread")
```

### Comparing `vban_cmd-2.4.1/PKG-INFO` & `vban_cmd-2.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vban-cmd
-Version: 2.4.1
+Version: 2.4.3
 Summary: Python interface for the VBAN RT Packet Service (Sendtext)
 Home-page: https://github.com/onyx-and-iris/vban-cmd-python
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

