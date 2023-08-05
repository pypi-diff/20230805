# Comparing `tmp/AIMM-1.1.dev2.tar.gz` & `tmp/AIMM-1.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AIMM-1.1.dev2.tar", last modified: Sat Feb 18 01:23:37 2023, max compression
+gzip compressed data, was "AIMM-1.1.dev3.tar", last modified: Sat Aug  5 19:32:52 2023, max compression
```

## Comparing `AIMM-1.1.dev2.tar` & `AIMM-1.1.dev3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 zlatan    (1000) zlatan    (1000)        0 2023-02-18 01:23:37.413120 AIMM-1.1.dev2/
-drwxr-xr-x   0 zlatan    (1000) zlatan    (1000)        0 2023-02-18 01:23:37.409787 AIMM-1.1.dev2/AIMM.egg-info/
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)     2238 2023-02-18 01:23:37.000000 AIMM-1.1.dev2/AIMM.egg-info/PKG-INFO
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)      779 2023-02-18 01:23:37.000000 AIMM-1.1.dev2/AIMM.egg-info/SOURCES.txt
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)        1 2023-02-18 01:23:37.000000 AIMM-1.1.dev2/AIMM.egg-info/dependency_links.txt
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)       54 2023-02-18 01:23:37.000000 AIMM-1.1.dev2/AIMM.egg-info/entry_points.txt
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)       54 2023-02-18 01:23:37.000000 AIMM-1.1.dev2/AIMM.egg-info/requires.txt
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)        5 2023-02-18 01:23:37.000000 AIMM-1.1.dev2/AIMM.egg-info/top_level.txt
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)    11357 2022-12-27 19:52:37.000000 AIMM-1.1.dev2/LICENSE
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)       51 2023-02-05 11:29:51.000000 AIMM-1.1.dev2/MANIFEST.in
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)     2238 2023-02-18 01:23:37.413120 AIMM-1.1.dev2/PKG-INFO
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)     1601 2022-12-27 19:52:37.000000 AIMM-1.1.dev2/README.rst
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)        9 2023-02-18 01:21:30.000000 AIMM-1.1.dev2/VERSION
-drwxr-xr-x   0 zlatan    (1000) zlatan    (1000)        0 2023-02-18 01:23:37.409787 AIMM-1.1.dev2/aimm/
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)        0 2022-12-27 19:52:37.000000 AIMM-1.1.dev2/aimm/__init__.py
-drwxr-xr-x   0 zlatan    (1000) zlatan    (1000)        0 2023-02-18 01:23:37.409787 AIMM-1.1.dev2/aimm/client/
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)        0 2022-12-27 19:52:37.000000 AIMM-1.1.dev2/aimm/client/__init__.py
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)     7831 2023-02-18 01:21:30.000000 AIMM-1.1.dev2/aimm/client/repl.py
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)      616 2023-02-18 00:15:42.000000 AIMM-1.1.dev2/aimm/common.py
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)     7734 2023-02-18 01:23:34.000000 AIMM-1.1.dev2/aimm/json_schema_repo.json
-drwxr-xr-x   0 zlatan    (1000) zlatan    (1000)        0 2023-02-18 01:23:37.413120 AIMM-1.1.dev2/aimm/plugins/
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)      704 2023-02-18 00:15:42.000000 AIMM-1.1.dev2/aimm/plugins/__init__.py
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)     3093 2023-02-18 00:15:42.000000 AIMM-1.1.dev2/aimm/plugins/common.py
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)     9945 2023-02-18 00:15:42.000000 AIMM-1.1.dev2/aimm/plugins/decorators.py
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)     2858 2023-02-18 00:15:42.000000 AIMM-1.1.dev2/aimm/plugins/execute.py
-drwxr-xr-x   0 zlatan    (1000) zlatan    (1000)        0 2023-02-18 01:23:37.413120 AIMM-1.1.dev2/aimm/server/
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)        0 2022-12-27 19:52:37.000000 AIMM-1.1.dev2/aimm/server/__init__.py
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)       96 2023-02-18 00:15:42.000000 AIMM-1.1.dev2/aimm/server/__main__.py
-drwxr-xr-x   0 zlatan    (1000) zlatan    (1000)        0 2023-02-18 01:23:37.413120 AIMM-1.1.dev2/aimm/server/backend/
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)        0 2022-12-27 19:52:37.000000 AIMM-1.1.dev2/aimm/server/backend/__init__.py
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)      681 2023-02-18 00:15:42.000000 AIMM-1.1.dev2/aimm/server/backend/dummy.py
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)     3118 2023-02-18 00:15:42.000000 AIMM-1.1.dev2/aimm/server/backend/event.py
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)     3297 2023-02-18 00:15:42.000000 AIMM-1.1.dev2/aimm/server/backend/sqlite.py
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)     9683 2023-02-18 00:15:42.000000 AIMM-1.1.dev2/aimm/server/common.py
-drwxr-xr-x   0 zlatan    (1000) zlatan    (1000)        0 2023-02-18 01:23:37.413120 AIMM-1.1.dev2/aimm/server/control/
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)        0 2022-12-27 19:52:37.000000 AIMM-1.1.dev2/aimm/server/control/__init__.py
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)     9510 2023-02-18 01:21:30.000000 AIMM-1.1.dev2/aimm/server/control/event.py
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)     8052 2023-02-18 00:15:42.000000 AIMM-1.1.dev2/aimm/server/control/repl.py
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)    10252 2023-02-18 00:15:42.000000 AIMM-1.1.dev2/aimm/server/engine.py
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)     5418 2023-02-18 00:15:42.000000 AIMM-1.1.dev2/aimm/server/main.py
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)     7435 2023-02-18 00:15:42.000000 AIMM-1.1.dev2/aimm/server/mprocess.py
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)       61 2023-02-18 00:39:48.000000 AIMM-1.1.dev2/pyproject.toml
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)       38 2023-02-18 01:23:37.413120 AIMM-1.1.dev2/setup.cfg
--rw-r--r--   0 zlatan    (1000) zlatan    (1000)     1338 2023-02-18 00:15:42.000000 AIMM-1.1.dev2/setup.py
+drwxr-xr-x   0 zlatan    (1000) zlatan    (1000)        0 2023-08-05 19:32:52.073220 AIMM-1.1.dev3/
+drwxr-xr-x   0 zlatan    (1000) zlatan    (1000)        0 2023-08-05 19:32:52.069887 AIMM-1.1.dev3/AIMM.egg-info/
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)     2238 2023-08-05 19:32:52.000000 AIMM-1.1.dev3/AIMM.egg-info/PKG-INFO
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)      779 2023-08-05 19:32:52.000000 AIMM-1.1.dev3/AIMM.egg-info/SOURCES.txt
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)        1 2023-08-05 19:32:52.000000 AIMM-1.1.dev3/AIMM.egg-info/dependency_links.txt
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)       54 2023-08-05 19:32:52.000000 AIMM-1.1.dev3/AIMM.egg-info/entry_points.txt
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)      128 2023-08-05 19:32:52.000000 AIMM-1.1.dev3/AIMM.egg-info/requires.txt
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)        5 2023-08-05 19:32:52.000000 AIMM-1.1.dev3/AIMM.egg-info/top_level.txt
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)    11357 2022-12-27 19:52:37.000000 AIMM-1.1.dev3/LICENSE
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)       51 2023-02-05 11:29:51.000000 AIMM-1.1.dev3/MANIFEST.in
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)     2238 2023-08-05 19:32:52.073220 AIMM-1.1.dev3/PKG-INFO
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)     1601 2022-12-27 19:52:37.000000 AIMM-1.1.dev3/README.rst
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)        9 2023-08-05 19:26:10.000000 AIMM-1.1.dev3/VERSION
+drwxr-xr-x   0 zlatan    (1000) zlatan    (1000)        0 2023-08-05 19:32:52.069887 AIMM-1.1.dev3/aimm/
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)        0 2022-12-27 19:52:37.000000 AIMM-1.1.dev3/aimm/__init__.py
+drwxr-xr-x   0 zlatan    (1000) zlatan    (1000)        0 2023-08-05 19:32:52.069887 AIMM-1.1.dev3/aimm/client/
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)        0 2022-12-27 19:52:37.000000 AIMM-1.1.dev3/aimm/client/__init__.py
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)     7831 2023-08-05 18:42:22.000000 AIMM-1.1.dev3/aimm/client/repl.py
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)      616 2023-02-18 00:15:42.000000 AIMM-1.1.dev3/aimm/common.py
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)     7734 2023-08-05 19:32:49.000000 AIMM-1.1.dev3/aimm/json_schema_repo.json
+drwxr-xr-x   0 zlatan    (1000) zlatan    (1000)        0 2023-08-05 19:32:52.069887 AIMM-1.1.dev3/aimm/plugins/
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)      704 2023-02-18 00:15:42.000000 AIMM-1.1.dev3/aimm/plugins/__init__.py
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)     3093 2023-02-18 00:15:42.000000 AIMM-1.1.dev3/aimm/plugins/common.py
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)     9945 2023-02-18 00:15:42.000000 AIMM-1.1.dev3/aimm/plugins/decorators.py
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)     2858 2023-02-18 00:15:42.000000 AIMM-1.1.dev3/aimm/plugins/execute.py
+drwxr-xr-x   0 zlatan    (1000) zlatan    (1000)        0 2023-08-05 19:32:52.069887 AIMM-1.1.dev3/aimm/server/
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)        0 2022-12-27 19:52:37.000000 AIMM-1.1.dev3/aimm/server/__init__.py
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)       96 2023-02-18 00:15:42.000000 AIMM-1.1.dev3/aimm/server/__main__.py
+drwxr-xr-x   0 zlatan    (1000) zlatan    (1000)        0 2023-08-05 19:32:52.069887 AIMM-1.1.dev3/aimm/server/backend/
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)        0 2022-12-27 19:52:37.000000 AIMM-1.1.dev3/aimm/server/backend/__init__.py
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)      681 2023-02-18 00:15:42.000000 AIMM-1.1.dev3/aimm/server/backend/dummy.py
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)     3118 2023-02-18 00:15:42.000000 AIMM-1.1.dev3/aimm/server/backend/event.py
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)     3297 2023-02-18 00:15:42.000000 AIMM-1.1.dev3/aimm/server/backend/sqlite.py
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)     9676 2023-08-05 14:14:36.000000 AIMM-1.1.dev3/aimm/server/common.py
+drwxr-xr-x   0 zlatan    (1000) zlatan    (1000)        0 2023-08-05 19:32:52.073220 AIMM-1.1.dev3/aimm/server/control/
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)        0 2022-12-27 19:52:37.000000 AIMM-1.1.dev3/aimm/server/control/__init__.py
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)     9510 2023-08-05 18:28:07.000000 AIMM-1.1.dev3/aimm/server/control/event.py
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)     8052 2023-02-18 00:15:42.000000 AIMM-1.1.dev3/aimm/server/control/repl.py
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)    10252 2023-02-18 00:15:42.000000 AIMM-1.1.dev3/aimm/server/engine.py
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)     5361 2023-08-05 19:25:33.000000 AIMM-1.1.dev3/aimm/server/main.py
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)     7435 2023-02-18 00:15:42.000000 AIMM-1.1.dev3/aimm/server/mprocess.py
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)       61 2023-02-18 00:39:48.000000 AIMM-1.1.dev3/pyproject.toml
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)       38 2023-08-05 19:32:52.073220 AIMM-1.1.dev3/setup.cfg
+-rw-r--r--   0 zlatan    (1000) zlatan    (1000)     1412 2023-08-05 19:31:37.000000 AIMM-1.1.dev3/setup.py
```

### Comparing `AIMM-1.1.dev2/AIMM.egg-info/PKG-INFO` & `AIMM-1.1.dev3/AIMM.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIMM
-Version: 1.1.dev2
+Version: 1.1.dev3
 Summary: Artificial intelligence model manager
 Home-page: https://github.com/hat-open/aimm
 Author: Zlatan Sičanica
 Author-email: zlatan.sicanica@koncar.hr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `AIMM-1.1.dev2/AIMM.egg-info/SOURCES.txt` & `AIMM-1.1.dev3/AIMM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AIMM-1.1.dev2/LICENSE` & `AIMM-1.1.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `AIMM-1.1.dev2/PKG-INFO` & `AIMM-1.1.dev3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIMM
