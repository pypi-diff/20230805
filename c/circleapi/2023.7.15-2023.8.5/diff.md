# Comparing `tmp/circleapi-2023.7.15.tar.gz` & `tmp/circleapi-2023.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circleapi-2023.7.15.tar", last modified: Sun Jul 30 20:29:04 2023, max compression
+gzip compressed data, was "circleapi-2023.8.5.tar", last modified: Sat Aug  5 11:06:09 2023, max compression
```

## Comparing `circleapi-2023.7.15.tar` & `circleapi-2023.8.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 20:29:04.308481 circleapi-2023.7.15/
--rw-rw-rw-   0        0        0      103 2023-07-30 20:29:04.307483 circleapi-2023.7.15/PKG-INFO
--rw-rw-rw-   0        0        0     1336 2023-07-15 19:17:32.000000 circleapi-2023.7.15/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 20:29:04.290339 circleapi-2023.7.15/circleapi/
--rw-rw-rw-   0        0        0      456 2023-07-23 12:23:54.000000 circleapi-2023.7.15/circleapi/__init__.py
--rw-rw-rw-   0        0        0    13161 2023-07-23 13:34:50.000000 circleapi-2023.7.15/circleapi/api.py
--rw-rw-rw-   0        0        0    10949 2023-07-23 13:33:41.000000 circleapi-2023.7.15/circleapi/async_api.py
--rw-rw-rw-   0        0        0     9614 2023-06-24 17:36:26.000000 circleapi-2023.7.15/circleapi/async_token.py
--rw-rw-rw-   0        0        0     1088 2023-07-09 11:05:09.000000 circleapi-2023.7.15/circleapi/logger.py
--rw-rw-rw-   0        0        0    11684 2023-07-23 13:33:41.000000 circleapi-2023.7.15/circleapi/models.py
--rw-rw-rw-   0        0        0     9340 2023-06-24 17:36:26.000000 circleapi-2023.7.15/circleapi/token.py
--rw-rw-rw-   0        0        0      610 2023-06-24 17:23:47.000000 circleapi-2023.7.15/circleapi/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-30 20:29:04.298401 circleapi-2023.7.15/circleapi.egg-info/
--rw-rw-rw-   0        0        0      103 2023-07-30 20:29:04.000000 circleapi-2023.7.15/circleapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      443 2023-07-30 20:29:04.000000 circleapi-2023.7.15/circleapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 20:29:04.000000 circleapi-2023.7.15/circleapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-07-30 20:29:04.000000 circleapi-2023.7.15/circleapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-30 20:29:04.000000 circleapi-2023.7.15/circleapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 20:29:04.308481 circleapi-2023.7.15/setup.cfg
--rw-rw-rw-   0        0        0      298 2023-07-30 20:19:54.000000 circleapi-2023.7.15/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 20:29:04.306379 circleapi-2023.7.15/tests/
--rw-rw-rw-   0        0        0     3333 2023-07-23 12:25:20.000000 circleapi-2023.7.15/tests/test_api.py
--rw-rw-rw-   0        0        0     3307 2023-07-16 09:37:06.000000 circleapi-2023.7.15/tests/test_async_api.py
--rw-rw-rw-   0        0        0     1369 2023-06-24 21:36:58.000000 circleapi-2023.7.15/tests/test_async_ratelimit.py
--rw-rw-rw-   0        0        0     1229 2023-07-02 09:32:49.000000 circleapi-2023.7.15/tests/test_ratelimit.py
+drwxrwxrwx   0        0        0        0 2023-08-05 11:06:09.845596 circleapi-2023.8.5/
+-rw-rw-rw-   0        0        0      247 2023-08-05 11:06:09.844589 circleapi-2023.8.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1377 2023-07-30 20:47:41.000000 circleapi-2023.8.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 11:06:09.825641 circleapi-2023.8.5/circleapi/
+-rw-rw-rw-   0        0        0      456 2023-07-23 12:23:54.000000 circleapi-2023.8.5/circleapi/__init__.py
+-rw-rw-rw-   0        0        0    13161 2023-07-23 13:34:50.000000 circleapi-2023.8.5/circleapi/api.py
+-rw-rw-rw-   0        0        0    10949 2023-07-23 13:33:41.000000 circleapi-2023.8.5/circleapi/async_api.py
+-rw-rw-rw-   0        0        0     9614 2023-06-24 17:36:26.000000 circleapi-2023.8.5/circleapi/async_token.py
+-rw-rw-rw-   0        0        0     1088 2023-07-09 11:05:09.000000 circleapi-2023.8.5/circleapi/logger.py
+-rw-rw-rw-   0        0        0    11684 2023-07-23 13:33:41.000000 circleapi-2023.8.5/circleapi/models.py
+-rw-rw-rw-   0        0        0     9340 2023-06-24 17:36:26.000000 circleapi-2023.8.5/circleapi/token.py
+-rw-rw-rw-   0        0        0      610 2023-06-24 17:23:47.000000 circleapi-2023.8.5/circleapi/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-05 11:06:09.835615 circleapi-2023.8.5/circleapi.egg-info/
+-rw-rw-rw-   0        0        0      247 2023-08-05 11:06:09.000000 circleapi-2023.8.5/circleapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      443 2023-08-05 11:06:09.000000 circleapi-2023.8.5/circleapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 11:06:09.000000 circleapi-2023.8.5/circleapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-08-05 11:06:09.000000 circleapi-2023.8.5/circleapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-05 11:06:09.000000 circleapi-2023.8.5/circleapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 11:06:09.845596 circleapi-2023.8.5/setup.cfg
+-rw-rw-rw-   0        0        0      490 2023-08-05 11:02:45.000000 circleapi-2023.8.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 11:06:09.842596 circleapi-2023.8.5/tests/
+-rw-rw-rw-   0        0        0     3333 2023-07-23 12:25:20.000000 circleapi-2023.8.5/tests/test_api.py
+-rw-rw-rw-   0        0        0     3307 2023-07-16 09:37:06.000000 circleapi-2023.8.5/tests/test_async_api.py
+-rw-rw-rw-   0        0        0     1369 2023-06-24 21:36:58.000000 circleapi-2023.8.5/tests/test_async_ratelimit.py
+-rw-rw-rw-   0        0        0     1229 2023-07-02 09:32:49.000000 circleapi-2023.8.5/tests/test_ratelimit.py
```

### Comparing `circleapi-2023.7.15/README.md` & `circleapi-2023.8.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 - Built-in rate limiting
 - Built-in thread support
 - Response validation (pydantic)
 
 Installation
 ------------
 
