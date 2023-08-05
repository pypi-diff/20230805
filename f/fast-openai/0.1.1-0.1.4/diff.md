# Comparing `tmp/fast_openai-0.1.1.tar.gz` & `tmp/fast_openai-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_openai-0.1.1.tar", max compression
+gzip compressed data, was "fast_openai-0.1.4.tar", max compression
```

## Comparing `fast_openai-0.1.1.tar` & `fast_openai-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,23 @@
--rw-r--r--   0        0        0        0 2023-08-04 23:36:33.206542 fast_openai-0.1.1/README.md
--rw-r--r--   0        0        0       84 2023-08-05 01:00:30.931425 fast_openai-0.1.1/fast_openai/__init__.py
--rw-r--r--   0        0        0     2110 2023-08-05 02:03:38.737275 fast_openai-0.1.1/fast_openai/application.py
--rw-r--r--   0        0        0    11120 2023-08-05 01:10:51.203081 fast_openai-0.1.1/fast_openai/client.py
--rw-r--r--   0        0        0        0 2023-08-04 23:45:49.334138 fast_openai-0.1.1/fast_openai/db/__init__.py
--rw-r--r--   0        0        0     7771 2023-08-04 23:57:15.297656 fast_openai-0.1.1/fast_openai/db/errors.py
--rw-r--r--   0        0        0     5659 2023-08-04 23:57:23.389650 fast_openai-0.1.1/fast_openai/db/objects.py
--rw-r--r--   0        0        0     1637 2023-08-04 23:57:19.373653 fast_openai-0.1.1/fast_openai/db/page.py
--rw-r--r--   0        0        0    17374 2023-08-04 23:57:19.269653 fast_openai-0.1.1/fast_openai/db/query.py
--rw-r--r--   0        0        0      231 2023-08-05 00:18:28.264808 fast_openai-0.1.1/fast_openai/fields.py
--rw-r--r--   0        0        0     6436 2023-08-04 23:57:30.649645 fast_openai-0.1.1/fast_openai/json.py
--rw-r--r--   0        0        0       55 2023-08-05 00:18:28.264808 fast_openai-0.1.1/fast_openai/llm/__init__.py
--rw-r--r--   0        0        0    10343 2023-08-05 00:18:28.464808 fast_openai-0.1.1/fast_openai/llm/llm.py
--rw-r--r--   0        0        0     2381 2023-08-05 00:18:28.332808 fast_openai-0.1.1/fast_openai/llm/schemas.py
--rw-r--r--   0        0        0     9745 2023-08-05 01:03:16.859335 fast_openai-0.1.1/fast_openai/odm.py
--rw-r--r--   0        0        0     1941 2023-08-05 00:18:28.364808 fast_openai-0.1.1/fast_openai/typedefs.py
--rw-r--r--   0        0        0     2914 2023-08-05 02:09:22.633053 fast_openai-0.1.1/fast_openai/utils.py
--rw-r--r--   0        0        0      519 2023-08-05 02:05:12.629216 fast_openai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 fast_openai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-04 23:36:33.206542 fast_openai-0.1.4/README.md
+-rw-r--r--   0        0        0      586 2023-08-05 02:14:43.696851 fast_openai-0.1.4/fast_openai/__init__.py
+-rw-r--r--   0        0        0     2156 2023-08-05 02:16:03.228802 fast_openai-0.1.4/fast_openai/application.py
+-rw-r--r--   0        0        0    11120 2023-08-05 01:10:51.203081 fast_openai-0.1.4/fast_openai/client.py
+-rw-r--r--   0        0        0        0 2023-08-04 23:45:49.334138 fast_openai-0.1.4/fast_openai/db/__init__.py
+-rw-r--r--   0        0        0     7771 2023-08-04 23:57:15.297656 fast_openai-0.1.4/fast_openai/db/errors.py
+-rw-r--r--   0        0        0     5659 2023-08-04 23:57:23.389650 fast_openai-0.1.4/fast_openai/db/objects.py
+-rw-r--r--   0        0        0     1637 2023-08-04 23:57:19.373653 fast_openai-0.1.4/fast_openai/db/page.py
+-rw-r--r--   0        0        0    17374 2023-08-04 23:57:19.269653 fast_openai-0.1.4/fast_openai/db/query.py
+-rw-r--r--   0        0        0      231 2023-08-05 00:18:28.264808 fast_openai-0.1.4/fast_openai/fields.py
+-rw-r--r--   0        0        0       81 2023-08-05 02:56:09.791354 fast_openai-0.1.4/fast_openai/fmt/__init__.py
+-rw-r--r--   0        0        0     2746 2023-08-05 02:55:17.503381 fast_openai-0.1.4/fast_openai/fmt/jinja.py
+-rw-r--r--   0        0        0      497 2023-08-05 02:31:27.844211 fast_openai-0.1.4/fast_openai/fmt/markdownit.py
+-rw-r--r--   0        0        0      388 2023-08-05 02:27:07.952361 fast_openai-0.1.4/fast_openai/fmt/pygments.py
+-rw-r--r--   0        0        0     6436 2023-08-04 23:57:30.649645 fast_openai-0.1.4/fast_openai/json.py
+-rw-r--r--   0        0        0       55 2023-08-05 02:56:29.459344 fast_openai-0.1.4/fast_openai/llm/__init__.py
+-rw-r--r--   0        0        0    10343 2023-08-05 00:18:28.464808 fast_openai-0.1.4/fast_openai/llm/llm.py
+-rw-r--r--   0        0        0     2381 2023-08-05 02:14:13.960870 fast_openai-0.1.4/fast_openai/llm/schemas.py
+-rw-r--r--   0        0        0     9745 2023-08-05 01:03:16.859335 fast_openai-0.1.4/fast_openai/odm.py
+-rw-r--r--   0        0        0     1941 2023-08-05 00:18:28.364808 fast_openai-0.1.4/fast_openai/typedefs.py
+-rw-r--r--   0        0        0     2914 2023-08-05 02:09:22.633053 fast_openai-0.1.4/fast_openai/utils.py
+-rw-r--r--   0        0        0      519 2023-08-05 02:57:01.619326 fast_openai-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 fast_openai-0.1.4/PKG-INFO
```

### Comparing `fast_openai-0.1.1/fast_openai/application.py` & `fast_openai-0.1.4/fast_openai/application.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from functools import wraps
 import itertools
 from typing import Any, Callable, Coroutine, Dict, List, Optional, ParamSpecKwargs, Tuple, Type, Union
 from fastapi import FastAPI, Request, Response, WebSocket, WebSocketDisconnect
 from fastapi.responses import StreamingResponse
 from typing_extensions import ParamSpec
