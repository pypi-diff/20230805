# Comparing `tmp/rucio-consistency-1.3.0.tar.gz` & `tmp/rucio-consistency-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio-consistency-1.3.0.tar", last modified: Thu Aug  3 14:02:42 2023, max compression
+gzip compressed data, was "rucio-consistency-1.4.0.tar", last modified: Sat Aug  5 15:44:53 2023, max compression
```

## Comparing `rucio-consistency-1.3.0.tar` & `rucio-consistency-1.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-08-03 14:02:42.218605 rucio-consistency-1.3.0/
--rw-r--r--   0 ivm        (503) staff       (20)    11357 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/LICENSE
--rw-r--r--   0 ivm        (503) staff       (20)      350 2023-08-03 14:02:42.218277 rucio-consistency-1.3.0/PKG-INFO
--rw-r--r--   0 ivm        (503) staff       (20)    12399 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/README.rst
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-08-03 14:02:42.210999 rucio-consistency-1.3.0/rucio_consistency/
--rw-r--r--   0 ivm        (503) staff       (20)      378 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/__init__.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     4635 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/cmplib.py
--rw-r--r--   0 ivm        (503) staff       (20)    11469 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/config.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     5417 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/part.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      372 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/py3.py
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-08-03 14:02:42.216381 rucio-consistency-1.3.0/rucio_consistency/scripts/
--rwxr-xr-x   0 ivm        (503) staff       (20)     3532 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/scripts/cmp2.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     3596 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/scripts/cmp3.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     4317 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/scripts/cmp5.py
--rwxr-xr-x   0 ivm        (503) staff       (20)    10323 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/scripts/db_dump.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     2737 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/scripts/partition.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     1069 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/scripts/update_stats.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     2523 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/stats.py
--rw-r--r--   0 ivm        (503) staff       (20)      125 2023-08-03 14:02:11.000000 rucio-consistency-1.3.0/rucio_consistency/version.py
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-08-03 14:02:42.217788 rucio-consistency-1.3.0/rucio_consistency/xrootd/
--rw-r--r--   0 ivm        (503) staff       (20)       39 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/xrootd/__init__.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     9449 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/rucio_consistency/xrootd/xrootd_client.py
--rwxr-xr-x   0 ivm        (503) staff       (20)    27819 2023-08-03 14:02:11.000000 rucio-consistency-1.3.0/rucio_consistency/xrootd/xrootd_scanner.py
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-08-03 14:02:42.213330 rucio-consistency-1.3.0/rucio_consistency.egg-info/
--rw-r--r--   0 ivm        (503) staff       (20)      350 2023-08-03 14:02:42.000000 rucio-consistency-1.3.0/rucio_consistency.egg-info/PKG-INFO
--rw-r--r--   0 ivm        (503) staff       (20)      850 2023-08-03 14:02:42.000000 rucio-consistency-1.3.0/rucio_consistency.egg-info/SOURCES.txt
--rw-r--r--   0 ivm        (503) staff       (20)        1 2023-08-03 14:02:42.000000 rucio-consistency-1.3.0/rucio_consistency.egg-info/dependency_links.txt
--rw-r--r--   0 ivm        (503) staff       (20)      388 2023-08-03 14:02:42.000000 rucio-consistency-1.3.0/rucio_consistency.egg-info/entry_points.txt
--rw-r--r--   0 ivm        (503) staff       (20)        1 2023-08-03 14:02:42.000000 rucio-consistency-1.3.0/rucio_consistency.egg-info/not-zip-safe
--rw-r--r--   0 ivm        (503) staff       (20)       22 2023-08-03 14:02:42.000000 rucio-consistency-1.3.0/rucio_consistency.egg-info/requires.txt
--rw-r--r--   0 ivm        (503) staff       (20)       18 2023-08-03 14:02:42.000000 rucio-consistency-1.3.0/rucio_consistency.egg-info/top_level.txt
--rw-r--r--   0 ivm        (503) staff       (20)       38 2023-08-03 14:02:42.218901 rucio-consistency-1.3.0/setup.cfg
--rw-r--r--   0 ivm        (503) staff       (20)     1391 2023-06-27 13:17:59.000000 rucio-consistency-1.3.0/setup.py
+drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-08-05 15:44:53.243804 rucio-consistency-1.4.0/
+-rw-r--r--   0 ivm        (503) staff       (20)    11357 2023-06-27 13:17:59.000000 rucio-consistency-1.4.0/LICENSE
+-rw-r--r--   0 ivm        (503) staff       (20)      350 2023-08-05 15:44:53.243111 rucio-consistency-1.4.0/PKG-INFO
+-rw-r--r--   0 ivm        (503) staff       (20)    12399 2023-06-27 13:17:59.000000 rucio-consistency-1.4.0/README.rst
+drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-08-05 15:44:53.236547 rucio-consistency-1.4.0/rucio_consistency/
+-rw-r--r--   0 ivm        (503) staff       (20)      378 2023-06-27 13:17:59.000000 rucio-consistency-1.4.0/rucio_consistency/__init__.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     4635 2023-06-27 13:17:59.000000 rucio-consistency-1.4.0/rucio_consistency/cmplib.py
+-rw-r--r--   0 ivm        (503) staff       (20)    11469 2023-06-27 13:17:59.000000 rucio-consistency-1.4.0/rucio_consistency/config.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     5417 2023-06-27 13:17:59.000000 rucio-consistency-1.4.0/rucio_consistency/part.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      372 2023-06-27 13:17:59.000000 rucio-consistency-1.4.0/rucio_consistency/py3.py
+drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-08-05 15:44:53.241212 rucio-consistency-1.4.0/rucio_consistency/scripts/
+-rwxr-xr-x   0 ivm        (503) staff       (20)     3532 2023-06-27 13:17:59.000000 rucio-consistency-1.4.0/rucio_consistency/scripts/cmp2.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     3596 2023-06-27 13:17:59.000000 rucio-consistency-1.4.0/rucio_consistency/scripts/cmp3.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     4317 2023-06-27 13:17:59.000000 rucio-consistency-1.4.0/rucio_consistency/scripts/cmp5.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)    10323 2023-06-27 13:17:59.000000 rucio-consistency-1.4.0/rucio_consistency/scripts/db_dump.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     2737 2023-06-27 13:17:59.000000 rucio-consistency-1.4.0/rucio_consistency/scripts/partition.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     1069 2023-06-27 13:17:59.000000 rucio-consistency-1.4.0/rucio_consistency/scripts/update_stats.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     2523 2023-06-27 13:17:59.000000 rucio-consistency-1.4.0/rucio_consistency/stats.py
+-rw-r--r--   0 ivm        (503) staff       (20)      125 2023-08-05 15:44:50.000000 rucio-consistency-1.4.0/rucio_consistency/version.py
+drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-08-05 15:44:53.242327 rucio-consistency-1.4.0/rucio_consistency/xrootd/
+-rw-r--r--   0 ivm        (503) staff       (20)       39 2023-06-27 13:17:59.000000 rucio-consistency-1.4.0/rucio_consistency/xrootd/__init__.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     9449 2023-06-27 13:17:59.000000 rucio-consistency-1.4.0/rucio_consistency/xrootd/xrootd_client.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)    29116 2023-08-05 15:41:35.000000 rucio-consistency-1.4.0/rucio_consistency/xrootd/xrootd_scanner.py
+drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-08-05 15:44:53.239058 rucio-consistency-1.4.0/rucio_consistency.egg-info/
+-rw-r--r--   0 ivm        (503) staff       (20)      350 2023-08-05 15:44:53.000000 rucio-consistency-1.4.0/rucio_consistency.egg-info/PKG-INFO
+-rw-r--r--   0 ivm        (503) staff       (20)      850 2023-08-05 15:44:53.000000 rucio-consistency-1.4.0/rucio_consistency.egg-info/SOURCES.txt
+-rw-r--r--   0 ivm        (503) staff       (20)        1 2023-08-05 15:44:53.000000 rucio-consistency-1.4.0/rucio_consistency.egg-info/dependency_links.txt
+-rw-r--r--   0 ivm        (503) staff       (20)      388 2023-08-05 15:44:53.000000 rucio-consistency-1.4.0/rucio_consistency.egg-info/entry_points.txt
+-rw-r--r--   0 ivm        (503) staff       (20)        1 2023-08-05 15:44:53.000000 rucio-consistency-1.4.0/rucio_consistency.egg-info/not-zip-safe
+-rw-r--r--   0 ivm        (503) staff       (20)       22 2023-08-05 15:44:53.000000 rucio-consistency-1.4.0/rucio_consistency.egg-info/requires.txt
+-rw-r--r--   0 ivm        (503) staff       (20)       18 2023-08-05 15:44:53.000000 rucio-consistency-1.4.0/rucio_consistency.egg-info/top_level.txt
+-rw-r--r--   0 ivm        (503) staff       (20)       38 2023-08-05 15:44:53.244310 rucio-consistency-1.4.0/setup.cfg
+-rw-r--r--   0 ivm        (503) staff       (20)     1391 2023-06-27 13:17:59.000000 rucio-consistency-1.4.0/setup.py
```

### Comparing `rucio-consistency-1.3.0/LICENSE` & `rucio-consistency-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.3.0/README.rst` & `rucio-consistency-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.3.0/rucio_consistency/cmplib.py` & `rucio-consistency-1.4.0/rucio_consistency/cmplib.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.3.0/rucio_consistency/config.py` & `rucio-consistency-1.4.0/rucio_consistency/config.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.3.0/rucio_consistency/part.py` & `rucio-consistency-1.4.0/rucio_consistency/part.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.3.0/rucio_consistency/scripts/cmp2.py` & `rucio-consistency-1.4.0/rucio_consistency/scripts/cmp2.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.3.0/rucio_consistency/scripts/cmp3.py` & `rucio-consistency-1.4.0/rucio_consistency/scripts/cmp3.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.3.0/rucio_consistency/scripts/cmp5.py` & `rucio-consistency-1.4.0/rucio_consistency/scripts/cmp5.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.3.0/rucio_consistency/scripts/db_dump.py` & `rucio-consistency-1.4.0/rucio_consistency/scripts/db_dump.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.3.0/rucio_consistency/scripts/partition.py` & `rucio-consistency-1.4.0/rucio_consistency/scripts/partition.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.3.0/rucio_consistency/scripts/update_stats.py` & `rucio-consistency-1.4.0/rucio_consistency/scripts/update_stats.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.3.0/rucio_consistency/stats.py` & `rucio-consistency-1.4.0/rucio_consistency/stats.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.3.0/rucio_consistency/xrootd/xrootd_client.py` & `rucio-consistency-1.4.0/rucio_consistency/xrootd/xrootd_client.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.3.0/rucio_consistency/xrootd/xrootd_scanner.py` & `rucio-consistency-1.4.0/rucio_consistency/xrootd/xrootd_scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pythreader import TaskQueue, Task, DEQueue, PyThread, synchronized, ShellCommand, Primitive
 import re, json, os, os.path, traceback, sys
 import subprocess, time, random, gzip
