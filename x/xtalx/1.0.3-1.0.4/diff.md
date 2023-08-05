# Comparing `tmp/xtalx-1.0.3.tar.gz` & `tmp/xtalx-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtalx-1.0.3.tar", last modified: Wed Jun  7 20:32:24 2023, max compression
+gzip compressed data, was "xtalx-1.0.4.tar", last modified: Sat Aug  5 01:49:14 2023, max compression
```

## Comparing `xtalx-1.0.3.tar` & `xtalx-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,44 @@
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-06-07 20:32:24.937243 xtalx-1.0.3/
--rw-r--r--   0 greent7    (502) staff       (20)     1092 2023-06-05 20:34:21.000000 xtalx-1.0.3/LICENSE
--rw-r--r--   0 greent7    (502) staff       (20)     2685 2023-06-07 20:32:24.937316 xtalx-1.0.3/PKG-INFO
--rw-r--r--   0 greent7    (502) staff       (20)     2190 2023-06-05 20:34:21.000000 xtalx-1.0.3/README.rst
--rw-r--r--   0 greent7    (502) staff       (20)      782 2023-06-07 20:32:24.937591 xtalx-1.0.3/setup.cfg
--rw-r--r--   0 greent7    (502) staff       (20)       38 2023-06-05 20:34:21.000000 xtalx-1.0.3/setup.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-06-07 20:32:24.936155 xtalx-1.0.3/xtalx/
--rw-r--r--   0 greent7    (502) staff       (20)      222 2023-06-05 20:34:21.000000 xtalx-1.0.3/xtalx/__init__.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-06-07 20:32:24.937144 xtalx-1.0.3/xtalx/tools/
--rw-r--r--   0 greent7    (502) staff       (20)        0 2023-06-05 20:34:21.000000 xtalx-1.0.3/xtalx/tools/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)      498 2023-06-05 20:34:21.000000 xtalx-1.0.3/xtalx/tools/discover.py
--rw-r--r--   0 greent7    (502) staff       (20)     1265 2023-06-05 20:34:21.000000 xtalx-1.0.3/xtalx/tools/xtalx_test_read.py
--rw-r--r--   0 greent7    (502) staff       (20)     3024 2023-06-07 19:01:41.000000 xtalx-1.0.3/xtalx/tools/xtalx_test_yield.py
--rw-r--r--   0 greent7    (502) staff       (20)    13776 2023-06-05 20:56:37.000000 xtalx-1.0.3/xtalx/xtalx.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-06-07 20:32:24.936738 xtalx-1.0.3/xtalx.egg-info/
--rw-r--r--   0 greent7    (502) staff       (20)     2685 2023-06-07 20:32:24.000000 xtalx-1.0.3/xtalx.egg-info/PKG-INFO
--rw-r--r--   0 greent7    (502) staff       (20)      357 2023-06-07 20:32:24.000000 xtalx-1.0.3/xtalx.egg-info/SOURCES.txt
--rw-r--r--   0 greent7    (502) staff       (20)        1 2023-06-07 20:32:24.000000 xtalx-1.0.3/xtalx.egg-info/dependency_links.txt
--rw-r--r--   0 greent7    (502) staff       (20)      110 2023-06-07 20:32:24.000000 xtalx-1.0.3/xtalx.egg-info/entry_points.txt
--rw-r--r--   0 greent7    (502) staff       (20)       26 2023-06-07 20:32:24.000000 xtalx-1.0.3/xtalx.egg-info/requires.txt
--rw-r--r--   0 greent7    (502) staff       (20)        6 2023-06-07 20:32:24.000000 xtalx-1.0.3/xtalx.egg-info/top_level.txt
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-08-05 01:49:14.861281 xtalx-1.0.4/
+-rw-r--r--   0 greent7    (502) staff       (20)     1092 2023-07-27 00:41:10.000000 xtalx-1.0.4/LICENSE
+-rw-r--r--   0 greent7    (502) staff       (20)     2695 2023-08-05 01:49:14.861335 xtalx-1.0.4/PKG-INFO
+-rw-r--r--   0 greent7    (502) staff       (20)     2190 2023-07-27 00:41:10.000000 xtalx-1.0.4/README.rst
+-rw-r--r--   0 greent7    (502) staff       (20)     1138 2023-08-05 01:49:14.861573 xtalx-1.0.4/setup.cfg
+-rw-r--r--   0 greent7    (502) staff       (20)       38 2023-07-27 00:41:10.000000 xtalx-1.0.4/setup.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-08-05 01:49:14.857997 xtalx-1.0.4/xtalx/
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-08-05 01:49:14.859242 xtalx-1.0.4/xtalx/p_sensor/
+-rw-r--r--   0 greent7    (502) staff       (20)      718 2023-08-04 23:44:45.000000 xtalx-1.0.4/xtalx/p_sensor/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)      109 2023-08-04 23:44:45.000000 xtalx-1.0.4/xtalx/p_sensor/exception.py
+-rw-r--r--   0 greent7    (502) staff       (20)    12809 2023-08-04 23:44:45.000000 xtalx-1.0.4/xtalx/p_sensor/xti.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-08-05 01:49:14.857947 xtalx-1.0.4/xtalx/tools/
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-08-05 01:49:14.859429 xtalx-1.0.4/xtalx/tools/math/
+-rw-r--r--   0 greent7    (502) staff       (20)      160 2023-08-04 23:45:01.000000 xtalx-1.0.4/xtalx/tools/math/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1273 2023-08-04 23:45:01.000000 xtalx-1.0.4/xtalx/tools/math/lorentz.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-08-05 01:49:14.859811 xtalx-1.0.4/xtalx/tools/p_sensor/
+-rw-r--r--   0 greent7    (502) staff       (20)        0 2023-08-04 23:44:45.000000 xtalx-1.0.4/xtalx/tools/p_sensor/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)      520 2023-08-04 23:44:45.000000 xtalx-1.0.4/xtalx/tools/p_sensor/discover.py
+-rw-r--r--   0 greent7    (502) staff       (20)      789 2023-08-04 23:44:45.000000 xtalx-1.0.4/xtalx/tools/p_sensor/xtalx_test_read.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2687 2023-08-04 23:44:45.000000 xtalx-1.0.4/xtalx/tools/p_sensor/xtalx_test_yield.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-08-05 01:49:14.859912 xtalx-1.0.4/xtalx/tools/usb/
+-rw-r--r--   0 greent7    (502) staff       (20)      977 2023-08-04 23:59:51.000000 xtalx-1.0.4/xtalx/tools/usb/__init__.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-08-05 01:49:14.860446 xtalx-1.0.4/xtalx/tools/z_sensor/
+-rw-r--r--   0 greent7    (502) staff       (20)        0 2023-08-04 23:45:01.000000 xtalx-1.0.4/xtalx/tools/z_sensor/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)      476 2023-08-04 23:45:01.000000 xtalx-1.0.4/xtalx/tools/z_sensor/discover.py
+-rw-r--r--   0 greent7    (502) staff       (20)     3047 2023-08-04 23:45:01.000000 xtalx-1.0.4/xtalx/tools/z_sensor/get_info.py
+-rw-r--r--   0 greent7    (502) staff       (20)     5345 2023-08-04 23:45:01.000000 xtalx-1.0.4/xtalx/tools/z_sensor/gl_scope_mode.py
+-rw-r--r--   0 greent7    (502) staff       (20)     7231 2023-08-04 23:45:01.000000 xtalx-1.0.4/xtalx/tools/z_sensor/gl_sweep_mode.py
+-rw-r--r--   0 greent7    (502) staff       (20)    21560 2023-08-05 01:25:47.000000 xtalx-1.0.4/xtalx/tools/z_sensor/gl_track_mode.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-08-05 01:49:14.861188 xtalx-1.0.4/xtalx/z_sensor/
+-rw-r--r--   0 greent7    (502) staff       (20)      903 2023-08-04 23:45:01.000000 xtalx-1.0.4/xtalx/z_sensor/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     9412 2023-08-05 01:25:47.000000 xtalx-1.0.4/xtalx/z_sensor/peak_tracker.py
+-rw-r--r--   0 greent7    (502) staff       (20)      861 2023-08-04 23:45:01.000000 xtalx-1.0.4/xtalx/z_sensor/scope_data.py
+-rw-r--r--   0 greent7    (502) staff       (20)     3588 2023-08-04 23:45:01.000000 xtalx-1.0.4/xtalx/z_sensor/sweeper.py
+-rw-r--r--   0 greent7    (502) staff       (20)    21005 2023-08-05 01:33:57.000000 xtalx-1.0.4/xtalx/z_sensor/tcsc.py
+-rw-r--r--   0 greent7    (502) staff       (20)      205 2023-08-04 23:45:01.000000 xtalx-1.0.4/xtalx/z_sensor/tcsc_u5.py
+-rw-r--r--   0 greent7    (502) staff       (20)      701 2023-08-04 23:45:01.000000 xtalx-1.0.4/xtalx/z_sensor/tincan.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-08-05 01:49:14.858946 xtalx-1.0.4/xtalx.egg-info/
+-rw-r--r--   0 greent7    (502) staff       (20)     2695 2023-08-05 01:49:14.000000 xtalx-1.0.4/xtalx.egg-info/PKG-INFO
+-rw-r--r--   0 greent7    (502) staff       (20)      922 2023-08-05 01:49:14.000000 xtalx-1.0.4/xtalx.egg-info/SOURCES.txt
+-rw-r--r--   0 greent7    (502) staff       (20)        1 2023-08-05 01:49:14.000000 xtalx-1.0.4/xtalx.egg-info/dependency_links.txt
+-rw-r--r--   0 greent7    (502) staff       (20)      306 2023-08-05 01:49:14.000000 xtalx-1.0.4/xtalx.egg-info/entry_points.txt
+-rw-r--r--   0 greent7    (502) staff       (20)       78 2023-08-05 01:49:14.000000 xtalx-1.0.4/xtalx.egg-info/requires.txt
+-rw-r--r--   0 greent7    (502) staff       (20)        6 2023-08-05 01:49:14.000000 xtalx-1.0.4/xtalx.egg-info/top_level.txt
```

### Comparing `xtalx-1.0.3/LICENSE` & `xtalx-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xtalx-1.0.3/PKG-INFO` & `xtalx-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: xtalx
-Version: 1.0.3
-Summary: Python library for the XtalX sensor.
+Version: 1.0.4
+Summary: Drivers and tools for the XtalX sensor family.
 Home-page: https://github.com/phasesensors/xtalx_python
 Author: Phase Advanced Sensor Systems Corp.
 Author-email: tgreeniaus@phasesensors.com
 License: MIT
 Keywords: xtalx
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `xtalx-1.0.3/README.rst` & `xtalx-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `xtalx-1.0.3/xtalx/tools/xtalx_test_read.py` & `xtalx-1.0.4/xtalx/tools/p_sensor/xtalx_test_read.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,27 @@
 #!/usr/bin/env python3
