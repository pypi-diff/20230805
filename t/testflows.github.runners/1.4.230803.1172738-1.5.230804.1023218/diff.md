# Comparing `tmp/testflows.github.runners-1.4.230803.1172738.tar.gz` & `tmp/testflows.github.runners-1.5.230804.1023218.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.4.230803.1172738.tar", last modified: Thu Aug  3 17:27:38 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.5.230804.1023218.tar", last modified: Fri Aug  4 02:32:18 2023, max compression
```

## Comparing `testflows.github.runners-1.4.230803.1172738.tar` & `testflows.github.runners-1.5.230804.1023218.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 17:27:38.865339 testflows.github.runners-1.4.230803.1172738/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230803.1172738/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-03 17:27:38.865339 testflows.github.runners-1.4.230803.1172738/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    63971 2023-08-03 02:12:02.000000 testflows.github.runners-1.4.230803.1172738/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-03 17:27:38.865339 testflows.github.runners-1.4.230803.1172738/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2043 2023-08-03 17:27:38.000000 testflows.github.runners-1.4.230803.1172738/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 17:27:38.861339 testflows.github.runners-1.4.230803.1172738/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 17:27:38.861339 testflows.github.runners-1.4.230803.1172738/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 17:27:38.865339 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-03 17:27:38.000000 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1741 2023-08-02 11:42:30.000000 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1995 2023-08-02 15:26:55.000000 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/api_watch.py
--rw-rw-r--   0 user      (1000) user      (1000)     3019 2023-08-02 18:47:51.000000 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 17:27:38.865339 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    26203 2023-08-03 17:09:40.000000 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    13640 2023-08-03 17:20:44.000000 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     5290 2023-08-03 17:26:51.000000 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/config.py
--rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/delete.py
--rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)    15656 2023-08-02 20:33:51.000000 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    27693 2023-08-03 16:56:37.000000 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 17:27:38.865339 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 17:27:38.865339 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/scripts/setup_docker.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     3032 2023-08-02 20:36:59.000000 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     5677 2023-08-03 17:20:44.000000 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1512 2023-08-02 11:42:30.000000 testflows.github.runners-1.4.230803.1172738/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-03 17:27:38.861339 testflows.github.runners-1.4.230803.1172738/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-03 17:27:38.000000 testflows.github.runners-1.4.230803.1172738/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1192 2023-08-03 17:27:38.000000 testflows.github.runners-1.4.230803.1172738/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-03 17:27:38.000000 testflows.github.runners-1.4.230803.1172738/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.4.230803.1172738/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       61 2023-08-03 17:27:38.000000 testflows.github.runners-1.4.230803.1172738/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-03 17:27:38.000000 testflows.github.runners-1.4.230803.1172738/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 02:32:18.377853 testflows.github.runners-1.5.230804.1023218/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1023218/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-04 02:32:18.377853 testflows.github.runners-1.5.230804.1023218/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    63971 2023-08-04 02:31:51.000000 testflows.github.runners-1.5.230804.1023218/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-04 02:32:18.377853 testflows.github.runners-1.5.230804.1023218/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2097 2023-08-04 02:32:18.000000 testflows.github.runners-1.5.230804.1023218/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 02:32:18.373853 testflows.github.runners-1.5.230804.1023218/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 02:32:18.373853 testflows.github.runners-1.5.230804.1023218/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 02:32:18.377853 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-04 02:32:18.000000 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1741 2023-08-02 11:42:30.000000 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1995 2023-08-02 15:26:55.000000 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/api_watch.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2817 2023-08-04 02:24:33.000000 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 02:32:18.377853 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    27175 2023-08-04 02:11:23.000000 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    13861 2023-08-04 02:24:33.000000 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6450 2023-08-04 02:24:33.000000 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/delete.py
+-rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15656 2023-08-02 20:33:51.000000 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    27597 2023-08-04 01:41:00.000000 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 02:32:18.377853 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 02:32:18.377853 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/scripts/setup_docker.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     3032 2023-08-02 20:36:59.000000 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2717 2023-08-04 02:24:33.000000 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/servers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5677 2023-08-03 17:20:44.000000 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1512 2023-08-02 11:42:30.000000 testflows.github.runners-1.5.230804.1023218/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 02:32:18.377853 testflows.github.runners-1.5.230804.1023218/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-04 02:32:18.000000 testflows.github.runners-1.5.230804.1023218/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1228 2023-08-04 02:32:18.000000 testflows.github.runners-1.5.230804.1023218/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-04 02:32:18.000000 testflows.github.runners-1.5.230804.1023218/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.5.230804.1023218/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       73 2023-08-04 02:32:18.000000 testflows.github.runners-1.5.230804.1023218/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-04 02:32:18.000000 testflows.github.runners-1.5.230804.1023218/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.4.230803.1172738/LICENSE` & `testflows.github.runners-1.5.230804.1023218/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1172738/PKG-INFO` & `testflows.github.runners-1.5.230804.1023218/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.4.230803.1172738
+Version: 1.5.230804.1023218
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.4.230803.1172738/README.rst` & `testflows.github.runners-1.5.230804.1023218/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1172738/setup.py` & `testflows.github.runners-1.5.230804.1023218/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.4.230803.1172738",
+    version="1.5.230804.1023218",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
@@ -45,10 +45,15 @@
     package_data={
         "testflows.github.runners.scripts": ["*.sh"],
         "testflows.github.runners.scripts.deploy": ["*.sh"],
         "testflows.github.runners.bin": ["github-runners"],
     },
     scripts=["testflows/github/runners/bin/github-runners"],
     zip_safe=False,
