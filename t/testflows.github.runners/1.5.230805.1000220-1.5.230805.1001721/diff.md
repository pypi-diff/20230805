# Comparing `tmp/testflows.github.runners-1.5.230805.1000220.tar.gz` & `tmp/testflows.github.runners-1.5.230805.1001721.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.5.230805.1000220.tar", last modified: Sat Aug  5 00:02:20 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.5.230805.1001721.tar", last modified: Sat Aug  5 00:17:21 2023, max compression
```

## Comparing `testflows.github.runners-1.5.230805.1000220.tar` & `testflows.github.runners-1.5.230805.1001721.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 00:02:20.554336 testflows.github.runners-1.5.230805.1000220/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230805.1000220/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-05 00:02:20.554336 testflows.github.runners-1.5.230805.1000220/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    63971 2023-08-04 02:31:51.000000 testflows.github.runners-1.5.230805.1000220/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-05 00:02:20.554336 testflows.github.runners-1.5.230805.1000220/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2195 2023-08-05 00:02:20.000000 testflows.github.runners-1.5.230805.1000220/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 00:02:20.550336 testflows.github.runners-1.5.230805.1000220/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 00:02:20.550336 testflows.github.runners-1.5.230805.1000220/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 00:02:20.550336 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-05 00:02:20.000000 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2837 2023-08-04 23:53:23.000000 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1995 2023-08-02 15:26:55.000000 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/api_watch.py
--rw-rw-r--   0 user      (1000) user      (1000)     2933 2023-08-04 06:28:52.000000 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 00:02:20.550336 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    25686 2023-08-04 23:37:17.000000 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    15038 2023-08-05 00:01:58.000000 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/cloud.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 00:02:20.554336 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/config/
--rw-rw-r--   0 user      (1000) user      (1000)      903 2023-08-04 23:32:22.000000 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/config/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    16642 2023-08-04 23:53:11.000000 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/config/config.py
--rw-rw-r--   0 user      (1000) user      (1000)    10337 2023-08-04 23:35:08.000000 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/config/schema.json
--rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/delete.py
--rw-rw-r--   0 user      (1000) user      (1000)     1844 2023-08-04 23:53:11.000000 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)    18206 2023-08-04 07:57:47.000000 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    30496 2023-08-04 14:49:19.000000 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 00:02:20.554336 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-08-04 04:50:46.000000 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 00:02:20.554336 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/scripts/setup_docker.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     3206 2023-08-04 19:52:52.000000 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     2714 2023-08-04 23:23:34.000000 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/servers.py
--rw-rw-r--   0 user      (1000) user      (1000)     5677 2023-08-03 17:20:44.000000 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1607 2023-08-04 23:22:51.000000 testflows.github.runners-1.5.230805.1000220/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 00:02:20.550336 testflows.github.runners-1.5.230805.1000220/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-05 00:02:20.000000 testflows.github.runners-1.5.230805.1000220/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1323 2023-08-05 00:02:20.000000 testflows.github.runners-1.5.230805.1000220/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-05 00:02:20.000000 testflows.github.runners-1.5.230805.1000220/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.5.230805.1000220/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       73 2023-08-05 00:02:20.000000 testflows.github.runners-1.5.230805.1000220/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-05 00:02:20.000000 testflows.github.runners-1.5.230805.1000220/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 00:17:21.926427 testflows.github.runners-1.5.230805.1001721/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230805.1001721/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-05 00:17:21.922428 testflows.github.runners-1.5.230805.1001721/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    63971 2023-08-04 02:31:51.000000 testflows.github.runners-1.5.230805.1001721/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-05 00:17:21.926427 testflows.github.runners-1.5.230805.1001721/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2195 2023-08-05 00:17:21.000000 testflows.github.runners-1.5.230805.1001721/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 00:17:21.922428 testflows.github.runners-1.5.230805.1001721/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 00:17:21.922428 testflows.github.runners-1.5.230805.1001721/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 00:17:21.922428 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-05 00:17:21.000000 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2836 2023-08-05 00:10:52.000000 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1995 2023-08-02 15:26:55.000000 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/api_watch.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2933 2023-08-04 06:28:52.000000 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 00:17:21.922428 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    25701 2023-08-05 00:12:56.000000 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    15053 2023-08-05 00:13:22.000000 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/cloud.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 00:17:21.922428 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/config/
+-rw-rw-r--   0 user      (1000) user      (1000)      903 2023-08-04 23:32:22.000000 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/config/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16661 2023-08-05 00:16:48.000000 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/config/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10337 2023-08-04 23:35:08.000000 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/config/schema.json
+-rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/delete.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1844 2023-08-04 23:53:11.000000 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)    18206 2023-08-04 07:57:47.000000 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    30496 2023-08-04 14:49:19.000000 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 00:17:21.922428 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-08-04 04:50:46.000000 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 00:17:21.922428 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/scripts/setup_docker.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     3206 2023-08-04 19:52:52.000000 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2714 2023-08-04 23:23:34.000000 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/servers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5677 2023-08-03 17:20:44.000000 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1607 2023-08-04 23:22:51.000000 testflows.github.runners-1.5.230805.1001721/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 00:17:21.922428 testflows.github.runners-1.5.230805.1001721/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-05 00:17:21.000000 testflows.github.runners-1.5.230805.1001721/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1323 2023-08-05 00:17:21.000000 testflows.github.runners-1.5.230805.1001721/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-05 00:17:21.000000 testflows.github.runners-1.5.230805.1001721/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.5.230805.1001721/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       73 2023-08-05 00:17:21.000000 testflows.github.runners-1.5.230805.1001721/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-05 00:17:21.000000 testflows.github.runners-1.5.230805.1001721/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.5.230805.1000220/LICENSE` & `testflows.github.runners-1.5.230805.1001721/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1000220/PKG-INFO` & `testflows.github.runners-1.5.230805.1001721/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.5.230805.1000220
+Version: 1.5.230805.1001721
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.5.230805.1000220/README.rst` & `testflows.github.runners-1.5.230805.1001721/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1000220/setup.py` & `testflows.github.runners-1.5.230805.1001721/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.5.230805.1000220",
+    version="1.5.230805.1001721",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows/github/runners/__init__.py` & `testflows.github.runners-1.5.230805.1001721/testflows/github/runners/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.5.230805.1000220"
+__version__ = "1.5.230805.1001721"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows/github/runners/actions.py` & `testflows.github.runners-1.5.230805.1001721/testflows/github/runners/actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             "run_id": run_id,
             "server_name": server_name,
             "interval": str(interval) if interval is not None else "",
         }
 
     def __enter__(self):
         logger.log(
-            msg=f"🍀 {self.name}",
+            msg=f"➤ {self.name}",
             stacklevel=self.stacklevel + 1,
             level=self.level,
             extra=self.extra,
         )
         return self
 
     def note(self, message, stacklevel=None):
