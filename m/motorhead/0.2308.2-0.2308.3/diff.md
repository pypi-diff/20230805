# Comparing `tmp/motorhead-0.2308.2.tar.gz` & `tmp/motorhead-0.2308.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motorhead-0.2308.2.tar", max compression
+gzip compressed data, was "motorhead-0.2308.3.tar", max compression
```

## Comparing `motorhead-0.2308.2.tar` & `motorhead-0.2308.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1067 2023-07-29 09:07:27.173242 motorhead-0.2308.2/LICENSE
--rw-r--r--   0        0        0     2941 2023-08-03 21:46:21.765328 motorhead-0.2308.2/README.md
--rw-r--r--   0        0        0     2038 2023-08-03 18:52:22.265079 motorhead-0.2308.2/motorhead/__init__.py
--rw-r--r--   0        0        0     3139 2023-07-30 12:39:04.829152 motorhead-0.2308.2/motorhead/bound_method_wrapper.py
--rw-r--r--   0        0        0     2631 2023-07-31 20:57:59.093587 motorhead-0.2308.2/motorhead/delete_rule.py
--rw-r--r--   0        0        0      259 2023-07-29 20:05:22.252317 motorhead-0.2308.2/motorhead/model/__init__.py
--rw-r--r--   0        0        0      133 2023-07-29 20:05:03.623604 motorhead-0.2308.2/motorhead/model/deleteresultmodel.py
--rw-r--r--   0        0        0      716 2023-07-29 20:03:57.265257 motorhead-0.2308.2/motorhead/model/document.py
--rw-r--r--   0        0        0     1677 2023-07-29 22:35:05.132760 motorhead-0.2308.2/motorhead/model/objectid.py
--rw-r--r--   0        0        0      877 2023-07-29 21:11:20.073753 motorhead-0.2308.2/motorhead/model/utcdatetime.py
--rw-r--r--   0        0        0     4900 2023-08-03 21:00:48.282511 motorhead-0.2308.2/motorhead/operator.py
--rw-r--r--   0        0        0        0 2023-07-29 09:07:27.173242 motorhead-0.2308.2/motorhead/py.typed
--rw-r--r--   0        0        0     6849 2023-08-03 20:55:30.603143 motorhead-0.2308.2/motorhead/query.py
--rw-r--r--   0        0        0    28508 2023-08-03 18:51:22.611747 motorhead-0.2308.2/motorhead/service.py
--rw-r--r--   0        0        0     6022 2023-08-03 18:52:05.408756 motorhead-0.2308.2/motorhead/typing.py
--rw-r--r--   0        0        0     1678 2023-08-03 18:51:37.484136 motorhead-0.2308.2/motorhead/validator.py
--rw-r--r--   0        0        0     2750 2023-08-03 21:48:32.459975 motorhead-0.2308.2/pyproject.toml
--rw-r--r--   0        0        0     3411 1970-01-01 00:00:00.000000 motorhead-0.2308.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-29 09:07:27.173242 motorhead-0.2308.3/LICENSE
+-rw-r--r--   0        0        0     3010 2023-08-04 20:45:36.374798 motorhead-0.2308.3/README.md
+-rw-r--r--   0        0        0     2096 2023-08-05 07:43:01.936504 motorhead-0.2308.3/motorhead/__init__.py
+-rw-r--r--   0        0        0     3139 2023-07-30 12:39:04.829152 motorhead-0.2308.3/motorhead/bound_method_wrapper.py
+-rw-r--r--   0        0        0     2631 2023-07-31 20:57:59.093587 motorhead-0.2308.3/motorhead/delete_rule.py
+-rw-r--r--   0        0        0      259 2023-07-29 20:05:22.252317 motorhead-0.2308.3/motorhead/model/__init__.py
+-rw-r--r--   0        0        0      133 2023-07-29 20:05:03.623604 motorhead-0.2308.3/motorhead/model/deleteresultmodel.py
+-rw-r--r--   0        0        0      716 2023-07-29 20:03:57.265257 motorhead-0.2308.3/motorhead/model/document.py
+-rw-r--r--   0        0        0     1677 2023-07-29 22:35:05.132760 motorhead-0.2308.3/motorhead/model/objectid.py
+-rw-r--r--   0        0        0      877 2023-07-29 21:11:20.073753 motorhead-0.2308.3/motorhead/model/utcdatetime.py
+-rw-r--r--   0        0        0     4900 2023-08-03 21:00:48.282511 motorhead-0.2308.3/motorhead/operator.py
+-rw-r--r--   0        0        0        0 2023-07-29 09:07:27.173242 motorhead-0.2308.3/motorhead/py.typed
+-rw-r--r--   0        0        0     6849 2023-08-03 20:55:30.603143 motorhead-0.2308.3/motorhead/query.py
+-rw-r--r--   0        0        0    30486 2023-08-05 08:23:16.647640 motorhead-0.2308.3/motorhead/service.py
+-rw-r--r--   0        0        0     6022 2023-08-03 18:52:05.408756 motorhead-0.2308.3/motorhead/typing.py
+-rw-r--r--   0        0        0     1678 2023-08-03 18:51:37.484136 motorhead-0.2308.3/motorhead/validator.py
+-rw-r--r--   0        0        0     2818 2023-08-05 11:33:40.609354 motorhead-0.2308.3/pyproject.toml
+-rw-r--r--   0        0        0     3480 1970-01-01 00:00:00.000000 motorhead-0.2308.3/PKG-INFO
```

### Comparing `motorhead-0.2308.2/LICENSE` & `motorhead-0.2308.3/LICENSE`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.2/README.md` & `motorhead-0.2308.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 ## Requirements
 
 The project depends on `motor` (the official asyncio MongoDB driver, which is built on top of `pymongo` and `bson`) and `pydantic` v2+.
 
 ## Development
 
-Use `black` for code formatting, `mypy` for static code analysis, and `ruff` for linting.
+Use `black` for code formatting, `mypy` for static code analysis, `ruff` for linting, and `pytest` (with `pytest-asyncio` and `pytest-docker`) an for testing.
 
 The documentation is built with `mkdocs-material` and `mkdocstrings`.
 
 ## Contributing
 
 All contributions are welcome.
```