-    install_requires=["PyGithub==1.59.0", "hcloud==1.26.0", "requests-cache==1.1.0"],
+    install_requires=[
+        "PyGithub==1.59.0",
+        "hcloud==1.26.0",
+        "requests-cache==1.1.0",
+        "PyYAML==6.0",
+    ],
     extras_require={"dev": []},
 )
```

### Comparing `testflows.github.runners-1.4.230803.1172738/testflows/github/runners/__init__.py` & `testflows.github.runners-1.5.230804.1023218/testflows/github/runners/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.4.230803.1172738"
+__version__ = "1.5.230804.1023218"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.4.230803.1172738/testflows/github/runners/actions.py` & `testflows.github.runners-1.5.230804.1023218/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1172738/testflows/github/runners/api_watch.py` & `testflows.github.runners-1.5.230804.1023218/testflows/github/runners/api_watch.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1172738/testflows/github/runners/args.py` & `testflows.github.runners-1.5.230804.1023218/testflows/github/runners/args.py`

 * *Files 7% similar despite different names*

```diff
@@ -87,19 +87,17 @@
 def server_type(v):
     """Server type argument. Example: cx11"""
     return ServerType(name=v)
 
 
 def config_type(v):
     """Program configuration file type."""
-    from .config import Config
+    from .config import parse_config
 
     v = path_type(v)
     try:
-        config_module = SourceFileLoader("config", v).load_module()
-        assert hasattr(config_module, "config"), "config not defined"
-        assert isinstance(config_module.config, Config), "invalid config type"
+        config = parse_config(v)
+        config.config_file = v
     except Exception as e:
         raise ArgumentTypeError(str(e))
 