-# Copyright (c) 2020-2021 by Phase Advanced Sensor Systems Corp.
+# Copyright (c) 2020-2023 by Phase Advanced Sensor Systems Corp.
 import argparse
 
-import xtalx
+import xtalx.p_sensor
 
 
 VERBOSE = False
 
 
 def xtalx_cb(m):
     print(m.tostring(VERBOSE))
 
 
 def main(args):
     global VERBOSE
     VERBOSE = args.verbose
 
-    if args.serial_number is not None:
-        sensors = xtalx.find(serial_number=args.serial_number)
-        if not sensors:
-            print('No matching sensors.')
-            for s in xtalx.find():
-                print('    %s' % s.serial_number)
-            return
-    else:
-        sensors = xtalx.find()
-        if not sensors:
-            print('No sensors found.')
-            return
-    if len(sensors) != 1:
-        print('Matching sensors:')
-        for s in sensors:
-            print('    %s' % s.serial_number)
-        return
-    d = sensors[0]
-
-    x = xtalx.XtalX(d)
+    d = xtalx.p_sensor.find_one_xti(serial_number=args.serial_number)
+    x = xtalx.p_sensor.make(d)
     x.read_measurements(xtalx_cb)
     try:
         x.join_read()
     except KeyboardInterrupt:
         x.halt_read()
         raise
