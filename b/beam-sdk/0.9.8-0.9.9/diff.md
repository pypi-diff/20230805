# Comparing `tmp/beam-sdk-0.9.8.tar.gz` & `tmp/beam-sdk-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beam-sdk-0.9.8.tar", max compression
+gzip compressed data, was "beam-sdk-0.9.9.tar", max compression
```

## Comparing `beam-sdk-0.9.8.tar` & `beam-sdk-0.9.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      104 2022-10-31 21:18:04.312680 beam-sdk-0.9.8/beam/__init__.py
--rw-r--r--   0        0        0     2918 2022-10-31 21:18:04.313384 beam-sdk-0.9.8/beam/app.py
--rw-r--r--   0        0        0     1826 2022-10-26 20:27:20.092585 beam-sdk-0.9.8/beam/base.py
--rw-r--r--   0        0        0        0 2022-09-22 16:32:45.841662 beam-sdk-0.9.8/beam/configs/__init__.py
--rw-r--r--   0        0        0      935 2022-10-27 16:48:40.049271 beam-sdk-0.9.8/beam/configs/mount.py
--rw-r--r--   0        0        0     1080 2022-10-26 20:27:20.093417 beam-sdk-0.9.8/beam/configs/outputs.py
--rw-r--r--   0        0        0     4060 2022-11-12 18:16:14.793458 beam-sdk-0.9.8/beam/configs/trigger.py
--rw-r--r--   0        0        0      153 2022-10-31 21:18:04.313594 beam-sdk-0.9.8/beam/exceptions.py
--rw-r--r--   0        0        0      836 2022-11-11 19:27:57.317496 beam-sdk-0.9.8/beam/scripts/build.py
--rw-r--r--   0        0        0     1264 2022-11-11 19:36:03.673439 beam-sdk-0.9.8/beam/scripts/init.py
--rw-r--r--   0        0        0     2117 2022-11-11 19:48:52.968739 beam-sdk-0.9.8/beam/serializer.py
--rw-r--r--   0        0        0      551 2022-11-11 19:27:57.321037 beam-sdk-0.9.8/beam/templates/base.jinja
--rw-r--r--   0        0        0     4322 2022-11-11 19:40:44.417881 beam-sdk-0.9.8/beam/tests/test_app.py
--rw-r--r--   0        0        0      656 2022-11-11 19:40:44.418626 beam-sdk-0.9.8/beam/tests/test_validators.py
--rw-r--r--   0        0        0    14392 2022-10-28 17:21:40.841329 beam-sdk-0.9.8/beam/types.py
--rw-r--r--   0        0        0     1866 2022-10-31 21:18:04.314126 beam-sdk-0.9.8/beam/utils.py
--rw-r--r--   0        0        0     3459 2022-11-12 18:07:02.213824 beam-sdk-0.9.8/beam/validators.py
--rw-r--r--   0        0        0      597 2022-11-12 18:51:44.901955 beam-sdk-0.9.8/pyproject.toml
--rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 beam-sdk-0.9.8/setup.py
--rw-r--r--   0        0        0      680 1970-01-01 00:00:00.000000 beam-sdk-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0      104 2022-10-31 21:18:04.312680 beam-sdk-0.9.9/beam/__init__.py
+-rw-r--r--   0        0        0     2918 2022-10-31 21:18:04.313384 beam-sdk-0.9.9/beam/app.py
+-rw-r--r--   0        0        0     1826 2022-10-26 20:27:20.092585 beam-sdk-0.9.9/beam/base.py
+-rw-r--r--   0        0        0        0 2022-09-22 16:32:45.841662 beam-sdk-0.9.9/beam/configs/__init__.py
+-rw-r--r--   0        0        0      935 2022-10-27 16:48:40.049271 beam-sdk-0.9.9/beam/configs/mount.py
+-rw-r--r--   0        0        0     1080 2022-10-26 20:27:20.093417 beam-sdk-0.9.9/beam/configs/outputs.py
+-rw-r--r--   0        0        0     4060 2022-11-12 18:59:53.544077 beam-sdk-0.9.9/beam/configs/trigger.py
+-rw-r--r--   0        0        0      153 2022-10-31 21:18:04.313594 beam-sdk-0.9.9/beam/exceptions.py
+-rw-r--r--   0        0        0      836 2022-11-12 18:59:53.545334 beam-sdk-0.9.9/beam/scripts/build.py
+-rw-r--r--   0        0        0     1264 2022-11-12 18:59:53.545569 beam-sdk-0.9.9/beam/scripts/init.py
+-rw-r--r--   0        0        0     2117 2022-11-11 19:48:52.968739 beam-sdk-0.9.9/beam/serializer.py
+-rw-r--r--   0        0        0      551 2022-11-12 18:59:53.545864 beam-sdk-0.9.9/beam/templates/base.jinja
+-rw-r--r--   0        0        0     4322 2022-11-11 19:40:44.417881 beam-sdk-0.9.9/beam/tests/test_app.py
+-rw-r--r--   0        0        0      656 2022-11-11 19:40:44.418626 beam-sdk-0.9.9/beam/tests/test_validators.py
+-rw-r--r--   0        0        0    14456 2022-11-14 20:38:04.449646 beam-sdk-0.9.9/beam/types.py
+-rw-r--r--   0        0        0     1866 2022-10-31 21:18:04.314126 beam-sdk-0.9.9/beam/utils.py
+-rw-r--r--   0        0        0     3459 2022-11-12 18:59:53.546161 beam-sdk-0.9.9/beam/validators.py
+-rw-r--r--   0        0        0      597 2022-11-15 17:51:09.956903 beam-sdk-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 beam-sdk-0.9.9/setup.py
+-rw-r--r--   0        0        0      680 1970-01-01 00:00:00.000000 beam-sdk-0.9.9/PKG-INFO
```

### Comparing `beam-sdk-0.9.8/beam/app.py` & `beam-sdk-0.9.9/beam/app.py`

 * *Files identical despite different names*

### Comparing `beam-sdk-0.9.8/beam/base.py` & `beam-sdk-0.9.9/beam/base.py`

 * *Files identical despite different names*

### Comparing `beam-sdk-0.9.8/beam/configs/mount.py` & `beam-sdk-0.9.9/beam/configs/mount.py`

 * *Files identical despite different names*

### Comparing `beam-sdk-0.9.8/beam/configs/outputs.py` & `beam-sdk-0.9.9/beam/configs/outputs.py`

 * *Files identical despite different names*

### Comparing `beam-sdk-0.9.8/beam/configs/trigger.py` & `beam-sdk-0.9.9/beam/configs/trigger.py`

 * *Files identical despite different names*

### Comparing `beam-sdk-0.9.8/beam/scripts/build.py` & `beam-sdk-0.9.9/beam/scripts/build.py`

 * *Files identical despite different names*

### Comparing `beam-sdk-0.9.8/beam/scripts/init.py` & `beam-sdk-0.9.9/beam/scripts/init.py`

 * *Files identical despite different names*

### Comparing `beam-sdk-0.9.8/beam/serializer.py` & `beam-sdk-0.9.9/beam/serializer.py`

 * *Files identical despite different names*

### Comparing `beam-sdk-0.9.8/beam/templates/base.jinja` & `beam-sdk-0.9.9/beam/templates/base.jinja`

 * *Files identical despite different names*

### Comparing `beam-sdk-0.9.8/beam/tests/test_app.py` & `beam-sdk-0.9.9/beam/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `beam-sdk-0.9.8/beam/tests/test_validators.py` & `beam-sdk-0.9.9/beam/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `beam-sdk-0.9.8/beam/types.py` & `beam-sdk-0.9.9/beam/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,19 +383,21 @@
         return self._to_boolean(data)
 
 
 class PythonVersion:
     Python37 = "python3.7"
     Python38 = "python3.8"
     Python39 = "python3.9"