+from datetime import datetime, timezone
 
 from rucio_consistency import to_str, Stats, PartitionedList, ScannerConfiguration
 from rucio_consistency.xrootd import XRootDClient
 
 Version = "4.0"
 
 GB = 1024*1024*1024
@@ -222,16 +223,18 @@
             self.Master.scanner_succeeded(self, location, self.WasRecursive, files, dirs, empty_dir_count, empty_dirs)
 
 class ScannerMaster(PyThread):
     
     MAX_RECURSION_FAILED_COUNT = 5
     REPORT_INTERVAL = 10.0
     RESULTS_BUFFER_SISZE = 100
+    HEARTBEAT_INTERVAL = 60
     
-    def __init__(self, client, path_converter, root, root_expected, recursive_threshold, max_scanners, timeout, quiet, display_progress, max_files = None,
+    def __init__(self, client, path_converter, root, root_expected, recursive_threshold, max_scanners, timeout, quiet, display_progress, 
+                stats=None, my_stats=None, max_files=None,
                 include_sizes=True, ignore_list=[], list_empty_dirs=False):
         PyThread.__init__(self)
         self.RecursiveThreshold = recursive_threshold
         self.PathConverter = path_converter
         self.Client = client
         self.Root = root
         self.MaxScanners = max_scanners
@@ -255,14 +258,16 @@
         self.IgnoreList = ignore_list
         self.IgnoredFiles = self.IgnoredDirs = 0
         self.IncludeSizes = include_sizes
         self.TotalSize = 0.0 if include_sizes else None                  # Megabytes
         self.Timeout = timeout
         self.RootExpected = root_expected
         self.ListEmptyDirs = list_empty_dirs
+        self.Stats = stats
+        self.MyStats = my_stats
 
     def taskFailed(self, queue, task, exc_type, exc_value, tb):
         traceback.print_exception(exc_type, exc_value, tb, file=sys.stderr)
 
     def taskFailed(self, queue, task, exc_type, exc_value, tb):
         traceback.print_exception(exc_type, exc_value, tb, file=sys.stderr)
 
@@ -270,14 +275,21 @@
         #
         # scan Root non-recursovely first, if failed, return immediarely
         #
         #server, location, recursive, timeout
         scanner_task = Scanner(self, self.Client, self.Timeout, self.Root, self.RecursiveThreshold == 0, include_sizes=self.IncludeSizes, 
                 report_empty_top=False, list_empty_dirs=self.ListEmptyDirs)
         self.ScannerQueue.addTask(scanner_task)
+        while not self.ScannerQueue.isEmpty():
+            self.sleep(self.HEARTBEAT_INTERVAL)
+            if self.MyStats is not None:
+                t = time.time()
+                self.MyStats["heartbeat"] = t
+                self.MyStats["heartbeat_utc"] = str(datetime.utcfromtimestamp(t))
+                self.Stats.save()
         self.ScannerQueue.waitUntilEmpty()
         self.Results.close()
         self.ScannerQueue.Delegate = None       # detach for garbage collection
         self.ScannerQueue = None
         
     def dir_ignored(self, logpath):
         # path is expected to be canonic here
@@ -318,28 +330,30 @@
         if time.time() > self.LastReport + self.REPORT_INTERVAL:
             waiting, active = self.ScannerQueue.tasks()
             #sys.stderr.write("--- Locations to scan: %d\n" % (len(active)+len(waiting),))
             self.LastReport = time.time()
 
     @synchronized
     def scanner_failed(self, scanner, error):
+        self.wakeup()               # do not sleep for the heatbeat any longer
         path = scanner.Location                
         retry = (scanner.RecAttempts > 0) or (scanner.FlatAttempts > 0)
         if retry:
             print("resubmitted because of error:", scanner.Location, scanner.RecAttempts, scanner.FlatAttempts)
             self.ScannerQueue.addTask(scanner)
         else:
             print("Gave up:", scanner.Location)
             self.GaveUp[scanner.Location] = error
             self.NScanned += 1  
             #sys.stderr.write("Gave up on: %s\n" % (path,))
             self.show_progress()            #"Error scanning %s: %s -- retrying" % (scanner.Location, error))
 
     @synchronized
     def scanner_succeeded(self, scanner, location, was_recursive, files, dirs, empty_dir_count, empty_dirs):
+        self.wakeup()               # do not sleep for the heatbeat any longer
         if not files and not dirs and was_recursive and scanner.ZeroAttempts > 0:
             scanner.ZeroAttempts -= 1
             print("resubmitted because recursive scan found nothing:", scanner.Location)
             self.ScannerQueue.addTask(scanner)
             return
 
         self.NScanned += 1
@@ -464,33 +478,35 @@
     server_root = config.ServerRoot
     ignore_subdirs = config.ignore_subdirs(root)
     is_redirector = config.ServerIsRedirector
     ignore_list = config.IgnoreList
 
     t0 = time.time()
     root_stats = {
-       "root": root,
-       "expected": root_expected,
-       "start_time":t0,
-       "timeout":timeout,
-       "recursive_threshold":recursive_threshold,
-       "max_scanners":max_scanners,
-       "ignore_subdirectories": ignore_subdirs,
-       "servers": client.Servers
+        "root": root,
+        "expected": root_expected,
+        "start_time":t0,
+        "timeout":timeout,
+        "recursive_threshold":recursive_threshold,
+        "max_scanners":max_scanners,
+        "ignore_subdirectories": ignore_subdirs,
+        "servers": client.Servers
     }
 
     my_stats["scanning"] = root_stats
     if stats is not None:
         stats.update_section(stats_key, my_stats)
+    next_stats_update = time.time() + 60
 
     remove_prefix = config.RemovePrefix
     add_prefix = config.AddPrefix
     path_converter = PathConverter(server_root, remove_prefix, add_prefix, root)
 
     master = ScannerMaster(client, path_converter, root, root_expected, recursive_threshold, max_scanners, timeout, quiet, display_progress,
+            stats=stats, my_stats=my_stats,
             max_files = max_files, include_sizes=include_sizes, list_empty_dirs=empty_dirs_file is not None,
             ignore_list = ignore_list)
 
     path_filter = None          # -- obsolete -- config.scanner_filter(rse)
     #if path_filter is not None:
     #    path_filter = re.compile(path_filter)
     rewrite_path, rewrite_out = None, None      # -- obsolete -- config.scanner_rewrite(rse)
@@ -517,14 +533,20 @@
     for t, logpath in master.paths():
         # here, path is absolute path, which includes site root
         if t == 'f':
             file_list.add(logpath)             
         elif t == 'e' and empty_dirs_file is not None:
             empty_dirs_file.write(logpath)
             empty_dirs_file.write("\n")
+        if stats is not None and time.time() > next_stats_update:
+            t = time.time()
+            my_stats["heartbeat"] = t
+            my_stats["heartbeat_utc"] = str(datetime.utcfromtimestamp(t))
+            stats.update_section(stats_key, my_stats)
+            next_stats_update += 60
 
     if display_progress:
         master.close_progress()
 
     if master.Failed:
         sys.stderr.write("Scanner failed to scan %s: %s\n" % (root, master.Error))
 
@@ -640,28 +662,31 @@
     server = config.Server
     server_root = config.ServerRoot
     include_sizes = config.IncludeSizes and not "-x" in opts
     if not server_root:
         print(f"Server root is not defined for {rse}. Should be defined as 'server_root'")
         sys.exit(2)
 
+    t = time.time()
     my_stats = {
         "rse":rse,
         "scanner":{
             "type":"xrootd",
             "version":Version
         },
-        "server_root":server_root,
-        "server":server,
-        "roots":[], 
-        "start_time":time.time(),
-        "end_time": None,
-        "status":   "started",
+        "server_root":                  server_root,
+        "server":                       server,
+        "roots":                        [],
+        "start_time":                   t,
+        "end_time":                     None,
+        "status":                       "started",
         "files_output_prefix":          output,
-        "empty_dirs_output_file":       empty_dir_output
+        "empty_dirs_output_file":       empty_dir_output,
+        "heartbeat":                    t,
+        "heartbeat_utc":                str(datetime.utcfromtimestamp(t))
     }
     
     if stats is not None:
         stats[stats_key] = my_stats
     
     root_paths = [canonic_path(root if root.startswith("/") else server_root + "/" + root) for root in config.RootList]
```

### Comparing `rucio-consistency-1.3.0/rucio_consistency.egg-info/SOURCES.txt` & `rucio-consistency-1.4.0/rucio_consistency.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.3.0/setup.py` & `rucio-consistency-1.4.0/setup.py`

 * *Files identical despite different names*