```

### Comparing `xtalx-1.0.3/xtalx/tools/xtalx_test_yield.py` & `xtalx-1.0.4/xtalx/tools/p_sensor/xtalx_test_yield.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
-# Copyright (c) 2020-2021 by Phase Advanced Sensor Systems Corp.
+# Copyright (c) 2020-2023 by Phase Advanced Sensor Systems Corp.
 import argparse
 import time
+import math
 
-import xtalx
+import xtalx.p_sensor
 
 
 def print_measurement(x, temp_c, pressure_psi):
     if pressure_psi is None:
         p = 'n/a'
     else:
         p = '%f' % pressure_psi
@@ -19,14 +20,18 @@
 
     print('%s: %s C, %s PSI' % (x, t, p))
 
 
 def xtalx_cb(x, t, dt, temp_c, pressure_psi, csv_file):
     print_measurement(x, temp_c, pressure_psi)
     if csv_file:
+        if temp_c is None:
+            temp_c = math.nan
+        if pressure_psi is None:
+            pressure_psi = math.nan
         csv_file.write('%.6f,%.6f,%.2f,%.5f\n' % (t, dt, temp_c, pressure_psi))
         csv_file.flush()
 
 
 def sample_gated(x, csv_file, sample_period):
     measurements   = []
     t0 = t0_period = time.time()