-Version: 1.1.dev2
+Version: 1.1.dev3
 Summary: Artificial intelligence model manager
 Home-page: https://github.com/hat-open/aimm
 Author: Zlatan Sičanica
 Author-email: zlatan.sicanica@koncar.hr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `AIMM-1.1.dev2/README.rst` & `AIMM-1.1.dev3/README.rst`

 * *Files identical despite different names*

### Comparing `AIMM-1.1.dev2/aimm/client/repl.py` & `AIMM-1.1.dev3/aimm/client/repl.py`

 * *Files identical despite different names*

### Comparing `AIMM-1.1.dev2/aimm/common.py` & `AIMM-1.1.dev3/aimm/common.py`

 * *Files identical despite different names*

### Comparing `AIMM-1.1.dev2/aimm/json_schema_repo.json` & `AIMM-1.1.dev3/aimm/json_schema_repo.json`

 * *Files identical despite different names*

### Comparing `AIMM-1.1.dev2/aimm/plugins/__init__.py` & `AIMM-1.1.dev3/aimm/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `AIMM-1.1.dev2/aimm/plugins/common.py` & `AIMM-1.1.dev3/aimm/plugins/common.py`

 * *Files identical despite different names*

### Comparing `AIMM-1.1.dev2/aimm/plugins/decorators.py` & `AIMM-1.1.dev3/aimm/plugins/decorators.py`

 * *Files identical despite different names*

