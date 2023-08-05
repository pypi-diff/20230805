# Comparing `tmp/remote-log-1.0.4.tar.gz` & `tmp/remote-log-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remote-log-1.0.4.tar", last modified: Sat Aug  5 14:07:29 2023, max compression
+gzip compressed data, was "remote-log-1.0.5.tar", last modified: Sat Aug  5 14:09:26 2023, max compression
```

## Comparing `remote-log-1.0.4.tar` & `remote-log-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-08-05 14:07:29.105124 remote-log-1.0.4/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1046 2023-08-05 14:07:29.105002 remote-log-1.0.4/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      824 2023-08-05 14:07:16.000000 remote-log-1.0.4/README.md
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-08-05 14:07:29.103979 remote-log-1.0.4/remote_log/
--rw-r--r--   0 brainspoof   (501) staff       (20)       25 2023-08-04 20:15:20.000000 remote-log-1.0.4/remote_log/__init__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)       34 2023-08-05 13:41:02.000000 remote-log-1.0.4/remote_log/__main__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     2540 2023-08-05 13:16:24.000000 remote-log-1.0.4/remote_log/remote_log.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     2180 2023-08-05 11:12:34.000000 remote-log-1.0.4/remote_log/sysinfo.py
--rw-r--r--   0 brainspoof   (501) staff       (20)       28 2023-08-04 20:15:20.000000 remote-log-1.0.4/remote_log/tests.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-08-05 14:07:29.104708 remote-log-1.0.4/remote_log.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1046 2023-08-05 14:07:29.000000 remote-log-1.0.4/remote_log.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      300 2023-08-05 14:07:29.000000 remote-log-1.0.4/remote_log.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-08-05 14:07:29.000000 remote-log-1.0.4/remote_log.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       27 2023-08-05 14:07:29.000000 remote-log-1.0.4/remote_log.egg-info/requires.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       11 2023-08-05 14:07:29.000000 remote-log-1.0.4/remote_log.egg-info/top_level.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-08-05 14:07:29.105169 remote-log-1.0.4/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      644 2023-08-05 14:07:25.000000 remote-log-1.0.4/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-08-05 14:09:26.581902 remote-log-1.0.5/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1046 2023-08-05 14:09:26.581790 remote-log-1.0.5/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      824 2023-08-05 14:09:03.000000 remote-log-1.0.5/README.md
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-08-05 14:09:26.580639 remote-log-1.0.5/remote_log/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       25 2023-08-04 20:15:20.000000 remote-log-1.0.5/remote_log/__init__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)       34 2023-08-05 13:41:02.000000 remote-log-1.0.5/remote_log/__main__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     2540 2023-08-05 13:16:24.000000 remote-log-1.0.5/remote_log/remote_log.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     2180 2023-08-05 11:12:34.000000 remote-log-1.0.5/remote_log/sysinfo.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)       28 2023-08-04 20:15:20.000000 remote-log-1.0.5/remote_log/tests.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-08-05 14:09:26.581397 remote-log-1.0.5/remote_log.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1046 2023-08-05 14:09:26.000000 remote-log-1.0.5/remote_log.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      300 2023-08-05 14:09:26.000000 remote-log-1.0.5/remote_log.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-08-05 14:09:26.000000 remote-log-1.0.5/remote_log.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       27 2023-08-05 14:09:26.000000 remote-log-1.0.5/remote_log.egg-info/requires.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       11 2023-08-05 14:09:26.000000 remote-log-1.0.5/remote_log.egg-info/top_level.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-08-05 14:09:26.581945 remote-log-1.0.5/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      644 2023-08-05 14:09:24.000000 remote-log-1.0.5/setup.py
```

### Comparing `remote-log-1.0.4/PKG-INFO` & `remote-log-1.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: remote-log
-Version: 1.0.4
+Version: 1.0.5
 Summary: A simple function to send logging data to a remote server.
 Author: Shubham Gupta
 Author-email: shubhastro2@gmail.com
 Description-Content-Type: text/markdown
 
 ```python
 import remote_log
 remote_log("https://myserver.com/log/", "log this my dear logging server")
 ```
 
 It sends a POST request to the server with the data you passed. If the system is offline, it stored the logs offline and sends all the data on the next call of `remote_log`.
 
 This way you are always assured you will receive the data to be logged.
 
