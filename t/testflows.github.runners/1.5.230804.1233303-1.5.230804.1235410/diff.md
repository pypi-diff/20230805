# Comparing `tmp/testflows.github.runners-1.5.230804.1233303.tar.gz` & `tmp/testflows.github.runners-1.5.230804.1235410.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.5.230804.1233303.tar", last modified: Fri Aug  4 23:33:03 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.5.230804.1235410.tar", last modified: Fri Aug  4 23:54:10 2023, max compression
```

## Comparing `testflows.github.runners-1.5.230804.1233303.tar` & `testflows.github.runners-1.5.230804.1235410.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:33:03.314327 testflows.github.runners-1.5.230804.1233303/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1233303/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-04 23:33:03.314327 testflows.github.runners-1.5.230804.1233303/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    63971 2023-08-04 02:31:51.000000 testflows.github.runners-1.5.230804.1233303/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-04 23:33:03.314327 testflows.github.runners-1.5.230804.1233303/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2195 2023-08-04 23:33:03.000000 testflows.github.runners-1.5.230804.1233303/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:33:03.314327 testflows.github.runners-1.5.230804.1233303/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:33:03.314327 testflows.github.runners-1.5.230804.1233303/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:33:03.314327 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-04 23:33:03.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2837 2023-08-04 14:50:53.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1995 2023-08-02 15:26:55.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/api_watch.py
--rw-rw-r--   0 user      (1000) user      (1000)     2933 2023-08-04 06:28:52.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:33:03.314327 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    25683 2023-08-04 23:27:50.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    14674 2023-08-04 19:52:38.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/cloud.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:33:03.314327 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/config/
--rw-rw-r--   0 user      (1000) user      (1000)      903 2023-08-04 23:32:22.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/config/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    16590 2023-08-04 23:22:09.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/config/config.py
--rw-rw-r--   0 user      (1000) user      (1000)    10338 2023-08-04 23:19:44.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/config/schema.json
--rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/delete.py
--rw-rw-r--   0 user      (1000) user      (1000)     2062 2023-08-04 16:38:03.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)    18206 2023-08-04 07:57:47.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    30496 2023-08-04 14:49:19.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:33:03.314327 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-08-04 04:50:46.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:33:03.314327 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/setup_docker.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     3206 2023-08-04 19:52:52.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     2714 2023-08-04 23:23:34.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/servers.py
--rw-rw-r--   0 user      (1000) user      (1000)     5677 2023-08-03 17:20:44.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1607 2023-08-04 23:22:51.000000 testflows.github.runners-1.5.230804.1233303/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:33:03.314327 testflows.github.runners-1.5.230804.1233303/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-04 23:33:03.000000 testflows.github.runners-1.5.230804.1233303/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1323 2023-08-04 23:33:03.000000 testflows.github.runners-1.5.230804.1233303/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-04 23:33:03.000000 testflows.github.runners-1.5.230804.1233303/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.5.230804.1233303/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       73 2023-08-04 23:33:03.000000 testflows.github.runners-1.5.230804.1233303/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-04 23:33:03.000000 testflows.github.runners-1.5.230804.1233303/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:54:10.754567 testflows.github.runners-1.5.230804.1235410/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1235410/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-04 23:54:10.754567 testflows.github.runners-1.5.230804.1235410/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    63971 2023-08-04 02:31:51.000000 testflows.github.runners-1.5.230804.1235410/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-04 23:54:10.754567 testflows.github.runners-1.5.230804.1235410/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2195 2023-08-04 23:54:10.000000 testflows.github.runners-1.5.230804.1235410/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:54:10.750567 testflows.github.runners-1.5.230804.1235410/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:54:10.750567 testflows.github.runners-1.5.230804.1235410/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:54:10.754567 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-04 23:54:10.000000 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2837 2023-08-04 23:53:23.000000 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1995 2023-08-02 15:26:55.000000 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/api_watch.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2933 2023-08-04 06:28:52.000000 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:54:10.754567 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    25686 2023-08-04 23:37:17.000000 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    14895 2023-08-04 23:53:11.000000 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/cloud.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:54:10.754567 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/config/
+-rw-rw-r--   0 user      (1000) user      (1000)      903 2023-08-04 23:32:22.000000 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/config/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16642 2023-08-04 23:53:11.000000 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/config/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10337 2023-08-04 23:35:08.000000 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/config/schema.json
+-rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/delete.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1844 2023-08-04 23:53:11.000000 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)    18206 2023-08-04 07:57:47.000000 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    30496 2023-08-04 14:49:19.000000 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:54:10.754567 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-08-04 04:50:46.000000 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:54:10.754567 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/scripts/setup_docker.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     3206 2023-08-04 19:52:52.000000 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2714 2023-08-04 23:23:34.000000 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/servers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5677 2023-08-03 17:20:44.000000 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1607 2023-08-04 23:22:51.000000 testflows.github.runners-1.5.230804.1235410/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 23:54:10.750567 testflows.github.runners-1.5.230804.1235410/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-04 23:54:10.000000 testflows.github.runners-1.5.230804.1235410/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1323 2023-08-04 23:54:10.000000 testflows.github.runners-1.5.230804.1235410/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-04 23:54:10.000000 testflows.github.runners-1.5.230804.1235410/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.5.230804.1235410/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       73 2023-08-04 23:54:10.000000 testflows.github.runners-1.5.230804.1235410/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-04 23:54:10.000000 testflows.github.runners-1.5.230804.1235410/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.5.230804.1233303/LICENSE` & `testflows.github.runners-1.5.230804.1235410/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233303/PKG-INFO` & `testflows.github.runners-1.5.230804.1235410/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.5.230804.1233303
+Version: 1.5.230804.1235410
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.5.230804.1233303/README.rst` & `testflows.github.runners-1.5.230804.1235410/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233303/setup.py` & `testflows.github.runners-1.5.230804.1235410/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.5.230804.1233303",
+    version="1.5.230804.1235410",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/__init__.py` & `testflows.github.runners-1.5.230804.1235410/testflows/github/runners/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.5.230804.1233303"
+__version__ = "1.5.230804.1235410"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/actions.py` & `testflows.github.runners-1.5.230804.1235410/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/api_watch.py` & `testflows.github.runners-1.5.230804.1235410/testflows/github/runners/api_watch.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/args.py` & `testflows.github.runners-1.5.230804.1235410/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.5.230804.1235410/testflows/github/runners/bin/github-runners`

 * *Files 0% similar despite different names*

```diff
@@ -815,15 +815,15 @@
             args.func(args=args, config=config)
         except KeyboardInterrupt:
             if config.debug:
                 raise
         except BaseException as exc:
             if config.debug:
                 raise
