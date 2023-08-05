# Comparing `tmp/graia-saya-0.0.8.tar.gz` & `tmp/graia-saya-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graia-saya-0.0.8.tar", last modified: Fri Feb 26 14:13:09 2021, max compression
+gzip compressed data, was "graia-saya-0.0.9.tar", last modified: Sun Apr 18 01:31:39 2021, max compression
```

## Comparing `graia-saya-0.0.8.tar` & `graia-saya-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,17 @@
--rw-r--r--   0        0        0      465 2021-02-26 14:11:56.000000 graia-saya-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     6522 2021-02-26 14:12:30.000000 graia-saya-0.0.8/src/graia/saya/__init__.py
--rw-r--r--   0        0        0     5281 2021-02-26 14:12:28.000000 graia-saya-0.0.8/src/graia/saya/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2437 2021-02-26 11:54:16.000000 graia-saya-0.0.8/src/graia/saya/__pycache__/channel.cpython-38.pyc
--rw-r--r--   0        0        0      246 2021-02-14 05:56:20.000000 graia-saya-0.0.8/src/graia/saya/__pycache__/context.cpython-38.pyc
--rw-r--r--   0        0        0      558 2021-02-15 12:18:02.000000 graia-saya-0.0.8/src/graia/saya/__pycache__/cube.cpython-38.pyc
--rw-r--r--   0        0        0     2390 2021-02-26 11:52:52.000000 graia-saya-0.0.8/src/graia/saya/__pycache__/event.cpython-38.pyc
--rw-r--r--   0        0        0      750 2021-02-14 06:07:38.000000 graia-saya-0.0.8/src/graia/saya/__pycache__/schema.cpython-38.pyc
--rw-r--r--   0        0        0      128 2021-02-12 13:16:54.000000 graia-saya-0.0.8/src/graia/saya/behaviour/__init__.py
--rw-r--r--   0        0        0      310 2021-02-14 05:56:20.000000 graia-saya-0.0.8/src/graia/saya/behaviour/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      800 2021-02-26 13:42:52.000000 graia-saya-0.0.8/src/graia/saya/behaviour/__pycache__/builtin.cpython-38.pyc
--rw-r--r--   0        0        0      993 2021-02-26 13:17:48.000000 graia-saya-0.0.8/src/graia/saya/behaviour/__pycache__/context.cpython-38.pyc
--rw-r--r--   0        0        0     1442 2021-02-26 13:32:02.000000 graia-saya-0.0.8/src/graia/saya/behaviour/__pycache__/entity.cpython-38.pyc
--rw-r--r--   0        0        0     3337 2021-02-26 13:17:48.000000 graia-saya-0.0.8/src/graia/saya/behaviour/__pycache__/interface.cpython-38.pyc
--rw-r--r--   0        0        0      377 2021-02-26 13:42:36.000000 graia-saya-0.0.8/src/graia/saya/behaviour/builtin.py
--rw-r--r--   0        0        0      420 2021-02-26 13:14:00.000000 graia-saya-0.0.8/src/graia/saya/behaviour/context.py
--rw-r--r--   0        0        0      605 2021-02-26 13:21:20.000000 graia-saya-0.0.8/src/graia/saya/behaviour/entity.py
--rw-r--r--   0        0        0     3398 2021-02-26 13:17:46.000000 graia-saya-0.0.8/src/graia/saya/behaviour/interface.py
--rw-r--r--   0        0        0        0 2021-02-14 06:25:58.000000 graia-saya-0.0.8/src/graia/saya/builtins/__init__.py
--rw-r--r--   0        0        0      143 2021-02-15 12:19:18.000000 graia-saya-0.0.8/src/graia/saya/builtins/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0       77 2021-02-15 12:12:18.000000 graia-saya-0.0.8/src/graia/saya/builtins/broadcast/__init__.py
--rw-r--r--   0        0        0      250 2021-02-15 12:19:18.000000 graia-saya-0.0.8/src/graia/saya/builtins/broadcast/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1407 2021-02-26 11:52:52.000000 graia-saya-0.0.8/src/graia/saya/builtins/broadcast/__pycache__/behaviour.cpython-38.pyc
--rw-r--r--   0        0        0     1343 2021-02-15 12:33:34.000000 graia-saya-0.0.8/src/graia/saya/builtins/broadcast/__pycache__/schema.cpython-38.pyc
--rw-r--r--   0        0        0     1034 2021-02-26 10:21:20.000000 graia-saya-0.0.8/src/graia/saya/builtins/broadcast/behaviour.py
--rw-r--r--   0        0        0     1076 2021-02-15 12:33:30.000000 graia-saya-0.0.8/src/graia/saya/builtins/broadcast/schema.py
--rw-r--r--   0        0        0     1420 2021-02-26 11:54:16.000000 graia-saya-0.0.8/src/graia/saya/channel.py
--rw-r--r--   0        0        0      123 2021-02-12 13:28:48.000000 graia-saya-0.0.8/src/graia/saya/context.py
--rw-r--r--   0        0        0      231 2021-02-14 07:55:48.000000 graia-saya-0.0.8/src/graia/saya/cube.py
--rw-r--r--   0        0        0     1945 2021-02-26 11:51:22.000000 graia-saya-0.0.8/src/graia/saya/event.py
--rw-r--r--   0        0        0      321 2021-02-14 06:07:34.000000 graia-saya-0.0.8/src/graia/saya/schema.py
--rw-r--r--   0        0        0      792 2021-02-26 14:13:09.803657 graia-saya-0.0.8/setup.py
--rw-r--r--   0        0        0      512 2021-02-26 14:13:09.803657 graia-saya-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      522 2021-04-18 01:29:00.000000 graia-saya-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    10035 2021-04-18 01:28:00.000000 graia-saya-0.0.9/src/graia/saya/__init__.py
+-rw-r--r--   0        0        0      128 2021-02-12 13:16:54.000000 graia-saya-0.0.9/src/graia/saya/behaviour/__init__.py
+-rw-r--r--   0        0        0      420 2021-02-26 13:14:00.000000 graia-saya-0.0.9/src/graia/saya/behaviour/context.py
+-rw-r--r--   0        0        0      307 2021-04-04 09:05:34.000000 graia-saya-0.0.9/src/graia/saya/behaviour/entity.py
+-rw-r--r--   0        0        0     2761 2021-04-04 09:05:40.000000 graia-saya-0.0.9/src/graia/saya/behaviour/interface.py
+-rw-r--r--   0        0        0     1124 2021-04-09 13:07:40.000000 graia-saya-0.0.9/src/graia/saya/builtins/__init__.py
+-rw-r--r--   0        0        0       77 2021-02-15 12:12:18.000000 graia-saya-0.0.9/src/graia/saya/builtins/broadcast/__init__.py
+-rw-r--r--   0        0        0     1034 2021-04-04 09:08:56.000000 graia-saya-0.0.9/src/graia/saya/builtins/broadcast/behaviour.py
+-rw-r--r--   0        0        0     1076 2021-02-15 12:33:30.000000 graia-saya-0.0.9/src/graia/saya/builtins/broadcast/schema.py
+-rw-r--r--   0        0        0     1420 2021-02-26 11:54:16.000000 graia-saya-0.0.9/src/graia/saya/channel.py
+-rw-r--r--   0        0        0      184 2021-04-18 01:17:30.000000 graia-saya-0.0.9/src/graia/saya/context.py
+-rw-r--r--   0        0        0      231 2021-02-14 07:55:48.000000 graia-saya-0.0.9/src/graia/saya/cube.py
+-rw-r--r--   0        0        0     1945 2021-02-26 11:51:22.000000 graia-saya-0.0.9/src/graia/saya/event.py
+-rw-r--r--   0        0        0      321 2021-02-14 06:07:34.000000 graia-saya-0.0.9/src/graia/saya/schema.py
+-rw-r--r--   0        0        0      792 2021-04-18 01:31:40.027471 graia-saya-0.0.9/setup.py
+-rw-r--r--   0        0        0      538 2021-04-18 01:31:40.028472 graia-saya-0.0.9/PKG-INFO
```

### Comparing `graia-saya-0.0.8/src/graia/saya/behaviour/interface.py` & `graia-saya-0.0.9/src/graia/saya/behaviour/interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,27 +78,8 @@
                 continue
 
             self.require_contents[-1]._index = 0
             return result
         else:
             raise RequirementCrashed(
                 f"the dispatching requirement crashed: {cube}"
-            )
-    
-    def find_route(self, route: str) -> Any:
-        start_offset = self._index + int(bool(self._index))
-
-        for self.require_contents[-1]._index, behaviour in enumerate(
-            itertools.islice(self.behaviour_generator(), start_offset, None, None),
-            start=start_offset
-        ):
-            result = behaviour.route(route)
-    
-            if result is None:
-                continue
-
-            self.require_contents[-1]._index = 0
-            return result
-        else:
-            raise RequirementCrashed(
-                f"the dispatching requirement crashed: {route}"
             )
