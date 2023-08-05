# Comparing `tmp/zrouter-0.5.8.tar.gz` & `tmp/zrouter-0.5.9.tar.gz`

## Comparing `zrouter-0.5.8.tar` & `zrouter-0.5.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 zrouter-0.5.8/src/zrouter/__init__.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 zrouter-0.5.8/src/zrouter/restful.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 zrouter-0.5.8/src/zrouter/router.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.5.8/src/zrouter/exceptions/__init__.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 zrouter-0.5.8/src/zrouter/utils/json.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 zrouter-0.5.8/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.5.8/LICENSE
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 zrouter-0.5.8/README.md
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 zrouter-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 zrouter-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 zrouter-0.5.9/src/zrouter/__init__.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 zrouter-0.5.9/src/zrouter/restful.py
+-rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 zrouter-0.5.9/src/zrouter/router.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.5.9/src/zrouter/exceptions/__init__.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 zrouter-0.5.9/src/zrouter/utils/json.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 zrouter-0.5.9/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.5.9/LICENSE
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 zrouter-0.5.9/README.md
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 zrouter-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 zrouter-0.5.9/PKG-INFO
```

### Comparing `zrouter-0.5.8/src/zrouter/__init__.py` & `zrouter-0.5.9/src/zrouter/__init__.py`

 * *Files identical despite different names*

### Comparing `zrouter-0.5.8/src/zrouter/restful.py` & `zrouter-0.5.9/src/zrouter/restful.py`

 * *Files identical despite different names*

### Comparing `zrouter-0.5.8/src/zrouter/router.py` & `zrouter-0.5.9/src/zrouter/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     def handle_error(self, e):
         """错误处理，通过继承覆盖此方法实现具体逻辑"""
         pass
     
     @staticmethod
     def decorator(func):
-        @wraps(func)
+        @functools.wraps(func)
         def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
         return wrapper
     
     def wrap_view_func(self, func, direct=False, open=False):
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
```

### Comparing `zrouter-0.5.8/src/zrouter/utils/json.py` & `zrouter-0.5.9/src/zrouter/utils/json.py`

 * *Files identical despite different names*

### Comparing `zrouter-0.5.8/LICENSE` & `zrouter-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zrouter-0.5.8/README.md` & `zrouter-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `zrouter-0.5.8/pyproject.toml` & `zrouter-0.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zrouter"
-version = "0.5.8"
+version = "0.5.9"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen router library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `zrouter-0.5.8/PKG-INFO` & `zrouter-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zrouter
-Version: 0.5.8
+Version: 0.5.9
 Summary: zen router library
 Project-URL: Homepage, https://github.com/inspirare6/zrouter
 Project-URL: Bug Tracker, https://github.com/inspirare6/zrouter/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