```

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows/github/runners/api_watch.py` & `testflows.github.runners-1.5.230805.1001721/testflows/github/runners/api_watch.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows/github/runners/args.py` & `testflows.github.runners-1.5.230805.1001721/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.5.230805.1001721/testflows/github/runners/bin/github-runners`

 * *Files 1% similar despite different names*

```diff
@@ -711,15 +711,15 @@
             config.server_prices = check_prices(client)
 
         with Action(f"Checking if SSH key exists"):
             ssh_keys.append(check_ssh_key(client, config.ssh_key))
 
             if config.additional_ssh_keys:
                 for key in config.additional_ssh_keys:
-                    ssh_keys.append(check_ssh_key(client, key))
+                    ssh_keys.append(check_ssh_key(client, key, is_file=False))
 
         try:
             with Action("Creating scale up service"):
                 scale_up_service: Future = worker_pool.submit(
                     scale_up,
                     terminate=terminate,
                     ssh_keys=ssh_keys,
```

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows/github/runners/cloud.py` & `testflows.github.runners-1.5.230805.1001721/testflows/github/runners/cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             )
 
         with Action(f"Checking if SSH key exists"):
             ssh_keys.append(check_ssh_key(client, config.ssh_key))
 
             if config.additional_ssh_keys:
                 for key in config.additional_ssh_keys:
