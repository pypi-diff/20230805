# Comparing `tmp/mbnk-0.4.0a1.tar.gz` & `tmp/mbnk-0.4.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbnk-0.4.0a1.tar", max compression
+gzip compressed data, was "mbnk-0.4.0a2.tar", max compression
```

## Comparing `mbnk-0.4.0a1.tar` & `mbnk-0.4.0a2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1394 2023-07-05 20:55:27.254522 mbnk-0.4.0a1/README.md
--rw-r--r--   0        0        0      132 2023-07-05 20:55:27.254522 mbnk-0.4.0a1/mbnk/__init__.py
--rw-r--r--   0        0        0     7014 2023-07-30 10:51:50.041765 mbnk-0.4.0a1/mbnk/api.py
--rw-r--r--   0        0        0      140 2023-07-03 20:40:21.439433 mbnk-0.4.0a1/mbnk/asyncio/__init__.py
--rw-r--r--   0        0        0     8717 2023-08-04 21:09:13.096196 mbnk-0.4.0a1/mbnk/asyncio/mbnk.py
--rw-r--r--   0        0        0     2856 2023-07-30 10:17:13.391876 mbnk-0.4.0a1/mbnk/enums.py
--rw-r--r--   0        0        0      596 2023-07-12 12:34:28.846440 mbnk-0.4.0a1/mbnk/exceptions.py
--rw-r--r--   0        0        0    11793 2023-07-30 10:50:58.712772 mbnk-0.4.0a1/mbnk/mbnk.py
--rw-r--r--   0        0        0        0 2023-07-30 10:06:38.366881 mbnk-0.4.0a1/mbnk/methods/__init__.py
--rw-r--r--   0        0        0      112 2023-07-05 20:55:27.254522 mbnk-0.4.0a1/mbnk/responses.py
--rw-r--r--   0        0        0     7358 2023-07-13 09:46:49.604104 mbnk-0.4.0a1/mbnk/types.py
--rw-r--r--   0        0        0       48 2023-07-12 09:42:11.106776 mbnk-0.4.0a1/mbnk/utils/__init__.py
--rw-r--r--   0        0        0      593 2023-07-30 10:07:56.175231 mbnk-0.4.0a1/mbnk/utils/signature.py
--rw-r--r--   0        0        0      475 2023-07-30 09:54:51.371750 mbnk-0.4.0a1/mbnk/utils/webhook.py
--rw-r--r--   0        0        0      412 2023-08-04 21:09:23.364148 mbnk-0.4.0a1/pyproject.toml
--rw-r--r--   0        0        0     2129 1970-01-01 00:00:00.000000 mbnk-0.4.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1394 2023-07-05 20:55:27.254522 mbnk-0.4.0a2/README.md
+-rw-r--r--   0        0        0      132 2023-07-05 20:55:27.254522 mbnk-0.4.0a2/mbnk/__init__.py
+-rw-r--r--   0        0        0     7032 2023-08-05 19:08:21.724196 mbnk-0.4.0a2/mbnk/api.py
+-rw-r--r--   0        0        0      140 2023-07-03 20:40:21.439433 mbnk-0.4.0a2/mbnk/asyncio/__init__.py
+-rw-r--r--   0        0        0     8717 2023-08-04 21:09:13.096196 mbnk-0.4.0a2/mbnk/asyncio/mbnk.py
+-rw-r--r--   0        0        0     2856 2023-07-30 10:17:13.391876 mbnk-0.4.0a2/mbnk/enums.py
+-rw-r--r--   0        0        0      596 2023-07-12 12:34:28.846440 mbnk-0.4.0a2/mbnk/exceptions.py
+-rw-r--r--   0        0        0    11793 2023-07-30 10:50:58.712772 mbnk-0.4.0a2/mbnk/mbnk.py
+-rw-r--r--   0        0        0        0 2023-07-30 10:06:38.366881 mbnk-0.4.0a2/mbnk/methods/__init__.py
+-rw-r--r--   0        0        0      112 2023-07-05 20:55:27.254522 mbnk-0.4.0a2/mbnk/responses.py
+-rw-r--r--   0        0        0     7358 2023-07-13 09:46:49.604104 mbnk-0.4.0a2/mbnk/types.py
+-rw-r--r--   0        0        0       48 2023-07-12 09:42:11.106776 mbnk-0.4.0a2/mbnk/utils/__init__.py
+-rw-r--r--   0        0        0      593 2023-07-30 10:07:56.175231 mbnk-0.4.0a2/mbnk/utils/signature.py
+-rw-r--r--   0        0        0      475 2023-07-30 09:54:51.371750 mbnk-0.4.0a2/mbnk/utils/webhook.py
+-rw-r--r--   0        0        0      412 2023-08-05 19:08:44.668063 mbnk-0.4.0a2/pyproject.toml
+-rw-r--r--   0        0        0     2129 1970-01-01 00:00:00.000000 mbnk-0.4.0a2/PKG-INFO
```

### Comparing `mbnk-0.4.0a1/README.md` & `mbnk-0.4.0a2/README.md`

 * *Files identical despite different names*

### Comparing `mbnk-0.4.0a1/mbnk/api.py` & `mbnk-0.4.0a2/mbnk/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,20 +182,20 @@
             def inner(self):
                 self.__headers["X-Sign"]: str = self.__create_signature(self)
             return inner
 
         return outer
 
     @staticmethod
-    def _async_request(
+    async def _async_request(
             method: str,
             path: str
     ):
-        def outer(func):
-            def inner(*args, **kwargs):
+        async def outer(func):
+            async def inner(*args, **kwargs):
                 self = args[0]
                 args = args[1:]
 
                 func_args = {
                     "method": method,
                     "path": path,
                     ("params" if request_method == "get" else "data"): self.__build_data(**kwargs)
```

### Comparing `mbnk-0.4.0a1/mbnk/asyncio/mbnk.py` & `mbnk-0.4.0a2/mbnk/asyncio/mbnk.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.4.0a1/mbnk/enums.py` & `mbnk-0.4.0a2/mbnk/enums.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.4.0a1/mbnk/exceptions.py` & `mbnk-0.4.0a2/mbnk/exceptions.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.4.0a1/mbnk/mbnk.py` & `mbnk-0.4.0a2/mbnk/mbnk.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.4.0a1/mbnk/types.py` & `mbnk-0.4.0a2/mbnk/types.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.4.0a1/mbnk/utils/signature.py` & `mbnk-0.4.0a2/mbnk/utils/signature.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.4.0a1/PKG-INFO` & `mbnk-0.4.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbnk
-Version: 0.4.0a1
+Version: 0.4.0a2
 Summary: Sync/Async version Monobank api
 License: MIT
 Author: yeghorkikhai
 Author-email: yeghorkikhai@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

