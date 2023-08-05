# Comparing `tmp/valvesmd-1.0.0.tar.gz` & `tmp/valvesmd-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/valvesmd-1.0.0.tar", last modified: Fri Aug 27 14:29:15 2021, max compression
+gzip compressed data, was "valvesmd-1.0.1.tar", last modified: Sat Aug  5 03:27:18 2023, max compression
```

## Comparing `valvesmd-1.0.0.tar` & `valvesmd-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,19 @@
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2021-08-27 14:29:15.000000 valvesmd-1.0.0/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      982 2021-08-27 14:29:15.000000 valvesmd-1.0.0/PKG-INFO
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       39 2021-07-09 17:34:26.000000 valvesmd-1.0.0/setup.cfg
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1116 2021-08-27 14:11:07.000000 valvesmd-1.0.0/setup.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2021-08-27 14:29:15.000000 valvesmd-1.0.0/valvesmd/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      364 2021-08-25 07:00:45.000000 valvesmd-1.0.0/valvesmd/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     6044 2021-08-27 13:41:15.000000 valvesmd-1.0.0/valvesmd/classes.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     3583 2021-08-27 13:23:13.000000 valvesmd-1.0.0/valvesmd/parser.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1429 2021-08-25 08:15:31.000000 valvesmd-1.0.0/valvesmd/smd.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     2945 2021-08-27 12:16:28.000000 valvesmd-1.0.0/valvesmd/utils.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      372 2021-07-18 21:13:30.000000 valvesmd-1.0.0/valvesmd/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:27:18.290788 valvesmd-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-05 03:27:09.000000 valvesmd-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-08-05 03:27:18.290788 valvesmd-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-08-05 03:27:09.000000 valvesmd-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 03:27:18.290788 valvesmd-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-08-05 03:27:17.000000 valvesmd-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:27:18.290788 valvesmd-1.0.1/valvesmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-05 03:27:09.000000 valvesmd-1.0.1/valvesmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-08-05 03:27:09.000000 valvesmd-1.0.1/valvesmd/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-08-05 03:27:09.000000 valvesmd-1.0.1/valvesmd/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-08-05 03:27:09.000000 valvesmd-1.0.1/valvesmd/smd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-08-05 03:27:09.000000 valvesmd-1.0.1/valvesmd/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-05 03:27:09.000000 valvesmd-1.0.1/valvesmd/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:27:18.290788 valvesmd-1.0.1/valvesmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-08-05 03:27:18.000000 valvesmd-1.0.1/valvesmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-05 03:27:18.000000 valvesmd-1.0.1/valvesmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 03:27:18.000000 valvesmd-1.0.1/valvesmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-05 03:27:18.000000 valvesmd-1.0.1/valvesmd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 03:27:18.000000 valvesmd-1.0.1/valvesmd.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `valvesmd-1.0.0/valvesmd/classes.py` & `valvesmd-1.0.1/valvesmd/classes.py`

 * *Files identical despite different names*

### Comparing `valvesmd-1.0.0/valvesmd/parser.py` & `valvesmd-1.0.1/valvesmd/parser.py`

 * *Files identical despite different names*

### Comparing `valvesmd-1.0.0/valvesmd/smd.py` & `valvesmd-1.0.1/valvesmd/smd.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,30 +15,30 @@
     This is the basic class to interact with smd files.
     To interact with the data, consult :py:class:`SmdRoot<SmdRoot>`
     which this class inherits
     """
 
     def __init__(self, path=None):
         """
-        initalize a pcf file.
+        initalize a smd file.
 
         :param path: The location of the smd file to be parsed
-        :type path: str
+        :type path: str, optional
         """
         self.source_path = path  #: :type: (str) - The location of the parsed file
 
         super().__init__()
 
         if self.source_path:
             data = SmdParse(self.source_path)
             self.version = data.version
             self.nodes = data.nodes
             self.skeleton = data.skeleton
             self.triangles = data.triangles
 
     def save(self, destination=None):
-        """Saves the current instance of the Pcf. Overwrites original pcf file if no destination is provided.
+        """Saves the current instance of the Smd. Overwrites original smd file if no destination is provided.
 
-        :param destination: A path (directory + filename) to determine where to save the pcf file.
+        :param destination: A path (directory + filename) to determine where to save the smd file.
         :type destination: str, optional
         """
         SmdWrite(self, destination or self.source_path)
```

### Comparing `valvesmd-1.0.0/valvesmd/utils.py` & `valvesmd-1.0.1/valvesmd/utils.py`

 * *Files identical despite different names*

