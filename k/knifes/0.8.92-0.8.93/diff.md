# Comparing `tmp/knifes-0.8.92.tar.gz` & `tmp/knifes-0.8.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knifes-0.8.92.tar", last modified: Sat Aug  5 07:42:52 2023, max compression
+gzip compressed data, was "knifes-0.8.93.tar", last modified: Sat Aug  5 15:45:43 2023, max compression
```

## Comparing `knifes-0.8.92.tar` & `knifes-0.8.93.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 hwei       (501) staff       (20)        0 2023-08-05 07:42:52.681356 knifes-0.8.92/
--rw-r--r--   0 hwei       (501) staff       (20)      766 2023-08-05 07:42:52.681189 knifes-0.8.92/PKG-INFO
--rw-r--r--   0 hwei       (501) staff       (20)      400 2022-09-02 05:25:28.000000 knifes-0.8.92/README.md
-drwxr-xr-x   0 hwei       (501) staff       (20)        0 2023-08-05 07:42:52.679915 knifes-0.8.92/knifes/
--rw-r--r--   0 hwei       (501) staff       (20)        0 2022-01-21 03:14:54.000000 knifes-0.8.92/knifes/__init__.py
--rw-r--r--   0 hwei       (501) staff       (20)     1161 2022-02-16 14:49:04.000000 knifes-0.8.92/knifes/aes.py
--rw-r--r--   0 hwei       (501) staff       (20)      573 2023-07-29 07:38:53.000000 knifes-0.8.92/knifes/alarm.py
--rw-r--r--   0 hwei       (501) staff       (20)      740 2022-01-21 03:14:54.000000 knifes-0.8.92/knifes/auth.py
--rw-r--r--   0 hwei       (501) staff       (20)      502 2023-07-29 10:19:19.000000 knifes-0.8.92/knifes/constants.py
--rw-r--r--   0 hwei       (501) staff       (20)     7226 2023-08-05 07:41:23.000000 knifes-0.8.92/knifes/decorators.py
--rw-r--r--   0 hwei       (501) staff       (20)     7567 2023-06-14 01:08:29.000000 knifes-0.8.92/knifes/deploy.py
--rw-r--r--   0 hwei       (501) staff       (20)     1140 2022-10-14 05:30:31.000000 knifes-0.8.92/knifes/digests.py
--rw-r--r--   0 hwei       (501) staff       (20)      363 2023-02-01 04:12:33.000000 knifes-0.8.92/knifes/envconfig.py
--rw-r--r--   0 hwei       (501) staff       (20)     1649 2022-11-17 08:15:03.000000 knifes-0.8.92/knifes/file.py
--rw-r--r--   0 hwei       (501) staff       (20)     5108 2023-06-15 01:37:33.000000 knifes-0.8.92/knifes/getui.py
--rw-r--r--   0 hwei       (501) staff       (20)      732 2022-03-13 09:06:03.000000 knifes-0.8.92/knifes/jsons.py
--rw-r--r--   0 hwei       (501) staff       (20)      403 2023-07-29 07:38:53.000000 knifes-0.8.92/knifes/logging.py
--rw-r--r--   0 hwei       (501) staff       (20)      474 2023-06-15 08:19:17.000000 knifes-0.8.92/knifes/media.py
--rw-r--r--   0 hwei       (501) staff       (20)      924 2023-02-21 04:17:56.000000 knifes-0.8.92/knifes/misc.py
--rw-r--r--   0 hwei       (501) staff       (20)      421 2023-08-04 10:48:49.000000 knifes-0.8.92/knifes/operators.py
--rw-r--r--   0 hwei       (501) staff       (20)      569 2022-11-23 13:58:35.000000 knifes-0.8.92/knifes/package.py
--rw-r--r--   0 hwei       (501) staff       (20)      863 2023-07-31 13:36:03.000000 knifes-0.8.92/knifes/randoms.py
--rw-r--r--   0 hwei       (501) staff       (20)     1527 2023-08-05 07:41:23.000000 knifes-0.8.92/knifes/results.py
--rw-r--r--   0 hwei       (501) staff       (20)     2235 2022-05-30 13:46:32.000000 knifes-0.8.92/knifes/roar.py
--rw-r--r--   0 hwei       (501) staff       (20)      446 2022-01-21 03:14:54.000000 knifes-0.8.92/knifes/shell.py
--rw-r--r--   0 hwei       (501) staff       (20)     2022 2023-07-31 14:57:01.000000 knifes-0.8.92/knifes/sms.py
--rw-r--r--   0 hwei       (501) staff       (20)      889 2023-02-01 04:20:34.000000 knifes-0.8.92/knifes/strings.py
--rw-r--r--   0 hwei       (501) staff       (20)     1335 2023-07-31 13:41:32.000000 knifes-0.8.92/knifes/times.py
--rw-r--r--   0 hwei       (501) staff       (20)     3245 2023-06-15 07:38:41.000000 knifes-0.8.92/knifes/urls.py
--rw-r--r--   0 hwei       (501) staff       (20)     4396 2022-11-25 02:07:08.000000 knifes-0.8.92/knifes/useragent.py
-drwxr-xr-x   0 hwei       (501) staff       (20)        0 2023-08-05 07:42:52.680962 knifes-0.8.92/knifes.egg-info/
--rw-r--r--   0 hwei       (501) staff       (20)      766 2023-08-05 07:42:52.000000 knifes-0.8.92/knifes.egg-info/PKG-INFO
--rw-r--r--   0 hwei       (501) staff       (20)      626 2023-08-05 07:42:52.000000 knifes-0.8.92/knifes.egg-info/SOURCES.txt
--rw-r--r--   0 hwei       (501) staff       (20)        1 2023-08-05 07:42:52.000000 knifes-0.8.92/knifes.egg-info/dependency_links.txt
--rw-r--r--   0 hwei       (501) staff       (20)       27 2023-08-05 07:42:52.000000 knifes-0.8.92/knifes.egg-info/requires.txt
--rw-r--r--   0 hwei       (501) staff       (20)        7 2023-08-05 07:42:52.000000 knifes-0.8.92/knifes.egg-info/top_level.txt
--rw-r--r--   0 hwei       (501) staff       (20)      103 2022-02-08 15:08:46.000000 knifes-0.8.92/pyproject.toml
--rw-r--r--   0 hwei       (501) staff       (20)       38 2023-08-05 07:42:52.681402 knifes-0.8.92/setup.cfg
--rw-r--r--   0 hwei       (501) staff       (20)      901 2023-08-05 07:42:44.000000 knifes-0.8.92/setup.py
+drwxr-xr-x   0 hwei       (501) staff       (20)        0 2023-08-05 15:45:43.214627 knifes-0.8.93/
+-rw-r--r--   0 hwei       (501) staff       (20)      766 2023-08-05 15:45:43.214470 knifes-0.8.93/PKG-INFO
+-rw-r--r--   0 hwei       (501) staff       (20)      400 2022-09-02 05:25:28.000000 knifes-0.8.93/README.md
+drwxr-xr-x   0 hwei       (501) staff       (20)        0 2023-08-05 15:45:43.213529 knifes-0.8.93/knifes/
+-rw-r--r--   0 hwei       (501) staff       (20)        0 2022-01-21 03:14:54.000000 knifes-0.8.93/knifes/__init__.py
+-rw-r--r--   0 hwei       (501) staff       (20)     1161 2022-02-16 14:49:04.000000 knifes-0.8.93/knifes/aes.py
+-rw-r--r--   0 hwei       (501) staff       (20)      573 2023-07-29 07:38:53.000000 knifes-0.8.93/knifes/alarm.py
+-rw-r--r--   0 hwei       (501) staff       (20)      740 2022-01-21 03:14:54.000000 knifes-0.8.93/knifes/auth.py
+-rw-r--r--   0 hwei       (501) staff       (20)      502 2023-07-29 10:19:19.000000 knifes-0.8.93/knifes/constants.py
+-rw-r--r--   0 hwei       (501) staff       (20)     7353 2023-08-05 15:44:37.000000 knifes-0.8.93/knifes/decorators.py
+-rw-r--r--   0 hwei       (501) staff       (20)     7567 2023-06-14 01:08:29.000000 knifes-0.8.93/knifes/deploy.py
+-rw-r--r--   0 hwei       (501) staff       (20)     1140 2022-10-14 05:30:31.000000 knifes-0.8.93/knifes/digests.py
+-rw-r--r--   0 hwei       (501) staff       (20)      363 2023-02-01 04:12:33.000000 knifes-0.8.93/knifes/envconfig.py
+-rw-r--r--   0 hwei       (501) staff       (20)     1649 2022-11-17 08:15:03.000000 knifes-0.8.93/knifes/file.py
+-rw-r--r--   0 hwei       (501) staff       (20)     5108 2023-06-15 01:37:33.000000 knifes-0.8.93/knifes/getui.py
+-rw-r--r--   0 hwei       (501) staff       (20)      732 2022-03-13 09:06:03.000000 knifes-0.8.93/knifes/jsons.py
+-rw-r--r--   0 hwei       (501) staff       (20)      403 2023-07-29 07:38:53.000000 knifes-0.8.93/knifes/logging.py
+-rw-r--r--   0 hwei       (501) staff       (20)      474 2023-06-15 08:19:17.000000 knifes-0.8.93/knifes/media.py
+-rw-r--r--   0 hwei       (501) staff       (20)      924 2023-02-21 04:17:56.000000 knifes-0.8.93/knifes/misc.py
+-rw-r--r--   0 hwei       (501) staff       (20)      421 2023-08-04 10:48:49.000000 knifes-0.8.93/knifes/operators.py
+-rw-r--r--   0 hwei       (501) staff       (20)      569 2022-11-23 13:58:35.000000 knifes-0.8.93/knifes/package.py
+-rw-r--r--   0 hwei       (501) staff       (20)      863 2023-07-31 13:36:03.000000 knifes-0.8.93/knifes/randoms.py
+-rw-r--r--   0 hwei       (501) staff       (20)     1527 2023-08-05 07:41:23.000000 knifes-0.8.93/knifes/results.py
+-rw-r--r--   0 hwei       (501) staff       (20)     2235 2022-05-30 13:46:32.000000 knifes-0.8.93/knifes/roar.py
+-rw-r--r--   0 hwei       (501) staff       (20)      446 2022-01-21 03:14:54.000000 knifes-0.8.93/knifes/shell.py
+-rw-r--r--   0 hwei       (501) staff       (20)     2022 2023-07-31 14:57:01.000000 knifes-0.8.93/knifes/sms.py
+-rw-r--r--   0 hwei       (501) staff       (20)      889 2023-02-01 04:20:34.000000 knifes-0.8.93/knifes/strings.py
+-rw-r--r--   0 hwei       (501) staff       (20)     1335 2023-07-31 13:41:32.000000 knifes-0.8.93/knifes/times.py
+-rw-r--r--   0 hwei       (501) staff       (20)     3245 2023-06-15 07:38:41.000000 knifes-0.8.93/knifes/urls.py
+-rw-r--r--   0 hwei       (501) staff       (20)     4396 2022-11-25 02:07:08.000000 knifes-0.8.93/knifes/useragent.py
+drwxr-xr-x   0 hwei       (501) staff       (20)        0 2023-08-05 15:45:43.214282 knifes-0.8.93/knifes.egg-info/
+-rw-r--r--   0 hwei       (501) staff       (20)      766 2023-08-05 15:45:43.000000 knifes-0.8.93/knifes.egg-info/PKG-INFO
+-rw-r--r--   0 hwei       (501) staff       (20)      626 2023-08-05 15:45:43.000000 knifes-0.8.93/knifes.egg-info/SOURCES.txt
+-rw-r--r--   0 hwei       (501) staff       (20)        1 2023-08-05 15:45:43.000000 knifes-0.8.93/knifes.egg-info/dependency_links.txt
+-rw-r--r--   0 hwei       (501) staff       (20)       27 2023-08-05 15:45:43.000000 knifes-0.8.93/knifes.egg-info/requires.txt
+-rw-r--r--   0 hwei       (501) staff       (20)        7 2023-08-05 15:45:43.000000 knifes-0.8.93/knifes.egg-info/top_level.txt
+-rw-r--r--   0 hwei       (501) staff       (20)      103 2022-02-08 15:08:46.000000 knifes-0.8.93/pyproject.toml
+-rw-r--r--   0 hwei       (501) staff       (20)       38 2023-08-05 15:45:43.214674 knifes-0.8.93/setup.cfg
+-rw-r--r--   0 hwei       (501) staff       (20)      901 2023-08-05 15:45:01.000000 knifes-0.8.93/setup.py
```

### Comparing `knifes-0.8.92/PKG-INFO` & `knifes-0.8.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knifes
-Version: 0.8.92
+Version: 0.8.93
 Summary: Swiss Army Knife
 Home-page: https://github.com/
 Author: knifes
 Author-email: author@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `knifes-0.8.92/knifes/aes.py` & `knifes-0.8.93/knifes/aes.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.92/knifes/alarm.py` & `knifes-0.8.93/knifes/alarm.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.92/knifes/auth.py` & `knifes-0.8.93/knifes/auth.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.92/knifes/decorators.py` & `knifes-0.8.93/knifes/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,18 @@
     return outer_wrapper
 
 
 def parse_and_verify_body_data(function=None, *, required_params: set = None, required_signature: bool = False):
     def actual_decorator(view_func):
         @functools.wraps(view_func)
         def wrapper(request: HttpRequest, *args, **kwargs):
-            request.data = json.loads(request.body or "{}")
+            try:
+                request.data = json.loads(request.body or '{}')
+            except json.decoder.JSONDecodeError:  # 非json格式数据
+                request.data = {}
             # 校验参数
             if required_params and next((True for i in required_params if i not in request.data), False):
                 return ApiResponse.missing_param()
             # 验证签名
             if not settings.DEBUG and required_signature:
                 # noinspection PyBroadException
                 try:
```