-
+from fastapi.templating import Jinja2Templates
 from .client import APIClient
 from .json import to_json
 from .llm import LLMStack
 from .odm import FaunaModel
 
 class FastOpenAI(FastAPI):
     """OpenAI Backend for FastAPI"""
```

### Comparing `fast_openai-0.1.1/fast_openai/client.py` & `fast_openai-0.1.4/fast_openai/client.py`

 * *Files identical despite different names*

### Comparing `fast_openai-0.1.1/fast_openai/db/errors.py` & `fast_openai-0.1.4/fast_openai/db/errors.py`

 * *Files identical despite different names*

### Comparing `fast_openai-0.1.1/fast_openai/db/objects.py` & `fast_openai-0.1.4/fast_openai/db/objects.py`

 * *Files identical despite different names*

### Comparing `fast_openai-0.1.1/fast_openai/db/page.py` & `fast_openai-0.1.4/fast_openai/db/page.py`

 * *Files identical despite different names*

### Comparing `fast_openai-0.1.1/fast_openai/db/query.py` & `fast_openai-0.1.4/fast_openai/db/query.py`

 * *Files identical despite different names*

### Comparing `fast_openai-0.1.1/fast_openai/json.py` & `fast_openai-0.1.4/fast_openai/json.py`

 * *Files identical despite different names*

### Comparing `fast_openai-0.1.1/fast_openai/llm/llm.py` & `fast_openai-0.1.4/fast_openai/llm/llm.py`

 * *Files identical despite different names*

### Comparing `fast_openai-0.1.1/fast_openai/llm/schemas.py` & `fast_openai-0.1.4/fast_openai/llm/schemas.py`

 * *Files identical despite different names*

### Comparing `fast_openai-0.1.1/fast_openai/odm.py` & `fast_openai-0.1.4/fast_openai/odm.py`

 * *Files identical despite different names*

### Comparing `fast_openai-0.1.1/fast_openai/typedefs.py` & `fast_openai-0.1.4/fast_openai/typedefs.py`

 * *Files identical despite different names*

### Comparing `fast_openai-0.1.1/fast_openai/utils.py` & `fast_openai-0.1.4/fast_openai/utils.py`

 * *Files identical despite different names*

### Comparing `fast_openai-0.1.1/pyproject.toml` & `fast_openai-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fast-openai"
-version = "0.1.1"
+version = "0.1.4"
 description = ""
 authors = ["Oscar Bahamonde <oscar.bahamonde@pucp.pe>"]
 readme = "README.md"
 packages = [{include = "fast_openai"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `fast_openai-0.1.1/PKG-INFO` & `fast_openai-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-openai
-Version: 0.1.1
+Version: 0.1.4
 Summary: 
 Author: Oscar Bahamonde
 Author-email: oscar.bahamonde@pucp.pe
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