-    config_module.config.config_file = v
-    return config_module.config
+    return config
```

### Comparing `testflows.github.runners-1.4.230803.1172738/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.5.230804.1023218/testflows/github/runners/bin/github-runners`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import sys
 import time
-import hashlib
 import tempfile
 import logging
 import threading
 import logging.config
 
 from contextlib import contextmanager
 from concurrent.futures import ThreadPoolExecutor, Future
@@ -42,14 +41,15 @@
 from testflows.github.runners.logger import logger
 from testflows.github.runners.config import Config, check_image, check_ssh_key
 
 import testflows.github.runners.args as args
 import testflows.github.runners.cloud as cloud
 import testflows.github.runners.service as service
 import testflows.github.runners.delete as delete
+import testflows.github.runners.servers as servers
 
 from requests_cache import DO_NOT_CACHE, EXPIRE_IMMEDIATELY, install_cache
 from requests_cache.backends.filesystem import FileCache
 
 description = """Auto-scaling GitHub Actions runners service using Hetzner Cloud.
 
     Service that starts and monitors queued up GitHub Actions workflows.
@@ -81,18 +81,18 @@
         help="show program's license and exit",
         version=f"{__license__}",
     )
 
     parser.add_argument(
         "-c",
         "--config",
-        metavar="path",
+        metavar="yaml",
         dest="config_file",
         type=args.config_type,
-        help="program configuration file",
+        help="program yaml configuration file",
         default=None,
     )
 
     parser.add_argument(
         "--github-token",
         type=str,
         help="GitHub token, default: $GITHUB_TOKEN environment variable",
@@ -276,14 +276,51 @@
             "'cloud delete' command to delete it."
         ),
         formatter_class=RawTextHelpFormatter,
     )
 
     delete_parser.set_defaults(func=delete.all)
 
+    list_parser = commands.add_parser(
+        "list",
+        help="list all servers",
+        description="List runner servers.",
+        formatter_class=RawTextHelpFormatter,
+    )
+
+    list_parser.set_defaults(func=servers.list)
+
+    ssh_client_parser = commands.add_parser(
+        "ssh",
+        help="ssh to a server",
+        description="Open SSH client to a server.",
+        formatter_class=RawTextHelpFormatter,
+    )
+
+    ssh_client_parser.add_argument(
+        "name",
+        help="name of the server",
+        type=str,
+    )
+
+    ssh_client_parser.set_defaults(func=servers.ssh_client)
+
+    ssh_client_commands = ssh_client_parser.add_subparsers(
+        title="commands", metavar="command", description=None, help=None
+    )
+
+    ssh_client_command_parser = ssh_client_commands.add_parser(
+        "command",
+        help="print ssh command to the server",
+        description="Get SSH command to connect to the server.",
+        formatter_class=RawTextHelpFormatter,
+    )
+
+    ssh_client_command_parser.set_defaults(func=servers.ssh_client_command)
+
     cloud_parser = commands.add_parser(
         "cloud",
         help="cloud service commands",
         description="Deploying and running application as a service on a cloud instance.",
         formatter_class=RawTextHelpFormatter,
     )
 
@@ -633,15 +670,15 @@
         yield
 
 
 def main(
     config, scripts: Scripts, worker_pool: ThreadPoolExecutor, terminate_timeout=30
 ):
     """Auto-scale runners service."""
-    user_ssh_keys: list[SSHKey] = []
+    ssh_keys: list[SSHKey] = []
     terminate = threading.Event()
 
     try:
         with Action("Logging in to Hetzner Cloud"):
             client = Client(token=config.hetzner_token)
 
         with Action("Logging in to GitHub"):
@@ -650,32 +687,30 @@
         with Action(f"Getting repository {config.github_repository}"):
             repo: Repository = github.get_repo(config.github_repository)
 
         with Action("Checking if default image exists"):
             config.default_image = check_image(client, config.default_image)
 
         with Action(f"Checking if SSH key exists"):
-            ssh_key: SSHKey = check_ssh_key(client, config.ssh_key)
+            ssh_keys.append(check_ssh_key(client, config.ssh_key))
 
-        if config.user_ssh_keys:
-            with Action(f"Checking if user SSH keys exist"):
-                for user_ssh_key in config.user_ssh_keys:
-                    user_ssh_keys.append(check_ssh_key(client, user_ssh_key))
+            if config.ssh_keys:
+                for key in config.ssh_keys:
+                    ssh_keys.append(check_ssh_key(client, key))
 
         try:
             with Action("Creating scale up service"):
                 scale_up_service: Future = worker_pool.submit(
                     scale_up,
                     terminate=terminate,
                     recycle=config.recycle,
                     server_prices=config.server_prices,
                     with_label=config.with_label,
                     scripts=scripts,
-                    ssh_key=ssh_key,
-                    user_ssh_keys=user_ssh_keys,
+                    ssh_keys=ssh_keys,
                     default_server_type=config.default_server_type,
                     default_image=config.default_image,
                     default_location=config.default_location,
                     worker_pool=worker_pool,
                     hetzner_token=config.hetzner_token,
                     github_token=config.github_token,
                     github_repository=config.github_repository,
@@ -688,15 +723,15 @@
                 )
 
             with Action("Creating scale down service"):
                 scale_down_service: Future = worker_pool.submit(
                     scale_down,
                     recycle=config.recycle,
                     end_of_life=config.end_of_life,
-                    ssh_key=ssh_key,
+                    ssh_key=ssh_keys[0],
                     hetzner_token=config.hetzner_token,
                     github_token=config.github_token,
                     github_repository=config.github_repository,
                     terminate=terminate,
                     max_powered_off_time=config.max_powered_off_time,
                     max_unused_runner_time=config.max_unused_runner_time,
                     max_runner_registration_time=config.max_runner_registration_time,
```

