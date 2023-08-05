# Comparing `tmp/fastapi_cruddy_framework-0.0.8.tar.gz` & `tmp/fastapi_cruddy_framework-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_cruddy_framework-0.0.8.tar", max compression
+gzip compressed data, was "fastapi_cruddy_framework-0.0.9.tar", max compression
```

## Comparing `fastapi_cruddy_framework-0.0.8.tar` & `fastapi_cruddy_framework-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1074 2023-04-15 22:07:32.387542 fastapi_cruddy_framework-0.0.8/LICENSE
--rw-r--r--   0        0        0    29689 2023-04-16 00:33:35.866892 fastapi_cruddy_framework-0.0.8/README.md
--rw-r--r--   0        0        0      979 2023-04-15 22:07:32.387542 fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/__init__.py
--rw-r--r--   0        0        0     4533 2023-04-15 22:07:32.387542 fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/adapters.py
--rw-r--r--   0        0        0    17772 2023-04-18 15:27:38.582224 fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/controller.py
--rw-r--r--   0        0        0       46 2023-04-15 22:07:32.387542 fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/inflector.py
--rw-r--r--   0        0        0    24682 2023-04-16 00:38:48.250535 fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/repository.py
--rw-r--r--   0        0        0    19346 2023-04-15 22:07:32.387542 fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/resource.py
--rw-r--r--   0        0        0     2282 2023-04-15 22:07:32.391543 fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/router.py
--rw-r--r--   0        0        0     2633 2023-04-15 22:07:32.391543 fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/schemas.py
--rw-r--r--   0        0        0      468 2023-04-15 22:07:32.391543 fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/util.py
--rw-r--r--   0        0        0     4840 2023-04-15 22:07:32.391543 fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/uuid.py
--rw-r--r--   0        0        0     1895 2023-04-18 15:28:22.744103 fastapi_cruddy_framework-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    31056 1970-01-01 00:00:00.000000 fastapi_cruddy_framework-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-15 22:07:32.387542 fastapi_cruddy_framework-0.0.9/LICENSE
+-rw-r--r--   0        0        0    29689 2023-04-16 00:33:35.866892 fastapi_cruddy_framework-0.0.9/README.md
+-rw-r--r--   0        0        0      979 2023-04-15 22:07:32.387542 fastapi_cruddy_framework-0.0.9/fastapi_cruddy_framework/__init__.py
+-rw-r--r--   0        0        0     4533 2023-04-15 22:07:32.387542 fastapi_cruddy_framework-0.0.9/fastapi_cruddy_framework/adapters.py
+-rw-r--r--   0        0        0    17772 2023-04-18 15:27:38.582224 fastapi_cruddy_framework-0.0.9/fastapi_cruddy_framework/controller.py
+-rw-r--r--   0        0        0       46 2023-04-15 22:07:32.387542 fastapi_cruddy_framework-0.0.9/fastapi_cruddy_framework/inflector.py
+-rw-r--r--   0        0        0    25084 2023-04-19 05:00:40.276499 fastapi_cruddy_framework-0.0.9/fastapi_cruddy_framework/repository.py
+-rw-r--r--   0        0        0    19346 2023-04-15 22:07:32.387542 fastapi_cruddy_framework-0.0.9/fastapi_cruddy_framework/resource.py
+-rw-r--r--   0        0        0     2282 2023-04-15 22:07:32.391543 fastapi_cruddy_framework-0.0.9/fastapi_cruddy_framework/router.py
+-rw-r--r--   0        0        0     2633 2023-04-15 22:07:32.391543 fastapi_cruddy_framework-0.0.9/fastapi_cruddy_framework/schemas.py
+-rw-r--r--   0        0        0      468 2023-04-15 22:07:32.391543 fastapi_cruddy_framework-0.0.9/fastapi_cruddy_framework/util.py
+-rw-r--r--   0        0        0     4840 2023-04-15 22:07:32.391543 fastapi_cruddy_framework-0.0.9/fastapi_cruddy_framework/uuid.py
+-rw-r--r--   0        0        0     1895 2023-04-19 05:03:20.434173 fastapi_cruddy_framework-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    31056 1970-01-01 00:00:00.000000 fastapi_cruddy_framework-0.0.9/PKG-INFO
```

### Comparing `fastapi_cruddy_framework-0.0.8/LICENSE` & `fastapi_cruddy_framework-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-0.0.8/README.md` & `fastapi_cruddy_framework-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/__init__.py` & `fastapi_cruddy_framework-0.0.9/fastapi_cruddy_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/adapters.py` & `fastapi_cruddy_framework-0.0.9/fastapi_cruddy_framework/adapters.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/controller.py` & `fastapi_cruddy_framework-0.0.9/fastapi_cruddy_framework/controller.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/repository.py` & `fastapi_cruddy_framework-0.0.9/fastapi_cruddy_framework/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import math
+from asyncio import gather
 from logging import getLogger
 from sqlalchemy import (
     update as _update,
     delete as _delete,
     or_,
     and_,
     not_,
     func,
     column,
 )