### Comparing `knifes-0.8.92/knifes/deploy.py` & `knifes-0.8.93/knifes/deploy.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.92/knifes/digests.py` & `knifes-0.8.93/knifes/digests.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.92/knifes/file.py` & `knifes-0.8.93/knifes/file.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.92/knifes/getui.py` & `knifes-0.8.93/knifes/getui.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.92/knifes/jsons.py` & `knifes-0.8.93/knifes/jsons.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.92/knifes/misc.py` & `knifes-0.8.93/knifes/misc.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.92/knifes/package.py` & `knifes-0.8.93/knifes/package.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.92/knifes/randoms.py` & `knifes-0.8.93/knifes/randoms.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.92/knifes/results.py` & `knifes-0.8.93/knifes/results.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.92/knifes/roar.py` & `knifes-0.8.93/knifes/roar.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.92/knifes/sms.py` & `knifes-0.8.93/knifes/sms.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.92/knifes/strings.py` & `knifes-0.8.93/knifes/strings.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.92/knifes/times.py` & `knifes-0.8.93/knifes/times.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.92/knifes/urls.py` & `knifes-0.8.93/knifes/urls.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.92/knifes/useragent.py` & `knifes-0.8.93/knifes/useragent.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.92/knifes.egg-info/PKG-INFO` & `knifes-0.8.93/knifes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knifes
-Version: 0.8.92
+Version: 0.8.93
 Summary: Swiss Army Knife
 Home-page: https://github.com/
 Author: knifes
 Author-email: author@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `knifes-0.8.92/knifes.egg-info/SOURCES.txt` & `knifes-0.8.93/knifes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `knifes-0.8.92/setup.py` & `knifes-0.8.93/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="knifes",
-    version="0.8.92",
+    version="0.8.93",
     author="knifes",
     author_email="author@example.com",
     description="Swiss Army Knife",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/",
     classifiers=[
```