+```bash
+$ pip install circleapi
+```
+
 Development setup
 ```bash
 $ git clone https://github.com/miinorii/circleapi.git
 $ cd circleapi
 $ python -m venv venv
 $ venv/bin/activate # linux
 $ venv/Scripts/activate.bat # windows
```

### Comparing `circleapi-2023.7.15/circleapi/api.py` & `circleapi-2023.8.5/circleapi/api.py`

 * *Files identical despite different names*

### Comparing `circleapi-2023.7.15/circleapi/async_api.py` & `circleapi-2023.8.5/circleapi/async_api.py`

 * *Files identical despite different names*

### Comparing `circleapi-2023.7.15/circleapi/async_token.py` & `circleapi-2023.8.5/circleapi/async_token.py`

 * *Files identical despite different names*

### Comparing `circleapi-2023.7.15/circleapi/logger.py` & `circleapi-2023.8.5/circleapi/logger.py`

 * *Files identical despite different names*

### Comparing `circleapi-2023.7.15/circleapi/models.py` & `circleapi-2023.8.5/circleapi/models.py`

 * *Files identical despite different names*

### Comparing `circleapi-2023.7.15/circleapi/token.py` & `circleapi-2023.8.5/circleapi/token.py`

 * *Files identical despite different names*

### Comparing `circleapi-2023.7.15/circleapi/utils.py` & `circleapi-2023.8.5/circleapi/utils.py`

 * *Files identical despite different names*

### Comparing `circleapi-2023.7.15/tests/test_api.py` & `circleapi-2023.8.5/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `circleapi-2023.7.15/tests/test_async_api.py` & `circleapi-2023.8.5/tests/test_async_api.py`

 * *Files identical despite different names*

### Comparing `circleapi-2023.7.15/tests/test_async_ratelimit.py` & `circleapi-2023.8.5/tests/test_async_ratelimit.py`

 * *Files identical despite different names*

### Comparing `circleapi-2023.7.15/tests/test_ratelimit.py` & `circleapi-2023.8.5/tests/test_ratelimit.py`

 * *Files identical despite different names*