### Comparing `testflows.github.runners-1.4.230803.1172738/testflows/github/runners/cloud.py` & `testflows.github.runners-1.5.230804.1023218/testflows/github/runners/cloud.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,38 +10,47 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import sys
-import hashlib
+import tempfile
 
 from hcloud import Client
 from hcloud.ssh_keys.domain import SSHKey
 from hcloud.servers.client import BoundServer
 
 from .actions import Action
-from .config import Config, check_image
+from .config import (
+    Config,
+    check_image,
+    check_ssh_key,
+    write as write_config,
+    read as read_config,
+)
 from . import __version__
 
 from .server import wait_ready, wait_ssh, ssh, scp, ip_address, ssh_command
+from .servers import ssh_client as server_ssh_client
+from .servers import ssh_client_command as server_ssh_client_command
 from .service import command_options
 
 current_dir = os.path.dirname(__file__)
 deploy_scripts_folder = "/home/ubuntu/.github-runners/scripts/"
 deploy_configs_folder = "/home/ubuntu/.github-runners/configs/"
 
 
 def deploy(args, config: Config, redeploy=False):
     """Deploy or redeploy github-runners as a service to a
     new Hetzner server instance."""
     config.check()
     version = args.version or __version__
     server_name = config.cloud.server_name
+    ssh_keys: list[SSHKey] = []
 
     with Action("Logging in to Hetzner Cloud"):
         client = Client(token=config.hetzner_token)
 
     if redeploy:
         with Action(f"Getting server {server_name}"):
             server: BoundServer = client.servers.get_by_name(server_name)
@@ -75,32 +84,27 @@
 
         with Action("Checking if server image exists"):
             config.cloud.deploy.image = check_image(
                 client=client, image=config.cloud.deploy.image
             )
 
         with Action(f"Checking if SSH key exists"):
-            with open(config.ssh_key, "r", encoding="utf-8") as ssh_key_file:
-                public_key = ssh_key_file.read()
-            key_name = hashlib.md5(public_key.encode("utf-8")).hexdigest()
-            ssh_key = SSHKey(name=key_name, public_key=public_key)
-
-            if not client.ssh_keys.get_by_name(name=ssh_key.name):
-                with Action(f"Creating SSH key {ssh_key.name}"):
-                    client.ssh_keys.create(
-                        name=ssh_key.name, public_key=ssh_key.public_key
-                    )
+            ssh_keys.append(check_ssh_key(client, config.ssh_key))
+
+            if config.ssh_keys:
+                for key in config.ssh_keys:
+                    ssh_keys.append(check_ssh_key(client, key))
 
         with Action(f"Creating new server"):
             response = client.servers.create(
                 name=server_name,
                 server_type=config.cloud.deploy.server_type,
                 image=config.cloud.deploy.image,
                 location=config.cloud.deploy.location,
-                ssh_keys=[ssh_key],
+                ssh_keys=ssh_keys,
             )
             server: BoundServer = response.server
 
         with Action(f"Waiting for server to be ready") as action:
             wait_ready(
                 server=server, timeout=config.max_server_ready_time, action=action
             )
