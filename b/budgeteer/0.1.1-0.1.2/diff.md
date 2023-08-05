# Comparing `tmp/budgeteer-0.1.1.tar.gz` & `tmp/budgeteer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "budgeteer-0.1.1.tar", last modified: Sun Jul 30 15:16:26 2023, max compression
+gzip compressed data, was "budgeteer-0.1.2.tar", last modified: Sat Aug  5 10:00:39 2023, max compression
```

## Comparing `budgeteer-0.1.1.tar` & `budgeteer-0.1.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:26.543699 budgeteer-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-30 15:16:04.000000 budgeteer-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-30 15:16:04.000000 budgeteer-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-07-30 15:16:26.543699 budgeteer-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-07-30 15:16:04.000000 budgeteer-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:26.539699 budgeteer-0.1.1/budgeteer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/budget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:26.539699 budgeteer-0.1.1/budgeteer/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/providers/common_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/providers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:26.539699 budgeteer-0.1.1/budgeteer/providers/http_requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/providers/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/providers/http_requests/cache_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/providers/http_requests/cloudflare_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/providers/http_requests/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/providers/sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/providers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:26.539699 budgeteer-0.1.1/budgeteer/web_interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/web_interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:26.539699 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:26.539699 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:26.543699 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    85787 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/@formkit-606708a1.js
--rw-r--r--   0 runner    (1001) docker     (123)    20752 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/@popperjs-8746c87e.js
--rw-r--r--   0 runner    (1001) docker     (123)    64371 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/@vue-de7d3d24.js
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/@vueuse-0fe84a4c.js
--rw-r--r--   0 runner    (1001) docker     (123)    28960 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/axios-4a70c6fc.js
--rw-r--r--   0 runner    (1001) docker     (123)   231964 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-39a9ac22.css
--rw-r--r--   0 runner    (1001) docker     (123)    60654 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-85852bd1.js
--rw-r--r--   0 runner    (1001) docker     (123)   164360 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
--rw-r--r--   0 runner    (1001) docker     (123)    76081 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-abbba2f8.css
--rw-r--r--   0 runner    (1001) docker     (123)   121340 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    23411 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/index-1f8a0d9a.js
--rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/index-e2d31524.css
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
--rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-router-4cd13335.js
--rw-r--r--   0 runner    (1001) docker     (123)    51150 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-tippy-7086acf8.js
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
--rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-6aa87443.js
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vuex-636235de.js
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/web_interface/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:26.539699 budgeteer-0.1.1/budgeteer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-07-30 15:16:26.000000 budgeteer-0.1.1/budgeteer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-30 15:16:26.000000 budgeteer-0.1.1/budgeteer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 15:16:26.000000 budgeteer-0.1.1/budgeteer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-30 15:16:26.000000 budgeteer-0.1.1/budgeteer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 15:16:26.000000 budgeteer-0.1.1/budgeteer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 15:16:26.000000 budgeteer-0.1.1/budgeteer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-30 15:16:26.000000 budgeteer-0.1.1/budgeteer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 15:16:26.543699 budgeteer-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-30 15:16:04.000000 budgeteer-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:39.301003 budgeteer-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-05 10:00:19.000000 budgeteer-0.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-05 10:00:19.000000 budgeteer-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-08-05 10:00:39.301003 budgeteer-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-08-05 10:00:19.000000 budgeteer-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:39.285003 budgeteer-0.1.2/budgeteer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/budget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:39.289003 budgeteer-0.1.2/budgeteer/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/providers/common_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/providers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:39.293003 budgeteer-0.1.2/budgeteer/providers/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/providers/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/providers/http_requests/cache_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/providers/http_requests/cloudflare_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/providers/http_requests/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/providers/sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/providers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:39.293003 budgeteer-0.1.2/budgeteer/web_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/web_interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:39.285003 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:39.293003 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:39.301003 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    85787 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/@formkit-606708a1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20752 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/@popperjs-8746c87e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    64371 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/@vue-de7d3d24.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/@vueuse-0fe84a4c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28960 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/axios-4a70c6fc.js
+-rw-r--r--   0 runner    (1001) docker     (123)   231964 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-39a9ac22.css
+-rw-r--r--   0 runner    (1001) docker     (123)    60654 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-85852bd1.js
+-rw-r--r--   0 runner    (1001) docker     (123)   164360 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    76081 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-abbba2f8.css
+-rw-r--r--   0 runner    (1001) docker     (123)   121340 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    24455 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/index-9c267a1e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/index-e2d31524.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-router-4cd13335.js
+-rw-r--r--   0 runner    (1001) docker     (123)    51150 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-tippy-7086acf8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-6aa87443.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vuex-636235de.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/web_interface/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:39.289003 budgeteer-0.1.2/budgeteer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-08-05 10:00:39.000000 budgeteer-0.1.2/budgeteer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-08-05 10:00:39.000000 budgeteer-0.1.2/budgeteer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 10:00:39.000000 budgeteer-0.1.2/budgeteer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-05 10:00:39.000000 budgeteer-0.1.2/budgeteer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 10:00:39.000000 budgeteer-0.1.2/budgeteer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 10:00:39.000000 budgeteer-0.1.2/budgeteer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-05 10:00:39.000000 budgeteer-0.1.2/budgeteer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 10:00:39.301003 budgeteer-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-08-05 10:00:19.000000 budgeteer-0.1.2/setup.py
```

### Comparing `budgeteer-0.1.1/LICENSE.md` & `budgeteer-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/PKG-INFO` & `budgeteer-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: budgeteer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Einfacher Überblick über das eigene Budget
 Home-page: https://github.com/rix1337/BudgeTeer
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `budgeteer-0.1.1/README.md` & `budgeteer-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/budget.py` & `budgeteer-0.1.2/budgeteer/budget.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/providers/common_functions.py` & `budgeteer-0.1.2/budgeteer/providers/common_functions.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/providers/config.py` & `budgeteer-0.1.2/budgeteer/providers/config.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/providers/http_requests/cache_handler.py` & `budgeteer-0.1.2/budgeteer/providers/http_requests/cache_handler.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/providers/http_requests/cloudflare_handlers.py` & `budgeteer-0.1.2/budgeteer/providers/http_requests/cloudflare_handlers.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/providers/http_requests/request_handler.py` & `budgeteer-0.1.2/budgeteer/providers/http_requests/request_handler.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/providers/shared_state.py` & `budgeteer-0.1.2/budgeteer/providers/shared_state.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/providers/sqlite_database.py` & `budgeteer-0.1.2/budgeteer/providers/sqlite_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 
 def remove_redundant_db_tables(file):
     conn = sqlite3.connect(file)
     cursor = conn.cursor()
 
     keep_tables = [
         'BudgeTeer',
-        'json'
+        'json',
+        'secrets'
     ]
 
     cursor.execute("SELECT name FROM sqlite_master WHERE type='table'")
     table_names = [row[0] for row in cursor.fetchall()]
 
     tables_to_drop = set(table_names) - set(keep_tables)
```

### Comparing `budgeteer-0.1.1/budgeteer/providers/version.py` & `budgeteer-0.1.2/budgeteer/providers/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import re
 from distutils.version import StrictVersion
 from urllib.request import urlopen
 
 
 def get_version():
-    return "0.1.1"
+    return "0.1.2"
 
 
 def create_version_file():
     version = get_version()
     version_clean = re.sub('[^\d\.]', '', version)
     if "a" in version:
         suffix = version.split("a")[1]
