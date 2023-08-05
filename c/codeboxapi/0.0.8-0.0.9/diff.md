# Comparing `tmp/codeboxapi-0.0.8.tar.gz` & `tmp/codeboxapi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeboxapi-0.0.8.tar", max compression
+gzip compressed data, was "codeboxapi-0.0.9.tar", max compression
```

## Comparing `codeboxapi-0.0.8.tar` & `codeboxapi-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1074 2023-07-09 12:26:51.625346 codeboxapi-0.0.8/LICENSE
--rw-r--r--   0        0        0     1124 2023-07-14 23:30:25.010671 codeboxapi-0.0.8/README.md
--rw-r--r--   0        0        0      447 2023-07-17 13:07:06.595127 codeboxapi-0.0.8/codeboxapi/__init__.py
--rw-r--r--   0        0        0       89 2023-07-17 13:07:06.595368 codeboxapi-0.0.8/codeboxapi/box/__init__.py
--rw-r--r--   0        0        0     2351 2023-07-17 13:07:06.595639 codeboxapi-0.0.8/codeboxapi/box/basebox.py
--rw-r--r--   0        0        0     5645 2023-07-17 13:22:59.484993 codeboxapi-0.0.8/codeboxapi/box/codebox.py
--rw-r--r--   0        0        0    16777 2023-07-17 13:22:59.488023 codeboxapi-0.0.8/codeboxapi/box/localbox.py
--rw-r--r--   0        0        0      396 2023-07-17 13:22:59.488093 codeboxapi-0.0.8/codeboxapi/config.py
--rw-r--r--   0        0        0     1822 2023-07-09 12:26:51.659184 codeboxapi-0.0.8/codeboxapi/errors.py
--rw-r--r--   0        0        0      628 2023-07-17 13:22:59.488147 codeboxapi-0.0.8/codeboxapi/schema.py
--rw-r--r--   0        0        0     2925 2023-07-17 13:22:59.488185 codeboxapi-0.0.8/codeboxapi/utils.py
--rw-r--r--   0        0        0      595 2023-07-17 13:23:59.278123 codeboxapi-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1918 1970-01-01 00:00:00.000000 codeboxapi-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-09 12:26:51.625346 codeboxapi-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1124 2023-07-14 23:30:25.010671 codeboxapi-0.0.9/README.md
+-rw-r--r--   0        0        0      190 2023-07-17 16:01:23.544872 codeboxapi-0.0.9/codeboxapi/__init__.py
+-rw-r--r--   0        0        0       89 2023-07-17 13:07:06.595368 codeboxapi-0.0.9/codeboxapi/box/__init__.py
+-rw-r--r--   0        0        0     2333 2023-07-22 18:12:22.204013 codeboxapi-0.0.9/codeboxapi/box/basebox.py
+-rw-r--r--   0        0        0     5935 2023-07-22 19:04:18.134230 codeboxapi-0.0.9/codeboxapi/box/codebox.py
+-rw-r--r--   0        0        0    16777 2023-07-17 13:22:59.488023 codeboxapi-0.0.9/codeboxapi/box/localbox.py
+-rw-r--r--   0        0        0      404 2023-07-17 20:31:29.809289 codeboxapi-0.0.9/codeboxapi/config.py
+-rw-r--r--   0        0        0     1822 2023-07-09 12:26:51.659184 codeboxapi-0.0.9/codeboxapi/errors.py
+-rw-r--r--   0        0        0      628 2023-07-17 13:22:59.488147 codeboxapi-0.0.9/codeboxapi/schema.py
+-rw-r--r--   0        0        0     2925 2023-07-17 13:22:59.488185 codeboxapi-0.0.9/codeboxapi/utils.py
+-rw-r--r--   0        0        0      611 2023-07-23 15:26:23.390777 codeboxapi-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1951 1970-01-01 00:00:00.000000 codeboxapi-0.0.9/PKG-INFO
```

### Comparing `codeboxapi-0.0.8/LICENSE` & `codeboxapi-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.0.8/README.md` & `codeboxapi-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.0.8/codeboxapi/box/basebox.py` & `codeboxapi-0.0.9/codeboxapi/box/basebox.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from uuid import uuid4
 from datetime import datetime
 from typing_extensions import Self
 from abc import ABC, abstractmethod
 from ..schema import (
     CodeBoxStatus, 
     CodeBoxOutput,
     CodeBoxFile,
@@ -11,15 +10,15 @@
 
 class BaseBox(ABC):
     """ 
     ABC for Isolated Execution Environments
     """
     
     def __init__(self) -> None:
-        self.id = uuid4().int
+        self.id: int | None = None
         self.last_interaction = datetime.now()
 
     def _update(self) -> None:
         self.last_interaction = datetime.now()
     
     @abstractmethod
     def start(self) -> CodeBoxStatus: ...
```

### Comparing `codeboxapi-0.0.8/codeboxapi/box/codebox.py` & `codeboxapi-0.0.9/codeboxapi/box/codebox.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,21 +22,14 @@
         else:
             return super().__new__(cls, *args, **kwargs)
     
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.session: Optional[ClientSession] = None
     
-    def start(self) -> CodeBoxStatus:
-        return self.status()
-    
-    async def astart(self) -> CodeBoxStatus:
-        self.session = ClientSession()
-        return await self.astatus()
-    
     def codebox_request(
         self, 
         method, 
         endpoint, 
         *args, **kwargs
     ) -> dict[str, Any]:
         self._update()
@@ -58,14 +51,30 @@
         return await abase_request(
             self.session,
             method,
             f"/codebox/{self.id}" + endpoint,
             *args, **kwargs
         )
     
+    def start(self) -> CodeBoxStatus:
+        self.id = base_request(
+            method="GET",
+            endpoint="/codebox/start",
+        )["id"]
+        return CodeBoxStatus(status="started")
+    
+    async def astart(self) -> CodeBoxStatus:
+        self.session = ClientSession()
+        self.id = (await abase_request(
+            self.session,
+            method="GET",
+            endpoint="/codebox/start",
+        ))["id"]
+        return CodeBoxStatus(status="started")
+    
     def status(self):
         return CodeBoxStatus(
             ** self.codebox_request(
                 method="GET",
                 endpoint="/",
             )
         )
```

### Comparing `codeboxapi-0.0.8/codeboxapi/box/localbox.py` & `codeboxapi-0.0.9/codeboxapi/box/localbox.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.0.8/codeboxapi/errors.py` & `codeboxapi-0.0.9/codeboxapi/errors.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.0.8/codeboxapi/schema.py` & `codeboxapi-0.0.9/codeboxapi/schema.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.0.8/codeboxapi/utils.py` & `codeboxapi-0.0.9/codeboxapi/utils.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.0.8/pyproject.toml` & `codeboxapi-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "codeboxapi"
-version = "0.0.8"
+version = "0.0.9"
 description = "CodeBox is the simplest cloud infrastructure for your LLM Apps and Services."
 authors = ["Shroominic <pleurae-berets.0u@icloud.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-python-dotenv = "^1.0.0"
-websockets = "^11.0.3"
-aiohttp = "^3.8.4"
+pydantic = "^1"
 requests = "^2.27.1"
+aiohttp = "^3.8.4"
+websockets = "^11.0.3"
+python-dotenv = "^1.0.0"
 jupyter-kernel-gateway = "^2.5.2"
 
 [tool.poetry.extras]
 image_support = ["Pillow"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.4.0"
```

### Comparing `codeboxapi-0.0.8/PKG-INFO` & `codeboxapi-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: codeboxapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: CodeBox is the simplest cloud infrastructure for your LLM Apps and Services.
 License: MIT
 Author: Shroominic
 Author-email: pleurae-berets.0u@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: image-support
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: jupyter-kernel-gateway (>=2.5.2,<3.0.0)
+Requires-Dist: pydantic (>=1,<2)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: websockets (>=11.0.3,<12.0.0)
 Description-Content-Type: text/markdown
 
 # CodeBox
```