### Comparing `motorhead-0.2308.2/motorhead/__init__.py` & `motorhead-0.2308.3/motorhead/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from .query import Field as Field
 from .query import Q as Q
 from .query import Query as Query
 from .query import Queryable as Queryable
 from .service import DeleteResult as DeleteResult
 from .service import InsertOneResult as InsertOneResult
 from .service import Service as Service
+from .service import ServiceException as ServiceException
 from .service import UpdateResult as UpdateResult
 from .typing import AgnosticClient as AgnosticClient
 from .typing import AgnosticCollection as AgnosticCollection
 from .typing import AgnosticDatabase as AgnosticDatabase
 from .typing import Clause as Clause
 from .typing import ClauseOrMongoQuery as ClauseOrMongoQuery
 from .typing import ClauseOrProjecttion as ClauseOrProjecttion
```

### Comparing `motorhead-0.2308.2/motorhead/bound_method_wrapper.py` & `motorhead-0.2308.3/motorhead/bound_method_wrapper.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.2/motorhead/delete_rule.py` & `motorhead-0.2308.3/motorhead/delete_rule.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.2/motorhead/model/document.py` & `motorhead-0.2308.3/motorhead/model/document.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.2/motorhead/model/objectid.py` & `motorhead-0.2308.3/motorhead/model/objectid.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.2/motorhead/model/utcdatetime.py` & `motorhead-0.2308.3/motorhead/model/utcdatetime.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.2/motorhead/operator.py` & `motorhead-0.2308.3/motorhead/operator.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.2/motorhead/query.py` & `motorhead-0.2308.3/motorhead/query.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.2/motorhead/service.py` & `motorhead-0.2308.3/motorhead/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,22 @@
     "UpdateResult",
 )
 
 TInsert = TypeVar("TInsert", bound=BaseModel)
 TUpdate = TypeVar("TUpdate", bound=BaseModel)
 
 
+class ServiceException(Exception):
+    """
+    Base class for custom exceptions that can be raised by `Service`.
+    """
+
+    ...
+
+
 class Service(Generic[TInsert, TUpdate]):
     """
     Base service with typed utility methods for MongoDB (`motor` asyncio).
 
     The service provides a limited subset of `motor`'s capabilities.
 
     For undocumented keyword arguments, please see the `motor` or `pymongo` documentation.
@@ -497,35 +505,88 @@
             options: Query options, see the arguments of `collection.find()` for details.
 
         Returns:
             The queried document if such a document exists.
         """
         return await self.find_one({"_id": id}, projection, options=options)
 
