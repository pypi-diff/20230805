# Comparing `tmp/vdaq_soap-1.0.4.tar.gz` & `tmp/vdaq_soap-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdaq_soap-1.0.4.tar", last modified: Thu Aug  3 15:36:58 2023, max compression
+gzip compressed data, was "vdaq_soap-1.0.5.tar", last modified: Sat Aug  5 08:22:04 2023, max compression
```

## Comparing `vdaq_soap-1.0.4.tar` & `vdaq_soap-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-08-03 15:36:58.991579 vdaq_soap-1.0.4/
--rw-r--r--   0 lacasta    (503) staff       (20)      839 2023-08-03 15:36:58.991101 vdaq_soap-1.0.4/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      408 2023-05-12 07:04:30.000000 vdaq_soap-1.0.4/README.md
--rw-r--r--   0 lacasta    (503) staff       (20)      957 2023-08-03 15:34:12.000000 vdaq_soap-1.0.4/pyproject.toml
--rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-08-03 15:36:58.991698 vdaq_soap-1.0.4/setup.cfg
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-08-03 15:36:58.987291 vdaq_soap-1.0.4/vdaq_soap/
--rw-r--r--   0 lacasta    (503) staff       (20)      334 2023-08-03 15:34:12.000000 vdaq_soap-1.0.4/vdaq_soap/__init__.py
--rw-r--r--   0 lacasta    (503) staff       (20)     3237 2023-05-11 20:13:13.000000 vdaq_soap-1.0.4/vdaq_soap/analyzeHoldDelay.py
--rw-r--r--   0 lacasta    (503) staff       (20)     4779 2023-05-11 20:06:02.000000 vdaq_soap-1.0.4/vdaq_soap/analyzeMbias.py
--rw-r--r--   0 lacasta    (503) staff       (20)     1645 2023-05-11 17:14:59.000000 vdaq_soap-1.0.4/vdaq_soap/data_utils.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)    25156 2023-05-12 06:55:29.000000 vdaq_soap-1.0.4/vdaq_soap/soapCheckMadDaq.py
--rw-r--r--   0 lacasta    (503) staff       (20)     3028 2023-08-03 11:21:38.000000 vdaq_soap-1.0.4/vdaq_soap/soapHoldDelay.py
--rw-r--r--   0 lacasta    (503) staff       (20)     3121 2023-08-03 11:22:53.000000 vdaq_soap-1.0.4/vdaq_soap/soapMbias.py
--rw-r--r--   0 lacasta    (503) staff       (20)     3153 2023-08-03 11:23:40.000000 vdaq_soap-1.0.4/vdaq_soap/soapTestChannel.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-08-03 15:36:58.990235 vdaq_soap-1.0.4/vdaq_soap.egg-info/
--rw-r--r--   0 lacasta    (503) staff       (20)      839 2023-08-03 15:36:58.000000 vdaq_soap-1.0.4/vdaq_soap.egg-info/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      434 2023-08-03 15:36:58.000000 vdaq_soap-1.0.4/vdaq_soap.egg-info/SOURCES.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-08-03 15:36:58.000000 vdaq_soap-1.0.4/vdaq_soap.egg-info/dependency_links.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      264 2023-08-03 15:36:58.000000 vdaq_soap-1.0.4/vdaq_soap.egg-info/entry_points.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       92 2023-08-03 15:36:58.000000 vdaq_soap-1.0.4/vdaq_soap.egg-info/requires.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       10 2023-08-03 15:36:58.000000 vdaq_soap-1.0.4/vdaq_soap.egg-info/top_level.txt
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-08-05 08:22:04.171962 vdaq_soap-1.0.5/
+-rw-r--r--   0 lacasta    (503) staff       (20)      839 2023-08-05 08:22:04.171624 vdaq_soap-1.0.5/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)      408 2023-05-12 07:04:30.000000 vdaq_soap-1.0.5/README.md
+-rw-r--r--   0 lacasta    (503) staff       (20)      957 2023-08-04 18:32:58.000000 vdaq_soap-1.0.5/pyproject.toml
+-rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-08-05 08:22:04.172034 vdaq_soap-1.0.5/setup.cfg
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-08-05 08:22:04.168053 vdaq_soap-1.0.5/vdaq_soap/
+-rw-r--r--   0 lacasta    (503) staff       (20)      334 2023-08-04 18:33:25.000000 vdaq_soap-1.0.5/vdaq_soap/__init__.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     3237 2023-05-11 20:13:13.000000 vdaq_soap-1.0.5/vdaq_soap/analyzeHoldDelay.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     4779 2023-05-11 20:06:02.000000 vdaq_soap-1.0.5/vdaq_soap/analyzeMbias.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     1645 2023-05-11 17:14:59.000000 vdaq_soap-1.0.5/vdaq_soap/data_utils.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)    25172 2023-08-04 18:33:24.000000 vdaq_soap-1.0.5/vdaq_soap/soapCheckMadDaq.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     3028 2023-08-03 11:21:38.000000 vdaq_soap-1.0.5/vdaq_soap/soapHoldDelay.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     3121 2023-08-03 11:22:53.000000 vdaq_soap-1.0.5/vdaq_soap/soapMbias.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     3153 2023-08-03 11:23:40.000000 vdaq_soap-1.0.5/vdaq_soap/soapTestChannel.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-08-05 08:22:04.171175 vdaq_soap-1.0.5/vdaq_soap.egg-info/
+-rw-r--r--   0 lacasta    (503) staff       (20)      839 2023-08-05 08:22:04.000000 vdaq_soap-1.0.5/vdaq_soap.egg-info/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)      434 2023-08-05 08:22:04.000000 vdaq_soap-1.0.5/vdaq_soap.egg-info/SOURCES.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-08-05 08:22:04.000000 vdaq_soap-1.0.5/vdaq_soap.egg-info/dependency_links.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)      264 2023-08-05 08:22:04.000000 vdaq_soap-1.0.5/vdaq_soap.egg-info/entry_points.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       92 2023-08-05 08:22:04.000000 vdaq_soap-1.0.5/vdaq_soap.egg-info/requires.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       10 2023-08-05 08:22:04.000000 vdaq_soap-1.0.5/vdaq_soap.egg-info/top_level.txt
```

### Comparing `vdaq_soap-1.0.4/PKG-INFO` & `vdaq_soap-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdaq_soap
-Version: 1.0.4
+Version: 1.0.5
 Summary: A collection of python scripts to control VDaq.
 Author-email: Carlos Lacasta <carlos.lacasta@alibavasystems.com>
 Project-URL: Homepage, https://igit.ific.uv.es
 Project-URL: Bug Tracker, https://igit.ific.uv.es
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `vdaq_soap-1.0.4/pyproject.toml` & `vdaq_soap-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vdaq_soap"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Carlos Lacasta", email="carlos.lacasta@alibavasystems.com" },
 ]
 description = "A collection of python scripts to control VDaq."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `vdaq_soap-1.0.4/vdaq_soap/analyzeHoldDelay.py` & `vdaq_soap-1.0.5/vdaq_soap/analyzeHoldDelay.py`

 * *Files identical despite different names*

### Comparing `vdaq_soap-1.0.4/vdaq_soap/analyzeMbias.py` & `vdaq_soap-1.0.5/vdaq_soap/analyzeMbias.py`

 * *Files identical despite different names*

### Comparing `vdaq_soap-1.0.4/vdaq_soap/data_utils.py` & `vdaq_soap-1.0.5/vdaq_soap/data_utils.py`

 * *Files identical despite different names*

### Comparing `vdaq_soap-1.0.4/vdaq_soap/soapCheckMadDaq.py` & `vdaq_soap-1.0.5/vdaq_soap/soapCheckMadDaq.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,15 @@
 
     # Reset all monitor data
     the_module.resetMonitorData()
 
     # Now we make the pedestal run
     if save_data:
         ofile = pathlib.Path.cwd().joinpath("pedestal_{}.h5".format(the_module.name))
