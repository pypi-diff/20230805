# Comparing `tmp/panther-2.0.0.tar.gz` & `tmp/panther-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panther-2.0.0.tar", last modified: Fri Aug  4 12:43:24 2023, max compression
+gzip compressed data, was "panther-2.1.0.tar", last modified: Fri Aug  4 15:59:14 2023, max compression
```

## Comparing `panther-2.0.0.tar` & `panther-2.1.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:43:24.552842 panther-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-08-04 12:43:09.000000 panther-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-08-04 12:43:24.552842 panther-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-08-04 12:43:09.000000 panther-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:43:24.548842 panther-2.0.0/panther/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-04 12:43:09.000000 panther-2.0.0/panther/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-08-04 12:43:09.000000 panther-2.0.0/panther/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-08-04 12:43:09.000000 panther-2.0.0/panther/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-08-04 12:43:09.000000 panther-2.0.0/panther/authentications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-08-04 12:43:09.000000 panther-2.0.0/panther/caching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:43:24.548842 panther-2.0.0/panther/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:43:09.000000 panther-2.0.0/panther/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-04 12:43:09.000000 panther-2.0.0/panther/cli/create_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-04 12:43:09.000000 panther-2.0.0/panther/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-08-04 12:43:09.000000 panther-2.0.0/panther/cli/monitor_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-04 12:43:09.000000 panther-2.0.0/panther/cli/run_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-08-04 12:43:09.000000 panther-2.0.0/panther/cli/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-08-04 12:43:09.000000 panther-2.0.0/panther/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-04 12:43:09.000000 panther-2.0.0/panther/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:43:24.548842 panther-2.0.0/panther/db/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-04 12:43:09.000000 panther-2.0.0/panther/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-08-04 12:43:09.000000 panther-2.0.0/panther/db/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-04 12:43:09.000000 panther-2.0.0/panther/db/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:43:24.552842 panther-2.0.0/panther/db/queries/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-04 12:43:09.000000 panther-2.0.0/panther/db/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-08-04 12:43:09.000000 panther-2.0.0/panther/db/queries/mongodb_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-04 12:43:09.000000 panther-2.0.0/panther/db/queries/pantherdb_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-08-04 12:43:09.000000 panther-2.0.0/panther/db/queries/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-08-04 12:43:09.000000 panther-2.0.0/panther/db/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-08-04 12:43:09.000000 panther-2.0.0/panther/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-08-04 12:43:09.000000 panther-2.0.0/panther/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-08-04 12:43:09.000000 panther-2.0.0/panther/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:43:24.552842 panther-2.0.0/panther/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-04 12:43:09.000000 panther-2.0.0/panther/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-08-04 12:43:09.000000 panther-2.0.0/panther/middlewares/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-04 12:43:09.000000 panther-2.0.0/panther/middlewares/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-08-04 12:43:09.000000 panther-2.0.0/panther/middlewares/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-04 12:43:09.000000 panther-2.0.0/panther/middlewares/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:43:24.552842 panther-2.0.0/panther/panel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:43:09.000000 panther-2.0.0/panther/panel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-04 12:43:09.000000 panther-2.0.0/panther/panel/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-04 12:43:09.000000 panther-2.0.0/panther/panel/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-08-04 12:43:09.000000 panther-2.0.0/panther/panel/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-04 12:43:09.000000 panther-2.0.0/panther/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-08-04 12:43:09.000000 panther-2.0.0/panther/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-08-04 12:43:09.000000 panther-2.0.0/panther/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-08-04 12:43:09.000000 panther-2.0.0/panther/routings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-08-04 12:43:09.000000 panther-2.0.0/panther/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-04 12:43:09.000000 panther-2.0.0/panther/throttling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-08-04 12:43:09.000000 panther-2.0.0/panther/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:43:24.548842 panther-2.0.0/panther.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-08-04 12:43:24.000000 panther-2.0.0/panther.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-04 12:43:24.000000 panther-2.0.0/panther.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:43:24.000000 panther-2.0.0/panther.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-04 12:43:24.000000 panther-2.0.0/panther.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-04 12:43:24.000000 panther-2.0.0/panther.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-04 12:43:24.000000 panther-2.0.0/panther.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-04 12:43:09.000000 panther-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:43:24.552842 panther-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-08-04 12:43:09.000000 panther-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:43:24.552842 panther-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-08-04 12:43:09.000000 panther-2.0.0/tests/test_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-08-04 12:43:09.000000 panther-2.0.0/tests/test_pantherdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    26448 2023-08-04 12:43:09.000000 panther-2.0.0/tests/test_routing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:59:14.269425 panther-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-08-04 15:58:55.000000 panther-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-08-04 15:59:14.269425 panther-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-08-04 15:58:55.000000 panther-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:59:14.265425 panther-2.1.0/panther/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-04 15:58:55.000000 panther-2.1.0/panther/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-08-04 15:58:55.000000 panther-2.1.0/panther/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-08-04 15:58:55.000000 panther-2.1.0/panther/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-08-04 15:58:55.000000 panther-2.1.0/panther/authentications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-08-04 15:58:55.000000 panther-2.1.0/panther/caching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:59:14.265425 panther-2.1.0/panther/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 15:58:55.000000 panther-2.1.0/panther/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-04 15:58:55.000000 panther-2.1.0/panther/cli/create_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-04 15:58:55.000000 panther-2.1.0/panther/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-08-04 15:58:55.000000 panther-2.1.0/panther/cli/monitor_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-04 15:58:55.000000 panther-2.1.0/panther/cli/run_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-08-04 15:58:55.000000 panther-2.1.0/panther/cli/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-08-04 15:58:55.000000 panther-2.1.0/panther/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-04 15:58:55.000000 panther-2.1.0/panther/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:59:14.269425 panther-2.1.0/panther/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-04 15:58:55.000000 panther-2.1.0/panther/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-08-04 15:58:55.000000 panther-2.1.0/panther/db/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-04 15:58:55.000000 panther-2.1.0/panther/db/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:59:14.269425 panther-2.1.0/panther/db/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-04 15:58:55.000000 panther-2.1.0/panther/db/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-08-04 15:58:55.000000 panther-2.1.0/panther/db/queries/mongodb_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-04 15:58:55.000000 panther-2.1.0/panther/db/queries/pantherdb_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-08-04 15:58:55.000000 panther-2.1.0/panther/db/queries/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-08-04 15:58:55.000000 panther-2.1.0/panther/db/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-08-04 15:58:55.000000 panther-2.1.0/panther/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-08-04 15:58:55.000000 panther-2.1.0/panther/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-08-04 15:58:55.000000 panther-2.1.0/panther/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:59:14.269425 panther-2.1.0/panther/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-04 15:58:55.000000 panther-2.1.0/panther/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-08-04 15:58:55.000000 panther-2.1.0/panther/middlewares/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-04 15:58:55.000000 panther-2.1.0/panther/middlewares/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-08-04 15:58:55.000000 panther-2.1.0/panther/middlewares/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-04 15:58:55.000000 panther-2.1.0/panther/middlewares/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:59:14.269425 panther-2.1.0/panther/panel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 15:58:55.000000 panther-2.1.0/panther/panel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-04 15:58:55.000000 panther-2.1.0/panther/panel/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-04 15:58:55.000000 panther-2.1.0/panther/panel/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-08-04 15:58:55.000000 panther-2.1.0/panther/panel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-04 15:58:55.000000 panther-2.1.0/panther/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-08-04 15:58:55.000000 panther-2.1.0/panther/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-08-04 15:58:55.000000 panther-2.1.0/panther/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-08-04 15:58:55.000000 panther-2.1.0/panther/routings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-08-04 15:58:55.000000 panther-2.1.0/panther/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-04 15:58:55.000000 panther-2.1.0/panther/throttling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-08-04 15:58:55.000000 panther-2.1.0/panther/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:59:14.265425 panther-2.1.0/panther.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-08-04 15:59:14.000000 panther-2.1.0/panther.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-04 15:59:14.000000 panther-2.1.0/panther.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:59:14.000000 panther-2.1.0/panther.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-04 15:59:14.000000 panther-2.1.0/panther.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-04 15:59:14.000000 panther-2.1.0/panther.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-04 15:59:14.000000 panther-2.1.0/panther.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-04 15:58:55.000000 panther-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 15:59:14.273424 panther-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-08-04 15:58:55.000000 panther-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:59:14.269425 panther-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-08-04 15:58:55.000000 panther-2.1.0/tests/test_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-08-04 15:58:55.000000 panther-2.1.0/tests/test_pantherdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26448 2023-08-04 15:58:55.000000 panther-2.1.0/tests/test_routing.py
```

### Comparing `panther-2.0.0/LICENSE` & `panther-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/PKG-INFO` & `panther-2.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,41 @@
-Metadata-Version: 2.1
-Name: panther
-Version: 2.0.0
-Summary: Fast &  Friendly, Web Framework For Building Async APIs
-Home-page: https://github.com/alirn76/panther
-Author: Ali RajabNezhad
-Author-email: alirn76@yahoo.com
-License: MIT
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: full
-License-File: LICENSE
 
 
 ## Panther 
 <b>Is A Fast &  Friendly Web Framework For Building Async APIs With Python 3.11+</b> 
 