### Comparing `AIMM-1.1.dev2/aimm/plugins/execute.py` & `AIMM-1.1.dev3/aimm/plugins/execute.py`

 * *Files identical despite different names*

### Comparing `AIMM-1.1.dev2/aimm/server/backend/dummy.py` & `AIMM-1.1.dev3/aimm/server/backend/dummy.py`

 * *Files identical despite different names*

### Comparing `AIMM-1.1.dev2/aimm/server/backend/event.py` & `AIMM-1.1.dev3/aimm/server/backend/event.py`

 * *Files identical despite different names*

### Comparing `AIMM-1.1.dev2/aimm/server/backend/sqlite.py` & `AIMM-1.1.dev3/aimm/server/backend/sqlite.py`

 * *Files identical despite different names*

### Comparing `AIMM-1.1.dev2/aimm/server/common.py` & `AIMM-1.1.dev3/aimm/server/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from hat import aio
 from hat import util
 from typing import Any, Dict, Callable, Iterable, List, NamedTuple, Optional
 import abc
-import hat.event.eventer_client
+import hat.event.eventer.client
 import hat.event.common
 
 from aimm.common import *  # NOQA
 
 
 CreateSubscription = Callable[[Dict], hat.event.common.Subscription]
 CreateSubscription.__doc__ = """
@@ -22,15 +22,15 @@
 
     Args:
         client: concrete client instance
         subscription: event types proxy subscribes to"""
 
     def __init__(
         self,
-        client: hat.event.eventer_client.EventerClient(),
+        client: hat.event.eventer.client.Client(),
         subscription: hat.event.common.Subscription,
     ):
         self._subscription = subscription
         self._queue = aio.Queue()
         self._client = client
 
     @property