-        run_manager.parameters['command'].set_value(
+        run_manager.getParameter("command").set_value(
             "logData|file={}".format(ofile))
 
     run_manager.setMaxEvents(10000)
     run_manager.startRun()
     wait_for_end_of_run(run_manager, 5.0)
 
     # Get the data and plot
@@ -293,22 +293,22 @@
     # Recompute scan range
     step = math.floor((last-first)/(npts-1))
     last = first + (npts-1) * step
     if last > 255:
         last -= step
 
     # Define the scan
-    run_manager.parameters['command'].set_value(
+    run_manager.getParameter("command").set_value(
         "scan|nevt={}:is_time=true:points=(1,1,0,0);(0,1,{},{});(11,{},{},{})".format(
             nsec, chan, chan, npts, first, last)
     )
 
     # Set the output file
     ofile = pathlib.Path.cwd().joinpath("hold_delay_{}.h5".format(the_module.name))
-    run_manager.parameters['command'].set_value(
+    run_manager.getParameter("command").set_value(
         "logData|file={}".format(ofile))
 
     # Start the run
     run_manager.startRun()
     wait_for_end_of_run(run_manager)
     time.sleep(0.5)
 
@@ -357,22 +357,22 @@
             nchan = 1
         step = 1
         last_chan = first_chan
 
     print("New scan range: {} {}-{} [{}]".format(nchan, first_chan, last_chan, step))
 
     # Define the scan
-    run_manager.parameters['command'].set_value(
+    run_manager.getParameter("command").set_value(
         "scan|nevt={}:is_time=false:points=(1,1,0,0);(0,{},{},{})".format(
             nevts, nchan, first_chan, last_chan)
     )
 
     # Set the output file
     ofile = pathlib.Path.cwd().joinpath("channel_scan_{}.h5".format(the_module.name))
-    run_manager.parameters['command'].set_value(
+    run_manager.getParameter("command").set_value(
         "logData|file={}".format(ofile))
 
     run_manager.startRun()
     wait_for_end_of_run(run_manager)
     run_status = run_manager.getStatus()
 
     # Get the data and check the hitmap.
@@ -429,15 +429,15 @@
     """
     # do a channel scan for this
     ofile = pathlib.Path.cwd().joinpath("channel_TDC_{}.h5".format(the_module.name))
     server.createRunManager("data", "main")
     run_manager = daqpp.soap.RunManager("main", server)
     set_module_param(run_manager, "channel", channel)
     run_manager.GetReady()
-    run_manager.parameters['command'].set_value("logData|file={}".format(ofile))
+    run_manager.getParameter("command").set_value("logData|file={}".format(ofile))
     # Reset all monitor data
     the_module.resetMonitorData()
 
     # Take data
     run_manager.startRun()
     wait_for_end_of_run(run_manager, nsec)
     status = run_manager.getStatus()
@@ -618,22 +618,22 @@
     if nchan > 1:
         step = math.floor((last_chan-first_chan)/(nchan-1))
         last_chan = first_chan + (nchan-1) * step
     else:
         last_chan = first_chan
 
     # Define the scan
-    run_manager.parameters['command'].set_value(
+    run_manager.getParameter("command").set_value(
         "scan|nevt={}:is_time=true:points=(1,1,0,0);(0,{},{},{});(4,{},{},{})".format(
             nsec, nchan, first_chan, last_chan, npts, first, last)
     )
 
     # Set the output file name
     ofile = pathlib.Path.cwd().joinpath("mbias_{}.h5".format(the_module.name))
-    run_manager.parameters['command'].set_value("logData|file={}".format(ofile))
+    run_manager.getParameter("command").set_value("logData|file={}".format(ofile))
 
     # start the run
     run_manager.startRun()
     wait_for_end_of_run(run_manager)
 
     # Wait to have data file closed
     time.sleep(0.5)
```

### Comparing `vdaq_soap-1.0.4/vdaq_soap/soapHoldDelay.py` & `vdaq_soap-1.0.5/vdaq_soap/soapHoldDelay.py`

 * *Files identical despite different names*

### Comparing `vdaq_soap-1.0.4/vdaq_soap/soapMbias.py` & `vdaq_soap-1.0.5/vdaq_soap/soapMbias.py`

 * *Files identical despite different names*

### Comparing `vdaq_soap-1.0.4/vdaq_soap/soapTestChannel.py` & `vdaq_soap-1.0.5/vdaq_soap/soapTestChannel.py`

 * *Files identical despite different names*

### Comparing `vdaq_soap-1.0.4/vdaq_soap.egg-info/PKG-INFO` & `vdaq_soap-1.0.5/vdaq_soap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdaq-soap
-Version: 1.0.4
+Version: 1.0.5
 Summary: A collection of python scripts to control VDaq.
 Author-email: Carlos Lacasta <carlos.lacasta@alibavasystems.com>
 Project-URL: Homepage, https://igit.ific.uv.es
 Project-URL: Bug Tracker, https://igit.ific.uv.es
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