@@ -163,19 +167,33 @@
                     deploy_scripts_folder,
                     os.path.basename(config.startup_arm64_script),
                 )
 
     with Action("Fixing ownership of any copied scripts"):
         ssh(server, f"chown -R ubuntu:ubuntu {deploy_scripts_folder}")
 
-    if config.config_file:
-        with Action(f"Copying config file {config.config_file}"):
+    with Action(
+        f"Copying config file{(' ' + config.config_file) if config.config_file else ''}"
+    ):
+        with tempfile.NamedTemporaryFile("w") as file:
+            with Action(
+                f"{'Modifying' if config.config_file else 'Creating'} "
+                "config file and adding this SSH key to the SSH keys list"
+            ):
+                raw_config = {}
+                if config.config_file:
+                    raw_config = read_config(config.config_file)
+                keys = raw_config.get("ssh_keys", [])
+                keys.append(ssh_keys[0].public_key)
+                raw_config["ssh_keys"] = list(set(keys))
+                write_config(file, raw_config)
+                file.flush()
             scp(
-                source=config.config_file,
-                destination=f"root@{ip}:{deploy_configs_folder}.",
+                source=file.name,
+                destination=f"root@{ip}:{deploy_configs_folder}config.yaml",
             )
             config.config_file = os.path.join(
                 deploy_configs_folder,
                 os.path.basename(config.config_file),
             )
 
     with Action("Fixing ownership of any copied configs"):
@@ -360,27 +378,18 @@
 def ssh_client(args, config: Config):
     """Open ssh client to github-runners service running
     on Hetzner server instance.
     """
     config.check("hetzner_token")
     server_name = config.cloud.server_name
 
-    with Action("Logging in to Hetzner Cloud"):
-        client = Client(token=config.hetzner_token)
-
-    with Action(f"Getting server {server_name}"):
-        server: BoundServer = client.servers.get_by_name(server_name)
-
-    with Action("Opening SSH client"):
-        os.system(ssh_command(server=server))
+    server_ssh_client(args=args, config=config, server_name=server_name)
 
 
 def ssh_client_command(args, config: Config):
     """Return ssh command to connect to github-runners service running
     on Hetzner server instance.
     """
     config.check("hetzner_token")
     server_name = config.cloud.server_name
 
-    client = Client(token=config.hetzner_token)
-    server: BoundServer = client.servers.get_by_name(server_name)
-    print(ssh_command(server=server), file=sys.stdout)
+    server_ssh_client_command(args=args, config=config, server_name=server_name)
```

### Comparing `testflows.github.runners-1.4.230803.1172738/testflows/github/runners/config.py` & `testflows.github.runners-1.5.230804.1023218/testflows/github/runners/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,37 @@
 import os
+import re
 import sys
+import yaml
 import hashlib
 
 from dataclasses import dataclass
 
 from hcloud import Client
 from hcloud.images.domain import Image
 from hcloud.ssh_keys.domain import SSHKey
 
 import testflows.github.runners.args as args
 
 from .actions import Action
 
+# add support for parsing ${ENV_VAR} in config
+env_pattern = re.compile(r".*?\${(.*?)}.*?")
+
+
+def env_constructor(loader, node):
+    value = loader.construct_scalar(node)
+    for group in env_pattern.findall(value):
+        value = value.replace(f"${{{group}}}", os.environ.get(group))
+    return value
+
+
+yaml.add_implicit_resolver("!pathex", env_pattern)
+yaml.add_constructor("!pathex", env_constructor)
+
 
 class ImageNotFoundError(Exception):
     pass
 
 
 path = args.path_type
 count = args.count_type
@@ -50,15 +66,15 @@
 class Config:
     """Program configuration class."""
 
     github_token: str = os.getenv("GITHUB_TOKEN")
     github_repository: str = os.getenv("GITHUB_REPOSITORY")
     hetzner_token: str = os.getenv("HETZNER_TOKEN")
     ssh_key: str = os.path.expanduser("~/.ssh/id_rsa.pub")