-            logger.fatal(f"❗ Error: {exc}")
+            logger.critical(f"❗ Error: {exc}")
 
     else:
         config.check()
 
         with http_cache():
             with ThreadPoolExecutor(
                 max_workers=config.workers + 3, thread_name_prefix="worker"
```

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/cloud.py` & `testflows.github.runners-1.5.230804.1235410/testflows/github/runners/cloud.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
-import sys
 import tempfile
 
 from hcloud import Client
 from hcloud.ssh_keys.domain import SSHKey
 from hcloud.servers.client import BoundServer
 
 from .actions import Action
@@ -56,18 +55,18 @@
     if redeploy:
         with Action(f"Getting server {server_name}"):
             server: BoundServer = client.servers.get_by_name(server_name)
 
         uninstall(args=args, config=config, server=server)
 
         with Action("Cleaning copied scripts"):
-            ssh(server, f"rm -rf {deploy_scripts_folder}*")
+            ssh(server, f"rm -rf {deploy_scripts_folder}*", stacklevel=4)
 
         with Action("Cleaning copied configs"):
-            ssh(server, f"rm -rf {deploy_configs_folder}*")
+            ssh(server, f"rm -rf {deploy_configs_folder}*", stacklevel=4)
 
     else:
         deploy_setup_script = config.cloud.deploy.setup_script or os.path.join(
             current_dir, "scripts", "deploy", "setup.sh"
         )
 
         if args.force:
@@ -88,27 +87,27 @@
             config.default_location = check_location(client, config.default_location)
 
         with Action("Checking if default server type exists"):
             config.default_server_type = check_server_type(
                 client, config.default_server_type
             )
 
-        with Action("Checking if server type exists"):
+        with Action("Checking if cloud service server type exists"):
             config.cloud.deploy.server_type = check_server_type(
-                client=client, image=config.cloud.deploy.server_type
+                client=client, server_type=config.cloud.deploy.server_type
             )
 
-        with Action("Checking if server image exists"):
+        with Action("Checking if cloud service server image exists"):
             config.cloud.deploy.image = check_image(
                 client=client, image=config.cloud.deploy.image
             )
 
-        with Action("Checking if server location exists"):
+        with Action("Checking if cloud service server location exists"):
             config.cloud.deploy.location = check_location(
-                client=client, image=config.cloud.deploy.location
+                client=client, location=config.cloud.deploy.location
             )
 
         with Action(f"Checking if SSH key exists"):
             ssh_keys.append(check_ssh_key(client, config.ssh_key))
 
             if config.additional_ssh_keys:
                 for key in config.additional_ssh_keys:
@@ -129,28 +128,25 @@
                 server=server, timeout=config.max_server_ready_time, action=action
             )
 
         with Action("Wait for SSH connection to be ready"):
             wait_ssh(server=server, timeout=config.max_server_ready_time)
 
         with Action("Executing setup.sh script"):
-            ssh(
-                server,
-                f"bash -s  < {deploy_setup_script}",
-            )
+            ssh(server, f"bash -s  < {deploy_setup_script}", stacklevel=4)
 
     with Action(f"Installing github-runners {version}"):
         command = f"'sudo -u ubuntu pip3 install testflows.github.runners=={version}'"
 
         if version.strip().lower() == "latest":
             command = f"'sudo -u ubuntu pip3 install testflows.github.runners'"
             if redeploy:
                 command.replace("pip3 install", "pip3 install --upgrade")
 
-        ssh(server, command)
+        ssh(server, command, stacklevel=4)
 
     with Action("Copying any custom scripts"):
         ip = ip_address(server)
 
         if config.setup_script:
             with Action(f"Copying custom setup script {config.setup_script}"):
                 scp(
@@ -185,15 +181,15 @@
                 )
                 config.startup_arm64_script = os.path.join(
                     deploy_scripts_folder,
                     os.path.basename(config.startup_arm64_script),
                 )
 
     with Action("Fixing ownership of any copied scripts"):
-        ssh(server, f"chown -R ubuntu:ubuntu {deploy_scripts_folder}")
+        ssh(server, f"chown -R ubuntu:ubuntu {deploy_scripts_folder}", stacklevel=4)
 
     with Action(
         f"Copying config file{(' ' + config.config_file) if config.config_file else ''}"
     ):
         with tempfile.NamedTemporaryFile("w") as file:
             with Action(
                 f"{'Modifying' if config.config_file else 'Creating'} "
@@ -213,15 +209,15 @@
             )
             config.config_file = os.path.join(
                 deploy_configs_folder,
                 "config.yaml",
             )
 
     with Action("Fixing ownership of any copied configs"):
-        ssh(server, f"chown -R ubuntu:ubuntu {deploy_configs_folder}")
+        ssh(server, f"chown -R ubuntu:ubuntu {deploy_configs_folder}", stacklevel=4)
 
     install(args, config=config, server=server)
 
 
 def redeploy(args, config: Config):
     """Redeploy service on a existing cloud instance."""
     deploy(args=args, config=config, redeploy=True)
@@ -268,20 +264,22 @@
     stop(args, config=config, server=server)
 
     if upgrade_version:
         with Action(f"Upgrading github-runners to version {upgrade_version}"):
             ssh(
                 server,
                 f"'sudo -u ubuntu pip3 install testflows.github.runners=={upgrade_version}'",
+                stacklevel=4,
             )
     else:
         with Action(f"Upgrading github-runners the latest version"):
             ssh(
                 server,
                 f"'sudo -u ubuntu pip3 install --upgrade testflows.github.runners'",
+                stacklevel=4,
             )
 
     start(args, config=config, server=server)
 
 
 def uninstall(args, config: Config, server: BoundServer = None):
     """Uninstall github-runners service from a cloud instance."""
@@ -293,15 +291,15 @@
             client = Client(token=config.hetzner_token)
 
         with Action(f"Getting server {server_name}"):
             server: BoundServer = client.servers.get_by_name(server_name)
 
     with Action("Uninstalling service"):
         command = f"\"su - ubuntu -c 'github-runners service uninstall'\""
-        ssh(server, command)
+        ssh(server, command, stacklevel=4)
 
 
 def delete(args, config: Config):
     """Delete github-runners service running
     on Hetzner server instance by stopping the service
     and deleting the server."""
     config.check("hetzner_token")
@@ -311,15 +309,15 @@
         client = Client(token=config.hetzner_token)
 
     with Action(f"Getting server {server_name}"):
         server: BoundServer = client.servers.get_by_name(server_name)
 
     with Action("Uninstalling service"):
         command = f"\"su - ubuntu -c 'github-runners service uninstall'\""
-        ssh(server, command)
+        ssh(server, command, stacklevel=4)
 
     with Action(f"Deleting server {server_name}"):
         server.delete()
 
 
 def logs(args, config: Config, server: BoundServer = None):
     """Get cloud server service logs."""
@@ -337,15 +335,15 @@
         raise ValueError("server not found")
 
     command = (
         f"\"su - ubuntu -c 'github-runners service logs"
         + (" -f" if args.follow else "")
         + "'\""
     )
-    ssh(server, command, use_logger=False)
+    ssh(server, command, use_logger=False, stacklevel=4)
 
 
 def status(args, config: Config, server: BoundServer = None):
     """Get cloud server service status."""
     if server is None:
         config.check("hetzner_token")
         server_name = config.cloud.server_name
@@ -354,15 +352,15 @@
             client = Client(token=config.hetzner_token)
 
         with Action(f"Getting server {server_name}"):
             server = client.servers.get_by_name(server_name)
 
     with Action("Getting status"):
         command = f"\"su - ubuntu -c 'github-runners service status'\""
-        ssh(server, command)
+        ssh(server, command, stacklevel=4)
 
 
 def start(args, config: Config, server: BoundServer = None):
     """Start cloud server service."""
     if server is None:
         config.check("hetzner_token")
         server_name = config.cloud.server_name
@@ -371,15 +369,15 @@
             client = Client(token=config.hetzner_token)
 
         with Action(f"Getting server {server_name}"):
             server = client.servers.get_by_name(server_name)
 
     with Action("Starting service"):
         command = f"\"su - ubuntu -c 'github-runners service start'\""
-        ssh(server, command)
+        ssh(server, command, stacklevel=4)
 
 
 def stop(args, config: Config, server: BoundServer = None):
     """Stop cloud server service."""
     if server is None:
         config.check("hetzner_token")
         server_name = config.cloud.server_name
@@ -388,15 +386,15 @@
             client = Client(token=config.hetzner_token)
 
         with Action(f"Getting server {server_name}"):
             server = client.servers.get_by_name(server_name)
 
     with Action("Stopping service"):
         command = f"\"su - ubuntu -c 'github-runners service stop'\""
-        ssh(server, command)
+        ssh(server, command, stacklevel=4)
 
 
 def ssh_client(args, config: Config):
     """Open ssh client to github-runners service running
     on Hetzner server instance.
     """
     config.check("hetzner_token")
```

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/config/__init__.py` & `testflows.github.runners-1.5.230804.1235410/testflows/github/runners/config/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/config/config.py` & `testflows.github.runners-1.5.230804.1235410/testflows/github/runners/config/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 
 @dataclass
 class deploy:
     server_type: ServerType = server_type("cpx11")
     image: Image = image("x86:system:ubuntu-22.04")
     location: Location = None
-    setup_script: str = os.path.join(current_dir, "scripts", "deploy", "setup.sh")
+    setup_script: str = os.path.join(current_dir, "..", "scripts", "deploy", "setup.sh")
 
 
 @dataclass
 class cloud:
     server_name: str = "github-runners"
     deploy: deploy = deploy()
 
@@ -93,17 +93,21 @@
     end_of_life: int = 50
     max_runners: int = 10
     max_runners_in_workflow_run: int = None
     default_image: Image = image("x86:system:ubuntu-22.04")
     default_server_type: ServerType = server_type("cx11")
     default_location: Location = None
     workers: int = 10
-    setup_script: str = os.path.join(current_dir, "scripts", "setup.sh")
-    startup_x64_script: str = os.path.join(current_dir, "scripts", "startup_x64.sh")
-    startup_arm64_script: str = os.path.join(current_dir, "scripts", "startup_arm64.sh")
+    setup_script: str = os.path.join(current_dir, "..", "scripts", "setup.sh")
+    startup_x64_script: str = os.path.join(
+        current_dir, "..", "scripts", "startup_x64.sh"
+    )
+    startup_arm64_script: str = os.path.join(
+        current_dir, "..", "scripts", "startup_arm64.sh"
+    )
     max_powered_off_time: int = 60
     max_unused_runner_time: int = 120
     max_runner_registration_time: int = 120
     max_server_ready_time: int = 120
     scale_up_interval: int = 15
     scale_down_interval: int = 15
     debug: bool = False
```

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/config/schema.json` & `testflows.github.runners-1.5.230804.1235410/testflows/github/runners/config/schema.json`

 * *Files 0% similar despite different names*

```diff
@@ -593,55 +593,55 @@
 00002500: 7465 6d73 223a 207b 0a20 2020 2020 2020  tems": {.       
 00002510: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002520: 2020 2020 2020 2020 2020 2020 2022 6465               "de
 00002530: 7363 7269 7074 696f 6e22 3a20 224c 6162  scription": "Lab
 00002540: 656c 206e 616d 6522 2c0a 2020 2020 2020  el name",.      
 00002550: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002560: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00002570: 7970 6522 3a20 2273 7472 696e 6722 2c0a  ype": "string",.
+00002570: 7970 6522 3a20 2273 7472 696e 6722 0a20  ype": "string". 
 00002580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025a0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-000025b0: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-000025c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000025d0: 2020 2020 2020 2020 2020 2020 2022 636f               "co
-000025e0: 756e 7422 3a20 7b0a 2020 2020 2020 2020  unt": {.        
+00002590: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+000025a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000025b0: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
+000025c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025d0: 2020 2020 2020 2020 2020 2020 2263 6f75              "cou
+000025e0: 6e74 223a 207b 0a20 2020 2020 2020 2020  nt": {.         
 000025f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002600: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-00002610: 7469 6f6e 223a 2022 4e75 6d62 6572 206f  tion": "Number o
-00002620: 6620 7275 6e6e 6572 7320 696e 2074 6869  f runners in thi
-00002630: 7320 6772 6f75 702c 2064 6566 6175 6c74  s group, default
-00002640: 3a20 312e 222c 0a20 2020 2020 2020 2020  : 1.",.         
+00002600: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
+00002610: 696f 6e22 3a20 224e 756d 6265 7220 6f66  ion": "Number of
+00002620: 2072 756e 6e65 7273 2069 6e20 7468 6973   runners in this
+00002630: 2067 726f 7570 2c20 6465 6661 756c 743a   group, default:
+00002640: 2031 2e22 2c0a 2020 2020 2020 2020 2020   1.",.          
 00002650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002660: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00002670: 696e 7465 6765 7222 2c0a 2020 2020 2020  integer",.      
+00002660: 2020 2020 2020 2274 7970 6522 3a20 2269        "type": "i
+00002670: 6e74 6567 6572 222c 0a20 2020 2020 2020  nteger",.       
 00002680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002690: 2020 2020 2020 2020 2020 2265 7861 6d70            "examp
-000026a0: 6c65 7322 3a20 5b31 5d0a 2020 2020 2020  les": [1].      
+00002690: 2020 2020 2020 2020 2022 6578 616d 706c           "exampl
+000026a0: 6573 223a 205b 315d 0a20 2020 2020 2020  es": [1].       
 000026b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026c0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+000026c0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
 000026d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026e0: 2020 2020 2022 7265 706c 656e 6973 685f       "replenish_
-000026f0: 696d 6d65 6469 6174 656c 7922 3a20 7b0a  immediately": {.
+000026e0: 2020 2020 2272 6570 6c65 6e69 7368 5f69      "replenish_i
+000026f0: 6d6d 6564 6961 7465 6c79 223a 207b 0a20  mmediately": {. 
 00002700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002720: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
-00002730: 456e 6162 6c65 2072 6570 6c65 6e69 7368  Enable replenish
-00002740: 696e 6720 7374 616e 6462 7920 7275 6e6e  ing standby runn
-00002750: 6572 2070 6f6f 6c20 696d 6d65 6469 6174  er pool immediat
-00002760: 656c 792c 2064 6566 6175 6c74 3a20 7472  ely, default: tr
-00002770: 7565 2e22 2c0a 2020 2020 2020 2020 2020  ue.",.          
+00002710: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002720: 6465 7363 7269 7074 696f 6e22 3a20 2245  description": "E
+00002730: 6e61 626c 6520 7265 706c 656e 6973 6869  nable replenishi
+00002740: 6e67 2073 7461 6e64 6279 2072 756e 6e65  ng standby runne
+00002750: 7220 706f 6f6c 2069 6d6d 6564 6961 7465  r pool immediate
+00002760: 6c79 2c20 6465 6661 756c 743a 2074 7275  ly, default: tru
+00002770: 652e 222c 0a20 2020 2020 2020 2020 2020  e.",.           
 00002780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002790: 2020 2020 2020 2274 7970 6522 3a20 2262        "type": "b
-000027a0: 6f6f 6c65 616e 222c 0a20 2020 2020 2020  oolean",.       
+00002790: 2020 2020 2022 7479 7065 223a 2022 626f       "type": "bo
+000027a0: 6f6c 6561 6e22 2c0a 2020 2020 2020 2020  olean",.        
 000027b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027c0: 2020 2020 2020 2020 2022 6578 616d 706c           "exampl
-000027d0: 6573 223a 205b 7472 7565 2c20 6661 6c73  es": [true, fals
-000027e0: 655d 0a20 2020 2020 2020 2020 2020 2020  e].             
-000027f0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00002800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002810: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00002820: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00002830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002840: 207d 0a20 2020 2020 2020 2020 2020 207d   }.            }
-00002850: 0a20 2020 2020 2020 207d 0a20 2020 207d  .        }.    }
-00002860: 0a7d                                     .}
+000027c0: 2020 2020 2020 2020 2265 7861 6d70 6c65          "example
+000027d0: 7322 3a20 5b74 7275 652c 2066 616c 7365  s": [true, false
+000027e0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+000027f0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00002800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002810: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00002820: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00002830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002840: 7d0a 2020 2020 2020 2020 2020 2020 7d0a  }.            }.
+00002850: 2020 2020 2020 2020 7d0a 2020 2020 7d0a          }.    }.
+00002860: 7d                                       }
```

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/delete.py` & `testflows.github.runners-1.5.230804.1235410/testflows/github/runners/delete.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/logger.py` & `testflows.github.runners-1.5.230804.1235410/testflows/github/runners/logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,21 +58,12 @@
 def default_config(level=logging.INFO):
     """Apply default logging configuration."""
     global logger
 
     logger.logger.setLevel(level)
     handler = logging.StreamHandler(sys.stdout)
     formatter = logging.Formatter(
-        fmt=(
-            "%(asctime)s "
-            "%(levelname)-5s "
-            "%(message)-70s "
-            "%(run_id)-12s "
-            "%(job_id)-12s "
-            "%(server_name)-30s "
-            "%(funcName)-10s "
-            "%(interval)s "
-        ),
-        datefmt="%H%M%S",
+        fmt=("%(asctime)s " "%(message)s"),
+        datefmt="%H:%M:%S",
     )
     handler.setFormatter(formatter)
     logger.logger.addHandler(handler)
```

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/request.py` & `testflows.github.runners-1.5.230804.1235410/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.5.230804.1235410/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.5.230804.1235410/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.5.230804.1235410/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.5.230804.1235410/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.5.230804.1235410/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/setup_docker.sh` & `testflows.github.runners-1.5.230804.1235410/testflows/github/runners/scripts/setup_docker.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.5.230804.1235410/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.5.230804.1235410/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/server.py` & `testflows.github.runners-1.5.230804.1235410/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/servers.py` & `testflows.github.runners-1.5.230804.1235410/testflows/github/runners/servers.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/service.py` & `testflows.github.runners-1.5.230804.1235410/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows/github/runners/shell.py` & `testflows.github.runners-1.5.230804.1235410/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.5.230804.1235410/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.5.230804.1233303
+Version: 1.5.230804.1235410
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.5.230804.1233303/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.5.230804.1235410/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

