# Comparing `tmp/testflows.github.runners-1.5.230805.1022415.tar.gz` & `tmp/testflows.github.runners-1.5.230805.1023308.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.5.230805.1022415.tar", last modified: Sat Aug  5 02:24:15 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.5.230805.1023308.tar", last modified: Sat Aug  5 02:33:08 2023, max compression
```

## Comparing `testflows.github.runners-1.5.230805.1022415.tar` & `testflows.github.runners-1.5.230805.1023308.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:24:15.628252 testflows.github.runners-1.5.230805.1022415/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230805.1022415/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-05 02:24:15.628252 testflows.github.runners-1.5.230805.1022415/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    63971 2023-08-04 02:31:51.000000 testflows.github.runners-1.5.230805.1022415/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-05 02:24:15.628252 testflows.github.runners-1.5.230805.1022415/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2195 2023-08-05 02:24:15.000000 testflows.github.runners-1.5.230805.1022415/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:24:15.624252 testflows.github.runners-1.5.230805.1022415/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:24:15.624252 testflows.github.runners-1.5.230805.1022415/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:24:15.628252 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-05 02:24:15.000000 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2835 2023-08-05 00:18:04.000000 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1995 2023-08-02 15:26:55.000000 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/api_watch.py
--rw-rw-r--   0 user      (1000) user      (1000)     2933 2023-08-04 06:28:52.000000 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:24:15.628252 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    25874 2023-08-05 02:05:41.000000 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    14938 2023-08-05 02:06:57.000000 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/cloud.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:24:15.628252 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/config/
--rw-rw-r--   0 user      (1000) user      (1000)      903 2023-08-04 23:32:22.000000 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/config/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    16804 2023-08-05 02:11:04.000000 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/config/config.py
--rw-rw-r--   0 user      (1000) user      (1000)    10337 2023-08-04 23:35:08.000000 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/config/schema.json
--rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/delete.py
--rw-rw-r--   0 user      (1000) user      (1000)     1949 2023-08-05 02:05:06.000000 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)    18206 2023-08-04 07:57:47.000000 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    30496 2023-08-04 14:49:19.000000 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:24:15.628252 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-08-04 04:50:46.000000 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:24:15.628252 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/scripts/setup_docker.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     3206 2023-08-05 02:14:33.000000 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     2714 2023-08-04 23:23:34.000000 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/servers.py
--rw-rw-r--   0 user      (1000) user      (1000)     5692 2023-08-05 01:59:34.000000 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1694 2023-08-05 02:23:54.000000 testflows.github.runners-1.5.230805.1022415/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:24:15.624252 testflows.github.runners-1.5.230805.1022415/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-05 02:24:15.000000 testflows.github.runners-1.5.230805.1022415/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1323 2023-08-05 02:24:15.000000 testflows.github.runners-1.5.230805.1022415/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-05 02:24:15.000000 testflows.github.runners-1.5.230805.1022415/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.5.230805.1022415/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       73 2023-08-05 02:24:15.000000 testflows.github.runners-1.5.230805.1022415/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-05 02:24:15.000000 testflows.github.runners-1.5.230805.1022415/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:33:08.415555 testflows.github.runners-1.5.230805.1023308/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230805.1023308/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-05 02:33:08.415555 testflows.github.runners-1.5.230805.1023308/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    63971 2023-08-04 02:31:51.000000 testflows.github.runners-1.5.230805.1023308/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-05 02:33:08.415555 testflows.github.runners-1.5.230805.1023308/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2195 2023-08-05 02:33:08.000000 testflows.github.runners-1.5.230805.1023308/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:33:08.411555 testflows.github.runners-1.5.230805.1023308/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:33:08.411555 testflows.github.runners-1.5.230805.1023308/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:33:08.415555 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-05 02:33:08.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2836 2023-08-05 02:32:20.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1995 2023-08-02 15:26:55.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/api_watch.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2933 2023-08-04 06:28:52.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:33:08.415555 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    25874 2023-08-05 02:05:41.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    14938 2023-08-05 02:06:57.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/cloud.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:33:08.415555 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/config/
+-rw-rw-r--   0 user      (1000) user      (1000)      903 2023-08-04 23:32:22.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/config/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16804 2023-08-05 02:11:04.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/config/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10337 2023-08-04 23:35:08.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/config/schema.json
+-rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/delete.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1953 2023-08-05 02:31:56.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)    18206 2023-08-04 07:57:47.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    30496 2023-08-04 14:49:19.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:33:08.415555 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-08-04 04:50:46.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:33:08.415555 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/setup_docker.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     3206 2023-08-05 02:14:33.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2714 2023-08-04 23:23:34.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/servers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5692 2023-08-05 01:59:34.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1694 2023-08-05 02:23:54.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:33:08.415555 testflows.github.runners-1.5.230805.1023308/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-05 02:33:08.000000 testflows.github.runners-1.5.230805.1023308/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1323 2023-08-05 02:33:08.000000 testflows.github.runners-1.5.230805.1023308/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-05 02:33:08.000000 testflows.github.runners-1.5.230805.1023308/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.5.230805.1023308/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       73 2023-08-05 02:33:08.000000 testflows.github.runners-1.5.230805.1023308/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-05 02:33:08.000000 testflows.github.runners-1.5.230805.1023308/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.5.230805.1022415/LICENSE` & `testflows.github.runners-1.5.230805.1023308/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1022415/PKG-INFO` & `testflows.github.runners-1.5.230805.1023308/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.5.230805.1022415
+Version: 1.5.230805.1023308
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.5.230805.1022415/README.rst` & `testflows.github.runners-1.5.230805.1023308/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1022415/setup.py` & `testflows.github.runners-1.5.230805.1023308/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.5.230805.1022415",
+    version="1.5.230805.1023308",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows/github/runners/__init__.py` & `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.5.230805.1022415"
+__version__ = "1.5.230805.1023308"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows/github/runners/actions.py` & `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         except Exception:
             pass
 
         self.extra = {
             "job_id": job_id,
             "run_id": run_id,
             "server_name": server_name,
-            "interval": str(interval) if interval is not None else "",
+            "interval": str(interval) if interval is not None else "-",
         }
 
     def __enter__(self):
         logger.log(
             msg=f"➤ {self.name}",
             stacklevel=self.stacklevel + 1,
             level=self.level,
```

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows/github/runners/api_watch.py` & `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/api_watch.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows/github/runners/args.py` & `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/bin/github-runners`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows/github/runners/cloud.py` & `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows/github/runners/config/__init__.py` & `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/config/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows/github/runners/config/config.py` & `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/config/config.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows/github/runners/config/schema.json` & `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/config/schema.json`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows/github/runners/delete.py` & `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/delete.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows/github/runners/logger.py` & `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,18 @@
             kwargs["extra"] = extra
         return msg, kwargs
 
 
 logger = LoggerAdapter(
     logger,
     {
-        "run_id": "",
-        "job_id": "",
-        "server_name": "",
-        "interval": "",
+        "run_id": "-",
+        "job_id": "-",
+        "server_name": "-",
+        "interval": "-",
     },
 )
 
 
 def default_config(level=logging.INFO, service_mode=False):
     """Apply default logging configuration."""
     global logger
```

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows/github/runners/request.py` & `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows/github/runners/scripts/setup_docker.sh` & `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/setup_docker.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows/github/runners/server.py` & `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows/github/runners/servers.py` & `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/servers.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows/github/runners/service.py` & `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows/github/runners/shell.py` & `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.5.230805.1023308/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.5.230805.1022415
+Version: 1.5.230805.1023308
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.5.230805.1022415/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.5.230805.1023308/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

