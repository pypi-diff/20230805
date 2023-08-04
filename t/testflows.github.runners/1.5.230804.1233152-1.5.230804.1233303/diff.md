# Comparing `tmp/testflows.github.runners-1.5.230804.1233152.tar.gz` & `tmp/testflows.github.runners-1.5.230804.1233303.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.5.230804.1233152.tar", last modified: Fri Aug  4 23:31:52 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.5.230804.1233303.tar", last modified: Fri Aug  4 23:33:03 2023, max compression
```

## Comparing `testflows.github.runners-1.5.230804.1233152.tar` & `testflows.github.runners-1.5.230804.1233303.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:31:52.949430 testflows.github.runners-1.5.230804.1233152/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1233152/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-04 23:31:52.945430 testflows.github.runners-1.5.230804.1233152/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    63971 2023-08-04 02:31:51.000000 testflows.github.runners-1.5.230804.1233152/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-04 23:31:52.949430 testflows.github.runners-1.5.230804.1233152/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2195 2023-08-04 23:31:52.000000 testflows.github.runners-1.5.230804.1233152/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:31:52.945430 testflows.github.runners-1.5.230804.1233152/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:31:52.945430 testflows.github.runners-1.5.230804.1233152/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:31:52.945430 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-04 23:31:52.000000 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2837 2023-08-04 14:50:53.000000 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1995 2023-08-02 15:26:55.000000 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/api_watch.py
--rw-rw-r--   0 user      (1000) user      (1000)     2933 2023-08-04 06:28:52.000000 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:31:52.945430 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    25683 2023-08-04 23:27:50.000000 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    14674 2023-08-04 19:52:38.000000 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/cloud.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:31:52.945430 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/config/
--rw-rw-r--   0 user      (1000) user      (1000)      844 2023-08-04 23:27:24.000000 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/config/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    16590 2023-08-04 23:22:09.000000 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/config/config.py
--rw-rw-r--   0 user      (1000) user      (1000)    10338 2023-08-04 23:19:44.000000 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/config/schema.json
--rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/delete.py
--rw-rw-r--   0 user      (1000) user      (1000)     2062 2023-08-04 16:38:03.000000 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)    18206 2023-08-04 07:57:47.000000 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    30496 2023-08-04 14:49:19.000000 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:31:52.945430 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-08-04 04:50:46.000000 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:31:52.945430 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/scripts/setup_docker.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     3206 2023-08-04 19:52:52.000000 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     2714 2023-08-04 23:23:34.000000 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/servers.py
--rw-rw-r--   0 user      (1000) user      (1000)     5677 2023-08-03 17:20:44.000000 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1607 2023-08-04 23:22:51.000000 testflows.github.runners-1.5.230804.1233152/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:31:52.945430 testflows.github.runners-1.5.230804.1233152/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-04 23:31:52.000000 testflows.github.runners-1.5.230804.1233152/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1323 2023-08-04 23:31:52.000000 testflows.github.runners-1.5.230804.1233152/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-04 23:31:52.000000 testflows.github.runners-1.5.230804.1233152/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.5.230804.1233152/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       73 2023-08-04 23:31:52.000000 testflows.github.runners-1.5.230804.1233152/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-04 23:31:52.000000 testflows.github.runners-1.5.230804.1233152/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:33:03.314327 testflows.github.runners-1.5.230804.1233303/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1233303/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-04 23:33:03.314327 testflows.github.runners-1.5.230804.1233303/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    63971 2023-08-04 02:31:51.000000 testflows.github.runners-1.5.230804.1233303/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-04 23:33:03.314327 testflows.github.runners-1.5.230804.1233303/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2195 2023-08-04 23:33:03.000000 testflows.github.runners-1.5.230804.1233303/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:33:03.314327 testflows.github.runners-1.5.230804.1233303/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:33:03.314327 testflows.github.runners-1.5.230804.1233303/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:33:03.314327 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-04 23:33:03.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2837 2023-08-04 14:50:53.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1995 2023-08-02 15:26:55.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/api_watch.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2933 2023-08-04 06:28:52.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:33:03.314327 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    25683 2023-08-04 23:27:50.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    14674 2023-08-04 19:52:38.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/cloud.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:33:03.314327 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/config/
+-rw-rw-r--   0 user      (1000) user      (1000)      903 2023-08-04 23:32:22.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/config/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16590 2023-08-04 23:22:09.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/config/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10338 2023-08-04 23:19:44.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/config/schema.json
+-rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/delete.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2062 2023-08-04 16:38:03.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)    18206 2023-08-04 07:57:47.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    30496 2023-08-04 14:49:19.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:33:03.314327 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-08-04 04:50:46.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:33:03.314327 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/setup_docker.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     3206 2023-08-04 19:52:52.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2714 2023-08-04 23:23:34.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/servers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5677 2023-08-03 17:20:44.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1607 2023-08-04 23:22:51.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:33:03.314327 testflows.github.runners-1.5.230804.1233303/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-04 23:33:03.000000 testflows.github.runners-1.5.230804.1233303/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1323 2023-08-04 23:33:03.000000 testflows.github.runners-1.5.230804.1233303/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-04 23:33:03.000000 testflows.github.runners-1.5.230804.1233303/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.5.230804.1233303/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       73 2023-08-04 23:33:03.000000 testflows.github.runners-1.5.230804.1233303/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-04 23:33:03.000000 testflows.github.runners-1.5.230804.1233303/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.5.230804.1233152/LICENSE` & `testflows.github.runners-1.5.230804.1233303/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233152/PKG-INFO` & `testflows.github.runners-1.5.230804.1233303/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.5.230804.1233152
+Version: 1.5.230804.1233303
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.5.230804.1233152/README.rst` & `testflows.github.runners-1.5.230804.1233303/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233152/setup.py` & `testflows.github.runners-1.5.230804.1233303/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.5.230804.1233152",
+    version="1.5.230804.1233303",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows/github/runners/__init__.py` & `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.5.230804.1233152"
+__version__ = "1.5.230804.1233303"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows/github/runners/actions.py` & `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows/github/runners/api_watch.py` & `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/api_watch.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows/github/runners/args.py` & `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/bin/github-runners`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows/github/runners/cloud.py` & `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows/github/runners/config/__init__.py` & `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/config/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,10 +9,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from .config import Config
-from .config import check_image, check_location, check_prices, check_server_type, check_ssh_key
+from .config import (
+    check_image,
+    check_location,
+    check_prices,
+    check_server_type,
+    check_ssh_key,
+)
 from .config import standby_runner
-from .config import read, write
+from .config import read, write
+from .config import parse_config
```

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows/github/runners/config/config.py` & `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/config/config.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows/github/runners/config/schema.json` & `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/config/schema.json`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows/github/runners/delete.py` & `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/delete.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows/github/runners/logger.py` & `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/logger.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows/github/runners/request.py` & `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows/github/runners/scripts/setup_docker.sh` & `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/setup_docker.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows/github/runners/server.py` & `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows/github/runners/servers.py` & `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/servers.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows/github/runners/service.py` & `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows/github/runners/shell.py` & `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.5.230804.1233303/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.5.230804.1233152
+Version: 1.5.230804.1233303
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.5.230804.1233152/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.5.230804.1233303/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