```

### Comparing `graia-saya-0.0.8/src/graia/saya/builtins/broadcast/behaviour.py` & `graia-saya-0.0.9/src/graia/saya/builtins/broadcast/behaviour.py`

 * *Files identical despite different names*

### Comparing `graia-saya-0.0.8/src/graia/saya/builtins/broadcast/schema.py` & `graia-saya-0.0.9/src/graia/saya/builtins/broadcast/schema.py`

 * *Files identical despite different names*

### Comparing `graia-saya-0.0.8/src/graia/saya/channel.py` & `graia-saya-0.0.9/src/graia/saya/channel.py`

 * *Files identical despite different names*

### Comparing `graia-saya-0.0.8/src/graia/saya/event.py` & `graia-saya-0.0.9/src/graia/saya/event.py`

 * *Files identical despite different names*

### Comparing `graia-saya-0.0.8/setup.py` & `graia-saya-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 {'': ['*']}
 
 install_requires = \
 ['graia-broadcast>=0.7.0', 'loguru>=0.5.3,<0.6.0']
 
 setup_kwargs = {
     'name': 'graia-saya',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': '',
     'long_description': None,
     'author': 'GreyElaina',
     'author_email': '31543961+GreyElaina@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `graia-saya-0.0.8/PKG-INFO` & `graia-saya-0.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: graia-saya
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 License: MIT
 Author: GreyElaina
 Author-email: 31543961+GreyElaina@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: scheduler
 Requires-Dist: graia-broadcast (>=0.7.0)
 Requires-Dist: loguru (>=0.5.3,<0.6.0)
```