```

### Comparing `AIMM-1.1.dev2/aimm/server/control/event.py` & `AIMM-1.1.dev3/aimm/server/control/event.py`

 * *Files identical despite different names*

### Comparing `AIMM-1.1.dev2/aimm/server/control/repl.py` & `AIMM-1.1.dev3/aimm/server/control/repl.py`

 * *Files identical despite different names*

### Comparing `AIMM-1.1.dev2/aimm/server/engine.py` & `AIMM-1.1.dev3/aimm/server/engine.py`

 * *Files identical despite different names*

### Comparing `AIMM-1.1.dev2/aimm/server/main.py` & `AIMM-1.1.dev3/aimm/server/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from functools import partial
 from hat import aio
 from hat import json
 from pathlib import Path
 import appdirs
 import argparse
 import asyncio
 import contextlib
 import importlib
 import hat.monitor.client
-import hat.event.eventer_client
+import hat.event.eventer.client
 import hat.event.common
 import logging.config
 import sys
 
 from aimm import plugins
 from aimm.server import common
 import aimm.server.backend
@@ -34,52 +33,52 @@
     logging.config.dictConfig(conf["log"])
     plugins.initialize(conf["plugins"])
     with contextlib.suppress(asyncio.CancelledError):
         aio.run_asyncio(async_main(conf))
 
 
 async def async_main(conf):