```

### Comparing `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/@formkit-606708a1.js` & `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/@formkit-606708a1.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/@popperjs-8746c87e.js` & `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/@popperjs-8746c87e.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/@vue-de7d3d24.js` & `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/@vue-de7d3d24.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/@vueuse-0fe84a4c.js` & `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/@vueuse-0fe84a4c.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/axios-4a70c6fc.js` & `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/axios-4a70c6fc.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-39a9ac22.css` & `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-39a9ac22.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-85852bd1.js` & `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-85852bd1.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff` & `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-abbba2f8.css` & `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-abbba2f8.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2` & `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/index-1f8a0d9a.js` & `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/index-9c267a1e.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,1026 +1,1075 @@
 import {
-    b as j,
-    r as V,
-    c as O,
-    U as a,
-    F as i,
+    c as P,
+    r as U,
+    U as i,
+    F as l,
     N as e,
-    q as B,
-    P as D,
-    O as N,
+    q as D,
+    P as C,
+    O as T,
     S as L,
-    _ as w,
+    _ as V,
     $ as S,
     u as s,
     a0 as W,
-    M as v,
-    s as P,
-    W as $,
+    M as f,
+    s as j,
+    W as y,
     J as I,
-    X as z
+    b as z,
+    X as R
 } from "./@vue-de7d3d24.js";
 import {
-    u as M,
-    c as R
+    u as N,
+    c as A
 } from "./vuex-636235de.js";
 import {
-    a as C
+    a as B
 } from "./axios-4a70c6fc.js";
 import {
-    c as A,
-    a as H
+    c as H,
+    a as q
 } from "./vue-router-4cd13335.js";
 import "./bootstrap-85852bd1.js"; /* empty css                        */
 import {
-    u as E,
-    s as q,
-    T
+    u as F,
+    s as J,
+    T as K
 } from "./vue-toastification-6aa87443.js";
 import {
     s as Y,
     p as G,
-    d as J,
-    a as X
+    d as X,
+    a as Q
 } from "./@formkit-606708a1.js";
 import {
-    V as Q
+    V as Z
 } from "./vue-tippy-7086acf8.js"; /* empty css                 */
 import {
-    u as Z,
-    a as x
+    u as x,
+    a as tt
 } from "./@vueuse-0fe84a4c.js";
 import "./@popperjs-8746c87e.js";
 (function() {
     const t = document.createElement("link").relList;
     if (t && t.supports && t.supports("modulepreload")) return;
-    for (const d of document.querySelectorAll('link[rel="modulepreload"]')) m(d);
-    new MutationObserver(d => {
-        for (const c of d)
-            if (c.type === "childList")
-                for (const p of c.addedNodes) p.tagName === "LINK" && p.rel === "modulepreload" && m(p)
+    for (const c of document.querySelectorAll('link[rel="modulepreload"]')) _(c);
+    new MutationObserver(c => {
+        for (const n of c)
+            if (n.type === "childList")
+                for (const p of n.addedNodes) p.tagName === "LINK" && p.rel === "modulepreload" && _(p)
     }).observe(document, {
         childList: !0,
         subtree: !0
     });
 
-    function f(d) {
-        const c = {};
-        return d.integrity && (c.integrity = d.integrity), d.referrerPolicy && (c.referrerPolicy = d.referrerPolicy), d.crossOrigin === "use-credentials" ? c.credentials = "include" : d.crossOrigin === "anonymous" ? c.credentials = "omit" : c.credentials = "same-origin", c
+    function v(c) {
+        const n = {};
+        return c.integrity && (n.integrity = c.integrity), c.referrerPolicy && (n.referrerPolicy = c.referrerPolicy), c.crossOrigin === "use-credentials" ? n.credentials = "include" : c.crossOrigin === "anonymous" ? n.credentials = "omit" : n.credentials = "same-origin", n
     }
 
-    function m(d) {
-        if (d.ep) return;
-        d.ep = !0;
-        const c = f(d);
-        fetch(d.href, c)
+    function _(c) {
+        if (c.ep) return;
+        c.ep = !0;
+        const n = v(c);
+        fetch(c.href, n)
     }
 })();
-const tt = {
+const et = {
         class: "container"
     },
-    et = {
+    st = {
         class: "row my-3"
     },
-    st = {
+    ot = {
         class: "col-md-10 offset-md-1"
     },
-    ot = {
+    nt = {
         class: "card text-center shadow my-3"
     },
-    nt = {
+    at = {
         class: "card-header"
     },
-    at = e("i", {
+    it = e("i", {
         class: "bi-cash-coin"
     }, null, -1),
-    it = {
-        class: "card-body"
-    },
     lt = {
-        class: "row justify-content-center mt-2"
+        class: "card-body"
     },
     ct = {
         class: "row justify-content-center mt-2"
     },
     dt = {
-        class: "input-group"
+        class: "row justify-content-center mt-2"
     },
     rt = {
+        class: "input-group"
+    },
+    ut = {
         class: "input-group-prepend"
     },
-    ut = ["disabled", "onUpdate:modelValue"],
+    pt = ["disabled", "onUpdate:modelValue"],
     bt = ["disabled", "onUpdate:modelValue"],
-    pt = e("div", {
+    _t = e("div", {
         class: "input-group-append"
     }, [e("span", {
         class: "input-group-text"
     }, " €")], -1),
-    _t = {
+    mt = {
         key: 0,
         class: "input-group-append"
     },
-    mt = ["disabled", "onUpdate:modelValue"],
-    ht = e("option", {
+    ht = ["disabled", "onUpdate:modelValue"],
+    gt = e("option", {
         value: "checking"
     }, "Girokonto", -1),
-    gt = e("option", {
+    ft = e("option", {
         value: "savings"
     }, "Sparkonto", -1),
-    ft = [ht, gt],
-    vt = {
+    vt = [gt, ft],
+    kt = {
         key: 1,
         class: "input-group-append"
     },
-    kt = ["onClick"],
-    $t = e("i", {
+    $t = ["onClick"],
+    yt = e("i", {
         class: "bi bi-arrow-up"
     }, null, -1),
-    yt = [$t],
-    wt = ["onClick"],
+    wt = [yt],
+    Vt = ["onClick"],
     Ct = e("i", {
         class: "bi bi-arrow-down"
     }, null, -1),
-    Vt = [Ct],
-    Dt = ["onClick"],
+    Dt = [Ct],
+    Bt = ["onClick"],
     St = e("i", {
         class: "bi bi-trash3"
     }, null, -1),
-    Bt = [St],
-    Ut = {
+    Ut = [St],
+    Mt = {
         key: 0,
         class: "row justify-content-center mt-2"
     },
-    Nt = {
+    Tt = {
         __name: "Head",
-        setup(_) {
-            const t = M(),
-                f = E();
-            t.commit("getBalances"), j(() => {
-                p(), setInterval(p, 300 * 1e3)
-            });
-
-            function m() {
-                window.open("https://github.com/rix1337/BudgeTeer/releases/latest", "_blank")
-            }
-            const d = V(""),
-                c = V(!1);
-
-            function p() {
-                C.get("api/version/").then(function(n) {
-                    d.value = n.data.version.ver, console.info("%c BudgeTeer %c ".concat(d.value, " "), "color: white; background: #303030; font-weight: 700; font-size: 24px; font-family: Monospace;", "color: #303030; background: white; font-weight: 700; font-size: 24px; font-family: Monospace;"), console.info("%c ❤ Projekt unterstützen %c ".concat("https://github.com/sponsors/rix1337 ❤", " "), "color: white; background: #dc3545; font-weight: 700;", "color: #dc3545; background: white; font-weight: 700;"), c.value = n.data.version.update_ready, t.commit("setDocker", n.data.version.docker), c.value && (h("BudgeTeer - Update verfügbar! - "), console.log("Update steht bereit! Weitere Informationen unter https://github.com/rix1337/BudgeTeer/releases/latest"), f.info(`Update steht bereit! Weitere Informationen unter:
-https://github.com/rix1337/BudgeTeer/releases/latest`, {
-                        timeout: 15e3,
-                        onClick: m
-                    }))
-                }, function() {
-                    console.log("Konnte Version nicht abrufen!"), f.error("Konnte Version nicht abrufen!")
-                })
-            }
-
-            function h(n) {
-                document.title = n, setTimeout(function() {
-                    h(n.substr(1) + n.substr(0, 1))
-                }, 200)
-            }
-            const u = O({
+        setup(b) {
+            const t = N();
+            t.commit("getBalances");
+            const v = P({
                 get() {
                     let n = 0;
-                    for (let r = 0; r < t.state.data.open_transactions.length; r++) {
-                        let l = parseFloat(t.state.data.open_transactions[r].amount);
-                        isNaN(l) || (n += l)
+                    for (let o = 0; o < t.state.data.open_transactions.length; o++) {
+                        let r = parseFloat(t.state.data.open_transactions[o].amount);
+                        isNaN(r) || (n += r)
                     }
-                    let g = 0;
-                    for (let r = 0; r < t.state.data.balances.length; r++) {
-                        let l = parseFloat(t.state.data.balances[r].balance);
-                        !isNaN(l) && t.state.data.balances[r].type === "checking" && (g += l)
+                    let p = 0;
+                    for (let o = 0; o < t.state.data.balances.length; o++) {
+                        let r = parseFloat(t.state.data.balances[o].balance);
+                        !isNaN(r) && t.state.data.balances[o].type === "checking" && (p += r)
                     }
-                    let o = 0;
-                    for (let r = 0; r < t.state.data.budgets.length; r++)
-                        for (let l = 0; l < t.state.data.budgets[r].entries.length; l++) {
-                            let k = parseFloat(t.state.data.budgets[r].entries[l].amount);
-                            !isNaN(k) && y(t.state.data.budgets[r].entries[l]) && (o += k)
+                    let m = 0;
+                    for (let o = 0; o < t.state.data.budgets.length; o++)
+                        for (let r = 0; r < t.state.data.budgets[o].entries.length; r++) {
+                            let k = parseFloat(t.state.data.budgets[o].entries[r].amount);
+                            !isNaN(k) && _(t.state.data.budgets[o].entries[r]) && (m += k)
                         }
-                    return (g + n + o).toFixed(2)
+                    return (p + n + m).toFixed(2)
                 }
             });
 
-            function y(n) {
-                if (!n.booked) {
-                    let g = new Date,
-                        o = new Date("1970-01-01"),
-                        r = new Date("2100-01-01");
-                    return n.valid_from_to[0] !== null && (o = new Date(n.valid_from_to[0])), n.valid_from_to[1] !== null && (r = new Date(n.valid_from_to[1])), g >= o && g <= r
+            function _(n) {
+                if (n.booked !== t.state.display_month) {
+                    let p = new Date,
+                        m = new Date("1970-01-01"),
+                        o = new Date("2100-01-01");
+                    return n.valid_from_to[0] !== null && (m = new Date(n.valid_from_to[0])), n.valid_from_to[1] !== null && (o = new Date(n.valid_from_to[1])), p >= m && p <= o
                 }
                 return !1
             }
-            const b = V(new Date().toLocaleString("default", {
+            const c = U(new Date().toLocaleString("default", {
                 month: "long"
             }));
-            return (n, g) => (a(), i("div", tt, [e("div", et, [e("div", st, [e("div", ot, [e("div", nt, [e("h1", null, [at, B(" Verfügbar im " + D(b.value) + ": " + D(u.value) + " €", 1)])]), e("div", it, [e("div", lt, [e("div", ct, [(a(!0), i(N, null, L(s(t).state.data.balances, (o, r) => (a(), i("div", {
-                key: o,
+            return (n, p) => (i(), l("div", et, [e("div", st, [e("div", ot, [e("div", nt, [e("div", at, [e("h1", null, [it, D(" Verfügbar im " + C(c.value) + ": " + C(v.value) + " €", 1)])]), e("div", lt, [e("div", ct, [e("div", dt, [(i(!0), l(T, null, L(s(t).state.data.balances, (m, o) => (i(), l("div", {
+                key: m,
                 class: "balance"
-            }, [e("div", dt, [e("div", rt, [w(e("input", {
+            }, [e("div", rt, [e("div", ut, [V(e("input", {
                 disabled: s(t).state.locked,
-                "onUpdate:modelValue": l => s(t).state.data.balances[r].label = l,
+                "onUpdate:modelValue": r => s(t).state.data.balances[o].label = r,
                 class: "form-control"
-            }, null, 8, ut), [
-                [S, s(t).state.data.balances[r].label]
-            ])]), w(e("input", {
+            }, null, 8, pt), [
+                [S, s(t).state.data.balances[o].label]
+            ])]), V(e("input", {
                 disabled: s(t).state.locked,
-                "onUpdate:modelValue": l => s(t).state.data.balances[r].balance = l,
+                "onUpdate:modelValue": r => s(t).state.data.balances[o].balance = r,
                 type: "number",
                 step: "0.01",
                 class: "form-control"
             }, null, 8, bt), [
-                [S, s(t).state.data.balances[r].balance]
-            ]), pt, s(t).state.locked ? v("", !0) : (a(), i("div", _t, [w(e("select", {
+                [S, s(t).state.data.balances[o].balance]
+            ]), _t, s(t).state.locked ? f("", !0) : (i(), l("div", mt, [V(e("select", {
                 disabled: s(t).state.locked,
-                "onUpdate:modelValue": l => s(t).state.data.balances[r].type = l,
+                "onUpdate:modelValue": r => s(t).state.data.balances[o].type = r,
                 class: "form-control"
-            }, ft, 8, mt), [
-                [W, s(t).state.data.balances[r].type]
-            ])])), s(t).state.locked ? v("", !0) : (a(), i("div", vt, [e("button", {
+            }, vt, 8, ht), [
+                [W, s(t).state.data.balances[o].type]
+            ])])), s(t).state.locked ? f("", !0) : (i(), l("div", kt, [e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: l => s(t).state.data.balances.splice(r - 1, 0, s(t).state.data.balances.splice(r, 1)[0])
-            }, yt, 8, kt), e("button", {
+                onClick: r => s(t).state.data.balances.splice(o - 1, 0, s(t).state.data.balances.splice(o, 1)[0])
+            }, wt, 8, $t), e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: l => s(t).state.data.balances.splice(r + 1, 0, s(t).state.data.balances.splice(r, 1)[0])
-            }, Vt, 8, wt), e("button", {
+                onClick: r => s(t).state.data.balances.splice(o + 1, 0, s(t).state.data.balances.splice(o, 1)[0])
+            }, Dt, 8, Vt), e("button", {
                 class: "btn btn-outline-danger",
                 type: "button",
-                onClick: l => s(t).state.data.balances.splice(r, 1)
-            }, Bt, 8, Dt)]))])]))), 128)), s(t).state.locked ? v("", !0) : (a(), i("div", Ut, [e("button", {
+                onClick: r => s(t).state.data.balances.splice(o, 1)
+            }, Ut, 8, Bt)]))])]))), 128)), s(t).state.locked ? f("", !0) : (i(), l("div", Mt, [e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: g[0] || (g[0] = o => s(t).state.data.balances.push({
+                onClick: p[0] || (p[0] = m => s(t).state.data.balances.push({
                     label: "",
                     amount: ""
                 }))
             }, " Konto hinzufügen ")]))])])])])])])]))
         }
     };
-const Mt = {
+const Nt = {
         class: "text-center"
     },
-    Tt = {
+    Kt = {
         id: "offcanvasBottomSettings",
         "aria-labelledby": "offcanvasBottomSettingsLabel",
         class: "offcanvas offcanvas-bottom",
         tabindex: "-1"
     },
-    Kt = e("div", {
+    Et = e("div", {
         class: "offcanvas-header"
     }, [e("h3", {
         id: "offcanvasBottomSettingsLabel",
         class: "offcanvas-title"
     }, [e("i", {
         class: "bi bi-gear"
-    }), B(" Einstellungen")]), e("button", {
+    }), D(" Einstellungen")]), e("button", {
         "aria-label": "Close",
         class: "btn-close text-reset",
         "data-bs-dismiss": "offcanvas",
         type: "button"
     })], -1),
     Lt = {
         class: "offcanvas-body"
     },
-    Et = {
+    Ft = {
         key: 0
     },
-    Ft = {
+    Ot = {
         key: 1,
         id: "accordionSettings",
         class: "accordion"
     },
-    Ot = {
+    Pt = {
         key: 0
     },
-    Pt = {
+    Wt = {
         key: 0,
         class: "spinner-border spinner-border-sm",
         role: "status"
     },
     jt = {
         key: 1,
         class: "bi bi-save"
     },
-    Wt = {
+    It = {
         key: 1,
         class: "btn btn-dark disabled"
     },
-    It = e("span", {
+    zt = e("span", {
         class: "spinner-border spinner-border-sm",
         role: "status"
     }, null, -1),
-    zt = {
+    Rt = {
         __name: "Settings",
-        setup(_) {
-            const t = M(),
-                f = E();
+        setup(b) {
+            const t = N(),
+                v = F();
 
-            function m() {
-                d.value = !0, C.post("api/settings/", t.state.settings).then(function() {
-                    console.log("Einstellungen gespeichert! Neustart des BudgeTeers wird dringend empfohlen!"), f.success("Einstellungen gespeichert! Neustart des BudgeTeers wird dringend empfohlen!"), t.commit("getSettings"), d.value = !1
+            function _() {
+                c.value = !0, B.post("api/settings/", t.state.settings).then(function() {
+                    console.log("Einstellungen gespeichert! Neustart des BudgeTeers wird dringend empfohlen!"), v.success("Einstellungen gespeichert! Neustart des BudgeTeers wird dringend empfohlen!"), t.commit("getSettings"), c.value = !1
                 }, function() {
-                    t.commit("getSettings"), d.value = !1, console.log("Konnte Einstellungen nicht speichern! Bitte die angegebenen Werte auf Richtigkeit prüfen."), f.error("Konnte Einstellungen nicht speichern! Bitte die angegebenen Werte auf Richtigkeit prüfen.")
+                    t.commit("getSettings"), c.value = !1, console.log("Konnte Einstellungen nicht speichern! Bitte die angegebenen Werte auf Richtigkeit prüfen."), v.error("Konnte Einstellungen nicht speichern! Bitte die angegebenen Werte auf Richtigkeit prüfen.")
                 })
             }
-            const d = V(!1),
-                c = O(() => t.state.settings.general.auth_hash.length > 0);
+            const c = U(!1),
+                n = P(() => t.state.settings.general.auth_hash.length > 0);
 
             function p() {
                 Y("settings")
             }
-            return (h, u) => {
-                const y = P("FormKit");
-                return a(), i("div", Mt, [e("div", Tt, [Kt, e("div", Lt, [s(t).state.misc.loaded_settings ? v("", !0) : (a(), i("h4", Et, "Einstellungen werden geladen...")), s(t).state.misc.loaded_settings ? (a(), i("div", Ft, [$(y, {
+            return (m, o) => {
+                const r = j("FormKit");
+                return i(), l("div", Nt, [e("div", Kt, [Et, e("div", Lt, [s(t).state.misc.loaded_settings ? f("", !0) : (i(), l("h4", Ft, "Einstellungen werden geladen...")), s(t).state.misc.loaded_settings ? (i(), l("div", Ot, [y(r, {
                     id: "settings",
                     actions: !1,
                     "incomplete-message": "Es müssen alle Felder korrekt ausgefüllt werden! Fehler sind rot markiert.",
                     "messages-class": "text-danger mt-4",
                     type: "form",
-                    onSubmit: u[4] || (u[4] = b => m())
+                    onSubmit: o[4] || (o[4] = k => _())
                 }, {
                     default: I(({
-                        value: b
-                    }) => [s(t).state.misc.docker ? v("", !0) : (a(), i("div", Ot, [$(y, {
+                        value: k
+                    }) => [s(t).state.misc.docker ? f("", !0) : (i(), l("div", Pt, [y(r, {
                         modelValue: s(t).state.settings.general.port,
-                        "onUpdate:modelValue": u[0] || (u[0] = n => s(t).state.settings.general.port = n),
+                        "onUpdate:modelValue": o[0] || (o[0] = d => s(t).state.settings.general.port = d),
                         help: "Hier den Port des Webservers wählen.",
                         "help-class": "text-muted",
                         "input-class": "form-control bg-light mb-2",
                         label: "Port",
                         "messages-class": "text-danger",
                         "outer-class": "mb-4",
                         placeholder: "Bspw. 9090",
                         type: "number",
                         validation: "required|between:1024,65535",
                         "validation-visibility": "live"
-                    }, null, 8, ["modelValue"])])), $(y, {
+                    }, null, 8, ["modelValue"])])), y(r, {
                         modelValue: s(t).state.settings.general.prefix,
-                        "onUpdate:modelValue": u[1] || (u[1] = n => s(t).state.settings.general.prefix = n),
+                        "onUpdate:modelValue": o[1] || (o[1] = d => s(t).state.settings.general.prefix = d),
                         help: "Hier den Prefix des Webservers wählen (nützlich für Reverse-Proxies).",
                         "help-class": "text-muted",
                         "input-class": "form-control bg-light mb-2",
                         label: "Prefix",
                         "messages-class": "text-danger",
                         "outer-class": "mb-4",
                         placeholder: "Bspw. budgeteer",
                         type: "text",
                         validation: "alpha",
                         "validation-visibility": "live"
-                    }, null, 8, ["modelValue"]), $(y, {
+                    }, null, 8, ["modelValue"]), y(r, {
                         modelValue: s(t).state.settings.general.auth_user,
-                        "onUpdate:modelValue": u[2] || (u[2] = n => s(t).state.settings.general.auth_user = n),
-                        validation: b.auth_hash ? "required" : "",
+                        "onUpdate:modelValue": o[2] || (o[2] = d => s(t).state.settings.general.auth_user = d),
+                        validation: k.auth_hash ? "required" : "",
                         help: "Hier den Nutzernamen für BudgeTeer eingeben.",
                         "help-class": "text-muted",
                         "input-class": "form-control bg-light mb-2",
                         label: "Nutzername",
                         "messages-class": "text-danger",
                         name: "auth_user",
                         "outer-class": "mb-4",
                         placeholder: "Bspw. rix1337",
                         type: "text"
-                    }, null, 8, ["modelValue", "validation"]), $(y, {
+                    }, null, 8, ["modelValue", "validation"]), y(r, {
                         modelValue: s(t).state.settings.general.auth_hash,
-                        "onUpdate:modelValue": u[3] || (u[3] = n => s(t).state.settings.general.auth_hash = n),
-                        validation: c.value && b.auth_user ? "required|length:6" : "",
+                        "onUpdate:modelValue": o[3] || (o[3] = d => s(t).state.settings.general.auth_hash = d),
+                        validation: n.value && k.auth_user ? "required|length:6" : "",
                         help: "Hier das Passwort für BudgeTeer angeben.",
                         "help-class": "text-muted",
                         "input-class": "form-control bg-light mb-2",
                         label: "Passwort",
                         "messages-class": "text-danger",
                         name: "auth_hash",
                         "outer-class": "mb-4",
                         placeholder: "Bspw. ●●●●●●●●",
                         type: "password",
                         "validation-visibility": "live"
                     }, null, 8, ["modelValue", "validation"])]),
                     _: 1
-                })])) : v("", !0), e("div", null, [s(t).state.misc.loaded_settings ? (a(), i("button", {
+                })])) : f("", !0), e("div", null, [s(t).state.misc.loaded_settings ? (i(), l("button", {
                     key: 0,
                     class: "btn btn-primary mt-4",
                     type: "submit",
                     onClick: p
-                }, [d.value ? (a(), i("span", Pt)) : v("", !0), d.value ? v("", !0) : (a(), i("i", jt)), B(" Speichern ")])) : (a(), i("button", Wt, [It, B(" Lädt... ")]))])])])])
+                }, [c.value ? (i(), l("span", Wt)) : f("", !0), c.value ? f("", !0) : (i(), l("i", jt)), D(" Speichern ")])) : (i(), l("button", It, [zt, D(" Lädt... ")]))])])])])
             }
         }
     },
-    Rt = {
+    At = {
         class: "container"
     },
-    At = {
+    Ht = {
         class: "row my-3"
     },
-    Ht = {
+    qt = {
         class: "col-md-10 offset-md-1"
     },
-    qt = {
+    Jt = {
         class: "card text-center shadow my-3"
     },
     Yt = e("div", {
         class: "card-header"
     }, [e("h1", null, [e("i", {
         class: "bi bi-clock-history"
-    }), B(" Offene Transaktionen ")])], -1),
+    }), D(" Offene Transaktionen ")])], -1),
     Gt = {
         class: "card-body"
     },
-    Jt = {
+    Xt = {
         class: "row justify-content-center mt-2"
     },
-    Xt = {
+    Qt = {
         class: "input-group"
     },
-    Qt = {
+    Zt = {
         class: "input-group-prepend"
     },
-    Zt = ["disabled", "onUpdate:modelValue"],
     xt = ["disabled", "onUpdate:modelValue"],
-    te = e("div", {
+    te = ["disabled", "onUpdate:modelValue"],
+    ee = e("div", {
         class: "input-group-append"
     }, [e("span", {
         class: "input-group-text"
     }, " €")], -1),
-    ee = {
+    se = {
         key: 0,
         class: "input-group-append"
     },
-    se = ["onClick"],
-    oe = e("i", {
+    oe = ["onClick"],
+    ne = e("i", {
         class: "bi bi-arrow-up"
     }, null, -1),
-    ne = [oe],
-    ae = ["onClick"],
-    ie = e("i", {
+    ae = [ne],
+    ie = ["onClick"],
+    le = e("i", {
         class: "bi bi-arrow-down"
     }, null, -1),
-    le = [ie],
-    ce = {
+    ce = [le],
+    de = {
         class: "input-group-append"
     },
-    de = ["onClick"],
-    re = e("i", {
+    re = ["onClick"],
+    ue = e("i", {
         class: "bi bi-trash3"
     }, null, -1),
-    ue = [re],
+    pe = [ue],
     be = {
         class: "row justify-content-center mt-2"
     },
-    pe = {
+    _e = {
         __name: "Transactions",
-        setup(_) {
-            const t = M();
-            return t.commit("getOpenTransactions"), (f, m) => (a(), i("div", Rt, [e("div", At, [e("div", Ht, [e("div", qt, [Yt, e("div", Gt, [e("div", Jt, [(a(!0), i(N, null, L(s(t).state.data.open_transactions, (d, c) => (a(), i("div", {
-                key: d,
+        setup(b) {
+            const t = N();
+            return t.commit("getOpenTransactions"), (v, _) => (i(), l("div", At, [e("div", Ht, [e("div", qt, [e("div", Jt, [Yt, e("div", Gt, [e("div", Xt, [(i(!0), l(T, null, L(s(t).state.data.open_transactions, (c, n) => (i(), l("div", {
+                key: c,
                 class: "transaction"
-            }, [e("div", Xt, [e("div", Qt, [w(e("input", {
+            }, [e("div", Qt, [e("div", Zt, [V(e("input", {
                 disabled: s(t).state.locked,
-                "onUpdate:modelValue": p => s(t).state.data.open_transactions[c].label = p,
+                "onUpdate:modelValue": p => s(t).state.data.open_transactions[n].label = p,
                 class: "form-control"
-            }, null, 8, Zt), [
-                [S, s(t).state.data.open_transactions[c].label]
-            ])]), w(e("input", {
+            }, null, 8, xt), [
+                [S, s(t).state.data.open_transactions[n].label]
+            ])]), V(e("input", {
                 disabled: s(t).state.locked,
-                "onUpdate:modelValue": p => s(t).state.data.open_transactions[c].amount = p,
+                "onUpdate:modelValue": p => s(t).state.data.open_transactions[n].amount = p,
                 type: "number",
                 step: "0.01",
                 class: "form-control"
-            }, null, 8, xt), [
-                [S, s(t).state.data.open_transactions[c].amount]
-            ]), te, s(t).state.locked ? v("", !0) : (a(), i("div", ee, [e("button", {
+            }, null, 8, te), [
+                [S, s(t).state.data.open_transactions[n].amount]
+            ]), ee, s(t).state.locked ? f("", !0) : (i(), l("div", se, [e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: p => s(t).state.data.open_transactions.splice(c - 1, 0, s(t).state.data.open_transactions.splice(c, 1)[0])
-            }, ne, 8, se), e("button", {
+                onClick: p => s(t).state.data.open_transactions.splice(n - 1, 0, s(t).state.data.open_transactions.splice(n, 1)[0])
+            }, ae, 8, oe), e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: p => s(t).state.data.open_transactions.splice(c + 1, 0, s(t).state.data.open_transactions.splice(c, 1)[0])
-            }, le, 8, ae)])), e("div", ce, [e("button", {
+                onClick: p => s(t).state.data.open_transactions.splice(n + 1, 0, s(t).state.data.open_transactions.splice(n, 1)[0])
+            }, ce, 8, ie)])), e("div", de, [e("button", {
                 class: "btn btn-outline-danger",
                 type: "button",
-                onClick: p => s(t).state.data.open_transactions.splice(c, 1) && s(t).commit("setModifiedWhileLocked", !0)
-            }, ue, 8, de)])])]))), 128)), e("div", be, [s(t).state.locked ? v("", !0) : (a(), i("button", {
+                onClick: p => s(t).state.data.open_transactions.splice(n, 1) && s(t).commit("setModifiedWhileLocked", !0)
+            }, pe, 8, re)])])]))), 128)), e("div", be, [s(t).state.locked ? f("", !0) : (i(), l("button", {
                 key: 0,
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: m[0] || (m[0] = d => s(t).state.data.open_transactions.push({
+                onClick: _[0] || (_[0] = c => s(t).state.data.open_transactions.push({
                     label: "",
                     amount: ""
                 }))
             }, " Transaktion hinzufügen "))])])])])])])]))
         }
     },
-    _e = {
+    me = {
         class: "col-md-auto p-1"
     },
-    me = e("i", {
+    he = e("i", {
         class: "bi bi-arrow-left"
     }, null, -1),
-    he = [me],
-    ge = {
+    ge = [he],
+    fe = {
         key: 0
     },
-    fe = {
+    ve = {
         key: 1
     },
-    ve = e("i", {
+    ke = e("i", {
         class: "bi bi-arrow-right"
     }, null, -1),
-    ke = [ve],
-    F = {
+    $e = [ke],
+    O = {
         __name: "DatePicker",
         props: {
             title: String,
             modelValue: String
         },
         emits: ["update:modelValue"],
-        setup(_, {
+        setup(b, {
             emit: t
         }) {
-            const f = _,
-                m = V(f.modelValue);
+            const v = b,
+                _ = U(v.modelValue);
 
-            function d(p) {
-                m.value === null && (m.value = new Date().toLocaleDateString("en-CA", {
+            function c(p) {
+                _.value === null && (_.value = new Date().toLocaleDateString("en-CA", {
                     year: "numeric",
                     month: "2-digit"
                 }));
-                const h = new Date(m.value);
-                h.setMonth(h.getMonth() + p), h.setDate(1);
-                const u = h.toLocaleDateString("en-CA", {
+                const m = new Date(_.value);
+                m.setMonth(m.getMonth() + p), m.setDate(1);
+                const o = m.toLocaleDateString("en-CA", {
                     year: "numeric",
                     month: "2-digit"
                 });
-                m.value = u, t("update:modelValue", u)
+                _.value = o, t("update:modelValue", o)
             }
 
-            function c() {
-                m.value = null, t("update:modelValue", null)
+            function n() {
+                _.value = null, t("update:modelValue", null)
             }
-            return (p, h) => (a(), i("div", _e, [e("button", {
+            return (p, m) => (i(), l("div", me, [e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: h[0] || (h[0] = u => d(-1))
-            }, he), B(D(f.title) + " ", 1), _.modelValue !== null ? (a(), i("span", ge, D(_.modelValue), 1)) : (a(), i("span", fe, "∞ ")), e("button", {
+                onClick: m[0] || (m[0] = o => c(-1))
+            }, ge), D(C(v.title) + " ", 1), b.modelValue !== null ? (i(), l("span", fe, C(b.modelValue), 1)) : (i(), l("span", ve, "∞ ")), e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: h[1] || (h[1] = u => d(1))
-            }, ke), e("button", {
+                onClick: m[1] || (m[1] = o => c(1))
+            }, $e), e("button", {
                 class: "btn btn-outline-secondary",
-                onClick: c
+                onClick: n
             }, " ∞ ")]))
         }
     },
-    $e = {
+    ye = {
         class: "container"
     },
-    ye = {
+    we = {
         class: "row my-3"
     },
-    we = {
+    Ve = {
         class: "col-md-10 offset-md-1"
     },
     Ce = {
         class: "card text-center shadow my-3"
     },
-    Ve = {
+    De = {
         class: "card-header"
     },
-    De = e("i", {
+    Be = e("i", {
         class: "bi bi-receipt-cutoff"
     }, null, -1),
     Se = ["disabled"],
-    Be = e("i", {
+    Ue = e("i", {
         class: "bi bi-arrow-left"
     }, null, -1),
-    Ue = [Be],
-    Ne = ["disabled"],
-    Me = e("i", {
+    Me = [Ue],
+    Te = ["disabled"],
+    Ne = e("i", {
         class: "bi bi-arrow-right"
     }, null, -1),
-    Te = [Me],
-    Ke = e("div", {
+    Ke = [Ne],
+    Ee = e("div", {
         class: "col-md-auto p-1"
     }, null, -1),
     Le = {
         class: "card-body"
     },
-    Ee = {
+    Fe = {
         class: "row justify-content-center mt-2"
     },
-    Fe = {
+    Oe = {
         class: "accordion",
         id: "accordionBudgets"
     },
-    Oe = ["id"],
-    Pe = ["data-bs-target", "aria-controls"],
+    Pe = ["id"],
+    We = ["data-bs-target", "aria-controls"],
     je = ["data-bs-target", "aria-controls"],
-    We = ["onUpdate:modelValue"],
-    Ie = ["onClick"],
-    ze = e("i", {
+    Ie = ["onUpdate:modelValue"],
+    ze = ["onClick"],
+    Re = e("i", {
         class: "bi bi-trash3"
     }, null, -1),
-    Re = [ze],
-    Ae = ["id", "aria-labelledby"],
-    He = {
+    Ae = [Re],
+    He = ["id", "aria-labelledby"],
+    qe = {
         class: "accordion-body"
     },
-    qe = {
+    Je = {
         key: 0,
         class: "input-group"
     },
     Ye = {
         class: "input-group-prepend"
     },
     Ge = ["disabled", "onUpdate:modelValue"],
-    Je = ["disabled", "onUpdate:modelValue"],
-    Xe = e("div", {
+    Xe = ["disabled", "onUpdate:modelValue"],
+    Qe = e("div", {
         class: "input-group-append"
     }, [e("span", {
         class: "input-group-text"
     }, " €")], -1),
-    Qe = {
+    Ze = {
         key: 0,
         class: "input-group-append"
     },
-    Ze = ["onClick"],
-    xe = e("i", {
+    xe = ["onClick"],
+    ts = e("i", {
         class: "bi bi-x"
     }, null, -1),
-    ts = [xe],
-    es = ["onClick"],
-    ss = e("i", {
+    es = [ts],
+    ss = ["onClick"],
+    os = e("i", {
         class: "bi bi-arrow-up"
     }, null, -1),
-    os = [ss],
-    ns = ["onClick"],
-    as = e("i", {
+    ns = [os],
+    as = ["onClick"],
+    is = e("i", {
         class: "bi bi-arrow-down"
     }, null, -1),
-    is = [as],
-    ls = ["onClick"],
-    cs = e("i", {
+    ls = [is],
+    cs = ["onClick"],
+    ds = e("i", {
         class: "bi bi-trash3"
     }, null, -1),
-    ds = [cs],
-    rs = {
+    rs = [ds],
+    us = {
+        key: 1,
+        class: "input-group-append"
+    },
+    ps = ["disabled", "onUpdate:modelValue"],
+    bs = e("option", {
+        value: "monthly"
+    }, "Monatlich", -1),
+    _s = e("option", {
+        value: "weekly"
+    }, "Wöchentlich", -1),
+    ms = e("option", {
+        value: "yearly"
+    }, "Jährlich", -1),
+    hs = e("option", {
+        value: "one-time"
+    }, "Einmalig", -1),
+    gs = [bs, _s, ms, hs],
+    fs = {
         class: "input-group-append"
     },
-    us = ["onClick"],
-    bs = e("i", {
+    vs = ["onClick"],
+    ks = e("i", {
         class: "bi bi-check"
     }, null, -1),
-    ps = [bs],
-    _s = ["onClick"],
-    ms = {
+    $s = [ks],
+    ys = ["onClick"],
+    ws = {
         class: "row justify-content-center mt-2"
     },
-    hs = {
+    Vs = {
         __name: "Budgets",
-        setup(_) {
-            const t = M();
+        setup(b) {
+            const t = N();
             t.commit("getBudgets");
 
-            function f(b) {
-                return parseFloat(b).toFixed(2)
+            function v(d) {
+                return parseFloat(d).toFixed(2)
+            }
+
+            function _(d) {
+                let u = 0;
+                for (let h = 0; h < t.state.data.budgets[d].entries.length; h++)
+                    if (m(t.state.data.budgets[d].entries[h])) {
+                        let a = parseFloat(t.state.data.budgets[d].entries[h].amount);
+                        isNaN(a) || (u += a)
+                    } return v(u)
             }
 
-            function m(b) {
-                let n = 0;
-                for (let g = 0; g < t.state.data.budgets[b].entries.length; g++)
-                    if (u(t.state.data.budgets[b].entries[g])) {
-                        let o = parseFloat(t.state.data.budgets[b].entries[g].amount);
-                        isNaN(o) || (n += o)
-                    } return f(n)
+            function c() {
+                let d = new Date(t.state.display_month),
+                    u = new Date;
+                return d.getMonth() === u.getMonth() && d.getFullYear() === u.getFullYear()
+            }
+            const n = U(0);
+
+            function p(d) {
+                n.value += d;
+                let u = new Date().setMonth(new Date().getMonth() + n.value);
+                t.commit("setDisplayMonth", new Date(u).toISOString().slice(0, 7))
             }
 
-            function d() {
-                let b = new Date(c.value),
-                    n = new Date;
-                return b.getMonth() === n.getMonth() && b.getFullYear() === n.getFullYear()
+            function m(d) {
+                return c() ? !k(d) && r(d) : r(d)
             }
-            const c = V(new Date().toISOString().slice(0, 7)),
-                p = V(0);
 
-            function h(b) {
-                p.value += b;
-                let n = new Date().setMonth(new Date().getMonth() + p.value);
-                c.value = new Date(n).toISOString().slice(0, 7)
+            function o(d) {
+                return t.state.locked && c() ? !k(d) && r(d) : r(d)
             }
 
-            function u(b) {
-                return t.state.locked && d() ? !b.booked && y(b) : b
+            function r(d) {
+                let u = new Date(t.state.display_month),
+                    h = new Date("1970-01-01"),
+                    a = new Date("2100-01-01");
+                return d.valid_from_to[0] !== null && (h = new Date(d.valid_from_to[0])), d.valid_from_to[1] !== null && (a = new Date(d.valid_from_to[1])), u >= h && u <= a
             }
 
-            function y(b) {
-                let n = new Date(c.value),
-                    g = new Date("1970-01-01"),
-                    o = new Date("2100-01-01");
-                return b.valid_from_to[0] !== null && (g = new Date(b.valid_from_to[0])), b.valid_from_to[1] !== null && (o = new Date(b.valid_from_to[1])), n >= g && n <= o
+            function k(d) {
+                return d.booked === t.state.display_month
             }
-            return (b, n) => (a(), i("div", $e, [e("div", ye, [e("div", we, [e("div", Ce, [e("div", Ve, [e("h1", null, [De, B(" Budgets " + D(c.value) + " ", 1), e("button", {
-                disabled: p.value <= 0,
+            return (d, u) => (i(), l("div", ye, [e("div", we, [e("div", Ve, [e("div", Ce, [e("div", De, [e("h1", null, [Be, D(" Budgets " + C(s(t).state.display_month) + " ", 1), e("button", {
+                disabled: n.value <= 0,
                 class: "btn btn-outline-primary m-1",
                 type: "button",
-                onClick: n[0] || (n[0] = g => h(-1))
-            }, Ue, 8, Se), e("button", {
-                disabled: p.value >= 13,
+                onClick: u[0] || (u[0] = h => p(-1))
+            }, Me, 8, Se), e("button", {
+                disabled: n.value >= 13,
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: n[1] || (n[1] = g => h(1))
-            }, Te, 8, Ne)]), Ke]), e("div", Le, [e("div", Ee, [e("div", Fe, [(a(!0), i(N, null, L(s(t).state.data.budgets, (g, o) => (a(), i("div", {
-                key: g,
+                onClick: u[1] || (u[1] = h => p(1))
+            }, Ke, 8, Te)]), Ee]), e("div", Le, [e("div", Fe, [e("div", Oe, [(i(!0), l(T, null, L(s(t).state.data.budgets, (h, a) => (i(), l("div", {
+                key: h,
                 class: "accordion-item"
             }, [e("h2", {
                 class: "accordion-header",
-                id: "heading" + o
-            }, [s(t).state.locked ? (a(), i("button", {
+                id: "heading" + a
+            }, [s(t).state.locked ? (i(), l("button", {
                 key: 0,
                 class: "accordion-button collapsed",
                 type: "button",
                 "data-bs-toggle": "collapse",
-                "data-bs-target": "#collapse" + o,
+                "data-bs-target": "#collapse" + a,
                 "aria-expanded": "false",
-                "aria-controls": "collapse" + o
-            }, D(s(t).state.data.budgets[o].category) + ": " + D(m(o)) + " € ", 9, Pe)) : (a(), i("button", {
+                "aria-controls": "collapse" + a
+            }, C(s(t).state.data.budgets[a].category) + ": " + C(_(a)) + " € ", 9, We)) : (i(), l("button", {
                 key: 1,
                 class: "accordion-button collapsed",
                 type: "button",
                 "data-bs-toggle": "collapse",
-                "data-bs-target": "#collapse" + o,
+                "data-bs-target": "#collapse" + a,
                 "aria-expanded": "false",
-                "aria-controls": "collapse" + o
-            }, [w(e("input", {
+                "aria-controls": "collapse" + a
+            }, [V(e("input", {
                 type: "text",
                 class: "form-control",
                 placeholder: "Kategorie",
-                "onUpdate:modelValue": r => s(t).state.data.budgets[o].category = r
-            }, null, 8, We), [
-                [S, s(t).state.data.budgets[o].category]
+                "onUpdate:modelValue": w => s(t).state.data.budgets[a].category = w
+            }, null, 8, Ie), [
+                [S, s(t).state.data.budgets[a].category]
             ]), e("button", {
                 class: "btn btn-outline-danger",
                 type: "button",
-                onClick: r => s(t).state.data.budgets.splice(o, 1) && s(t).commit("setModifiedWhileLocked", !0)
-            }, Re, 8, Ie)], 8, je))], 8, Oe), e("div", {
-                id: "collapse" + o,
+                onClick: w => s(t).state.data.budgets.splice(a, 1) && s(t).commit("setModifiedWhileLocked", !0)
+            }, Ae, 8, ze)], 8, je))], 8, Pe), e("div", {
+                id: "collapse" + a,
                 class: "accordion-collapse collapse",
-                "aria-labelledby": "heading" + o,
+                "aria-labelledby": "heading" + a,
                 "data-bs-parent": "#accordionBudgets"
-            }, [e("div", He, [(a(!0), i(N, null, L(s(t).state.data.budgets[o].entries, (r, l) => (a(), i("div", {
-                key: r
-            }, [u(s(t).state.data.budgets[o].entries[l]) ? (a(), i("div", qe, [e("div", Ye, [w(e("input", {
+            }, [e("div", qe, [(i(!0), l(T, null, L(s(t).state.data.budgets[a].entries, (w, g) => (i(), l("div", {
+                key: w
+            }, [o(s(t).state.data.budgets[a].entries[g]) ? (i(), l("div", Je, [e("div", Ye, [V(e("input", {
                 disabled: s(t).state.locked,
-                "onUpdate:modelValue": k => s(t).state.data.budgets[o].entries[l].label = k,
+                "onUpdate:modelValue": $ => s(t).state.data.budgets[a].entries[g].label = $,
                 class: "form-control"
             }, null, 8, Ge), [
-                [S, s(t).state.data.budgets[o].entries[l].label]
-            ])]), w(e("input", {
+                [S, s(t).state.data.budgets[a].entries[g].label]
+            ])]), V(e("input", {
                 disabled: s(t).state.locked,
-                "onUpdate:modelValue": k => s(t).state.data.budgets[o].entries[l].amount = k,
+                "onUpdate:modelValue": $ => s(t).state.data.budgets[a].entries[g].amount = $,
                 type: "number",
                 step: "0.01",
                 class: "form-control"
-            }, null, 8, Je), [
-                [S, s(t).state.data.budgets[o].entries[l].amount]
-            ]), Xe, s(t).state.locked ? v("", !0) : (a(), i("div", Qe, [d() && s(t).state.data.budgets[o].entries[l].booked ? (a(), i("button", {
+            }, null, 8, Xe), [
+                [S, s(t).state.data.budgets[a].entries[g].amount]
+            ]), Qe, s(t).state.locked ? f("", !0) : (i(), l("div", Ze, [c() && k(s(t).state.data.budgets[a].entries[g]) ? (i(), l("button", {
                 key: 0,
                 class: "btn btn-outline-danger",
                 type: "button",
-                onClick: k => s(t).state.data.budgets[o].entries[l].booked = !1
-            }, ts, 8, Ze)) : v("", !0), e("button", {
+                onClick: $ => s(t).state.data.budgets[a].entries[g].booked = ""
+            }, es, 8, xe)) : f("", !0), e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: k => s(t).state.data.budgets[o].entries.splice(l - 1, 0, s(t).state.data.budgets[o].entries.splice(l, 1)[o])
-            }, os, 8, es), e("button", {
+                onClick: $ => s(t).state.data.budgets[a].entries.splice(g - 1, 0, s(t).state.data.budgets[a].entries.splice(g, 1)[a])
+            }, ns, 8, ss), e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: k => s(t).state.data.budgets[o].entries.splice(l + 1, 0, s(t).state.data.budgets[o].entries.splice(l, 1)[o])
-            }, is, 8, ns), e("button", {
+                onClick: $ => s(t).state.data.budgets[a].entries.splice(g + 1, 0, s(t).state.data.budgets[a].entries.splice(g, 1)[a])
+            }, ls, 8, as), e("button", {
                 class: "btn btn-outline-danger",
                 type: "button",
-                onClick: k => s(t).state.data.budgets[o].entries.splice(l, 1)
-            }, ds, 8, ls), $(F, {
+                onClick: $ => s(t).state.data.budgets[a].entries.splice(g, 1)
+            }, rs, 8, cs), s(t).state.locked ? f("", !0) : (i(), l("div", us, [V(e("select", {
+                disabled: s(t).state.locked,
+                "onUpdate:modelValue": $ => s(t).state.data.budgets[a].entries[g].type = $,
+                class: "form-control"
+            }, gs, 8, ps), [
+                [W, s(t).state.data.budgets[a].entries[g].type]
+            ])])), y(O, {
                 title: "von",
-                modelValue: s(t).state.data.budgets[o].entries[l].valid_from_to[0],
-                "onUpdate:modelValue": k => s(t).state.data.budgets[o].entries[l].valid_from_to[0] = k
-            }, null, 8, ["modelValue", "onUpdate:modelValue"]), $(F, {
+                modelValue: s(t).state.data.budgets[a].entries[g].valid_from_to[0],
+                "onUpdate:modelValue": $ => s(t).state.data.budgets[a].entries[g].valid_from_to[0] = $
+            }, null, 8, ["modelValue", "onUpdate:modelValue"]), y(O, {
                 title: "bis",
-                modelValue: s(t).state.data.budgets[o].entries[l].valid_from_to[1],
-                "onUpdate:modelValue": k => s(t).state.data.budgets[o].entries[l].valid_from_to[1] = k
-            }, null, 8, ["modelValue", "onUpdate:modelValue"])])), e("div", rs, [d() && s(t).state.locked && !s(t).state.data.budgets[o].entries[l].booked ? (a(), i("button", {
+                modelValue: s(t).state.data.budgets[a].entries[g].valid_from_to[1],
+                "onUpdate:modelValue": $ => s(t).state.data.budgets[a].entries[g].valid_from_to[1] = $
+            }, null, 8, ["modelValue", "onUpdate:modelValue"])])), e("div", fs, [c() && s(t).state.locked && !k(s(t).state.data.budgets[a].entries[g]) ? (i(), l("button", {
                 key: 0,
                 class: "btn btn-outline-success",
                 type: "button",
-                onClick: k => {
-                    s(t).commit("setModifiedWhileLocked", !0), s(t).state.data.budgets[o].entries[l].booked = !0
+                onClick: $ => {
+                    s(t).commit("setModifiedWhileLocked", !0), s(t).state.data.budgets[a].entries[g].booked = s(t).state.display_month
                 }
-            }, ps, 8, us)) : v("", !0)])])) : v("", !0)]))), 128)), s(t).state.locked ? v("", !0) : (a(), i("button", {
+            }, $s, 8, vs)) : f("", !0)])])) : f("", !0)]))), 128)), s(t).state.locked ? f("", !0) : (i(), l("button", {
                 key: 0,
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: r => s(t).state.data.budgets[o].entries.push({
+                onClick: w => s(t).state.data.budgets[a].entries.push({
                     label: "",
                     amount: "",
                     valid_from_to: [null, null],
-                    booked: !1
+                    booked: ""
                 })
-            }, " Eintrag hinzufügen ", 8, _s))])], 8, Ae)]))), 128))]), e("div", ms, [s(t).state.locked ? v("", !0) : (a(), i("button", {
+            }, " Eintrag hinzufügen ", 8, ys))])], 8, He)]))), 128))]), e("div", ws, [s(t).state.locked ? f("", !0) : (i(), l("button", {
                 key: 0,
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: n[2] || (n[2] = g => s(t).state.data.budgets.push({
+                onClick: u[2] || (u[2] = h => s(t).state.data.budgets.push({
                     category: "Kategorie",
                     amount: "",
                     entries: []
                 }))
             }, " Kategorie hinzufügen "))])])])])])])]))
         }
     },
-    gs = {
+    Cs = {
         __name: "_Main",
-        setup(_) {
-            return (t, f) => (a(), i("main", null, [$(Nt), $(pe), $(hs), $(zt)]))
+        setup(b) {
+            return (t, v) => (i(), l("main", null, [y(Tt), y(_e), y(Vs), y(Rt)]))
         }
     },
-    fs = A({
-        history: H(),
+    Ds = H({
+        history: q(),
         routes: [{
             path: "/:pathMatch(.*)*",
-            component: gs
+            component: Cs
         }]
     });
-const vs = {
+const Bs = {
+        id: "footer"
+    },
+    Ss = {
+        class: "container text-center"
+    },
+    Us = {
+        class: "text-bg-dark credit"
+    },
+    Ms = e("a", {
+        href: "https://github.com/rix1337/BudgeTeer/",
+        target: "_blank",
+        rel: "noopener noreferrer"
+    }, "RiX", -1),
+    Ts = {
         class: "sticky-bottom float-end"
     },
-    ks = {
+    Ns = {
         class: "col-md-auto p-1"
     },
-    $s = e("i", {
+    Ks = e("i", {
         class: "bi bi-save"
     }, null, -1),
-    ys = [$s],
-    ws = e("i", {
+    Es = [Ks],
+    Ls = e("i", {
         class: "bi bi-unlock"
     }, null, -1),
-    Cs = [ws],
-    Vs = e("i", {
+    Fs = [Ls],
+    Os = e("i", {
         class: "bi bi-lock"
     }, null, -1),
-    Ds = [Vs],
-    Ss = {
+    Ps = [Os],
+    Ws = {
         key: 0,
         class: "bi bi-sun"
     },
-    Bs = {
+    js = {
         key: 1,
         class: "bi bi-moon-stars"
     },
-    Us = e("i", {
+    Is = e("i", {
         class: "bi bi-gear"
     }, null, -1),
-    Ns = [Us],
-    Ms = {
+    zs = [Is],
+    Rs = {
         __name: "App",
-        setup(_) {
-            const t = Z(),
-                f = x(t),
-                m = M(),
-                d = E();
+        setup(b) {
+            const t = x(),
+                v = tt(t),
+                _ = N(),
+                c = F();
 
-            function c(h) {
-                C.post("api/json/" + h + "/", m.state.data[h]).then(function() {
-                    console.log(h + " gespeichert.")
+            function n(u) {
+                B.post("api/json/" + u + "/", _.state.data[u]).then(function() {
+                    console.log(u + " gespeichert.")
                 }, function() {
-                    console.log("Konnte " + h + " nicht speichern!"), d.error("Konnte " + h + " nicht speichern!")
+                    console.log("Konnte " + u + " nicht speichern!"), c.error("Konnte " + u + " nicht speichern!")
                 })
             }
 
             function p() {
-                c("balances"), c("budgets"), c("open_transactions"), m.commit("setLocked", !0), m.commit("setModifiedWhileLocked", !1)
+                n("balances"), n("budgets"), n("open_transactions"), _.commit("setLocked", !0), _.commit("setModifiedWhileLocked", !1)
             }
-            return (h, u) => {
-                const y = P("router-view");
-                return a(), i(N, null, [$(y), e("div", vs, [e("div", ks, [s(m).state.modified_while_locked ? (a(), i("button", {
+            z(() => {
+                k(), setInterval(k, 300 * 1e3)
+            });
+
+            function m() {
+                window.open("https://github.com/rix1337/BudgeTeer/releases/latest", "_blank")
+            }
+            const o = U(""),
+                r = U(!1);
+
+            function k() {
+                B.get("api/version/").then(function(u) {
+                    o.value = u.data.version.ver, console.info("%c BudgeTeer %c ".concat(o.value, " "), "color: white; background: #303030; font-weight: 700; font-size: 24px; font-family: Monospace;", "color: #303030; background: white; font-weight: 700; font-size: 24px; font-family: Monospace;"), console.info("%c ❤ Projekt unterstützen %c ".concat("https://github.com/sponsors/rix1337 ❤", " "), "color: white; background: #dc3545; font-weight: 700;", "color: #dc3545; background: white; font-weight: 700;"), r.value = u.data.version.update_ready, _.commit("setDocker", u.data.version.docker), r.value && (d("BudgeTeer - Update verfügbar! - "), console.log("Update steht bereit! Weitere Informationen unter https://github.com/rix1337/BudgeTeer/releases/latest"), c.info(`Update steht bereit! Weitere Informationen unter:
+https://github.com/rix1337/BudgeTeer/releases/latest`, {
+                        timeout: 15e3,
+                        onClick: m
+                    }))
+                }, function() {
+                    console.log("Konnte Version nicht abrufen!"), c.error("Konnte Version nicht abrufen!")
+                })
+            }
+
+            function d(u) {
+                document.title = u, setTimeout(function() {
+                    d(u.substr(1) + u.substr(0, 1))
+                }, 200)
+            }
+            return (u, h) => {
+                const a = j("router-view");
+                return i(), l(T, null, [y(a), e("div", Bs, [e("div", Ss, [e("p", Us, [D("BudgeTeer " + C(o.value) + " by ", 1), Ms])])]), e("div", Ts, [e("div", Ns, [s(_).state.modified_while_locked ? (i(), l("button", {
                     key: 0,
                     class: "btn btn-outline-warning bg-dark m-1",
                     type: "button",
-                    onClick: u[0] || (u[0] = b => p())
-                }, ys)) : s(m).state.locked ? (a(), i("button", {
+                    onClick: h[0] || (h[0] = w => p())
+                }, Es)) : s(_).state.locked ? (i(), l("button", {
                     key: 1,
                     class: "btn btn-outline-success bg-dark m-1",
                     type: "button",
-                    onClick: u[1] || (u[1] = b => s(m).commit("setLocked", !1))
-                }, Cs)) : (a(), i("button", {
+                    onClick: h[1] || (h[1] = w => s(_).commit("setLocked", !1))
+                }, Fs)) : (i(), l("button", {
                     key: 2,
                     class: "btn btn-outline-danger bg-dark m-1",
                     type: "button",
-                    onClick: u[2] || (u[2] = b => p())
-                }, Ds)), e("button", {
+                    onClick: h[2] || (h[2] = w => p())
+                }, Ps)), e("button", {
                     type: "button",
                     class: "btn btn-outline-secondary bg-dark text-warning m-1",
-                    onClick: u[3] || (u[3] = b => s(f)())
-                }, [s(t) ? (a(), i("i", Ss)) : (a(), i("i", Bs))]), e("button", {
+                    onClick: h[3] || (h[3] = w => s(v)())
+                }, [s(t) ? (i(), l("i", Ws)) : (i(), l("i", js))]), e("button", {
                     "aria-controls": "offcanvasBottomSettings",
                     class: "btn btn-outline-primary bg-dark m-1",
                     "data-bs-target": "#offcanvasBottomSettings",
                     "data-bs-toggle": "offcanvas",
                     type: "button",
-                    onClick: u[4] || (u[4] = b => s(m).commit("getSettings"))
-                }, Ns)])])], 64)
+                    onClick: h[4] || (h[4] = w => s(_).commit("getSettings"))
+                }, zs)])])], 64)
             }
         }
     },
-    K = E(),
-    Ts = R({
+    E = F(),
+    As = A({
         state() {
             return {
                 data: {
                     balances: [],
                     open_transactions: [],
                     budgets: []
                 },
+                display_month: new Date().toISOString().slice(0, 7),
                 locked: !0,
                 modified_while_locked: !1,
                 settings: {},
                 misc: {
                     loaded_settings: !1,
                     docker: !1
                 }
             }
         },
         mutations: {
-            getSettings(_) {
-                C.get("api/settings/").then(function(t) {
-                    _.settings = t.data.settings, _.misc.loaded_settings = !0
+            setDisplayMonth(b, t) {
+                b.display_month = t
+            },
+            getSettings(b) {
+                B.get("api/settings/").then(function(t) {
+                    b.settings = t.data.settings, b.misc.loaded_settings = !0
                 }, function() {
-                    console.log("Konnte Einstellungen nicht abrufen!"), K.error("Konnte Einstellungen nicht abrufen!")
+                    console.log("Konnte Einstellungen nicht abrufen!"), E.error("Konnte Einstellungen nicht abrufen!")
                 })
             },
-            getBalances(_) {
-                C.get("api/json/balances/").then(function(t) {
-                    _.data.balances = t.data.balances
+            getBalances(b) {
+                B.get("api/json/balances/").then(function(t) {
+                    b.data.balances = t.data.balances
                 }, function() {
-                    console.log("Konnte Kontostände nicht abrufen!"), K.error("Konnte Kontostände nicht abrufen!")
+                    console.log("Konnte Kontostände nicht abrufen!"), E.error("Konnte Kontostände nicht abrufen!")
                 })
             },
-            getOpenTransactions(_) {
-                C.get("api/json/open_transactions/").then(function(t) {
-                    _.data.open_transactions = t.data.open_transactions
+            getOpenTransactions(b) {
+                B.get("api/json/open_transactions/").then(function(t) {
+                    b.data.open_transactions = t.data.open_transactions
                 }, function() {
-                    console.log("Konnte offene Transaktionen nicht abrufen!"), K.error("Konnte offene Transaktionen nicht abrufen!")
+                    console.log("Konnte offene Transaktionen nicht abrufen!"), E.error("Konnte offene Transaktionen nicht abrufen!")
                 })
             },
-            getBudgets(_) {
-                C.get("api/json/budgets/").then(function(t) {
-                    _.data.budgets = t.data.budgets
+            getBudgets(b) {
+                B.get("api/json/budgets/").then(function(t) {
+                    b.data.budgets = t.data.budgets
                 }, function() {
-                    console.log("Konnte Budgets nicht abrufen!"), K.error("Konnte Budgets nicht abrufen!")
+                    console.log("Konnte Budgets nicht abrufen!"), E.error("Konnte Budgets nicht abrufen!")
                 })
             },
-            setDocker(_, t) {
-                _.misc.docker = t
+            setDocker(b, t) {
+                b.misc.docker = t
             },
-            setLocked(_, t) {
-                _.locked = t
+            setLocked(b, t) {
+                b.locked = t
             },
-            setModifiedWhileLocked(_, t) {
-                _.modified_while_locked = t
+            setModifiedWhileLocked(b, t) {
+                b.modified_while_locked = t
             }
         }
     }),
-    U = z(Ms);
-U.use(Ts);
-U.use(fs);
-U.use(q, {
+    M = R(Rs);
+M.use(As);
+M.use(Ds);
+M.use(J, {
     position: "top-center",
     draggable: !1,
     maxToasts: 1,
     bodyClassName: ["toast-body"],
     toastDefaults: {
-        [T.ERROR]: {
+        [K.ERROR]: {
             icon: "bi bi-exclamation-triangle"
         },
-        [T.WARNING]: {
+        [K.WARNING]: {
             icon: "bi bi-exclamation-circle"
         },
-        [T.INFO]: {
+        [K.INFO]: {
             icon: "bi bi-info-circle"
         },
-        [T.SUCCESS]: {
+        [K.SUCCESS]: {
             icon: "bi bi-check-circle-fill",
             timeout: 3e3
         }
     }
 });
-U.use(Q);
-U.use(G, J({
+M.use(Z);
+M.use(G, X({
     locales: {
-        de: X
+        de: Q
     },
     locale: "de"
 }));
-U.mount("#app");
+M.mount("#app");
```

### Comparing `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/index-e2d31524.css` & `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/index-e2d31524.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css` & `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-router-4cd13335.js` & `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-router-4cd13335.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-tippy-7086acf8.js` & `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-tippy-7086acf8.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css` & `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-6aa87443.js` & `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-6aa87443.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vuex-636235de.js` & `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vuex-636235de.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/favicon.ico` & `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/index.html` & `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 <head>
     <meta charset="UTF-8">
     <meta content="width=device-width, initial-scale=1, shrink-to-fit=no" name="viewport">
 
     <link href="./favicon.ico" rel="icon" type="image/x-icon">
 
     <title>BudgeTeer</title>
-  <script type="module" crossorigin src="./assets/index-1f8a0d9a.js"></script>
+  <script type="module" crossorigin src="./assets/index-9c267a1e.js"></script>
   <link rel="modulepreload" crossorigin href="./assets/@vue-de7d3d24.js">
   <link rel="modulepreload" crossorigin href="./assets/vuex-636235de.js">
   <link rel="modulepreload" crossorigin href="./assets/axios-4a70c6fc.js">
   <link rel="modulepreload" crossorigin href="./assets/vue-router-4cd13335.js">
   <link rel="modulepreload" crossorigin href="./assets/@popperjs-8746c87e.js">
   <link rel="modulepreload" crossorigin href="./assets/bootstrap-85852bd1.js">
   <link rel="modulepreload" crossorigin href="./assets/vue-toastification-6aa87443.js">
```

### Comparing `budgeteer-0.1.1/budgeteer/web_interface/web_server.py` & `budgeteer-0.1.2/budgeteer/web_interface/web_server.py`

 * *Files 5% similar despite different names*

```diff
@@ -163,24 +163,17 @@
 
     def to_int(i):
         if isinstance(i, bytes):
             i = i.decode()
         i = str(i).strip().replace("None", "")
         return int(i) if i else ""
 
-    def to_float(i):
-        i = str(i).strip().replace("None", "")
-        return float(i) if i else ""
-
     def to_str(i):
         return '' if i is None else str(i)
 
-    def to_bool(i):
-        return True if i == "True" else False
-
     @app.get(prefix + "/api/settings/")
     @auth_basic(is_authenticated_user)
     def get_settings():
         try:
             general_conf = BudgetConfig('BudgeTeer')
             return {
                 "settings": {
```

### Comparing `budgeteer-0.1.1/budgeteer.egg-info/PKG-INFO` & `budgeteer-0.1.2/budgeteer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: budgeteer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Einfacher Überblick über das eigene Budget
 Home-page: https://github.com/rix1337/BudgeTeer
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `budgeteer-0.1.1/budgeteer.egg-info/SOURCES.txt` & `budgeteer-0.1.2/budgeteer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 budgeteer/web_interface/vuejs_frontend/dist/assets/@vueuse-0fe84a4c.js
 budgeteer/web_interface/vuejs_frontend/dist/assets/axios-4a70c6fc.js
 budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-39a9ac22.css
 budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-85852bd1.js
 budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
 budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-abbba2f8.css
 budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
-budgeteer/web_interface/vuejs_frontend/dist/assets/index-1f8a0d9a.js
+budgeteer/web_interface/vuejs_frontend/dist/assets/index-9c267a1e.js
 budgeteer/web_interface/vuejs_frontend/dist/assets/index-e2d31524.css
 budgeteer/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
 budgeteer/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
 budgeteer/web_interface/vuejs_frontend/dist/assets/vue-router-4cd13335.js
 budgeteer/web_interface/vuejs_frontend/dist/assets/vue-tippy-7086acf8.js
 budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
 budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-6aa87443.js
```

### Comparing `budgeteer-0.1.1/setup.py` & `budgeteer-0.1.2/setup.py`

 * *Files identical despite different names*