+    Python310 = "python3.10"
 
     Types = (
         (Python37, "python3.7"),
         (Python38, "python3.8"),
         (Python39, "python3.9"),
+        (Python310, "python3.10"),
     )
 
 
 class OutputType:
     Directory = "directory"
     File = "file"
```

### Comparing `beam-sdk-0.9.8/beam/utils.py` & `beam-sdk-0.9.9/beam/utils.py`

 * *Files identical despite different names*

### Comparing `beam-sdk-0.9.8/beam/validators.py` & `beam-sdk-0.9.9/beam/validators.py`

 * *Files identical despite different names*

### Comparing `beam-sdk-0.9.8/pyproject.toml` & `beam-sdk-0.9.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beam-sdk"
-version = "0.9.8"
+version = "0.9.9"
 description = ""
 authors = ["luke lombardi <luke@slai.io>"]
 packages = [
     { include = "beam" },
     { include = "beam/**/*.py" },
 ]
```

### Comparing `beam-sdk-0.9.8/setup.py` & `beam-sdk-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'marshmallow==3.18.0',
  'mypy>=0.981,<0.982',
  'packaging>=21.3,<22.0',
  'typeguard>=2.13.3,<3.0.0']
 
 setup_kwargs = {
     'name': 'beam-sdk',
-    'version': '0.9.8',
+    'version': '0.9.9',
     'description': '',
     'long_description': 'None',
     'author': 'luke lombardi',
     'author_email': 'luke@slai.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `beam-sdk-0.9.8/PKG-INFO` & `beam-sdk-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beam-sdk
-Version: 0.9.8
+Version: 0.9.9
 Summary: 
 Author: luke lombardi
 Author-email: luke@slai.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