-    async_group = aio.Group()
     hat_conf = conf.get("hat") or {}
     if "monitor" in hat_conf:
         monitor = await hat.monitor.client.connect(hat_conf["monitor"])
-        _bind_resource(async_group, monitor)
-
         component = hat.monitor.client.Component(
-            monitor, run_monitor_component, conf, monitor
+            monitor, run_monitor_component, conf
         )
         component.set_ready(True)
-        _bind_resource(async_group, component)
-
-        try:
-            await async_group.wait_closing()
-        finally:
-            await aio.uncancellable(monitor.async_close())
+        await component.wait_closed()
     elif "event_server_address" in hat_conf:
-        client = await hat.event.eventer_client.connect(
+        async_group = aio.Group()
+        client = await hat.event.eventer.client.connect(
             hat_conf["event_server_address"], list(_get_subscriptions(conf))
         )
         _bind_resource(async_group, client)
         await async_group.spawn(run, conf, client)
     else:
         mlog.debug("running without hat compatibility")
         await run(conf)
 
 
-async def run_monitor_component(_, conf, monitor):
+async def run_monitor_component(monitor, conf):
     if "event_server_group" not in conf["hat"]:
         mlog.info("running without hat event compatibility")
         return await run(conf)
-    run_conf = partial(run, conf)
-    return await hat.event.eventer_client.run_eventer_client(
-        monitor_client=monitor,
-        server_group=conf["hat"]["event_server_group"],
-        run_cb=run_conf,
-        subscriptions=list(_get_subscriptions(conf)),
-    )
+
+    async with aio.Group() as group:
+
+        def runner_cb(client):
+            group.spawn(run, conf, client)
+            return group
+
+        component = hat.event.eventer.client.Component(
+            monitor_client=monitor.client,
+            server_group=conf["hat"]["event_server_group"],
+            component_cb=runner_cb,
+            subscriptions=list(_get_subscriptions(conf)),
+        )
+        await component.wait_closed()
 
 
 async def run(conf, client=None):
     group = aio.Group()
 
     try:
         proxies = []
```

### Comparing `AIMM-1.1.dev2/aimm/server/mprocess.py` & `AIMM-1.1.dev3/aimm/server/mprocess.py`

 * *Files identical despite different names*

### Comparing `AIMM-1.1.dev2/setup.py` & `AIMM-1.1.dev3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         "Topic :: Software Development :: Libraries",
         "Topic :: Utilities",
     ],
     entry_points={"console_scripts": ["aimm-server = aimm.server.main:main"]},
     package_data={"": ["json_schema_repo.json"]},
     include_package_data=True,
     install_requires=[
-        "appdirs",
-        "hat-aio",
-        "hat-json",
-        "hat-monitor",
-        "hat-event",
-        "psutil",
+        "appdirs>=1.4.4,<1.5",
+        "hat-aio>=0.7.8,<0.8",
+        "hat-json>=0.5.19,<0.6",
+        "hat-monitor>=0.7.2,<0.8",
+        "hat-event>=0.8.8,<0.9",
+        "psutil>=5.9.5,<5.10",
     ],
 )
```