@@ -50,32 +55,15 @@
     t0 = time.time()
     for m in x.yield_measurements():
         t = time.time()
         xtalx_cb(x, t, t - t0, m.temp_c, m.pressure_psi, csv_file)
 
 
 def main(args):
-    if args.serial_number is not None:
-        sensors = xtalx.find(serial_number=args.serial_number)
-        if not sensors:
-            print('No matching sensors.')
-            for s in xtalx.find():
-                print('    %s' % s.serial_number)
-            return
-    else:
-        sensors = xtalx.find()
-        if not sensors:
-            print('No sensors found.')
-            return
-    if len(sensors) != 1:
-        print('Matching sensors:')
-        for s in sensors:
-            print('    %s' % s.serial_number)
-        return
-    d = sensors[0]
+    d = xtalx.p_sensor.find_one_xti(serial_number=args.serial_number)
 
     if args.csv_file:
         csv_file = open(  # pylint: disable=R1732
             args.csv_file, 'a+', encoding='utf8')
 
         pos = csv_file.tell()
         if pos != 0:
@@ -87,15 +75,15 @@
             csv_file.seek(pos)
         else:
             csv_file.write('time,dt,temp_c,pressure_psi\n')
             csv_file.flush()
     else:
         csv_file = None
 
-    x = xtalx.XtalX(d)
+    x = xtalx.p_sensor.make(d)
     if args.sample_period:
         sample_gated(x, csv_file, args.sample_period)
     else:
         sample_continuous(x, csv_file)
 
 
 def _main():
```

### Comparing `xtalx-1.0.3/xtalx/xtalx.py` & `xtalx-1.0.4/xtalx/p_sensor/xti.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-# Copyright (c) 2020-2021 by Phase Advanced Sensor Systems Corp.
+# Copyright (c) 2020-2023 by Phase Advanced Sensor Systems Corp.
 import threading
 import errno
 import usb
 import usb.util
 
 import btype
 
+from .exception import XtalXException
+
 
 FC_FLAGS_VALID              = (1 << 15)
 FC_FLAG_NO_TEMP_PRESSURE    = (1 << 4)
 FC_FLAG_PRESSURE_FAILED     = (1 << 3)
 FC_FLAG_TEMP_FAILED         = (1 << 2)
 FC_FLAG_PRESSURE_UPDATE     = (1 << 1)
 FC_FLAG_TEMP_UPDATE         = (1 << 0)