-                    ssh_keys.append(check_ssh_key(client, key))
+                    ssh_keys.append(check_ssh_key(client, key, is_file=False))
 
         with Action(f"Creating new server"):
             response = client.servers.create(
                 name=server_name,
                 server_type=config.cloud.deploy.server_type,
                 image=config.cloud.deploy.image,
                 location=config.cloud.deploy.location,
```

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows/github/runners/config/__init__.py` & `testflows.github.runners-1.5.230805.1001721/testflows/github/runners/config/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows/github/runners/config/config.py` & `testflows.github.runners-1.5.230805.1001721/testflows/github/runners/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,33 +201,31 @@
 
     if doc.get("config") is None:
         assert False, "config: entry is missing"
 
     doc = doc["config"]
 
     if doc.get("ssh_key") is not None:
-        assert isinstance(doc["ssh_key"], str), "config.ssh_key: not a string"
+        assert isinstance(doc["ssh_key"], str), "config.ssh_key: is not a string"
         doc["ssh_key"] = path(doc["ssh_key"], check_exists=False)
 
     if doc.get("additional_ssh_keys") is not None:
-        keys = []
         assert isinstance(
             doc["additional_ssh_keys"], list
         ), "config.additional_ssh_keys: not a list"
         for i, key in enumerate(doc["additional_ssh_keys"]):
             assert isinstance(
                 key, str
-            ), f"config.additional_ssh_keys[{i}]: not a string"
-            keys.append(path(key, check_exists=False))
+            ), f"config.additional_ssh_keys[{i}]: is not a string"
 
     if doc.get("with_label") is not None:
-        assert isinstance(doc["with_label"], str), "config.with_label: not a string"
+        assert isinstance(doc["with_label"], str), "config.with_label: is not a string"
 
     if doc.get("recycle") is not None:
-        assert isinstance(doc["recycle"], bool), "config.recycle: not a boolean"
+        assert isinstance(doc["recycle"], bool), "config.recycle: is not a boolean"
 
     if doc.get("end_of_life") is not None:
         v = doc["end_of_life"]
         assert isinstance(v, int), "config.end_of_life: is not integer"
         assert v > 0 and v < 60, "config.end_of_life: is not > 0 and < 60"
 
     if doc.get("max_runners") is not None:
@@ -251,15 +249,15 @@
             doc["default_server_type"] = server_type(doc["default_server_type"])
         except Exception as e:
             assert False, f"config.default_server_type: {e}"
 
     if doc.get("default_location") is not None:
         try:
             v = doc["default_location"]
-            assert isinstance(v, str), "not a string"
+            assert isinstance(v, str), "is not a string"
             doc["default_location"] = location(v)
         except Exception as e:
             assert False, f"config.default_location: {e}"
 
     if doc.get("workers") is not None:
         v = doc["workers"]
         assert isinstance(v, int) and v > 0, "config.workers: is not an integer > 0"
@@ -410,19 +408,22 @@
 
     try:
         return Config(**doc)
     except Exception as e:
         assert False, f"config: {e}"
 
 
-def check_ssh_key(client: Client, ssh_key: str):
+def check_ssh_key(client: Client, ssh_key: str, is_file=True):
     """Check that ssh key exists if not create it."""
 
-    with open(ssh_key, "r", encoding="utf-8") as ssh_key_file:
-        public_key = ssh_key_file.read()
+    if is_file:
+        with open(ssh_key, "r", encoding="utf-8") as ssh_key_file:
+            public_key = ssh_key_file.read()
+    else:
+        public_key = ssh_key
 
     key_name = hashlib.md5(public_key.encode("utf-8")).hexdigest()
     ssh_key = SSHKey(name=key_name, public_key=public_key)
 
     if not client.ssh_keys.get_by_name(name=ssh_key.name):
         with Action(f"Creating SSH key {ssh_key.name}", stacklevel=3):
             client.ssh_keys.create(name=ssh_key.name, public_key=ssh_key.public_key)
```

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows/github/runners/config/schema.json` & `testflows.github.runners-1.5.230805.1001721/testflows/github/runners/config/schema.json`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows/github/runners/delete.py` & `testflows.github.runners-1.5.230805.1001721/testflows/github/runners/delete.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows/github/runners/logger.py` & `testflows.github.runners-1.5.230805.1001721/testflows/github/runners/logger.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows/github/runners/request.py` & `testflows.github.runners-1.5.230805.1001721/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.5.230805.1001721/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.5.230805.1001721/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.5.230805.1001721/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.5.230805.1001721/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.5.230805.1001721/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows/github/runners/scripts/setup_docker.sh` & `testflows.github.runners-1.5.230805.1001721/testflows/github/runners/scripts/setup_docker.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.5.230805.1001721/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.5.230805.1001721/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows/github/runners/server.py` & `testflows.github.runners-1.5.230805.1001721/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows/github/runners/servers.py` & `testflows.github.runners-1.5.230805.1001721/testflows/github/runners/servers.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows/github/runners/service.py` & `testflows.github.runners-1.5.230805.1001721/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows/github/runners/shell.py` & `testflows.github.runners-1.5.230805.1001721/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.5.230805.1001721/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.5.230805.1000220
+Version: 1.5.230805.1001721
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.5.230805.1000220/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.5.230805.1001721/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