-<p align="center">
-<img src="https://github.com/AliRn76/panther/raw/master/docs/docs/images/logo-vertical.png" alt="logo" style="width: 450px">
+<p style="text-align: center">
+  <img src="https://github.com/AliRn76/panther/raw/master/docs/docs/images/logo-vertical.png" alt="logo" style="width: 450px">
 </p>
 
 <p>
   <img src="https://resources.jetbrains.com/storage/products/company/brand/logos/jb_beam.png" alt="logo" style="width: 50px;">
-   <b>Supported by </b><a href="https://jb.gg/OpenSourceSupport">JetBrain</a>
+   <b>Supported by </b><a href="https://drive.google.com/file/d/17xe1hicIiRF7SQ-clg9SETdc19SktCbV/view?usp=sharing">JetBrain</a>
 </p>
 
 **_Full Documentation:_** [https://pantherpy.github.io](https://pantherpy.github.io)
 
+**_PyPI:_** [https://pypi.org/project/panther/](https://pypi.org/project/panther/)
+
 ---
 
-### Why Use Panther?
+### Why Use Panther ?
 - Document-oriented Databases ODM ([PantherDB](https://pypi.org/project/pantherdb/), MongoDB)
 - Visual API Monitoring (In Terminal)
-- Caching for APIs (In Memory, In Redis)
+- Cache APIs (In Memory, In Redis)
 - Built-in Authentication Classes (Customizable)
 - Built-in Permission Classes (Customizable)
 - Handle Custom Middlewares
 - Handle Custom Throttling 
 ---
 
 ### Installation
 - <details>
     <summary>Create a Virtual Environment</summary>
-    <pre>$ python -m venv .venv</pre>
+    <pre>$ python3 -m venv .venv</pre>
   
   </details>
   
 - <details>
     <summary>Active The Environment</summary>
     * Linux & Mac
       <pre>$ source .venv/bin/activate</pre>
@@ -59,42 +44,46 @@
   
   </details>
  
 - <details open>
     <summary>Install Panther</summary>
     * Normal
       <pre>$ pip install panther</pre>
-    * Include JWT Authentication
+    * Include MongoDB Requirements
       <pre>$ pip install panther[full]</pre>
   </details>
   
 ---
 
 ### Usage
 
 - #### Create Project
 
     ```console
     $ panther create <project_name> <directory>
     ```
 
 - #### Run Project
-    Panther Uses [Uvicorn](https://github.com/encode/uvicorn) as ASGI (Asynchronous Server Gateway Interface)
+
+    Panther uses [Uvicorn](https://github.com/encode/uvicorn) as ASGI (Asynchronous Server Gateway Interface)
+    
     ```console
     $ panther run 
     ```
 
 - #### Monitoring Requests
 
     ```console
     $ panther monitor 
     ```
 
 - #### Python Shell
+
     Panther Uses [bpython](https://bpython-interpreter.org) for shell
+    
     ```console
     $ panther shell 
     ```
 ---
 
 ### Example
 
@@ -142,38 +131,45 @@
     from panther.configs import config
     from panther import version, status
     from panther.request import Request
     from panther.response import Response
     from panther.throttling import Throttling
     
     
+    InfoThrottling = Throttling(rate=5, duration=timedelta(minutes=1))
+  
     @API()
     async def hello_world():
         return {'detail': 'Hello World'}
     
     
-    @API(cache=True, throttling=Throttling(rate=5, duration=timedelta(minutes=1)))
+    @API(cache=True, throttling=InfoThrottling)
     async def info(request: Request):
         data = {
             'version': version(),
             'datetime_now': datetime.now().isoformat(),
             'user_agent': request.headers.user_agent,
             'db_engine': config['db_engine'],
         }
         return Response(data=data, status_code=status.HTTP_202_ACCEPTED)
     ```
 
-- <b> Then run (`$ panther run`) the project, now you can see these two urls:</b>
+- Then **run** the project:
+  
+  - `$ cd myproject`
+  - `$ panther run` or `$ panther run --reload` 
+  
+  now you can see these two urls:</b>
 
   * [http://127.0.0.1:8000/](http://127.0.0.1:8000/)
 
   * [http://127.0.0.1:8000/info/](http://127.0.0.1:8000/info/)
 
 
-  
+
 > **Writing Your First CRUD: [First CRUD](https://pantherpy.github.io/first_crud)**
 
 ---
 
 
 **<details>
     <summary>TODOs**</summary>
@@ -193,22 +189,22 @@
     - &#x2705; Log Queries
     - &#x2705; Add Package Requirements
     - &#x2705; Custom Logging
     - &#x2705; Caching
     - &#x2705; Handle Path Variable
     - &#x2705; Handle Simple Form-Data
     - &#x2705; Handle Throttling
+    - &#x2705; Handle ClassBase APIs
     - &#9744; Handle Complex Form-Data
     - &#9744; Handle File 
     - &#9744; Handle Cookie
     - &#9744; Handle WS 
     - &#9744; Handle GraphQL
     - &#9744; Handle Testing
     - &#9744; Generate Swagger For APIs
-    - &#9744; Handle ClassBase APIs
   
   </details>
 
 - <details>
     <summary>Database</summary>
   
     - &#x2705; Structure Of DB Connection
```

#### html2text {}

```diff
@@ -1,82 +1,77 @@
-Metadata-Version: 2.1 Name: panther Version: 2.0.0 Summary: Fast & Friendly,
-Web Framework For Building Async APIs Home-page: https://github.com/alirn76/
-panther Author: Ali RajabNezhad Author-email: alirn76@yahoo.com License: MIT
-Classifier: Operating System :: OS Independent Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.12 Requires-Python: >=3.10 Description-Content-Type:
-text/markdown Provides-Extra: full License-File: LICENSE ## Panther Is A Fast &
-Friendly Web Framework For Building Async APIs With Python 3.11+
-                                    [logo]
+ ## Panther Is A Fast & Friendly Web Framework For Building Async APIs With
+Python 3.11+
+[logo]
 [logo] Supported byJetBrain
 **_Full Documentation:_** [https://pantherpy.github.io](https://
-pantherpy.github.io) --- ### Why Use Panther? - Document-oriented Databases ODM
-([PantherDB](https://pypi.org/project/pantherdb/), MongoDB) - Visual API
-Monitoring (In Terminal) - Caching for APIs (In Memory, In Redis) - Built-in
-Authentication Classes (Customizable) - Built-in Permission Classes
+pantherpy.github.io) **_PyPI:_** [https://pypi.org/project/panther/](https://
+pypi.org/project/panther/) --- ### Why Use Panther ? - Document-oriented
+Databases ODM ([PantherDB](https://pypi.org/project/pantherdb/), MongoDB) -
+Visual API Monitoring (In Terminal) - Cache APIs (In Memory, In Redis) - Built-
+in Authentication Classes (Customizable) - Built-in Permission Classes
 (Customizable) - Handle Custom Middlewares - Handle Custom Throttling --- ###
 Installation -  Create a Virtual Environment
-$ python -m venv .venv
+$ python3 -m venv .venv
  -  Active The Environment * Linux & Mac
 $ source .venv/bin/activate
 * Windows
 $ .\.venv\Scripts\activate
  -  Install Panther * Normal
 $ pip install panther
-* Include JWT Authentication
+* Include MongoDB Requirements
 $ pip install panther[full]
  --- ### Usage - #### Create Project ```console $ panther create   ``` - ####
-Run Project Panther Uses [Uvicorn](https://github.com/encode/uvicorn) as ASGI
+Run Project Panther uses [Uvicorn](https://github.com/encode/uvicorn) as ASGI
 (Asynchronous Server Gateway Interface) ```console $ panther run ``` - ####
 Monitoring Requests ```console $ panther monitor ``` - #### Python Shell
 Panther Uses [bpython](https://bpython-interpreter.org) for shell ```console $
 panther shell ``` --- ### Example - #### You can create project with ```console
 $ panther create myproject ``` - #### or create it yourself: **core/
 configs.py**: ```python URLs = 'core/urls.py' ``` **core/urls.py**: ```python
 from app.urls import urls as app_urls urls = { '/': app_urls, } ``` **app/
 urls.py**: ```python from app.apis import hello_world, info urls = { '':
 hello_world, 'info/': info, } ``` **app/apis.py**: ```python from datetime
 import datetime, timedelta from panther.app import API from panther.configs
 import config from panther import version, status from panther.request import
 Request from panther.response import Response from panther.throttling import
-Throttling @API() async def hello_world(): return {'detail': 'Hello World'}
-@API(cache=True, throttling=Throttling(rate=5, duration=timedelta(minutes=1)))
-async def info(request: Request): data = { 'version': version(),
-'datetime_now': datetime.now().isoformat(), 'user_agent':
-request.headers.user_agent, 'db_engine': config['db_engine'], } return Response
-(data=data, status_code=status.HTTP_202_ACCEPTED) ``` - Then run (`$ panther
-run`) the project, now you can see these two urls: * [http://127.0.0.1:8000/]
-(http://127.0.0.1:8000/) * [http://127.0.0.1:8000/info/](http://127.0.0.1:8000/
-info/) > **Writing Your First CRUD: [First CRUD](https://pantherpy.github.io/
-first_crud)** --- ** TODOs** -  Base - &#x2705; Start with Uvicorn - &#x2705;
-Fix URL Routing - &#x2705; Read Configs - &#x2705; Handle Exceptions - &#x2705;
-Add Custom Logger - &#x2705; Request Class - &#x2705; Response Class - &#x2705;
-Validate Input - &#x2705; Custom Output Model - &#x2705; Log Queries - &#x2705;
-Add Package Requirements - &#x2705; Custom Logging - &#x2705; Caching -
-&#x2705; Handle Path Variable - &#x2705; Handle Simple Form-Data - &#x2705;
-Handle Throttling - ☐ Handle Complex Form-Data - ☐ Handle File - ☐ Handle
-Cookie - ☐ Handle WS - ☐ Handle GraphQL - ☐ Handle Testing - ☐ Generate Swagger
-For APIs - ☐ Handle ClassBase APIs  -  Database - &#x2705; Structure Of DB
-Connection - &#x2705; PantherDB Connection - &#x2705; MongoDB Connection -
-&#x2705; Create Custom BaseModel For All Type Of Databases - &#x2705; Set
-PantherDB As Default  -  Custom ODM - &#x2705; Find One - &#x2705; Find -
-&#x2705; Last - &#x2705; Count - &#x2705; Insert One - &#x2705; Insert Many -
-&#x2705; Delete One - &#x2705; Delete Many - &#x2705; Delete Itself - &#x2705;
-Update One - &#x2705; Update Many - &#x2705; Update Itself - &#x2705; Find or
-Insert - &#x2705; Save - ☐ Find or Raise - ☐ Find with Pagination - ☐
-Aggregation - ☐ Complex Pipelines - ☐ ...  -  Middleware - &#x2705; Add
-Middlewares To Structure - &#x2705; Create BaseMiddleware - &#x2705; Pass
-Custom Parameters To Middlewares - &#x2705; Handle Custom Middlewares  -
-Authentication - &#x2705; JWT Authentication - &#x2705; Separate Auth For Every
-API - &#x2705; Handle Permissions - ☐ Token Storage Authentication - ☐ Cookie
-Authentication - ☐ Query Param Authentication - ☐ Store JWT After Logout In
-Redis/ Memory  -  Cache - &#x2705; Add Redis To Structure - &#x2705; Create
-Cache Decorator - &#x2705; Handle In-Memory Caching - &#x2705; Handle In Redis
-Caching - ☐ Write Async LRU_Caching With TTL (Replace it with in-memory ...)  -
-CLI - &#x2705; Create Project - &#x2705; Run Project - &#x2705; Create Project
-with Options - &#x2705; Monitoring With Textual - &#x2705; Monitor Requests,
-Response & Time  -  Documentation - &#x2705; Create MkDocs For Project -
-&#x2705; Benchmarks - &#x2705; Release Notes - &#x2705; Features - ☐ Complete
-The MkDoc  -  Tests - &#x2705; Start Writing Tests For Panther - ☐ Test Client
---- ### Support **If you find this project useful, please give it a star
-â­ï¸.**
+Throttling InfoThrottling = Throttling(rate=5, duration=timedelta(minutes=1))
+@API() async def hello_world(): return {'detail': 'Hello World'} @API
+(cache=True, throttling=InfoThrottling) async def info(request: Request): data
+= { 'version': version(), 'datetime_now': datetime.now().isoformat(),
+'user_agent': request.headers.user_agent, 'db_engine': config['db_engine'], }
+return Response(data=data, status_code=status.HTTP_202_ACCEPTED) ``` - Then
+**run** the project: - `$ cd myproject` - `$ panther run` or `$ panther run --
+reload` now you can see these two urls:
+ * [http://127.0.0.1:8000/](http://127.0.0.1:8000/) * [http://127.0.0.1:8000/
+info/](http://127.0.0.1:8000/info/) > **Writing Your First CRUD: [First CRUD]
+(https://pantherpy.github.io/first_crud)** --- ** TODOs** -  Base - &#x2705;
+Start with Uvicorn - &#x2705; Fix URL Routing - &#x2705; Read Configs -
+&#x2705; Handle Exceptions - &#x2705; Add Custom Logger - &#x2705; Request
+Class - &#x2705; Response Class - &#x2705; Validate Input - &#x2705; Custom
+Output Model - &#x2705; Log Queries - &#x2705; Add Package Requirements -
+&#x2705; Custom Logging - &#x2705; Caching - &#x2705; Handle Path Variable -
+&#x2705; Handle Simple Form-Data - &#x2705; Handle Throttling - &#x2705; Handle
+ClassBase APIs - ☐ Handle Complex Form-Data - ☐ Handle File - ☐ Handle Cookie -
+☐ Handle WS - ☐ Handle GraphQL - ☐ Handle Testing - ☐ Generate Swagger For APIs
+-  Database - &#x2705; Structure Of DB Connection - &#x2705; PantherDB
+Connection - &#x2705; MongoDB Connection - &#x2705; Create Custom BaseModel For
+All Type Of Databases - &#x2705; Set PantherDB As Default  -  Custom ODM -
+&#x2705; Find One - &#x2705; Find - &#x2705; Last - &#x2705; Count - &#x2705;
+Insert One - &#x2705; Insert Many - &#x2705; Delete One - &#x2705; Delete Many
+- &#x2705; Delete Itself - &#x2705; Update One - &#x2705; Update Many -
+&#x2705; Update Itself - &#x2705; Find or Insert - &#x2705; Save - ☐ Find or
+Raise - ☐ Find with Pagination - ☐ Aggregation - ☐ Complex Pipelines - ☐ ...  -
+Middleware - &#x2705; Add Middlewares To Structure - &#x2705; Create
+BaseMiddleware - &#x2705; Pass Custom Parameters To Middlewares - &#x2705;
+Handle Custom Middlewares  -  Authentication - &#x2705; JWT Authentication -
+&#x2705; Separate Auth For Every API - &#x2705; Handle Permissions - ☐ Token
+Storage Authentication - ☐ Cookie Authentication - ☐ Query Param Authentication
+- ☐ Store JWT After Logout In Redis/ Memory  -  Cache - &#x2705; Add Redis To
+Structure - &#x2705; Create Cache Decorator - &#x2705; Handle In-Memory Caching
+- &#x2705; Handle In Redis Caching - ☐ Write Async LRU_Caching With TTL
+(Replace it with in-memory ...)  -  CLI - &#x2705; Create Project - &#x2705;
+Run Project - &#x2705; Create Project with Options - &#x2705; Monitoring With
+Textual - &#x2705; Monitor Requests, Response & Time  -  Documentation -
+&#x2705; Create MkDocs For Project - &#x2705; Benchmarks - &#x2705; Release
+Notes - &#x2705; Features - ☐ Complete The MkDoc  -  Tests - &#x2705; Start
+Writing Tests For Panther - ☐ Test Client   --- ### Support **If you find this
+project useful, please give it a star â­ï¸.**
```

### Comparing `panther-2.0.0/README.md` & `panther-2.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,59 @@
+Metadata-Version: 2.1
+Name: panther
+Version: 2.1.0
+Summary: Fast &  Friendly, Web Framework For Building Async APIs
+Home-page: https://github.com/alirn76/panther
+Author: Ali RajabNezhad
+Author-email: alirn76@yahoo.com
+License: MIT
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: full
+License-File: LICENSE
+
+
 
 ## Panther 
 <b>Is A Fast &  Friendly Web Framework For Building Async APIs With Python 3.11+</b> 
 
-<p align="center">
-<img src="https://github.com/AliRn76/panther/raw/master/docs/docs/images/logo-vertical.png" alt="logo" style="width: 450px">
+<p style="text-align: center">
+  <img src="https://github.com/AliRn76/panther/raw/master/docs/docs/images/logo-vertical.png" alt="logo" style="width: 450px">
 </p>
 
 <p>
   <img src="https://resources.jetbrains.com/storage/products/company/brand/logos/jb_beam.png" alt="logo" style="width: 50px;">
-   <b>Supported by </b><a href="https://jb.gg/OpenSourceSupport">JetBrain</a>
+   <b>Supported by </b><a href="https://drive.google.com/file/d/17xe1hicIiRF7SQ-clg9SETdc19SktCbV/view?usp=sharing">JetBrain</a>
 </p>
 
 **_Full Documentation:_** [https://pantherpy.github.io](https://pantherpy.github.io)
 
+**_PyPI:_** [https://pypi.org/project/panther/](https://pypi.org/project/panther/)
+
 ---
 
-### Why Use Panther?
+### Why Use Panther ?
 - Document-oriented Databases ODM ([PantherDB](https://pypi.org/project/pantherdb/), MongoDB)
 - Visual API Monitoring (In Terminal)
-- Caching for APIs (In Memory, In Redis)
+- Cache APIs (In Memory, In Redis)
 - Built-in Authentication Classes (Customizable)
 - Built-in Permission Classes (Customizable)
 - Handle Custom Middlewares
 - Handle Custom Throttling 
 ---
 
 ### Installation
 - <details>
     <summary>Create a Virtual Environment</summary>
-    <pre>$ python -m venv .venv</pre>
+    <pre>$ python3 -m venv .venv</pre>
   
   </details>
   
 - <details>
     <summary>Active The Environment</summary>
     * Linux & Mac
       <pre>$ source .venv/bin/activate</pre>
@@ -41,42 +62,46 @@
   
   </details>
  
 - <details open>
     <summary>Install Panther</summary>
     * Normal
       <pre>$ pip install panther</pre>
-    * Include JWT Authentication
+    * Include MongoDB Requirements
       <pre>$ pip install panther[full]</pre>
   </details>
   
 ---
 
 ### Usage
 
 - #### Create Project
 
     ```console
     $ panther create <project_name> <directory>
     ```
 
 - #### Run Project
-    Panther Uses [Uvicorn](https://github.com/encode/uvicorn) as ASGI (Asynchronous Server Gateway Interface)
+
+    Panther uses [Uvicorn](https://github.com/encode/uvicorn) as ASGI (Asynchronous Server Gateway Interface)
+    
     ```console
     $ panther run 
     ```
 
 - #### Monitoring Requests
 
     ```console
     $ panther monitor 
     ```
 
 - #### Python Shell
+
     Panther Uses [bpython](https://bpython-interpreter.org) for shell
+    
     ```console
     $ panther shell 
     ```
 ---
 
 ### Example
 
@@ -124,38 +149,45 @@
     from panther.configs import config
     from panther import version, status
     from panther.request import Request
     from panther.response import Response
     from panther.throttling import Throttling
     
     
+    InfoThrottling = Throttling(rate=5, duration=timedelta(minutes=1))
+  
     @API()
     async def hello_world():
         return {'detail': 'Hello World'}
     
     
-    @API(cache=True, throttling=Throttling(rate=5, duration=timedelta(minutes=1)))
+    @API(cache=True, throttling=InfoThrottling)
     async def info(request: Request):
         data = {
             'version': version(),
             'datetime_now': datetime.now().isoformat(),
             'user_agent': request.headers.user_agent,
             'db_engine': config['db_engine'],
         }
         return Response(data=data, status_code=status.HTTP_202_ACCEPTED)
     ```
 
-- <b> Then run (`$ panther run`) the project, now you can see these two urls:</b>
+- Then **run** the project:
+  
+  - `$ cd myproject`
+  - `$ panther run` or `$ panther run --reload` 
+  
+  now you can see these two urls:</b>
 
   * [http://127.0.0.1:8000/](http://127.0.0.1:8000/)
 
   * [http://127.0.0.1:8000/info/](http://127.0.0.1:8000/info/)
 
 
-  
+
 > **Writing Your First CRUD: [First CRUD](https://pantherpy.github.io/first_crud)**
 
 ---
 
 
 **<details>
     <summary>TODOs**</summary>
@@ -175,22 +207,22 @@
     - &#x2705; Log Queries
     - &#x2705; Add Package Requirements
     - &#x2705; Custom Logging
     - &#x2705; Caching
     - &#x2705; Handle Path Variable
     - &#x2705; Handle Simple Form-Data
     - &#x2705; Handle Throttling
+    - &#x2705; Handle ClassBase APIs
     - &#9744; Handle Complex Form-Data
     - &#9744; Handle File 
     - &#9744; Handle Cookie
     - &#9744; Handle WS 
     - &#9744; Handle GraphQL
     - &#9744; Handle Testing
     - &#9744; Generate Swagger For APIs
-    - &#9744; Handle ClassBase APIs
   
   </details>
 
 - <details>
     <summary>Database</summary>
   
     - &#x2705; Structure Of DB Connection
@@ -292,8 +324,8 @@
 </details>
 
 
 ---
 
 ### Support
 
-**If you find this project useful, please give it a star ⭐️.**
+**If you find this project useful, please give it a star ⭐️.**
```

#### html2text {}

```diff
@@ -1,75 +1,84 @@
- ## Panther Is A Fast & Friendly Web Framework For Building Async APIs With
-Python 3.11+
-                                    [logo]
+Metadata-Version: 2.1 Name: panther Version: 2.1.0 Summary: Fast & Friendly,
+Web Framework For Building Async APIs Home-page: https://github.com/alirn76/
+panther Author: Ali RajabNezhad Author-email: alirn76@yahoo.com License: MIT
+Classifier: Operating System :: OS Independent Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Requires-Python: >=3.10 Description-Content-Type:
+text/markdown Provides-Extra: full License-File: LICENSE ## Panther Is A Fast &
+Friendly Web Framework For Building Async APIs With Python 3.11+
+[logo]
 [logo] Supported byJetBrain
 **_Full Documentation:_** [https://pantherpy.github.io](https://
-pantherpy.github.io) --- ### Why Use Panther? - Document-oriented Databases ODM
-([PantherDB](https://pypi.org/project/pantherdb/), MongoDB) - Visual API
-Monitoring (In Terminal) - Caching for APIs (In Memory, In Redis) - Built-in
-Authentication Classes (Customizable) - Built-in Permission Classes
+pantherpy.github.io) **_PyPI:_** [https://pypi.org/project/panther/](https://
+pypi.org/project/panther/) --- ### Why Use Panther ? - Document-oriented
+Databases ODM ([PantherDB](https://pypi.org/project/pantherdb/), MongoDB) -
+Visual API Monitoring (In Terminal) - Cache APIs (In Memory, In Redis) - Built-
+in Authentication Classes (Customizable) - Built-in Permission Classes
 (Customizable) - Handle Custom Middlewares - Handle Custom Throttling --- ###
 Installation -  Create a Virtual Environment
-$ python -m venv .venv
+$ python3 -m venv .venv
  -  Active The Environment * Linux & Mac
 $ source .venv/bin/activate
 * Windows
 $ .\.venv\Scripts\activate
  -  Install Panther * Normal
 $ pip install panther
-* Include JWT Authentication
+* Include MongoDB Requirements
 $ pip install panther[full]
  --- ### Usage - #### Create Project ```console $ panther create   ``` - ####
-Run Project Panther Uses [Uvicorn](https://github.com/encode/uvicorn) as ASGI
+Run Project Panther uses [Uvicorn](https://github.com/encode/uvicorn) as ASGI
 (Asynchronous Server Gateway Interface) ```console $ panther run ``` - ####
 Monitoring Requests ```console $ panther monitor ``` - #### Python Shell
 Panther Uses [bpython](https://bpython-interpreter.org) for shell ```console $
 panther shell ``` --- ### Example - #### You can create project with ```console
 $ panther create myproject ``` - #### or create it yourself: **core/
 configs.py**: ```python URLs = 'core/urls.py' ``` **core/urls.py**: ```python
 from app.urls import urls as app_urls urls = { '/': app_urls, } ``` **app/
 urls.py**: ```python from app.apis import hello_world, info urls = { '':
 hello_world, 'info/': info, } ``` **app/apis.py**: ```python from datetime
 import datetime, timedelta from panther.app import API from panther.configs
 import config from panther import version, status from panther.request import
 Request from panther.response import Response from panther.throttling import
-Throttling @API() async def hello_world(): return {'detail': 'Hello World'}
-@API(cache=True, throttling=Throttling(rate=5, duration=timedelta(minutes=1)))
-async def info(request: Request): data = { 'version': version(),
-'datetime_now': datetime.now().isoformat(), 'user_agent':
-request.headers.user_agent, 'db_engine': config['db_engine'], } return Response
-(data=data, status_code=status.HTTP_202_ACCEPTED) ``` - Then run (`$ panther
-run`) the project, now you can see these two urls: * [http://127.0.0.1:8000/]
-(http://127.0.0.1:8000/) * [http://127.0.0.1:8000/info/](http://127.0.0.1:8000/
-info/) > **Writing Your First CRUD: [First CRUD](https://pantherpy.github.io/
-first_crud)** --- ** TODOs** -  Base - &#x2705; Start with Uvicorn - &#x2705;
-Fix URL Routing - &#x2705; Read Configs - &#x2705; Handle Exceptions - &#x2705;
-Add Custom Logger - &#x2705; Request Class - &#x2705; Response Class - &#x2705;
-Validate Input - &#x2705; Custom Output Model - &#x2705; Log Queries - &#x2705;
-Add Package Requirements - &#x2705; Custom Logging - &#x2705; Caching -
-&#x2705; Handle Path Variable - &#x2705; Handle Simple Form-Data - &#x2705;
-Handle Throttling - ☐ Handle Complex Form-Data - ☐ Handle File - ☐ Handle
-Cookie - ☐ Handle WS - ☐ Handle GraphQL - ☐ Handle Testing - ☐ Generate Swagger
-For APIs - ☐ Handle ClassBase APIs  -  Database - &#x2705; Structure Of DB
-Connection - &#x2705; PantherDB Connection - &#x2705; MongoDB Connection -
-&#x2705; Create Custom BaseModel For All Type Of Databases - &#x2705; Set
-PantherDB As Default  -  Custom ODM - &#x2705; Find One - &#x2705; Find -
-&#x2705; Last - &#x2705; Count - &#x2705; Insert One - &#x2705; Insert Many -
-&#x2705; Delete One - &#x2705; Delete Many - &#x2705; Delete Itself - &#x2705;
-Update One - &#x2705; Update Many - &#x2705; Update Itself - &#x2705; Find or
-Insert - &#x2705; Save - ☐ Find or Raise - ☐ Find with Pagination - ☐
-Aggregation - ☐ Complex Pipelines - ☐ ...  -  Middleware - &#x2705; Add
-Middlewares To Structure - &#x2705; Create BaseMiddleware - &#x2705; Pass
-Custom Parameters To Middlewares - &#x2705; Handle Custom Middlewares  -
-Authentication - &#x2705; JWT Authentication - &#x2705; Separate Auth For Every
-API - &#x2705; Handle Permissions - ☐ Token Storage Authentication - ☐ Cookie
-Authentication - ☐ Query Param Authentication - ☐ Store JWT After Logout In
-Redis/ Memory  -  Cache - &#x2705; Add Redis To Structure - &#x2705; Create
-Cache Decorator - &#x2705; Handle In-Memory Caching - &#x2705; Handle In Redis
-Caching - ☐ Write Async LRU_Caching With TTL (Replace it with in-memory ...)  -
-CLI - &#x2705; Create Project - &#x2705; Run Project - &#x2705; Create Project
-with Options - &#x2705; Monitoring With Textual - &#x2705; Monitor Requests,
-Response & Time  -  Documentation - &#x2705; Create MkDocs For Project -
-&#x2705; Benchmarks - &#x2705; Release Notes - &#x2705; Features - ☐ Complete
-The MkDoc  -  Tests - &#x2705; Start Writing Tests For Panther - ☐ Test Client
---- ### Support **If you find this project useful, please give it a star
-â­ï¸.**
+Throttling InfoThrottling = Throttling(rate=5, duration=timedelta(minutes=1))
+@API() async def hello_world(): return {'detail': 'Hello World'} @API
+(cache=True, throttling=InfoThrottling) async def info(request: Request): data
+= { 'version': version(), 'datetime_now': datetime.now().isoformat(),
+'user_agent': request.headers.user_agent, 'db_engine': config['db_engine'], }
+return Response(data=data, status_code=status.HTTP_202_ACCEPTED) ``` - Then
+**run** the project: - `$ cd myproject` - `$ panther run` or `$ panther run --
+reload` now you can see these two urls:
+ * [http://127.0.0.1:8000/](http://127.0.0.1:8000/) * [http://127.0.0.1:8000/
+info/](http://127.0.0.1:8000/info/) > **Writing Your First CRUD: [First CRUD]
+(https://pantherpy.github.io/first_crud)** --- ** TODOs** -  Base - &#x2705;
+Start with Uvicorn - &#x2705; Fix URL Routing - &#x2705; Read Configs -
+&#x2705; Handle Exceptions - &#x2705; Add Custom Logger - &#x2705; Request
+Class - &#x2705; Response Class - &#x2705; Validate Input - &#x2705; Custom
+Output Model - &#x2705; Log Queries - &#x2705; Add Package Requirements -
+&#x2705; Custom Logging - &#x2705; Caching - &#x2705; Handle Path Variable -
+&#x2705; Handle Simple Form-Data - &#x2705; Handle Throttling - &#x2705; Handle
+ClassBase APIs - ☐ Handle Complex Form-Data - ☐ Handle File - ☐ Handle Cookie -
+☐ Handle WS - ☐ Handle GraphQL - ☐ Handle Testing - ☐ Generate Swagger For APIs
+-  Database - &#x2705; Structure Of DB Connection - &#x2705; PantherDB
+Connection - &#x2705; MongoDB Connection - &#x2705; Create Custom BaseModel For
+All Type Of Databases - &#x2705; Set PantherDB As Default  -  Custom ODM -
+&#x2705; Find One - &#x2705; Find - &#x2705; Last - &#x2705; Count - &#x2705;
+Insert One - &#x2705; Insert Many - &#x2705; Delete One - &#x2705; Delete Many
+- &#x2705; Delete Itself - &#x2705; Update One - &#x2705; Update Many -
+&#x2705; Update Itself - &#x2705; Find or Insert - &#x2705; Save - ☐ Find or
+Raise - ☐ Find with Pagination - ☐ Aggregation - ☐ Complex Pipelines - ☐ ...  -
+Middleware - &#x2705; Add Middlewares To Structure - &#x2705; Create
+BaseMiddleware - &#x2705; Pass Custom Parameters To Middlewares - &#x2705;
+Handle Custom Middlewares  -  Authentication - &#x2705; JWT Authentication -
+&#x2705; Separate Auth For Every API - &#x2705; Handle Permissions - ☐ Token
+Storage Authentication - ☐ Cookie Authentication - ☐ Query Param Authentication
+- ☐ Store JWT After Logout In Redis/ Memory  -  Cache - &#x2705; Add Redis To
+Structure - &#x2705; Create Cache Decorator - &#x2705; Handle In-Memory Caching
+- &#x2705; Handle In Redis Caching - ☐ Write Async LRU_Caching With TTL
+(Replace it with in-memory ...)  -  CLI - &#x2705; Create Project - &#x2705;
+Run Project - &#x2705; Create Project with Options - &#x2705; Monitoring With
+Textual - &#x2705; Monitor Requests, Response & Time  -  Documentation -
+&#x2705; Create MkDocs For Project - &#x2705; Benchmarks - &#x2705; Release
+Notes - &#x2705; Features - ☐ Complete The MkDoc  -  Tests - &#x2705; Start
+Writing Tests For Panther - ☐ Test Client   --- ### Support **If you find this
+project useful, please give it a star â­ï¸.**
```

### Comparing `panther-2.0.0/panther/_utils.py` & `panther-2.1.0/panther/_utils.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/panther/app.py` & `panther-2.1.0/panther/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import inspect
 import functools
 from pydantic import ValidationError
 from datetime import timedelta, datetime
 from orjson.orjson import JSONDecodeError
 
 from panther import status
 from panther.logger import logger
@@ -68,15 +69,20 @@
                     return Response(data=cached.data, status_code=cached.status_code)
 
             # 7. Put Request In kwargs
             if req_arg := [k for k, v in func.__annotations__.items() if v == Request]:
                 kwargs[req_arg[0]] = self.request
 
             # 8. Call Endpoint
-            response = await func(**kwargs)
+            if inspect.iscoroutinefunction(func):
+                # It's an async function
+                response = await func(**kwargs)
+            else:
+                # It's a sync function
+                response = func(**kwargs)
 
             # 9. Clean Output
             if not isinstance(response, Response):
                 response = Response(data=response)
             data = self.serialize_response_data(data=response._data)  # NOQA: Access to a protected member
             response.set_data(data)
 
@@ -85,14 +91,15 @@
                 set_cache_response(request=self.request, response=response, cache_exp_time=self.cache_exp_time)
 
             # 11. Warning CacheExpTime
             if self.cache_exp_time and self.cache is False:
                 logger.warning('"cache_exp_time" won\'t work while "cache" is False')
 
             return response
+
         return wrapper
 
     def handle_authentications(self) -> None:
         auth_class = config['authentication']
         if self.auth:
             if not auth_class:
                 raise TypeError('"AUTHENTICATION" has not been set in core/configs')
@@ -172,15 +179,15 @@
     input_model = None
     output_model = None
     auth: bool = False
     permissions: list | None = None
     throttling: Throttling = None
     cache: bool = False
     cache_exp_time: timedelta | int | None = None
-    
+
     async def get(self, *args, **kwargs):
         raise MethodNotAllowed
 
     async def post(self, *args, **kwargs):
         raise MethodNotAllowed
 
     async def put(self, *args, **kwargs):
```

### Comparing `panther-2.0.0/panther/authentications.py` & `panther-2.1.0/panther/authentications.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/panther/caching.py` & `panther-2.1.0/panther/caching.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/panther/cli/create_command.py` & `panther-2.1.0/panther/cli/create_command.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/panther/cli/main.py` & `panther-2.1.0/panther/cli/main.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/panther/cli/monitor_command.py` & `panther-2.1.0/panther/cli/monitor_command.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/panther/cli/run_command.py` & `panther-2.1.0/panther/cli/run_command.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/panther/cli/template.py` & `panther-2.1.0/panther/cli/template.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/panther/cli/utils.py` & `panther-2.1.0/panther/cli/utils.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/panther/configs.py` & `panther-2.1.0/panther/configs.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/panther/db/connection.py` & `panther-2.1.0/panther/db/connection.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/panther/db/models.py` & `panther-2.1.0/panther/db/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,11 +30,14 @@
     @property
     def _id(self):
         if IDType is int:
             return self.id
         else:
             return bson.ObjectId(self.id) if self.id else None
 
+    def dict(self, *args, **kwargs):
+        return self.model_dump(*args, **kwargs)
+
 
 class BaseUser(Model):
     first_name: str | None
     last_name: str | None
```

### Comparing `panther-2.0.0/panther/db/queries/mongodb_queries.py` & `panther-2.1.0/panther/db/queries/mongodb_queries.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/panther/db/queries/pantherdb_queries.py` & `panther-2.1.0/panther/db/queries/pantherdb_queries.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/panther/db/queries/queries.py` & `panther-2.1.0/panther/db/queries/queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         *. If is_updating is True & exception happens but the message was empty
         """
         try:
             cls(**data)
         except ValidationError as validation_error:
             error = ', '.join(
                 '{field}="{error}"'.format(field=e['loc'][0], error=e['msg'])
-                for e in validation_error.errors() if not is_updating or e['type'] != 'value_error.missing')
+                for e in validation_error.errors() if not is_updating or e['type'] != 'missing')
             if error:
                 message = f'{cls.__name__}({error})'
                 raise DBException(message)
 
     # # # # # Find # # # # #
     @classmethod
     @log_query
```

### Comparing `panther-2.0.0/panther/db/utils.py` & `panther-2.1.0/panther/db/utils.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/panther/exceptions.py` & `panther-2.1.0/panther/exceptions.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/panther/logger.py` & `panther-2.1.0/panther/logger.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/panther/main.py` & `panther-2.1.0/panther/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import ast
 import sys
+import types
 import asyncio
 from pathlib import Path
 from runpy import run_path
 from pydantic._internal._model_construction import ModelMetaclass
 
 from panther import status
 from panther.app import GenericAPI
@@ -192,44 +193,45 @@
         path_variables = collect_path_variables(request_path=request.path, found_path=found_path)
 
         if endpoint is None:
             return await http_response(
                 send, status_code=status.HTTP_404_NOT_FOUND, monitoring=monitoring_middleware, exception=True,
             )
 
-        try:  # They Both Have The Save Exception (APIException)
+        try:  # They Both(middleware.before() & _endpoint()) Have The Same Exception (APIException)
             # Call 'Before' Middlewares
             for middleware in config['middlewares']:
                 request = await middleware.before(request=request)
 
-            if type(endpoint).__name__ == 'function':
+            # Function
+            if isinstance(endpoint, types.FunctionType):
                 # User Didn't Use @API Decorator
                 if not hasattr(endpoint, '__wrapped__'):
                     logger.critical(f'You may have forgotten to use @API on the {endpoint.__name__}()')
                     return await http_response(
                         send,
                         status_code=status.HTTP_510_NOT_EXTENDED,
                         monitoring=monitoring_middleware,
                         exception=True,
                     )
 
-                # Prepare Endpoint
+                # Declare Endpoint
                 _endpoint = endpoint
 
+            # Class
             else:
                 if not issubclass(endpoint, GenericAPI):
                     logger.critical(f'You may have forgotten to inherit from GenericAPI on the {endpoint.__name__}()')
                     return await http_response(
                         send,
                         status_code=status.HTTP_510_NOT_EXTENDED,
                         monitoring=monitoring_middleware,
                         exception=True,
                     )
-
-                # Prepare Endpoint
+                # Declare Endpoint
                 _endpoint = endpoint.call_method
 
             # Call Endpoint
             response = await _endpoint(request=request, **path_variables)
 
         except APIException as e:
             response = self.handle_exceptions(e)
```

### Comparing `panther-2.0.0/panther/middlewares/monitoring.py` & `panther-2.1.0/panther/middlewares/monitoring.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/panther/middlewares/redis.py` & `panther-2.1.0/panther/middlewares/redis.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/panther/panel/apis.py` & `panther-2.1.0/panther/panel/apis.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/panther/request.py` & `panther-2.1.0/panther/request.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/panther/response.py` & `panther-2.1.0/panther/response.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/panther/routings.py` & `panther-2.1.0/panther/routings.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/panther/status.py` & `panther-2.1.0/panther/status.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/panther/utils.py` & `panther-2.1.0/panther/utils.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/panther.egg-info/PKG-INFO` & `panther-2.1.0/panther.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panther
-Version: 2.0.0
+Version: 2.1.0
 Summary: Fast &  Friendly, Web Framework For Building Async APIs
 Home-page: https://github.com/alirn76/panther
 Author: Ali RajabNezhad
 Author-email: alirn76@yahoo.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
@@ -13,44 +13,47 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: full
 License-File: LICENSE
 
 
+
 ## Panther 
 <b>Is A Fast &  Friendly Web Framework For Building Async APIs With Python 3.11+</b> 
 
-<p align="center">
-<img src="https://github.com/AliRn76/panther/raw/master/docs/docs/images/logo-vertical.png" alt="logo" style="width: 450px">
+<p style="text-align: center">
+  <img src="https://github.com/AliRn76/panther/raw/master/docs/docs/images/logo-vertical.png" alt="logo" style="width: 450px">
 </p>
 
 <p>
   <img src="https://resources.jetbrains.com/storage/products/company/brand/logos/jb_beam.png" alt="logo" style="width: 50px;">
-   <b>Supported by </b><a href="https://jb.gg/OpenSourceSupport">JetBrain</a>
+   <b>Supported by </b><a href="https://drive.google.com/file/d/17xe1hicIiRF7SQ-clg9SETdc19SktCbV/view?usp=sharing">JetBrain</a>
 </p>
 
 **_Full Documentation:_** [https://pantherpy.github.io](https://pantherpy.github.io)
 
+**_PyPI:_** [https://pypi.org/project/panther/](https://pypi.org/project/panther/)
+
 ---
 
-### Why Use Panther?
+### Why Use Panther ?
 - Document-oriented Databases ODM ([PantherDB](https://pypi.org/project/pantherdb/), MongoDB)
 - Visual API Monitoring (In Terminal)
-- Caching for APIs (In Memory, In Redis)
+- Cache APIs (In Memory, In Redis)
 - Built-in Authentication Classes (Customizable)
 - Built-in Permission Classes (Customizable)
 - Handle Custom Middlewares
 - Handle Custom Throttling 
 ---
 
 ### Installation
 - <details>
     <summary>Create a Virtual Environment</summary>
-    <pre>$ python -m venv .venv</pre>
+    <pre>$ python3 -m venv .venv</pre>
   
   </details>
   
 - <details>
     <summary>Active The Environment</summary>
     * Linux & Mac
       <pre>$ source .venv/bin/activate</pre>
@@ -59,42 +62,46 @@
   
   </details>
  
 - <details open>
     <summary>Install Panther</summary>
     * Normal
       <pre>$ pip install panther</pre>
-    * Include JWT Authentication
+    * Include MongoDB Requirements
       <pre>$ pip install panther[full]</pre>
   </details>
   
 ---
 
 ### Usage
 
 - #### Create Project
 
     ```console
     $ panther create <project_name> <directory>
     ```
 
 - #### Run Project
-    Panther Uses [Uvicorn](https://github.com/encode/uvicorn) as ASGI (Asynchronous Server Gateway Interface)
+
+    Panther uses [Uvicorn](https://github.com/encode/uvicorn) as ASGI (Asynchronous Server Gateway Interface)
+    
     ```console
     $ panther run 
     ```
 
 - #### Monitoring Requests
 
     ```console
     $ panther monitor 
     ```
 
 - #### Python Shell
+
     Panther Uses [bpython](https://bpython-interpreter.org) for shell
+    
     ```console
     $ panther shell 
     ```
 ---
 
 ### Example
 
@@ -142,38 +149,45 @@
     from panther.configs import config
     from panther import version, status
     from panther.request import Request
     from panther.response import Response
     from panther.throttling import Throttling
     
     
+    InfoThrottling = Throttling(rate=5, duration=timedelta(minutes=1))
+  
     @API()
     async def hello_world():
         return {'detail': 'Hello World'}
     
     
-    @API(cache=True, throttling=Throttling(rate=5, duration=timedelta(minutes=1)))
+    @API(cache=True, throttling=InfoThrottling)
     async def info(request: Request):
         data = {
             'version': version(),
             'datetime_now': datetime.now().isoformat(),
             'user_agent': request.headers.user_agent,
             'db_engine': config['db_engine'],
         }
         return Response(data=data, status_code=status.HTTP_202_ACCEPTED)
     ```
 
-- <b> Then run (`$ panther run`) the project, now you can see these two urls:</b>
+- Then **run** the project:
+  
+  - `$ cd myproject`
+  - `$ panther run` or `$ panther run --reload` 
+  
+  now you can see these two urls:</b>
 
   * [http://127.0.0.1:8000/](http://127.0.0.1:8000/)
 
   * [http://127.0.0.1:8000/info/](http://127.0.0.1:8000/info/)
 
 
-  
+
 > **Writing Your First CRUD: [First CRUD](https://pantherpy.github.io/first_crud)**
 
 ---
 
 
 **<details>
     <summary>TODOs**</summary>
@@ -193,22 +207,22 @@
     - &#x2705; Log Queries
     - &#x2705; Add Package Requirements
     - &#x2705; Custom Logging
     - &#x2705; Caching
     - &#x2705; Handle Path Variable
     - &#x2705; Handle Simple Form-Data
     - &#x2705; Handle Throttling
+    - &#x2705; Handle ClassBase APIs
     - &#9744; Handle Complex Form-Data
     - &#9744; Handle File 
     - &#9744; Handle Cookie
     - &#9744; Handle WS 
     - &#9744; Handle GraphQL
     - &#9744; Handle Testing
     - &#9744; Generate Swagger For APIs
-    - &#9744; Handle ClassBase APIs
   
   </details>
 
 - <details>
     <summary>Database</summary>
   
     - &#x2705; Structure Of DB Connection
```

#### html2text {}

```diff
@@ -1,82 +1,84 @@
-Metadata-Version: 2.1 Name: panther Version: 2.0.0 Summary: Fast & Friendly,
+Metadata-Version: 2.1 Name: panther Version: 2.1.0 Summary: Fast & Friendly,
 Web Framework For Building Async APIs Home-page: https://github.com/alirn76/
 panther Author: Ali RajabNezhad Author-email: alirn76@yahoo.com License: MIT
 Classifier: Operating System :: OS Independent Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Python: >=3.10 Description-Content-Type:
 text/markdown Provides-Extra: full License-File: LICENSE ## Panther Is A Fast &
 Friendly Web Framework For Building Async APIs With Python 3.11+
-                                    [logo]
+[logo]
 [logo] Supported byJetBrain
 **_Full Documentation:_** [https://pantherpy.github.io](https://
-pantherpy.github.io) --- ### Why Use Panther? - Document-oriented Databases ODM
-([PantherDB](https://pypi.org/project/pantherdb/), MongoDB) - Visual API
-Monitoring (In Terminal) - Caching for APIs (In Memory, In Redis) - Built-in
-Authentication Classes (Customizable) - Built-in Permission Classes
+pantherpy.github.io) **_PyPI:_** [https://pypi.org/project/panther/](https://
+pypi.org/project/panther/) --- ### Why Use Panther ? - Document-oriented
+Databases ODM ([PantherDB](https://pypi.org/project/pantherdb/), MongoDB) -
+Visual API Monitoring (In Terminal) - Cache APIs (In Memory, In Redis) - Built-
+in Authentication Classes (Customizable) - Built-in Permission Classes
 (Customizable) - Handle Custom Middlewares - Handle Custom Throttling --- ###
 Installation -  Create a Virtual Environment
-$ python -m venv .venv
+$ python3 -m venv .venv
  -  Active The Environment * Linux & Mac
 $ source .venv/bin/activate
 * Windows
 $ .\.venv\Scripts\activate
  -  Install Panther * Normal
 $ pip install panther
-* Include JWT Authentication
+* Include MongoDB Requirements
 $ pip install panther[full]
  --- ### Usage - #### Create Project ```console $ panther create   ``` - ####
-Run Project Panther Uses [Uvicorn](https://github.com/encode/uvicorn) as ASGI
+Run Project Panther uses [Uvicorn](https://github.com/encode/uvicorn) as ASGI
 (Asynchronous Server Gateway Interface) ```console $ panther run ``` - ####
 Monitoring Requests ```console $ panther monitor ``` - #### Python Shell
 Panther Uses [bpython](https://bpython-interpreter.org) for shell ```console $
 panther shell ``` --- ### Example - #### You can create project with ```console
 $ panther create myproject ``` - #### or create it yourself: **core/
 configs.py**: ```python URLs = 'core/urls.py' ``` **core/urls.py**: ```python
 from app.urls import urls as app_urls urls = { '/': app_urls, } ``` **app/
 urls.py**: ```python from app.apis import hello_world, info urls = { '':
 hello_world, 'info/': info, } ``` **app/apis.py**: ```python from datetime
 import datetime, timedelta from panther.app import API from panther.configs
 import config from panther import version, status from panther.request import
 Request from panther.response import Response from panther.throttling import
-Throttling @API() async def hello_world(): return {'detail': 'Hello World'}
-@API(cache=True, throttling=Throttling(rate=5, duration=timedelta(minutes=1)))
-async def info(request: Request): data = { 'version': version(),
-'datetime_now': datetime.now().isoformat(), 'user_agent':
-request.headers.user_agent, 'db_engine': config['db_engine'], } return Response
-(data=data, status_code=status.HTTP_202_ACCEPTED) ``` - Then run (`$ panther
-run`) the project, now you can see these two urls: * [http://127.0.0.1:8000/]
-(http://127.0.0.1:8000/) * [http://127.0.0.1:8000/info/](http://127.0.0.1:8000/
-info/) > **Writing Your First CRUD: [First CRUD](https://pantherpy.github.io/
-first_crud)** --- ** TODOs** -  Base - &#x2705; Start with Uvicorn - &#x2705;
-Fix URL Routing - &#x2705; Read Configs - &#x2705; Handle Exceptions - &#x2705;
-Add Custom Logger - &#x2705; Request Class - &#x2705; Response Class - &#x2705;
-Validate Input - &#x2705; Custom Output Model - &#x2705; Log Queries - &#x2705;
-Add Package Requirements - &#x2705; Custom Logging - &#x2705; Caching -
-&#x2705; Handle Path Variable - &#x2705; Handle Simple Form-Data - &#x2705;
-Handle Throttling - ☐ Handle Complex Form-Data - ☐ Handle File - ☐ Handle
-Cookie - ☐ Handle WS - ☐ Handle GraphQL - ☐ Handle Testing - ☐ Generate Swagger
-For APIs - ☐ Handle ClassBase APIs  -  Database - &#x2705; Structure Of DB
-Connection - &#x2705; PantherDB Connection - &#x2705; MongoDB Connection -
-&#x2705; Create Custom BaseModel For All Type Of Databases - &#x2705; Set
-PantherDB As Default  -  Custom ODM - &#x2705; Find One - &#x2705; Find -
-&#x2705; Last - &#x2705; Count - &#x2705; Insert One - &#x2705; Insert Many -
-&#x2705; Delete One - &#x2705; Delete Many - &#x2705; Delete Itself - &#x2705;
-Update One - &#x2705; Update Many - &#x2705; Update Itself - &#x2705; Find or
-Insert - &#x2705; Save - ☐ Find or Raise - ☐ Find with Pagination - ☐
-Aggregation - ☐ Complex Pipelines - ☐ ...  -  Middleware - &#x2705; Add
-Middlewares To Structure - &#x2705; Create BaseMiddleware - &#x2705; Pass
-Custom Parameters To Middlewares - &#x2705; Handle Custom Middlewares  -
-Authentication - &#x2705; JWT Authentication - &#x2705; Separate Auth For Every
-API - &#x2705; Handle Permissions - ☐ Token Storage Authentication - ☐ Cookie
-Authentication - ☐ Query Param Authentication - ☐ Store JWT After Logout In
-Redis/ Memory  -  Cache - &#x2705; Add Redis To Structure - &#x2705; Create
-Cache Decorator - &#x2705; Handle In-Memory Caching - &#x2705; Handle In Redis
-Caching - ☐ Write Async LRU_Caching With TTL (Replace it with in-memory ...)  -
-CLI - &#x2705; Create Project - &#x2705; Run Project - &#x2705; Create Project
-with Options - &#x2705; Monitoring With Textual - &#x2705; Monitor Requests,
-Response & Time  -  Documentation - &#x2705; Create MkDocs For Project -
-&#x2705; Benchmarks - &#x2705; Release Notes - &#x2705; Features - ☐ Complete
-The MkDoc  -  Tests - &#x2705; Start Writing Tests For Panther - ☐ Test Client
---- ### Support **If you find this project useful, please give it a star
-â­ï¸.**
+Throttling InfoThrottling = Throttling(rate=5, duration=timedelta(minutes=1))
+@API() async def hello_world(): return {'detail': 'Hello World'} @API
+(cache=True, throttling=InfoThrottling) async def info(request: Request): data
+= { 'version': version(), 'datetime_now': datetime.now().isoformat(),
+'user_agent': request.headers.user_agent, 'db_engine': config['db_engine'], }
+return Response(data=data, status_code=status.HTTP_202_ACCEPTED) ``` - Then
+**run** the project: - `$ cd myproject` - `$ panther run` or `$ panther run --
+reload` now you can see these two urls:
+ * [http://127.0.0.1:8000/](http://127.0.0.1:8000/) * [http://127.0.0.1:8000/
+info/](http://127.0.0.1:8000/info/) > **Writing Your First CRUD: [First CRUD]
+(https://pantherpy.github.io/first_crud)** --- ** TODOs** -  Base - &#x2705;
+Start with Uvicorn - &#x2705; Fix URL Routing - &#x2705; Read Configs -
+&#x2705; Handle Exceptions - &#x2705; Add Custom Logger - &#x2705; Request
+Class - &#x2705; Response Class - &#x2705; Validate Input - &#x2705; Custom
+Output Model - &#x2705; Log Queries - &#x2705; Add Package Requirements -
+&#x2705; Custom Logging - &#x2705; Caching - &#x2705; Handle Path Variable -
+&#x2705; Handle Simple Form-Data - &#x2705; Handle Throttling - &#x2705; Handle
+ClassBase APIs - ☐ Handle Complex Form-Data - ☐ Handle File - ☐ Handle Cookie -
+☐ Handle WS - ☐ Handle GraphQL - ☐ Handle Testing - ☐ Generate Swagger For APIs
+-  Database - &#x2705; Structure Of DB Connection - &#x2705; PantherDB
+Connection - &#x2705; MongoDB Connection - &#x2705; Create Custom BaseModel For
+All Type Of Databases - &#x2705; Set PantherDB As Default  -  Custom ODM -
+&#x2705; Find One - &#x2705; Find - &#x2705; Last - &#x2705; Count - &#x2705;
+Insert One - &#x2705; Insert Many - &#x2705; Delete One - &#x2705; Delete Many
+- &#x2705; Delete Itself - &#x2705; Update One - &#x2705; Update Many -
+&#x2705; Update Itself - &#x2705; Find or Insert - &#x2705; Save - ☐ Find or
+Raise - ☐ Find with Pagination - ☐ Aggregation - ☐ Complex Pipelines - ☐ ...  -
+Middleware - &#x2705; Add Middlewares To Structure - &#x2705; Create
+BaseMiddleware - &#x2705; Pass Custom Parameters To Middlewares - &#x2705;
+Handle Custom Middlewares  -  Authentication - &#x2705; JWT Authentication -
+&#x2705; Separate Auth For Every API - &#x2705; Handle Permissions - ☐ Token
+Storage Authentication - ☐ Cookie Authentication - ☐ Query Param Authentication
+- ☐ Store JWT After Logout In Redis/ Memory  -  Cache - &#x2705; Add Redis To
+Structure - &#x2705; Create Cache Decorator - &#x2705; Handle In-Memory Caching
+- &#x2705; Handle In Redis Caching - ☐ Write Async LRU_Caching With TTL
+(Replace it with in-memory ...)  -  CLI - &#x2705; Create Project - &#x2705;
+Run Project - &#x2705; Create Project with Options - &#x2705; Monitoring With
+Textual - &#x2705; Monitor Requests, Response & Time  -  Documentation -
+&#x2705; Create MkDocs For Project - &#x2705; Benchmarks - &#x2705; Release
+Notes - &#x2705; Features - ☐ Complete The MkDoc  -  Tests - &#x2705; Start
+Writing Tests For Panther - ☐ Test Client   --- ### Support **If you find this
+project useful, please give it a star â­ï¸.**
```

### Comparing `panther-2.0.0/panther.egg-info/SOURCES.txt` & `panther-2.1.0/panther.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/setup.py` & `panther-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/tests/test_mongodb.py` & `panther-2.1.0/tests/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/tests/test_pantherdb.py` & `panther-2.1.0/tests/test_pantherdb.py`

 * *Files identical despite different names*

### Comparing `panther-2.0.0/tests/test_routing.py` & `panther-2.1.0/tests/test_routing.py`

 * *Files identical despite different names*

