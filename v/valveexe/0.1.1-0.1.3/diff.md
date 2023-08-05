# Comparing `tmp/valveexe-0.1.1.tar.gz` & `tmp/valveexe-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valveexe-0.1.1.tar", last modified: Tue Sep 28 03:54:23 2021, max compression
+gzip compressed data, was "valveexe-0.1.3.tar", last modified: Sat Aug  5 04:36:57 2023, max compression
```

## Comparing `valveexe-0.1.1.tar` & `valveexe-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,18 @@
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2021-09-28 03:54:23.277948 valveexe-0.1.1/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      694 2021-09-28 03:54:23.277948 valveexe-0.1.1/PKG-INFO
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       39 2021-09-25 20:30:56.136221 valveexe-0.1.1/setup.cfg
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      850 2021-09-28 03:50:51.938020 valveexe-0.1.1/setup.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2021-09-28 03:54:23.277948 valveexe-0.1.1/valveexe/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      133 2021-09-27 03:12:16.397621 valveexe-0.1.1/valveexe/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     2905 2021-09-28 03:43:19.670788 valveexe-0.1.1/valveexe/console.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     5366 2021-09-28 03:43:19.670788 valveexe-0.1.1/valveexe/exe.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1664 2021-09-28 03:43:19.670788 valveexe-0.1.1/valveexe/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:36:57.126070 valveexe-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-05 04:36:46.000000 valveexe-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-08-05 04:36:57.126070 valveexe-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-08-05 04:36:46.000000 valveexe-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 04:36:57.126070 valveexe-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-08-05 04:36:55.000000 valveexe-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:36:57.126070 valveexe-0.1.3/valveexe/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-05 04:36:46.000000 valveexe-0.1.3/valveexe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-08-05 04:36:46.000000 valveexe-0.1.3/valveexe/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-08-05 04:36:46.000000 valveexe-0.1.3/valveexe/exe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-05 04:36:46.000000 valveexe-0.1.3/valveexe/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-05 04:36:46.000000 valveexe-0.1.3/valveexe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:36:57.126070 valveexe-0.1.3/valveexe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-08-05 04:36:57.000000 valveexe-0.1.3/valveexe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-05 04:36:57.000000 valveexe-0.1.3/valveexe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 04:36:57.000000 valveexe-0.1.3/valveexe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-05 04:36:57.000000 valveexe-0.1.3/valveexe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 04:36:57.000000 valveexe-0.1.3/valveexe.egg-info/top_level.txt
```

### Comparing `valveexe-0.1.1/valveexe/console.py` & `valveexe-0.1.3/valveexe/console.py`

 * *Files identical despite different names*

### Comparing `valveexe-0.1.1/valveexe/exe.py` & `valveexe-0.1.3/valveexe/exe.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import time
 import subprocess
 import psutil
 import glob
 
 from rcon import Client
 
+from valveexe.utils import find_process, terminate_process
 from valveexe.logger import Logger
 from valveexe.console import RconConsole, ExecConsole
 
 
 class ValveExe(object):
     def __init__(self, gameExe, gameDir, steamExe=None, appid=None):
         '''Defines a launchable source engine game to be interacted with.
@@ -55,18 +56,19 @@
         '''Launches the game as specified in :any:`__init__` with the
         launch parameters supplied as arguments.
 
         :param \*params: The launch parameters to be supplied to the executable.
         :type \*params: str
         '''
         if self.steamExe and self.appid:
-            self._terminate_process()  # Steam launches cannot be hijacked
+            # Steam launches cannot be hijacked
+            terminate_process(self.exeName)
             launch_params = [self.steamExe, '-applaunch', str(self.appid)]
         else:
-            self.hijacked = bool(self._find_process())
+            self.hijacked = bool(find_process(self.exeName))
             launch_params = [self.gameExe, '-hijack']
 
         launch_params.extend(['-game', self.gameDir])
         launch_params.extend(['+log', '0', '+sv_logflush', '1',
                               '+con_logfile', self.logName])
 
         if self._check_rcon_eligible() is not False:
@@ -89,56 +91,51 @@
 
         :param command: A Source Engine `console command \
         <https://developer.valvesoftware.com/wiki/Console_Command_List>`_.
         :type command: str
         :param \*params: The values to be included with the command.
         :type \*params: str
         '''
-
+        if not self.process:
+            return
         if self.console:
             self.console.run(command, *params)
         else:
             with self as console:
                 console.run(command, *params)
 
     def quit(self):
         '''Closes the game client'''
-        process = self.process or self._find_process(self)
+        process = self.process or find_process(self.exeName)
         if process:
             process.terminate()
+        self.process = None
 
     def _check_rcon_eligible(self):
         '''
         None: Unknown
         True: Eligible
         False: Not eligible
         '''
-        process = self._find_process()
+        process = find_process(self.exeName)
         if not process:
             # no process running
             return None
-        elif self.gameDir not in process.cmdline():
-            # wrong game open
+        elif self.gameDir not in process.cmdline() and \
+                self.gameDir.split('\\')[-1] not in process.cmdline():
+            # wrong game
             process.terminate()
             return None
         elif '-usercon' not in process.cmdline():
             # doesn't have rcon enabled
             return False
         else:
             # 'connections' confirms game is listening for rcon
             return bool(process.connections())
 
-    def _find_process(self):
-        return next((p for p in psutil.process_iter() if
-                     p.name() == self.exeName), None)
-
-    def _terminate_process(self):
-        process = self._find_process()
-        process and process.terminate()
-
     def __enter__(self):
         while self._check_rcon_eligible() is None:
             time.sleep(3)
 
         if self._check_rcon_eligible():
             self.console = RconConsole("127.0.0.1", 27015, self.uuid)
         else:
```

### Comparing `valveexe-0.1.1/valveexe/logger.py` & `valveexe-0.1.3/valveexe/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,19 +33,20 @@
                 logs_since_bookmark += line
                 self._bookmark = f.tell()
         return logs_since_bookmark
 
     def log_until(self, until=None):
         '''
         Will :any:`log_ingest()<log_ingest>` until a specified regex is
-        found within the logs.
+        found within the logs and returns the logs until that point.
 
         :param until: A regex string to match against the logs
         :type until: str
-         '''
+        :rtype: str
+        '''
         logs_since_until = ''  # all logs since the previous log_until()
         with open(self.logPath, mode='r') as f:
 
             while not re.search(until, logs_since_until):
                 time.sleep(0.5)
                 logs_since_until += self.log_ingest()
                 if not until:
```