-    user_ssh_keys: dict[str, str] = None
+    ssh_keys: list[str] = None
     with_label: str = None
     recycle: bool = True
     end_of_life: count = 50
     max_runners: count = 10
     max_runners_in_workflow_run: count = None
     default_image: image = image("x86:system:ubuntu-22.04")
     default_server_type: server_type = server_type("cx11")
@@ -81,26 +97,26 @@
     server_prices: dict[str, float] = None
     config_file: path = None
 
     def __post_init__(self):
         if self.standby_runners is None:
             self.standby_runners = []
 
-        if self.user_ssh_keys is None:
-            self.user_ssh_keys = []
+        if self.ssh_keys is None:
+            self.ssh_keys = []
 
     def update(self, args):
         """Update configuration file using command line arguments."""
         for attr in vars(self):
             if attr in [
                 "config_file",
                 "logger_config",
                 "cloud",
                 "standby_runners",
-                "user_ssh_keys",
+                "ssh_keys",
                 "server_prices",
             ]:
                 continue
 
             arg_value = getattr(args, attr)
 
             if arg_value is not None:
@@ -134,14 +150,43 @@
             print(
                 f"argument error: --{name.lower().replace('_','-')} is not defined",
                 file=sys.stderr,
             )
             sys.exit(1)
 
 
+def read(path: str):
+    """Load raw configuration document."""
+    with open(path, "r") as f:
+        return yaml.load(f, Loader=yaml.SafeLoader)
+
+
+def write(file, doc: dict):
+    """Write raw configuration document to file."""
+    yaml.dump(doc, file)
+
+
+def parse_config(path: str):
+    """Load and parse yaml configuration file into config object."""
+    with open(path, "r") as f:
+        doc = yaml.load(f, Loader=yaml.SafeLoader)
+
+    if doc.get("cloud"):
+        doc["cloud"] = cloud(
+            doc["cloud"], deploy=deploy(**doc["cloud"].get("deploy", {}))
+        )
+
+    if doc.get("standby_runners"):
+        doc["standby_runners"] = [
+            standby_runner(**entry) for entry in doc["standby_runners"]
+        ]
+
+    return Config(**doc)
+
+
 def check_ssh_key(client: Client, ssh_key: str):
     """Check that ssh key exists if not create it."""
 
     with open(ssh_key, "r", encoding="utf-8") as ssh_key_file:
         public_key = ssh_key_file.read()
 
     key_name = hashlib.md5(public_key.encode("utf-8")).hexdigest()
```

### Comparing `testflows.github.runners-1.4.230803.1172738/testflows/github/runners/delete.py` & `testflows.github.runners-1.5.230804.1023218/testflows/github/runners/delete.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1172738/testflows/github/runners/logger.py` & `testflows.github.runners-1.5.230804.1023218/testflows/github/runners/logger.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1172738/testflows/github/runners/request.py` & `testflows.github.runners-1.5.230804.1023218/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1172738/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.5.230804.1023218/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1172738/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.5.230804.1023218/testflows/github/runners/scale_up.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,38 +194,37 @@
     server_type: ServerType,
     server_location: Location,
     server_image: Image,
     startup_script: str,
     setup_script: str,
     github_token: str,
     github_repository: str,
-    ssh_key: SSHKey,
-    user_ssh_keys: list[SSHKey],
+    ssh_keys: list[SSHKey],
     timeout=60,
 ):
     """Create specified number of server instances."""
     client = Client(token=hetzner_token)
 
     server_labels = {
         f"github-runner-label-{i}": value for i, value in enumerate(labels)
     }