+    async def create(self, data: TInsert, *, options: InsertOneOptions | None = None) -> dict[str, Any]:
+        """
+        Inserts the given data into the collection and immediately queries
+        and returns the created document.
+
+        Arguments:
+            data: The data to be inserted.
+            options: Insert options, see the arguments of `collection.insert_one()` for details.
+
+        Returns:
+            The result of the operation.
+
+        Raises:
+            ServiceException: If the service failed to access the newly created document.
+            Exception: If the data is invalid.
+        """
+        insert_result = await self.insert_one(data, options=options)
+        result = await self.get_by_id(insert_result.inserted_id)
+        if result is None:
+            raise ServiceException("Failed to query the inserted document by its ID.")
+
+        return result
+
     async def insert_one(
         self, data: TInsert, *, options: InsertOneOptions | None = None
     ) -> InsertOneResult:
         """
         Inserts the given data into the collection.
 
         Arguments:
             data: The data to be inserted.
             options: Insert options, see the arguments of `collection.insert_one()` for details.
 
         Returns:
             The result of the operation.
 
         Raises:
-            Exception: if the data is invalid.
+            Exception: If the data is invalid.
         """
         return await self.collection.insert_one(  # type: ignore[no-any-return]
             await self._prepare_for_insert(None, data),
             **(options or {}),
         )
 
+    async def update(
+        self,
+        id: ObjectId,
+        changes: TUpdate,
+        *,
+        options: UpdateOneOptions | None = None,
+    ) -> dict[str, Any]:
+        """
+        Updates the document with the given ID and immediately queries and returns
+        the updated document.
+
+        Arguments:
+            id: The ID of the document to update.
+            changes: The changes to make.
+            options: Update options, see the arguments of `collection.update_one()` for details.
+
+        Returns:
+            The updated document.
+
+        Raises:
+            ServiceException: If the service failed to query the updated document.
+            Exception: If the data is invalid.
+        """
+        await self.update_by_id(id, changes, options=options)
+        result = await self.get_by_id(id)
+        if result is None:
+            raise ServiceException("Failed to query the updated document by its ID.")
+
+        return result
+
     async def update_by_id(
         self,
         id: ObjectId,
         changes: TUpdate,
         *,
         options: UpdateOneOptions | None = None,
     ) -> UpdateResult:
@@ -537,15 +598,15 @@
             changes: The changes to make.
             options: Update options, see the arguments of `collection.update_one()` for details.
 
         Returns:
             The result of the operation.
 
         Raises:
-            Exception: if the data is invalid.
+            Exception: If the data is invalid.
         """
         return await self.update_one({"_id": id}, changes, options=options)
 
     async def update_many(
         self,
         query: ClauseOrMongoQuery | None,
         changes: TUpdate,
@@ -560,15 +621,15 @@
             changes: The changes to make.
             options: Update options, see the arguments of `collection.update_many()` for details.
 
         Returns:
             The result of the operation.
 
         Raises:
-            Exception: if the data is invalid.
+            Exception: If the data is invalid.
         """
         query = None if query is None else ensure_dict(query)
         return await self.collection.update_many(  # type: ignore[no-any-return]
             query,
             await self._prepare_for_update(query, changes),
             **(options or {}),
         )
@@ -588,15 +649,15 @@
             changes: The changes to make.
             options: Update options, see the arguments of `collection.update_one()` for details.
 
         Returns:
             The result of the operation.
 
         Raises:
-            Exception: if the data is invalid.
+            Exception: If the data is invalid.
         """
         query = None if query is None else ensure_dict(query)
         return await self.collection.update_one(  # type: ignore[no-any-return]
             query,
             await self._prepare_for_update(query, changes),
             **(options or {}),
         )
@@ -631,15 +692,15 @@
         Arguments:
             data: The data to be inserted.
 
         Returns:
             The MongoDB-compatible, insertable data.
 
         Raises:
-            Exception: if the data is invalid.
+            Exception: If the data is invalid.
         """
         return self._mongo_dump(data)
 
     async def _convert_for_update(self, data: TUpdate) -> UpdateObject | Sequence[UpdateObject]:
         """
         Converts the given piece of data into an update object.
 
@@ -648,15 +709,15 @@
         Arguments:
             data: The update data.
 
         Returns:
             The MongoDB-compatible update object.
 
         Raises:
-            Exception: if the data is invalid.
+            Exception: If the data is invalid.
         """
         return {"$set": self._mongo_dump(data)}
 
     def _create_collection(self) -> AgnosticCollection:
         """
         Creates a new `AgnosticCollection` instance for the service.
         """