-It also sends basic system information. Any uniquely identifiable information is not sent as plain text. It is hashed on the system using SHA256 before being sent. This way the logging server can still uniquely identify a log request but have no traceability back to the system that sent it thus allowing you to take a privacy first approach to logging.
+It also sends basic system information. Any uniquely identifiable information is not sent as plain text. It is hashed on the system using SHA256 before being sent. This way the logging server can still uniquely identify a log request but have no traceability back to the system that sent it thus allowing you to take a PRIVACY FIRST approach to logging.
 
 The function `remote_log` is non blocking and doesn't return anything. It's only purpose is to send logging data.
```

### Comparing `remote-log-1.0.4/README.md` & `remote-log-1.0.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 00000230: 6971 7565 6c79 2069 6465 6e74 6966 7920  iquely identify 
 00000240: 6120 6c6f 6720 7265 7175 6573 7420 6275  a log request bu
 00000250: 7420 6861 7665 206e 6f20 7472 6163 6561  t have no tracea
 00000260: 6269 6c69 7479 2062 6163 6b20 746f 2074  bility back to t
 00000270: 6865 2073 7973 7465 6d20 7468 6174 2073  he system that s
 00000280: 656e 7420 6974 2074 6875 7320 616c 6c6f  ent it thus allo
 00000290: 7769 6e67 2079 6f75 2074 6f20 7461 6b65  wing you to take
-000002a0: 2061 2070 7269 7661 6379 2066 6972 7374   a privacy first
+000002a0: 2061 2050 5249 5641 4359 2046 4952 5354   a PRIVACY FIRST
 000002b0: 2061 7070 726f 6163 6820 746f 206c 6f67   approach to log
 000002c0: 6769 6e67 2e0a 0a54 6865 2066 756e 6374  ging...The funct
 000002d0: 696f 6e20 6072 656d 6f74 655f 6c6f 6760  ion `remote_log`
 000002e0: 2069 7320 6e6f 6e20 626c 6f63 6b69 6e67   is non blocking
 000002f0: 2061 6e64 2064 6f65 736e 2774 2072 6574   and doesn't ret
 00000300: 7572 6e20 616e 7974 6869 6e67 2e20 4974  urn anything. It
 00000310: 2773 206f 6e6c 7920 7075 7270 6f73 6520  's only purpose
```

### Comparing `remote-log-1.0.4/remote_log/remote_log.py` & `remote-log-1.0.5/remote_log/remote_log.py`

 * *Files identical despite different names*

### Comparing `remote-log-1.0.4/remote_log/sysinfo.py` & `remote-log-1.0.5/remote_log/sysinfo.py`

 * *Files identical despite different names*

### Comparing `remote-log-1.0.4/remote_log.egg-info/PKG-INFO` & `remote-log-1.0.5/remote_log.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: remote-log
-Version: 1.0.4
+Version: 1.0.5
 Summary: A simple function to send logging data to a remote server.
 Author: Shubham Gupta
 Author-email: shubhastro2@gmail.com
 Description-Content-Type: text/markdown
 
 ```python
 import remote_log
 remote_log("https://myserver.com/log/", "log this my dear logging server")
 ```
 
 It sends a POST request to the server with the data you passed. If the system is offline, it stored the logs offline and sends all the data on the next call of `remote_log`.
 
 This way you are always assured you will receive the data to be logged.
 
-It also sends basic system information. Any uniquely identifiable information is not sent as plain text. It is hashed on the system using SHA256 before being sent. This way the logging server can still uniquely identify a log request but have no traceability back to the system that sent it thus allowing you to take a privacy first approach to logging.
+It also sends basic system information. Any uniquely identifiable information is not sent as plain text. It is hashed on the system using SHA256 before being sent. This way the logging server can still uniquely identify a log request but have no traceability back to the system that sent it thus allowing you to take a PRIVACY FIRST approach to logging.
 
 The function `remote_log` is non blocking and doesn't return anything. It's only purpose is to send logging data.
```

### Comparing `remote-log-1.0.4/setup.py` & `remote-log-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='remote-log',
-    version='1.0.4',
+    version='1.0.5',
     packages=find_packages(),
     description = 'A simple function to send logging data to a remote server.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Shubham Gupta',
     author_email = 'shubhastro2@gmail.com',
     install_requires=[
```