-    server_labels[server_ssh_key_label] = ssh_key.name
+    server_labels[server_ssh_key_label] = ssh_keys[0].name
 
     with Action(f"Validating server {name} labels"):
         valid, error_msg = LabelValidator.validate_verbose(labels=server_labels)
         if not valid:
             raise ValueError(f"invalid server labels {server_labels}: {error_msg}")
 
     with Action(f"Creating server {name} with labels {labels}"):
         response = client.servers.create(
             name=name,
             server_type=server_type,
             location=server_location,
             image=server_image,
-            ssh_keys=[ssh_key] + user_ssh_keys,
+            ssh_keys=ssh_keys,
             labels=server_labels,
         )
         server: BoundServer = response.server
 
     with Action(f"Waiting for server {server.name} to be ready") as action:
         wait_ready(server=server, timeout=timeout, action=action)
 
@@ -370,16 +369,15 @@
     server_prices: dict[str, float],
     with_label: str,
     scripts: Scripts,
     worker_pool: ThreadPoolExecutor,
     github_token: str,
     github_repository: str,
     hetzner_token: str,
-    ssh_key: SSHKey,
-    user_ssh_keys: list[SSHKey],
+    ssh_keys: list[SSHKey],
     default_server_type: ServerType,
     default_location: Location,
     default_image: Image,
     interval: int,
     max_servers: int,
     max_servers_in_workflow_run: int,
     max_server_ready_time: int,
@@ -426,29 +424,29 @@
                     ):
                         pass
 
                     if recyclable_server_match(
                         server=server,
                         server_type=server_type,
                         server_location=server_location,
-                        ssh_key=ssh_key,
+                        ssh_key=ssh_keys[0],
                     ):
                         future = worker_pool.submit(
                             recycle_server,
                             server_name=server.name,
                             hetzner_token=hetzner_token,
                             setup_worker_pool=setup_worker_pool,
                             labels=labels,
                             name=name,
                             server_image=server_image,
                             startup_script=startup_script,
                             setup_script=scripts.setup,
                             github_token=github_token,
                             github_repository=github_repository,
-                            ssh_key=ssh_key,
+                            ssh_key=ssh_keys[0],
                             timeout=max_server_ready_time,
                         )
                         future.server_name = name
                         futures.append(future)
                         servers.pop(servers.index(server))
                         servers.append(
                             RunnerServer(
@@ -519,16 +517,15 @@
             server_type=server_type,
             server_location=server_location,
             server_image=server_image,
             setup_script=scripts.setup,
             startup_script=startup_script,
             github_token=github_token,
             github_repository=github_repository,
-            ssh_key=ssh_key,
-            user_ssh_keys=user_ssh_keys,
+            ssh_keys=ssh_keys,
             timeout=max_server_ready_time,
         )
         future.server_name = name
         futures.append(future)
         servers.append(
             RunnerServer(
                 name=name,
```

### Comparing `testflows.github.runners-1.4.230803.1172738/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.5.230804.1023218/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1172738/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.5.230804.1023218/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1172738/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.5.230804.1023218/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1172738/testflows/github/runners/scripts/setup_docker.sh` & `testflows.github.runners-1.5.230804.1023218/testflows/github/runners/scripts/setup_docker.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1172738/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.5.230804.1023218/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1172738/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.5.230804.1023218/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1172738/testflows/github/runners/server.py` & `testflows.github.runners-1.5.230804.1023218/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1172738/testflows/github/runners/service.py` & `testflows.github.runners-1.5.230804.1023218/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1172738/testflows/github/runners/shell.py` & `testflows.github.runners-1.5.230804.1023218/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230803.1172738/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.5.230804.1023218/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.4.230803.1172738
+Version: 1.5.230804.1023218
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.4.230803.1172738/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.5.230804.1023218/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 testflows/github/runners/config.py
 testflows/github/runners/delete.py
 testflows/github/runners/logger.py
 testflows/github/runners/request.py
 testflows/github/runners/scale_down.py
 testflows/github/runners/scale_up.py
 testflows/github/runners/server.py
+testflows/github/runners/servers.py
 testflows/github/runners/service.py
 testflows/github/runners/shell.py
 testflows/github/runners/bin/github-runners
 testflows/github/runners/scripts/__init__.py
 testflows/github/runners/scripts/setup.sh
 testflows/github/runners/scripts/setup_docker.sh
 testflows/github/runners/scripts/startup_arm64.sh
```

