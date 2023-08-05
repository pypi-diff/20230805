# Comparing `tmp/companycam-unofficial-0.1.6.tar.gz` & `tmp/companycam-unofficial-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "companycam-unofficial-0.1.6.tar", last modified: Wed Feb  1 01:47:48 2023, max compression
+gzip compressed data, was "companycam-unofficial-0.2.0.tar", last modified: Sat Jun 24 22:42:48 2023, max compression
```

## Comparing `companycam-unofficial-0.1.6.tar` & `companycam-unofficial-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 01:47:48.950600 companycam-unofficial-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-02-01 01:47:32.000000 companycam-unofficial-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-02-01 01:47:48.950600 companycam-unofficial-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-02-01 01:47:32.000000 companycam-unofficial-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 01:47:48.950600 companycam-unofficial-0.1.6/companycam/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-02-01 01:47:32.000000 companycam-unofficial-0.1.6/companycam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-02-01 01:47:32.000000 companycam-unofficial-0.1.6/companycam/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-02-01 01:47:32.000000 companycam-unofficial-0.1.6/companycam/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-02-01 01:47:32.000000 companycam-unofficial-0.1.6/companycam/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-02-01 01:47:32.000000 companycam-unofficial-0.1.6/companycam/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-02-01 01:47:32.000000 companycam-unofficial-0.1.6/companycam/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-02-01 01:47:32.000000 companycam-unofficial-0.1.6/companycam/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 01:47:48.950600 companycam-unofficial-0.1.6/companycam/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-01 01:47:32.000000 companycam-unofficial-0.1.6/companycam/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-01 01:47:32.000000 companycam-unofficial-0.1.6/companycam/v2/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-02-01 01:47:32.000000 companycam-unofficial-0.1.6/companycam/v2/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-02-01 01:47:32.000000 companycam-unofficial-0.1.6/companycam/v2/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 01:47:48.950600 companycam-unofficial-0.1.6/companycam_unofficial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-02-01 01:47:48.000000 companycam-unofficial-0.1.6/companycam_unofficial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-02-01 01:47:48.000000 companycam-unofficial-0.1.6/companycam_unofficial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 01:47:48.000000 companycam-unofficial-0.1.6/companycam_unofficial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-01 01:47:48.000000 companycam-unofficial-0.1.6/companycam_unofficial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-01 01:47:48.000000 companycam-unofficial-0.1.6/companycam_unofficial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-01 01:47:32.000000 companycam-unofficial-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-02-01 01:47:48.954600 companycam-unofficial-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 01:47:48.950600 companycam-unofficial-0.1.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 01:47:48.950600 companycam-unofficial-0.1.6/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 01:47:32.000000 companycam-unofficial-0.1.6/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-02-01 01:47:32.000000 companycam-unofficial-0.1.6/tests/fixtures/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-02-01 01:47:32.000000 companycam-unofficial-0.1.6/tests/fixtures/v2_model_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:42:48.171184 companycam-unofficial-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-24 22:42:36.000000 companycam-unofficial-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-24 22:42:48.171184 companycam-unofficial-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-24 22:42:36.000000 companycam-unofficial-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:42:48.167184 companycam-unofficial-0.2.0/companycam/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-24 22:42:36.000000 companycam-unofficial-0.2.0/companycam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-24 22:42:36.000000 companycam-unofficial-0.2.0/companycam/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-24 22:42:36.000000 companycam-unofficial-0.2.0/companycam/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-24 22:42:36.000000 companycam-unofficial-0.2.0/companycam/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-06-24 22:42:36.000000 companycam-unofficial-0.2.0/companycam/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-24 22:42:36.000000 companycam-unofficial-0.2.0/companycam/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 22:42:36.000000 companycam-unofficial-0.2.0/companycam/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-24 22:42:36.000000 companycam-unofficial-0.2.0/companycam/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:42:48.167184 companycam-unofficial-0.2.0/companycam_unofficial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-24 22:42:48.000000 companycam-unofficial-0.2.0/companycam_unofficial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-24 22:42:48.000000 companycam-unofficial-0.2.0/companycam_unofficial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 22:42:48.000000 companycam-unofficial-0.2.0/companycam_unofficial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-24 22:42:48.000000 companycam-unofficial-0.2.0/companycam_unofficial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-24 22:42:48.000000 companycam-unofficial-0.2.0/companycam_unofficial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-24 22:42:36.000000 companycam-unofficial-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 22:42:48.171184 companycam-unofficial-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 22:42:48.171184 companycam-unofficial-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-24 22:42:36.000000 companycam-unofficial-0.2.0/tests/test_companycam_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-24 22:42:36.000000 companycam-unofficial-0.2.0/tests/test_companycam_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-24 22:42:36.000000 companycam-unofficial-0.2.0/tests/test_companycam_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-24 22:42:36.000000 companycam-unofficial-0.2.0/tests/test_companycam_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-24 22:42:36.000000 companycam-unofficial-0.2.0/tests/test_companycam_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-24 22:42:36.000000 companycam-unofficial-0.2.0/tests/test_companycam_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-24 22:42:36.000000 companycam-unofficial-0.2.0/tests/test_companycam_v2_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-06-24 22:42:36.000000 companycam-unofficial-0.2.0/tests/test_companycam_v2_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-24 22:42:36.000000 companycam-unofficial-0.2.0/tests/test_companycam_v2_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-24 22:42:36.000000 companycam-unofficial-0.2.0/tests/test_tests_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-24 22:42:36.000000 companycam-unofficial-0.2.0/tests/test_tests_utils.py
```

### Comparing `companycam-unofficial-0.1.6/LICENSE` & `companycam-unofficial-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `companycam-unofficial-0.1.6/PKG-INFO` & `companycam-unofficial-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: companycam-unofficial
-Version: 0.1.6
+Version: 0.2.0
 Summary: Python client and bindings for CompanyCam API.
-Home-page: https://github.com/ely-as/python-companycam
-Author: Elyas Khan
-Author-email: mail@ely.as
+Author-email: elyas <elyas@ely.as>
 License: MIT
+Project-URL: Issue Tracker, https://github.com/ely-as/python-companycam/issues
 Project-URL: Source, https://github.com/ely-as/python-companycam
-Project-URL: Tracker, https://github.com/ely-as/python-companycam/issues
+Keywords: python,companycam
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 # python-companycam
 
-![Test](https://github.com/ely-as/python-companycam/workflows/Test/badge.svg)
+[![Test](https://github.com/ely-as/python-companycam/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/ely-as/python-companycam/actions/workflows/test.yml)
+[![Coverage](https://cov.ely.as/github/ely-as/python-companycam/main/badge.svg)](https://cov.ely.as/github/ely-as/python-companycam/main/latest/)
+[![Version](https://img.shields.io/pypi/v/companycam-unofficial)](https://pypi.org/project/companycam-unofficial/)
 ![Python](https://img.shields.io/pypi/pyversions/companycam-unofficial)
-![License](https://img.shields.io/pypi/l/companycam-unofficial)
 
 ## Installation
 
 ```sh
 python -m pip install companycam-unofficial
 ```
```

