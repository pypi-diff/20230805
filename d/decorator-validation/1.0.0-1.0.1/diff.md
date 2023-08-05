# Comparing `tmp/decorator_validation-1.0.0.tar.gz` & `tmp/decorator_validation-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decorator_validation-1.0.0.tar", max compression
+gzip compressed data, was "decorator_validation-1.0.1.tar", max compression
```

## Comparing `decorator_validation-1.0.0.tar` & `decorator_validation-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       38 2023-08-03 14:40:11.351648 decorator_validation-1.0.0/decorator_validation/__init__.py
--rw-r--r--   0        0        0     2642 2023-08-03 14:13:48.790369 decorator_validation-1.0.0/decorator_validation/decorators.py
--rw-r--r--   0        0        0      518 2023-08-03 14:45:33.376432 decorator_validation-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1310 2023-08-03 14:45:15.137378 decorator_validation-1.0.0/README.md
--rw-r--r--   0        0        0     1658 1970-01-01 00:00:00.000000 decorator_validation-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      116 2023-08-05 05:49:37.771287 decorator_validation-1.0.1/decorator_validation/__init__.py
+-rw-r--r--   0        0        0     2646 2023-08-05 05:30:05.838165 decorator_validation-1.0.1/decorator_validation/decorators.py
+-rw-r--r--   0        0        0      603 2023-08-05 05:40:40.584014 decorator_validation-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2196 2023-08-05 05:49:18.386963 decorator_validation-1.0.1/README.md
+-rw-r--r--   0        0        0     2562 1970-01-01 00:00:00.000000 decorator_validation-1.0.1/PKG-INFO
```

### Comparing `decorator_validation-1.0.0/decorator_validation/decorators.py` & `decorator_validation-1.0.1/decorator_validation/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 class ValidationError(Exception):
     ...
 
 
 class SkipTypeCheck(type):
     ...
 
-def convert_with(converter: Callable):
 
+def convert_with(converter: Callable):
     # fmt: off
     def inner(func):
         @wraps(func)
         def inner_inner(*args, **kwargs):
             new_args, new_kwargs = converter(*args, **kwargs)
             return func(*new_args, **new_kwargs)
         return inner_inner
     return inner
 
+
 def validate_with(validator: Callable):
     """Decorator that validates args and kwargs passed to the decorated function with the validator.
 
     The Validator has to return either 0, None or False, or directly throw an exception.
 
     Parameters
     ----------
@@ -77,8 +78,8 @@
                 allowed_types = type_kwargs[key]
                 if SkipTypeCheck not in allowed_types and not isinstance(val, allowed_types):
                     raise TypeError(f"Type Mismatch {type(val)} not in {allowed_types}")
             return func(*args, **kwargs)
 
         return inner_inner
 
-    return inner
+    return inner
```

### Comparing `decorator_validation-1.0.0/pyproject.toml` & `decorator_validation-1.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "decorator_validation"
-version = "1.0.0"
-description = ""
-    authors = ["FailedRobot <sry@nomail.com>"]
+version = "1.0.1"
+description = "Fast Argument validation for functions using decorators"
+authors = ["FailedRobot <sry@nomail.com>"]
 readme = "README.md"
 packages = [{include = "decorator_validation"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 
 [tool.poetry.group.dev]
@@ -18,8 +18,11 @@
 pytest-cov = "^4.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
+line-length = 120
+
+[tool.ruff]
 line-length = 120
```

### Comparing `decorator_validation-1.0.0/PKG-INFO` & `decorator_validation-1.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: decorator-validation
-Version: 1.0.0
-Summary: 
+Version: 1.0.1
+Summary: Fast Argument validation for functions using decorators
 Author: FailedRobot
 Author-email: sry@nomail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -57,7 +57,44 @@
 
 @convert_with(from_dict)
 def foo(bar: int, message:str, some_additional_info: dict):
     ...
 
 ```
 
+Skip Type-checks by providing the `SkipTypecheck` class as a type, this is very usefull for methods.
+
+```python
+from decorator_validation.decorators import validate_types, SkipTypeCheck
+
+class FileReader:
+
+    @validate_types((SkipTypeCheck,), file_path=(str,))
+    def __init__(self, file_path: str):
+        ...
+
+```
+
+Of course, sometimes you want to have custom error messages.
+Then, just use the following code:
+
+
+```python
+from decorator_validation.decorators import validate_with
+from pathlib import Path
+
+def my_validation_func(obj, file_path:str) -> True:
+    
+    if not isinstance(file_path, str):
+        raise TypeError(...)
+    if not Path(file_path).resolver().is_file():
+        raise ValueError(...)
+    return True
+
+class FileReader:
+
+    @validate_with(my_validation_func)
+    def __init__(self, file_path: str):
+        ...
+
+```
+
```