@@ -739,15 +800,15 @@
             query: Query that matches the documents that will be updated.
             data: The data to be inserted.
 
         Returns:
             The MongoDB-compatible, insertable data.
 
         Raises:
-            Exception: if the data is invalid.
+            Exception: If the data is invalid.
         """
         await self._validate_insert(query, data)
         return await self._convert_for_insert(data)
 
     async def _prepare_for_update(
         self, query: ClauseOrMongoQuery | None, data: TUpdate
     ) -> UpdateObject | Sequence[UpdateObject]:
@@ -758,15 +819,15 @@
             query: Query that matches the documents that will be updated.
             data: The update data.
 
         Returns:
             The MongoDB-compatible update object.
 
         Raises:
-            Exception: if the data is invalid.
+            Exception: If the data is invalid.
         """
         await self._validate_update(query, data)
         return await self._convert_for_update(data)
 
     async def _validate_insert(self, query: ClauseOrMongoQuery | None, data: TInsert) -> None:
         """
         Validates the given piece of data for insertion by executing all insert validators.
```

### Comparing `motorhead-0.2308.2/motorhead/typing.py` & `motorhead-0.2308.3/motorhead/typing.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.2/motorhead/validator.py` & `motorhead-0.2308.3/motorhead/validator.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.2/pyproject.toml` & `motorhead-0.2308.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 [project.urls]
 Homepage = "https://github.com/volfpeter/motorhead"
 Documentation = "https://volfpeter.github.io/motorhead"
 
 [tool.poetry]
 name = "motorhead"
-version = "0.2308.2"
+version = "0.2308.3"
 description = "Async MongoDB with vanilla Pydantic v2+ - made easy."
 authors = ["Peter Volf <do.volfp@gmail.com>"]
 readme = "README.md"
 packages = [{include = "motorhead"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -45,27 +45,29 @@
 black = "^23.7.0"
 mkdocs-material = "^9.1.21"
 mkdocstrings = {extras = ["python"], version = "^0.22.0"}
 mypy = "^1.4.1"
 ruff = "^0.0.280"
 poethepoet = "^0.21.1"
 pytest = "^7.4.0"
+pytest-asyncio = "^0.21.1"
+pytest-docker = "^2.0.0"
 
 [tool.poetry.group.fastapi.dependencies]
 fastapi = {extras = ["all"], version = "^0.100.1"}
 
 [tool.black]
 line-length = 108
 
 [tool.mypy]
 strict = true
 show_error_codes = true
 
 [[tool.mypy.overrides]]
-module = "motor.core.*"
+module = ["motor.*", "pytest_docker.*"]
 ignore_missing_imports = true
 
 [tool.ruff]
 line-length = 108
 exclude = [
     ".git",
     ".mypy_cache",
```

### Comparing `motorhead-0.2308.2/PKG-INFO` & `motorhead-0.2308.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motorhead
-Version: 0.2308.2
+Version: 0.2308.3
 Summary: Async MongoDB with vanilla Pydantic v2+ - made easy.
 Author: Peter Volf
 Author-email: do.volfp@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -53,15 +53,15 @@
 
 ## Requirements
 
 The project depends on `motor` (the official asyncio MongoDB driver, which is built on top of `pymongo` and `bson`) and `pydantic` v2+.
 
 ## Development
 
-Use `black` for code formatting, `mypy` for static code analysis, and `ruff` for linting.
+Use `black` for code formatting, `mypy` for static code analysis, `ruff` for linting, and `pytest` (with `pytest-asyncio` and `pytest-docker`) an for testing.
 
 The documentation is built with `mkdocs-material` and `mkdocstrings`.
 
 ## Contributing
 
 All contributions are welcome.
```

