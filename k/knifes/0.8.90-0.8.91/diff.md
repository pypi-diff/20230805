# Comparing `tmp/knifes-0.8.90.tar.gz` & `tmp/knifes-0.8.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knifes-0.8.90.tar", last modified: Fri Aug  4 10:49:26 2023, max compression
+gzip compressed data, was "knifes-0.8.91.tar", last modified: Sat Aug  5 07:18:34 2023, max compression
```

## Comparing `knifes-0.8.90.tar` & `knifes-0.8.91.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 hwei       (501) staff       (20)        0 2023-08-04 10:49:26.150734 knifes-0.8.90/
--rw-r--r--   0 hwei       (501) staff       (20)      766 2023-08-04 10:49:26.150575 knifes-0.8.90/PKG-INFO
--rw-r--r--   0 hwei       (501) staff       (20)      400 2022-09-02 05:25:28.000000 knifes-0.8.90/README.md
-drwxr-xr-x   0 hwei       (501) staff       (20)        0 2023-08-04 10:49:26.149607 knifes-0.8.90/knifes/
--rw-r--r--   0 hwei       (501) staff       (20)        0 2022-01-21 03:14:54.000000 knifes-0.8.90/knifes/__init__.py
--rw-r--r--   0 hwei       (501) staff       (20)     1161 2022-02-16 14:49:04.000000 knifes-0.8.90/knifes/aes.py
--rw-r--r--   0 hwei       (501) staff       (20)      573 2023-07-29 07:38:53.000000 knifes-0.8.90/knifes/alarm.py
--rw-r--r--   0 hwei       (501) staff       (20)      740 2022-01-21 03:14:54.000000 knifes-0.8.90/knifes/auth.py
--rw-r--r--   0 hwei       (501) staff       (20)      502 2023-07-29 10:19:19.000000 knifes-0.8.90/knifes/constants.py
--rw-r--r--   0 hwei       (501) staff       (20)     7208 2023-07-31 13:37:02.000000 knifes-0.8.90/knifes/decorators.py
--rw-r--r--   0 hwei       (501) staff       (20)     7567 2023-06-14 01:08:29.000000 knifes-0.8.90/knifes/deploy.py
--rw-r--r--   0 hwei       (501) staff       (20)     1140 2022-10-14 05:30:31.000000 knifes-0.8.90/knifes/digests.py
--rw-r--r--   0 hwei       (501) staff       (20)      363 2023-02-01 04:12:33.000000 knifes-0.8.90/knifes/envconfig.py
--rw-r--r--   0 hwei       (501) staff       (20)     1649 2022-11-17 08:15:03.000000 knifes-0.8.90/knifes/file.py
--rw-r--r--   0 hwei       (501) staff       (20)     5108 2023-06-15 01:37:33.000000 knifes-0.8.90/knifes/getui.py
--rw-r--r--   0 hwei       (501) staff       (20)      732 2022-03-13 09:06:03.000000 knifes-0.8.90/knifes/jsons.py
--rw-r--r--   0 hwei       (501) staff       (20)      403 2023-07-29 07:38:53.000000 knifes-0.8.90/knifes/logging.py
--rw-r--r--   0 hwei       (501) staff       (20)      474 2023-06-15 08:19:17.000000 knifes-0.8.90/knifes/media.py
--rw-r--r--   0 hwei       (501) staff       (20)      924 2023-02-21 04:17:56.000000 knifes-0.8.90/knifes/misc.py
--rw-r--r--   0 hwei       (501) staff       (20)      421 2023-08-04 10:48:49.000000 knifes-0.8.90/knifes/operators.py
--rw-r--r--   0 hwei       (501) staff       (20)      569 2022-11-23 13:58:35.000000 knifes-0.8.90/knifes/package.py
--rw-r--r--   0 hwei       (501) staff       (20)      863 2023-07-31 13:36:03.000000 knifes-0.8.90/knifes/randoms.py
--rw-r--r--   0 hwei       (501) staff       (20)     1895 2023-07-30 11:26:01.000000 knifes-0.8.90/knifes/results.py
--rw-r--r--   0 hwei       (501) staff       (20)     2235 2022-05-30 13:46:32.000000 knifes-0.8.90/knifes/roar.py
--rw-r--r--   0 hwei       (501) staff       (20)      446 2022-01-21 03:14:54.000000 knifes-0.8.90/knifes/shell.py
--rw-r--r--   0 hwei       (501) staff       (20)     2022 2023-07-31 14:57:01.000000 knifes-0.8.90/knifes/sms.py
--rw-r--r--   0 hwei       (501) staff       (20)      889 2023-02-01 04:20:34.000000 knifes-0.8.90/knifes/strings.py
--rw-r--r--   0 hwei       (501) staff       (20)     1335 2023-07-31 13:41:32.000000 knifes-0.8.90/knifes/times.py
--rw-r--r--   0 hwei       (501) staff       (20)     3245 2023-06-15 07:38:41.000000 knifes-0.8.90/knifes/urls.py
--rw-r--r--   0 hwei       (501) staff       (20)     4396 2022-11-25 02:07:08.000000 knifes-0.8.90/knifes/useragent.py
-drwxr-xr-x   0 hwei       (501) staff       (20)        0 2023-08-04 10:49:26.150369 knifes-0.8.90/knifes.egg-info/
--rw-r--r--   0 hwei       (501) staff       (20)      766 2023-08-04 10:49:26.000000 knifes-0.8.90/knifes.egg-info/PKG-INFO
--rw-r--r--   0 hwei       (501) staff       (20)      626 2023-08-04 10:49:26.000000 knifes-0.8.90/knifes.egg-info/SOURCES.txt
--rw-r--r--   0 hwei       (501) staff       (20)        1 2023-08-04 10:49:26.000000 knifes-0.8.90/knifes.egg-info/dependency_links.txt
--rw-r--r--   0 hwei       (501) staff       (20)       27 2023-08-04 10:49:26.000000 knifes-0.8.90/knifes.egg-info/requires.txt
--rw-r--r--   0 hwei       (501) staff       (20)        7 2023-08-04 10:49:26.000000 knifes-0.8.90/knifes.egg-info/top_level.txt
--rw-r--r--   0 hwei       (501) staff       (20)      103 2022-02-08 15:08:46.000000 knifes-0.8.90/pyproject.toml
--rw-r--r--   0 hwei       (501) staff       (20)       38 2023-08-04 10:49:26.150782 knifes-0.8.90/setup.cfg
--rw-r--r--   0 hwei       (501) staff       (20)      901 2023-08-04 10:49:11.000000 knifes-0.8.90/setup.py
+drwxr-xr-x   0 hwei       (501) staff       (20)        0 2023-08-05 07:18:34.189406 knifes-0.8.91/
+-rw-r--r--   0 hwei       (501) staff       (20)      766 2023-08-05 07:18:34.189285 knifes-0.8.91/PKG-INFO
+-rw-r--r--   0 hwei       (501) staff       (20)      400 2022-09-02 05:25:28.000000 knifes-0.8.91/README.md
+drwxr-xr-x   0 hwei       (501) staff       (20)        0 2023-08-05 07:18:34.188428 knifes-0.8.91/knifes/
+-rw-r--r--   0 hwei       (501) staff       (20)        0 2022-01-21 03:14:54.000000 knifes-0.8.91/knifes/__init__.py
+-rw-r--r--   0 hwei       (501) staff       (20)     1161 2022-02-16 14:49:04.000000 knifes-0.8.91/knifes/aes.py
+-rw-r--r--   0 hwei       (501) staff       (20)      573 2023-07-29 07:38:53.000000 knifes-0.8.91/knifes/alarm.py
+-rw-r--r--   0 hwei       (501) staff       (20)      740 2022-01-21 03:14:54.000000 knifes-0.8.91/knifes/auth.py
+-rw-r--r--   0 hwei       (501) staff       (20)      502 2023-07-29 10:19:19.000000 knifes-0.8.91/knifes/constants.py
+-rw-r--r--   0 hwei       (501) staff       (20)     7208 2023-07-31 13:37:02.000000 knifes-0.8.91/knifes/decorators.py
+-rw-r--r--   0 hwei       (501) staff       (20)     7567 2023-06-14 01:08:29.000000 knifes-0.8.91/knifes/deploy.py
+-rw-r--r--   0 hwei       (501) staff       (20)     1140 2022-10-14 05:30:31.000000 knifes-0.8.91/knifes/digests.py
+-rw-r--r--   0 hwei       (501) staff       (20)      363 2023-02-01 04:12:33.000000 knifes-0.8.91/knifes/envconfig.py
+-rw-r--r--   0 hwei       (501) staff       (20)     1649 2022-11-17 08:15:03.000000 knifes-0.8.91/knifes/file.py
+-rw-r--r--   0 hwei       (501) staff       (20)     5108 2023-06-15 01:37:33.000000 knifes-0.8.91/knifes/getui.py
+-rw-r--r--   0 hwei       (501) staff       (20)      732 2022-03-13 09:06:03.000000 knifes-0.8.91/knifes/jsons.py
+-rw-r--r--   0 hwei       (501) staff       (20)      403 2023-07-29 07:38:53.000000 knifes-0.8.91/knifes/logging.py
+-rw-r--r--   0 hwei       (501) staff       (20)      474 2023-06-15 08:19:17.000000 knifes-0.8.91/knifes/media.py
+-rw-r--r--   0 hwei       (501) staff       (20)      924 2023-02-21 04:17:56.000000 knifes-0.8.91/knifes/misc.py
+-rw-r--r--   0 hwei       (501) staff       (20)      421 2023-08-04 10:48:49.000000 knifes-0.8.91/knifes/operators.py
+-rw-r--r--   0 hwei       (501) staff       (20)      569 2022-11-23 13:58:35.000000 knifes-0.8.91/knifes/package.py
+-rw-r--r--   0 hwei       (501) staff       (20)      863 2023-07-31 13:36:03.000000 knifes-0.8.91/knifes/randoms.py
+-rw-r--r--   0 hwei       (501) staff       (20)     2187 2023-08-05 07:17:23.000000 knifes-0.8.91/knifes/results.py
+-rw-r--r--   0 hwei       (501) staff       (20)     2235 2022-05-30 13:46:32.000000 knifes-0.8.91/knifes/roar.py
+-rw-r--r--   0 hwei       (501) staff       (20)      446 2022-01-21 03:14:54.000000 knifes-0.8.91/knifes/shell.py
+-rw-r--r--   0 hwei       (501) staff       (20)     2022 2023-07-31 14:57:01.000000 knifes-0.8.91/knifes/sms.py
+-rw-r--r--   0 hwei       (501) staff       (20)      889 2023-02-01 04:20:34.000000 knifes-0.8.91/knifes/strings.py
+-rw-r--r--   0 hwei       (501) staff       (20)     1335 2023-07-31 13:41:32.000000 knifes-0.8.91/knifes/times.py
+-rw-r--r--   0 hwei       (501) staff       (20)     3245 2023-06-15 07:38:41.000000 knifes-0.8.91/knifes/urls.py
+-rw-r--r--   0 hwei       (501) staff       (20)     4396 2022-11-25 02:07:08.000000 knifes-0.8.91/knifes/useragent.py
+drwxr-xr-x   0 hwei       (501) staff       (20)        0 2023-08-05 07:18:34.189138 knifes-0.8.91/knifes.egg-info/
+-rw-r--r--   0 hwei       (501) staff       (20)      766 2023-08-05 07:18:34.000000 knifes-0.8.91/knifes.egg-info/PKG-INFO
+-rw-r--r--   0 hwei       (501) staff       (20)      626 2023-08-05 07:18:34.000000 knifes-0.8.91/knifes.egg-info/SOURCES.txt
+-rw-r--r--   0 hwei       (501) staff       (20)        1 2023-08-05 07:18:34.000000 knifes-0.8.91/knifes.egg-info/dependency_links.txt
+-rw-r--r--   0 hwei       (501) staff       (20)       27 2023-08-05 07:18:34.000000 knifes-0.8.91/knifes.egg-info/requires.txt
+-rw-r--r--   0 hwei       (501) staff       (20)        7 2023-08-05 07:18:34.000000 knifes-0.8.91/knifes.egg-info/top_level.txt
+-rw-r--r--   0 hwei       (501) staff       (20)      103 2022-02-08 15:08:46.000000 knifes-0.8.91/pyproject.toml
+-rw-r--r--   0 hwei       (501) staff       (20)       38 2023-08-05 07:18:34.189446 knifes-0.8.91/setup.cfg
+-rw-r--r--   0 hwei       (501) staff       (20)      901 2023-08-05 07:18:01.000000 knifes-0.8.91/setup.py
```

### Comparing `knifes-0.8.90/PKG-INFO` & `knifes-0.8.91/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knifes
-Version: 0.8.90
+Version: 0.8.91
 Summary: Swiss Army Knife
 Home-page: https://github.com/
 Author: knifes
 Author-email: author@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `knifes-0.8.90/knifes/aes.py` & `knifes-0.8.91/knifes/aes.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.90/knifes/alarm.py` & `knifes-0.8.91/knifes/alarm.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.90/knifes/auth.py` & `knifes-0.8.91/knifes/auth.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.90/knifes/decorators.py` & `knifes-0.8.91/knifes/decorators.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.90/knifes/deploy.py` & `knifes-0.8.91/knifes/deploy.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.90/knifes/digests.py` & `knifes-0.8.91/knifes/digests.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.90/knifes/file.py` & `knifes-0.8.91/knifes/file.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.90/knifes/getui.py` & `knifes-0.8.91/knifes/getui.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.90/knifes/jsons.py` & `knifes-0.8.91/knifes/jsons.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.90/knifes/misc.py` & `knifes-0.8.91/knifes/misc.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.90/knifes/package.py` & `knifes-0.8.91/knifes/package.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.90/knifes/randoms.py` & `knifes-0.8.91/knifes/randoms.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.90/knifes/results.py` & `knifes-0.8.91/knifes/results.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,46 +15,56 @@
         self.msg = msg
 
     @classmethod
     def get_by_code(cls, code) -> Optional[BaseErrorEnum]:
         return next(filter(lambda x: x.code == code, cls.__members__.values()), None)
 
 
-class ApiResult:
-    def __init__(self, code, *, msg=None, msg_detail=None, data=None):
+class ApiResponse:
+    def __init__(self, code, *, msg=None, data=None):
         self.code = code
         self.succ = (code == 200)
         self.msg = msg
-        self.msg_detail = msg_detail
         self.data = data
 
-    @classmethod
-    def fail(cls, msg, code=400, msg_detail=None):
-        return ApiResult(code, msg=msg, msg_detail=msg_detail)
+    # @classmethod
+    # def fail(cls, msg, code=400, msg_detail=None):
+    #     return ApiResult(code, msg=msg, msg_detail=msg_detail)
+    #
+    # @classmethod
+    # def succ(cls, data=None):
+    #     return ApiResult(200, data=data)
 
     @classmethod
-    def succ(cls, data=None):
-        return ApiResult(200, data=data)
+    def success(cls, data=None):
+        return JsonResponse(ApiResponse(200, data=data), encoder=ObjectEncoder, safe=False)
 
     @classmethod
-    def succResponse(cls, data=None):
-        return JsonResponse(cls.succ(data), encoder=ObjectEncoder, safe=False)
+    def failure(cls, msg, code=400):
+        return JsonResponse(ApiResponse(code, msg=msg), encoder=ObjectEncoder, safe=False)
 
     @classmethod
-    def failResponse(cls, msg, code=400, msg_detail=None):
-        return JsonResponse(cls.fail(msg, code=code, msg_detail=msg_detail), encoder=ObjectEncoder, safe=False)
+    def error(cls, error_enum: BaseErrorEnum):
+        return JsonResponse(ApiResponse(error_enum.code, msg=error_enum.msg), encoder=ObjectEncoder, safe=False)
 
     @classmethod
-    def errorResponse(cls, error_enum: BaseErrorEnum, msg_detail=None):
-        return JsonResponse(cls.fail(error_enum.msg, code=error_enum.code, msg_detail=msg_detail), encoder=ObjectEncoder, safe=False)
-
-    @classmethod
-    def missingParam(cls, msg=_('缺少参数')):
-        return cls.failResponse(msg)
+    def missing_param(cls, msg=_('缺少参数')):
+        return cls.failure(msg)
 
     @classmethod
     def unauthorized(cls, msg=_('请先登录')):
-        return cls.failResponse(msg, code=401)
+        return cls.failure(msg, code=401)
+
+    # @classmethod
+    # def tokenInvalid(cls, msg=_('请先登录')):
+    #     return cls.failResponse(msg, code=300)
+
+
+class InternalApiResponse(ApiResponse):
+    def __init__(self, code, *, msg=None, data=None, msg_detail=None):
+        super().__init__(code, msg=msg, data=data)
+        self.msg_detail = msg_detail
 
     @classmethod
-    def tokenInvalid(cls, msg=_('请先登录')):    # TODO 废弃
-        return cls.failResponse(msg, code=300)
+    def error(cls, error_enum: BaseErrorEnum, msg_detail=None):
+        return JsonResponse(InternalApiResponse(error_enum.code, msg=error_enum.msg, msg_detail=msg_detail), encoder=ObjectEncoder, safe=False)
+
```

### Comparing `knifes-0.8.90/knifes/roar.py` & `knifes-0.8.91/knifes/roar.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.90/knifes/sms.py` & `knifes-0.8.91/knifes/sms.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.90/knifes/strings.py` & `knifes-0.8.91/knifes/strings.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.90/knifes/times.py` & `knifes-0.8.91/knifes/times.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.90/knifes/urls.py` & `knifes-0.8.91/knifes/urls.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.90/knifes/useragent.py` & `knifes-0.8.91/knifes/useragent.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.90/knifes.egg-info/PKG-INFO` & `knifes-0.8.91/knifes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knifes
-Version: 0.8.90
+Version: 0.8.91
 Summary: Swiss Army Knife
 Home-page: https://github.com/
 Author: knifes
 Author-email: author@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `knifes-0.8.90/knifes.egg-info/SOURCES.txt` & `knifes-0.8.91/knifes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `knifes-0.8.90/setup.py` & `knifes-0.8.91/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="knifes",
-    version="0.8.90",
+    version="0.8.91",
     author="knifes",
     author_email="author@example.com",
     description="Swiss Army Knife",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/",
     classifiers=[
```