@@ -71,18 +73,18 @@
     mcu_temp_c          = btype.float64_t()
     rsrv2               = btype.Array(btype.uint8_t(), 8)
     _EXPECTED_SIZE      = 56
 
 
 class Measurement:
     '''
-    Object encapsulating the results of an XtalX sensor measurement.  The
+    Object encapsulating the results of an XTI sensor measurement.  The
     following fields are defined:
 
-        sensor - Reference to the XtalX that generated the Measurement.
+        sensor - Reference to the XTI that generated the Measurement.
         ref_freq - Frequency of the sensor's reference crystal.
         pressure_edges - Number of pressure crystal ticks used to generate the
             Measurement.
         pressure_ref_clocks - Number of reference clock ticks that elapsed
             while counting pressure_edges pressure crystal ticks.
         pressure_freq - Measured pressure crystal frequency.
         temp_edges - Number of temperature crystal ticks used to generate the
@@ -195,22 +197,18 @@
             else:
                 t = '%f' % self.temp_c
             s += '%s PSI, %s C' % (p, t)
 
         return s
 
 
-class XtalXException(Exception):
-    pass
-
-
-class XtalX:
+class XTI:
     '''
     Given a USB device handle acquired via find() or find_one(), creates an
-    XtalX object that can be used to communicate with a sensor.
+    XTI object that can be used to communicate with a sensor.
     '''
     def __init__(self, usb_dev):
         self.usb_dev     = usb_dev
         self.lock        = threading.RLock()
         self._halt_yield = True
         self.thread      = None
 
@@ -231,15 +229,15 @@
         else:
             self.report_id = None
 
         self.usb_path = '%s:%s' % (
             usb_dev.bus, '.'.join('%u' % n for n in usb_dev.port_numbers))
 
     def __str__(self):
-        return 'XtalX(%s)' % self.serial_num
+        return 'XTI(%s)' % self.serial_num
 
     def _set_configuration(self, bConfigurationValue):
         with self.lock:
             cfg = None
             try:
                 cfg = self.usb_dev.get_active_configuration()
             except usb.core.USBError as e:
@@ -312,44 +310,18 @@
             self.thread.start()
 
     def join_read(self):
         '''
         Blocks the current thread until the asynchronous read thread completes.
         Typically this blocks indefinitely until some error occurs, however the
         read thread will also exit if someone sets the _halt_yield field to
-        True (see XtalX.halt_read()).
+        True (see XTI.halt_read()).
         '''
         self.thread.join()
 
     def halt_read(self):
         '''
         Halts any asynchronous measurement thread and waits for it to finish
         cleanly.
         '''
         self._halt_yield = True
         self.join_read()
-
-
-def find(**kwargs):
-    '''
-    Returns a list of USB device handles for all XtalX sensors.  **kwargs can
-    be any keyword argument accepted by usb.core.find(); typically you will
-    leave it empty.
-    '''
-    return list(usb.core.find(find_all=True, idVendor=0x0483, idProduct=0xA34E,
-                              product='XtalX', **kwargs))
-
-
-def find_one(**kwargs):
-    '''
-    Returns a single USB device handle for an XtalX sensor if only a single
-    sensor is attached.  If multiple sensors are found, an exception is raised.
-    **kwargs can be any keyword argument accepted by usb.core.find(); typically
-    you will leave it empty.
-    '''
-    usb_devs = find(**kwargs)
-    if len(usb_devs) > 1:
-        raise XtalXException('Multiple matching devices: %s' %
-                             ', '.join(ud.serial_number for ud in usb_devs))
-    if not usb_devs:
-        raise XtalXException('No matching devices.')
-    return usb_devs[0]
```

### Comparing `xtalx-1.0.3/xtalx.egg-info/PKG-INFO` & `xtalx-1.0.4/xtalx.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: xtalx
-Version: 1.0.3
-Summary: Python library for the XtalX sensor.
+Version: 1.0.4
+Summary: Drivers and tools for the XtalX sensor family.
 Home-page: https://github.com/phasesensors/xtalx_python
 Author: Phase Advanced Sensor Systems Corp.
 Author-email: tgreeniaus@phasesensors.com
 License: MIT
 Keywords: xtalx
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

