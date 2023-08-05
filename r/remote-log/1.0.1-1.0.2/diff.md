# Comparing `tmp/remote-log-1.0.1.tar.gz` & `tmp/remote-log-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remote-log-1.0.1.tar", last modified: Sat Aug  5 13:58:53 2023, max compression
+gzip compressed data, was "remote-log-1.0.2.tar", last modified: Sat Aug  5 14:00:27 2023, max compression
```

## Comparing `remote-log-1.0.1.tar` & `remote-log-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-08-05 13:58:53.167390 remote-log-1.0.1/
--rw-r--r--   0 brainspoof   (501) staff       (20)      922 2023-08-05 13:58:53.167225 remote-log-1.0.1/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-08-05 13:58:53.166359 remote-log-1.0.1/remote_log/
--rw-r--r--   0 brainspoof   (501) staff       (20)       25 2023-08-04 20:15:20.000000 remote-log-1.0.1/remote_log/__init__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)       34 2023-08-05 13:41:02.000000 remote-log-1.0.1/remote_log/__main__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     2540 2023-08-05 13:16:24.000000 remote-log-1.0.1/remote_log/remote_log.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     2180 2023-08-05 11:12:34.000000 remote-log-1.0.1/remote_log/sysinfo.py
--rw-r--r--   0 brainspoof   (501) staff       (20)       28 2023-08-04 20:15:20.000000 remote-log-1.0.1/remote_log/tests.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-08-05 13:58:53.167032 remote-log-1.0.1/remote_log.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)      922 2023-08-05 13:58:53.000000 remote-log-1.0.1/remote_log.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      290 2023-08-05 13:58:53.000000 remote-log-1.0.1/remote_log.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-08-05 13:58:53.000000 remote-log-1.0.1/remote_log.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       27 2023-08-05 13:58:53.000000 remote-log-1.0.1/remote_log.egg-info/requires.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       11 2023-08-05 13:58:53.000000 remote-log-1.0.1/remote_log.egg-info/top_level.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-08-05 13:58:53.167438 remote-log-1.0.1/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)     1159 2023-08-05 13:57:11.000000 remote-log-1.0.1/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-08-05 14:00:27.379175 remote-log-1.0.2/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1031 2023-08-05 14:00:27.379064 remote-log-1.0.2/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-08-05 14:00:27.378260 remote-log-1.0.2/remote_log/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       25 2023-08-04 20:15:20.000000 remote-log-1.0.2/remote_log/__init__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)       34 2023-08-05 13:41:02.000000 remote-log-1.0.2/remote_log/__main__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     2540 2023-08-05 13:16:24.000000 remote-log-1.0.2/remote_log/remote_log.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     2180 2023-08-05 11:12:34.000000 remote-log-1.0.2/remote_log/sysinfo.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)       28 2023-08-04 20:15:20.000000 remote-log-1.0.2/remote_log/tests.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-08-05 14:00:27.378910 remote-log-1.0.2/remote_log.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1031 2023-08-05 14:00:27.000000 remote-log-1.0.2/remote_log.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      290 2023-08-05 14:00:27.000000 remote-log-1.0.2/remote_log.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-08-05 14:00:27.000000 remote-log-1.0.2/remote_log.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       27 2023-08-05 14:00:27.000000 remote-log-1.0.2/remote_log.egg-info/requires.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       11 2023-08-05 14:00:27.000000 remote-log-1.0.2/remote_log.egg-info/top_level.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-08-05 14:00:27.379215 remote-log-1.0.2/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1271 2023-08-05 14:00:24.000000 remote-log-1.0.2/setup.py
```

### Comparing `remote-log-1.0.1/PKG-INFO` & `remote-log-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 Metadata-Version: 2.1
 Name: remote-log
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple function to send logging data to a remote server.
 Author: Shubham Gupta
 Author-email: shubhastro2@gmail.com
 
 
+    import remote_log
+
+    remote_log("https://myserver.com/log/", "log this my dear logging server")
+
+    
+
     It sends a POST request to the server with the data you passed. If the system is offline, it stored the logs offline and sends all the data on the next call of remote_log.
 
     This way you are always assured you will receive the data to be logged.
 
     It also sends basic system information. Any uniquely identifiable information is not sent as plain text. It is hashed on the system using SHA256 before being sent. This way the logging server can still uniquely identify a log request but have no traceability back to the system that sent it thus allowing you to take a privacy first approach to logging.
```

### Comparing `remote-log-1.0.1/remote_log/remote_log.py` & `remote-log-1.0.2/remote_log/remote_log.py`

 * *Files identical despite different names*

### Comparing `remote-log-1.0.1/remote_log/sysinfo.py` & `remote-log-1.0.2/remote_log/sysinfo.py`

 * *Files identical despite different names*

### Comparing `remote-log-1.0.1/remote_log.egg-info/PKG-INFO` & `remote-log-1.0.2/remote_log.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 Metadata-Version: 2.1
 Name: remote-log
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple function to send logging data to a remote server.
 Author: Shubham Gupta
 Author-email: shubhastro2@gmail.com
 
 
+    import remote_log
+
+    remote_log("https://myserver.com/log/", "log this my dear logging server")
+
+    
+
     It sends a POST request to the server with the data you passed. If the system is offline, it stored the logs offline and sends all the data on the next call of remote_log.
 
     This way you are always assured you will receive the data to be logged.
 
     It also sends basic system information. Any uniquely identifiable information is not sent as plain text. It is hashed on the system using SHA256 before being sent. This way the logging server can still uniquely identify a log request but have no traceability back to the system that sent it thus allowing you to take a privacy first approach to logging.
```

### Comparing `remote-log-1.0.1/setup.py` & `remote-log-1.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from setuptools import setup, find_packages
 setup(
     name='remote-log',
-    version='1.0.1',
+    version='1.0.2',
     packages=find_packages(),
     description = 'A simple function to send logging data to a remote server.',
     long_description='''
+    import remote_log\n
+    remote_log("https://myserver.com/log/", "log this my dear logging server")\n
+    \n
     It sends a POST request to the server with the data you passed. If the system is offline, it stored the logs offline and sends all the data on the next call of remote_log.\n
     This way you are always assured you will receive the data to be logged.\n
     It also sends basic system information. Any uniquely identifiable information is not sent as plain text. It is hashed on the system using SHA256 before being sent. This way the logging server can still uniquely identify a log request but have no traceability back to the system that sent it thus allowing you to take a privacy first approach to logging.
     \n\n
     The function remote_log is non blocking and doesn't return anything. It's only purpose is to send logging data.
     ''',
     author = 'Shubham Gupta',
```