### Comparing `companycam-unofficial-0.1.6/README.md` & `companycam-unofficial-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # python-companycam
 
-![Test](https://github.com/ely-as/python-companycam/workflows/Test/badge.svg)
+[![Test](https://github.com/ely-as/python-companycam/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/ely-as/python-companycam/actions/workflows/test.yml)
+[![Coverage](https://cov.ely.as/github/ely-as/python-companycam/main/badge.svg)](https://cov.ely.as/github/ely-as/python-companycam/main/latest/)
+[![Version](https://img.shields.io/pypi/v/companycam-unofficial)](https://pypi.org/project/companycam-unofficial/)
 ![Python](https://img.shields.io/pypi/pyversions/companycam-unofficial)
-![License](https://img.shields.io/pypi/l/companycam-unofficial)
 
 ## Installation
 
 ```sh
 python -m pip install companycam-unofficial
 ```
```

### Comparing `companycam-unofficial-0.1.6/companycam/api.py` & `companycam-unofficial-0.2.0/companycam/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from __future__ import annotations
-
 import typing
+from collections.abc import Generator
 
 import httpx
 
 from companycam import v2
 from companycam.client import LazyClient
 from companycam.exceptions import map_status_codes_to_exceptions
 
 STATUS_CODES_TO_EXCEPTIONS = map_status_codes_to_exceptions()
-SUPPORTED_VERSIONS: typing.List[str] = ["v2"]
+SUPPORTED_VERSIONS: list[str] = ["v2"]
 
 
 def raise_on_4xx_5xx(response: httpx.Response) -> None:
     """Raise a custom CompanyCam exception if the response has a status code which
     matches a code used by CompanyCam.
 
     See https://docs.companycam.com/reference/codes for a list of status codes used by
@@ -31,15 +30,15 @@
 
 class BasicTokenAuth(httpx.Auth):
     def __init__(self, token: str) -> None:
         self.token = token
 
     def auth_flow(
         self, request: httpx.Request
-    ) -> typing.Generator[httpx.Request, httpx.Response, None]:
+    ) -> Generator[httpx.Request, httpx.Response, None]:
         request.headers["authorization"] = f"Bearer {self.token}"
         yield request
 
 
 class API(object):
     """
     Usage:
```

### Comparing `companycam-unofficial-0.1.6/companycam/client.py` & `companycam-unofficial-0.2.0/companycam/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from __future__ import annotations
-
 import typing
+from collections.abc import Callable, Mapping
 
 import httpx
 
-EventHook = typing.Callable[..., typing.Any]
-EventHooks = typing.Mapping[str, typing.List[EventHook]]
+EventHook = Callable[..., typing.Any]
+EventHooks = Mapping[str, list[EventHook]]
 
 
 class LazyClient(object):
     """Thin wrapper around `httpx.Client`.
 
     Clients are useful because you can configure common parameters to use between
     requests e.g. auth, headers, base URL etc. However they are best used in context
@@ -21,15 +20,15 @@
     later time, so we can leverage the benefits of `httpx.Client` and its configuration
     merging while also observing HTTPX's recommended best practice.
     """
 
     def __init__(
         self,
         auth: httpx.Auth | None = None,
-        headers: typing.Mapping | None = None,
+        headers: Mapping | None = None,
         event_hooks: EventHooks | None = None,
         base_url: str = "",
     ) -> None:
         self.auth = auth
         self.headers = httpx.Headers(headers) if headers else headers
         self.event_hooks = event_hooks
         self.base_url = httpx.URL(base_url)
```

### Comparing `companycam-unofficial-0.1.6/companycam/exceptions.py` & `companycam-unofficial-0.2.0/companycam/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,28 +10,26 @@
 except companycam.Forbidden as exc:
     ...
 ```
 
 The class names, status codes and docstrings used for subclasses of
 `BaseCompanyCamException` are based on: https://docs.companycam.com/reference/codes.
 """
-from typing import Dict, Type
-
 import httpx
 
 
 class BaseCompanyCamException(httpx.HTTPStatusError):
     """Subclasses should have unique status codes, and should not themselves be
     subclassed.
     """
 
     status_code: int
 
 
-def map_status_codes_to_exceptions() -> Dict[int, Type[BaseCompanyCamException]]:
+def map_status_codes_to_exceptions() -> dict[int, type[BaseCompanyCamException]]:
     # Using `__subclasses__()` relies on all subclasses being defined in this file
     return {exc.status_code: exc for exc in BaseCompanyCamException.__subclasses__()}
 
 
 class BadRequest(BaseCompanyCamException):
     """The request is invalid"""
```

### Comparing `companycam-unofficial-0.1.6/companycam/manager.py` & `companycam-unofficial-0.2.0/companycam/manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,50 @@
-from __future__ import annotations
-
 import functools
 import inspect
 import logging
+from collections.abc import Callable
 from string import Formatter
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Literal, Type, Union
+from typing import Any, Literal
 
+import httpx
 from pydantic import BaseModel, ValidationError, parse_obj_as
 
 from companycam.client import LazyClient
 
-if TYPE_CHECKING:
-    import httpx
-
 formatter = Formatter()
 logger = logging.getLogger(__name__)
 
 
 class BaseManager(object):
     client: LazyClient
 
     def __init__(self, client: LazyClient) -> None:
         self.client = client
 
 
-def field_names_in_format_string(format_string: str) -> List[str]:
+def field_names_in_format_string(format_string: str) -> list[str]:
     """For a given format string return the field_name's
 
     More on format strings: https://docs.python.org/3/library/string.html#formatstrings
     """
     return [x[1] for x in formatter.parse(format_string) if x[1]]
 
 
-def get_string_from_object(obj: Union[BaseModel, str]) -> str:
+def get_string_from_object(obj: BaseModel | str) -> str:
     if isinstance(obj, str):
         return obj
     elif isinstance(obj, BaseModel) and hasattr(obj, "id"):
-        return getattr(obj, "id")
+        return obj.id
     elif isinstance(obj, BaseModel):
         raise ValueError(f"Failed to extract 'id' from {obj}: Model has no 'id' field")
     else:
         raise TypeError()
 
 
-def format_url(url: str, kwargs: Dict) -> str:
+def format_url(url: str, kwargs: dict) -> str:
     expected_fields = field_names_in_format_string(url)
     url_kwargs = {}
     for field in expected_fields:
         url_kwargs[field] = get_string_from_object(kwargs[field])
     return url.format(**url_kwargs)
 
 
@@ -59,31 +56,26 @@
     decorator.
     """
     return request_dict
 
 
 class BaseRequest(object):
     method: Literal["get", "post", "put", "delete"]
-    return_type: Type
+    return_type: type
     url: str
 
-    def __init__(self, url: str, return_type: Type) -> None:
+    def __init__(self, url: str) -> None:
         super().__init__()
         self.url = url
-        # It would be cleaner to get the return_type from the decorated method e.g.
-        # `decorated_method.__annotations__.get("return", Any)`, but in the future this
-        # may only contain strings rather than actual types due to PEP 563 (unless it
-        # is superceded by PEP 649). See:
-        # - https://peps.python.org/pep-0563/
-        # - https://peps.python.org/pep-0649/
-        self.return_type = return_type
 
     def __call__(self, decorated_method: Callable[..., Any]) -> Callable[..., Any]:
         # store decorator object for introspection of decorated_method (e.g. unit tests)
         decorated_method._decorated_by = self  # type: ignore[attr-defined]
+        # store return_type
+        self.return_type = decorated_method.__annotations__.get("return")  # type: ignore[assignment]
 
         @functools.wraps(decorated_method)
         def wrapper(obj, *args, **kwargs):
             # Call method
             request_dict = decorated_method(obj, *args, **kwargs)
             if "url" not in request_dict:
                 # Convert any args to kwargs for format_url
```

### Comparing `companycam-unofficial-0.1.6/companycam/models.py` & `companycam-unofficial-0.2.0/companycam/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     preserves the original field name in any outputs.
 
     Cannot simply use @property setters with pydantic, see
     https://github.com/pydantic/pydantic/issues/1577.
     """
 
     class Config:
-        assignment_aliases: typing.Dict[str, str]
+        assignment_aliases: dict[str, str]
 
     def __init__(self, *args, **kwargs) -> None:
         config = super().__getattribute__("__config__")
         assignment_aliases = getattr(config, "assignment_aliases", {})
         for alias, field_name in assignment_aliases.items():
             if alias in kwargs and field_name not in kwargs:
                 kwargs[field_name] = kwargs.pop(alias)
@@ -33,15 +33,15 @@
     def __setattr__(self, name: str, value: typing.Any) -> None:
         config = super().__getattribute__("__config__")
         assignment_aliases = getattr(config, "assignment_aliases", {})
         if name in assignment_aliases:
             name = assignment_aliases[name]
         return super().__setattr__(name, value)
 
-    def dict(self, exclude_none: bool = True, **kwargs) -> typing.Dict[str, typing.Any]:
+    def dict(self, exclude_none: bool = True, **kwargs) -> dict[str, typing.Any]:
         return super().dict(exclude_none=exclude_none, **kwargs)
 
 
 class ModelWithRequiredID(Model):
     # 'id' is a required field in most models where it is a field, but we want users to
     # be able to construct model objects without an 'id' since that is set by the API
-    id: typing.Optional[str]
+    id: str | None
```

### Comparing `companycam-unofficial-0.1.6/companycam/types.py` & `companycam-unofficial-0.2.0/companycam/types.py`

 * *Files identical despite different names*

### Comparing `companycam-unofficial-0.1.6/companycam_unofficial.egg-info/PKG-INFO` & `companycam-unofficial-0.2.0/companycam_unofficial.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: companycam-unofficial
-Version: 0.1.6
+Version: 0.2.0
 Summary: Python client and bindings for CompanyCam API.
-Home-page: https://github.com/ely-as/python-companycam
-Author: Elyas Khan
-Author-email: mail@ely.as
+Author-email: elyas <elyas@ely.as>
 License: MIT
+Project-URL: Issue Tracker, https://github.com/ely-as/python-companycam/issues
 Project-URL: Source, https://github.com/ely-as/python-companycam
-Project-URL: Tracker, https://github.com/ely-as/python-companycam/issues
+Keywords: python,companycam
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 # python-companycam
 
-![Test](https://github.com/ely-as/python-companycam/workflows/Test/badge.svg)
+[![Test](https://github.com/ely-as/python-companycam/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/ely-as/python-companycam/actions/workflows/test.yml)
+[![Coverage](https://cov.ely.as/github/ely-as/python-companycam/main/badge.svg)](https://cov.ely.as/github/ely-as/python-companycam/main/latest/)
+[![Version](https://img.shields.io/pypi/v/companycam-unofficial)](https://pypi.org/project/companycam-unofficial/)
 ![Python](https://img.shields.io/pypi/pyversions/companycam-unofficial)
-![License](https://img.shields.io/pypi/l/companycam-unofficial)
 
 ## Installation
 
 ```sh
 python -m pip install companycam-unofficial
 ```
```