+from sqlalchemy.engine import Result
 from sqlalchemy.sql import select, update
 from sqlalchemy.sql.schema import Table, Column
 from sqlalchemy.orm import RelationshipProperty, ONETOMANY, MANYTOMANY
 from sqlmodel import inspect
 from typing import Union, List, Dict
 from pydantic.types import Json
 from .schemas import (
@@ -240,17 +242,22 @@
         # pagination
         query = query.offset(offset_page * query_conf["limit"]).limit(
             query_conf["limit"]
         )
         # total record
 
         async with self.adapter.getSession() as session:
-            total_record = (await session.execute(count_query)).scalar() or 0
-            # result
-            result = (await session.execute(query)).fetchall()
+            results = await gather(
+                *[session.execute(count_query), session.execute(query)],
+                return_exceptions=False,
+            )
+            count: Result = results[0]
+            records: Result = results[1]
+            total_record = count.scalar() or 0
+            result = records.fetchall()
 
         # possible pass in outside functions to map/alter data?
         # total page
         total_page = math.ceil(total_record / query_conf["limit"])
         result = BulkDTO(
             total_pages=total_page,
             total_records=total_record,
@@ -340,17 +347,22 @@
         # pagination
         query = query.offset(offset_page * query_conf["limit"]).limit(
             query_conf["limit"]
         )
         # total record
 
         async with self.adapter.getSession() as session:
-            total_record = (await session.execute(count_query)).scalar() or 0
-            # result
-            result = (await session.execute(query)).fetchall()
+            results = await gather(
+                *[session.execute(count_query), session.execute(query)],
+                return_exceptions=False,
+            )
+            count: Result = results[0]
+            records: Result = results[1]
+            total_record = count.scalar() or 0
+            result = records.fetchall()
 
         # possible pass in outside functions to map/alter data?
         # total page
         total_page = math.ceil(total_record / query_conf["limit"])
         result = BulkDTO(
             total_pages=total_page,
             total_records=total_record,
```

### Comparing `fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/resource.py` & `fastapi_cruddy_framework-0.0.9/fastapi_cruddy_framework/resource.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/router.py` & `fastapi_cruddy_framework-0.0.9/fastapi_cruddy_framework/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/schemas.py` & `fastapi_cruddy_framework-0.0.9/fastapi_cruddy_framework/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/uuid.py` & `fastapi_cruddy_framework-0.0.9/fastapi_cruddy_framework/uuid.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-0.0.8/pyproject.toml` & `fastapi_cruddy_framework-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-cruddy-framework"
-version = "0.0.8"
+version = "0.0.9"
 description = "A holistic CRUD/MVC framework for FastAPI, with endpoint policies and relationships"
 authors = ["mdconaway <mdconaway@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "fastapi_cruddy_framework"}]
 homepage = "https://github.com/mdconaway/fastapi-cruddy-framework"
 repository = "https://github.com/mdconaway/fastapi-cruddy-framework"
 keywords = ["fastapi", "crud", "mvc", "orm", "ember", "sails", "json"]
```

### Comparing `fastapi_cruddy_framework-0.0.8/PKG-INFO` & `fastapi_cruddy_framework-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-cruddy-framework
-Version: 0.0.8
+Version: 0.0.9
 Summary: A holistic CRUD/MVC framework for FastAPI, with endpoint policies and relationships
 Home-page: https://github.com/mdconaway/fastapi-cruddy-framework
 Keywords: fastapi,crud,mvc,orm,ember,sails,json
 Author: mdconaway
 Author-email: mdconaway@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-cruddy-framework Version: 0.0.8 Summary: A
+Metadata-Version: 2.1 Name: fastapi-cruddy-framework Version: 0.0.9 Summary: A
 holistic CRUD/MVC framework for FastAPI, with endpoint policies and
 relationships Home-page: https://github.com/mdconaway/fastapi-cruddy-framework
 Keywords: fastapi,crud,mvc,orm,ember,sails,json Author: mdconaway Author-email:
 mdconaway@users.noreply.github.com Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

