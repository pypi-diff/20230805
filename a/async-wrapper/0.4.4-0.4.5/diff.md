# Comparing `tmp/async_wrapper-0.4.4.tar.gz` & `tmp/async_wrapper-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_wrapper-0.4.4.tar", max compression
+gzip compressed data, was "async_wrapper-0.4.5.tar", max compression
```

## Comparing `async_wrapper-0.4.4.tar` & `async_wrapper-0.4.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1070 2023-08-04 11:43:37.356345 async_wrapper-0.4.4/LICENSE
--rw-r--r--   0        0        0     1681 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/README.md
--rw-r--r--   0        0        0     3493 2023-08-04 11:43:56.468479 async_wrapper-0.4.4/pyproject.toml
--rw-r--r--   0        0        0      391 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/__init__.py
--rw-r--r--   0        0        0       63 2023-08-04 11:43:56.520480 async_wrapper-0.4.4/src/async_wrapper/_version.py
--rw-r--r--   0        0        0      157 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/convert/__init__.py
--rw-r--r--   0        0        0      595 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/convert/_async.py
--rw-r--r--   0        0        0     1186 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/convert/_sync.py
--rw-r--r--   0        0        0     1261 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/convert/abc.py
--rw-r--r--   0        0        0     1101 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/convert/main.py
--rw-r--r--   0        0        0      551 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/exception.py
--rw-r--r--   0        0        0        0 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/py.typed
--rw-r--r--   0        0        0     8007 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/queue.py
--rw-r--r--   0        0        0      151 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/task_group/__init__.py
--rw-r--r--   0        0        0     5976 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/task_group/task_group.py
--rw-r--r--   0        0        0      806 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/task_group/value.py
--rw-r--r--   0        0        0     4267 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/wait.py
--rw-r--r--   0        0        0     2593 1970-01-01 00:00:00.000000 async_wrapper-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/LICENSE
+-rw-r--r--   0        0        0     1681 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/README.md
+-rw-r--r--   0        0        0     3449 2023-08-05 08:43:52.787309 async_wrapper-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0      419 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/__init__.py
+-rw-r--r--   0        0        0       63 2023-08-05 08:43:52.819309 async_wrapper-0.4.5/src/async_wrapper/_version.py
+-rw-r--r--   0        0        0      157 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/convert/__init__.py
+-rw-r--r--   0        0        0      595 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/convert/_async.py
+-rw-r--r--   0        0        0     1186 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/convert/_sync.py
+-rw-r--r--   0        0        0     1407 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/convert/abc.py
+-rw-r--r--   0        0        0     1101 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/convert/main.py
+-rw-r--r--   0        0        0      551 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/exception.py
+-rw-r--r--   0        0        0        0 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/py.typed
+-rw-r--r--   0        0        0     8007 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/queue.py
+-rw-r--r--   0        0        0      151 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/task_group/__init__.py
+-rw-r--r--   0        0        0     6794 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/task_group/task_group.py
+-rw-r--r--   0        0        0      837 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/task_group/value.py
+-rw-r--r--   0        0        0    10749 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/wait.py
+-rw-r--r--   0        0        0     2593 1970-01-01 00:00:00.000000 async_wrapper-0.4.5/PKG-INFO
```

### Comparing `async_wrapper-0.4.4/LICENSE` & `async_wrapper-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.4/README.md` & `async_wrapper-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.4/pyproject.toml` & `async_wrapper-0.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-wrapper"
-version = "0.4.4"
+version = "0.4.5"
 description = "async wrapper"
 authors = ["phi <phi.friday@gmail.com>"]
 readme = "README.md"
 license = "MIT License"
 homepage = "https://github.com/phi-friday/async-wrapper"
 repository = "https://github.com/phi-friday/async-wrapper"
 packages = [{ include = "async_wrapper", from = 'src' }]
@@ -86,15 +86,14 @@
     "PGH003", # blanket-type-ignore
     "SIM117", # multiple-with-statements # python3.8
     "B905",   # zip-without-explicit-strict
     "PD010",  # use-of-dot-pivot-or-unstack
     "D105",   # undocumented-magic-method
     "TD",     # flake8-todos
     "FIX",    # flake8-fixme
-    "D101",   # "undocumented-public-class"
 ]
 
 [tool.ruff.per-file-ignores]
 "./tests/**/*.py" = [
     "TCH001",
     "TCH002",
     "TCH003",
```

### Comparing `async_wrapper-0.4.4/src/async_wrapper/convert/_async.py` & `async_wrapper-0.4.5/src/async_wrapper/convert/_async.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.4/src/async_wrapper/convert/_sync.py` & `async_wrapper-0.4.5/src/async_wrapper/convert/_sync.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.4/src/async_wrapper/convert/main.py` & `async_wrapper-0.4.5/src/async_wrapper/convert/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.4/src/async_wrapper/exception.py` & `async_wrapper-0.4.5/src/async_wrapper/exception.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.4/src/async_wrapper/queue.py` & `async_wrapper-0.4.5/src/async_wrapper/queue.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.4/src/async_wrapper/task_group/task_group.py` & `async_wrapper-0.4.5/src/async_wrapper/task_group/task_group.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,14 +17,44 @@
 ValueT_co = TypeVar("ValueT_co", covariant=True)
 OtherValueT_co = TypeVar("OtherValueT_co", covariant=True)
 ParamT = ParamSpec("ParamT")
 OtherParamT = ParamSpec("OtherParamT")
 
 
 class TaskGroupWrapper(_TaskGroup):
+    """wrap anyio.TaskGroup
+
+    how to use:
+    >>> import anyio
+    >>>
+    >>> from async_wrapper import TaskGroupWrapper
+    >>>
+    >>>
+    >>> async def test(x: int) -> int:
+    >>>     await anyio.sleep(0.1)
+    >>>     return x
+    >>>
+    >>>
+    >>> async def main() -> None:
+    >>>     async with anyio.create_task_group() as task_group:
+    >>>         async with TaskGroupWrapper(task_group) as tg:
+    >>>             func = tg.wrap(test)
+    >>>             soon_1 = func(1)
+    >>>             soon_2 = func(2)
+    >>>
+    >>>     assert soon_1.is_ready
+    >>>     assert soon_2.is_ready
+    >>>     assert soon_1.value == 1
+    >>>     assert soon_2.value == 2
+    >>>
+    >>>
+    >>> if __name__ == "__main__":
+    >>>     anyio.run(main)
+    """
+
     def __init__(self, task_group: _TaskGroup) -> None:
         self._task_group = task_group
         self._active_self = False
 
     @property
     @override
     def cancel_scope(self) -> CancelScope:
@@ -96,14 +126,16 @@
         Returns:
             wrapped func
         """
         return SoonWrapper(func, self, semaphore=semaphore, limiter=limiter, lock=lock)
 
 
 class SoonWrapper(Generic[ParamT, ValueT_co]):
+    """wrapped func using in TaskGroupWrapper"""
+
     def __init__(  # noqa: PLR0913
         self,
         func: Callable[ParamT, Awaitable[ValueT_co]],
         task_group: _TaskGroup,
         semaphore: Semaphore | None = None,
         limiter: CapacityLimiter | None = None,
         lock: Lock | None = None,
```

### Comparing `async_wrapper-0.4.4/src/async_wrapper/task_group/value.py` & `async_wrapper-0.4.5/src/async_wrapper/task_group/value.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 ValueT_co = TypeVar("ValueT_co", covariant=True)
 Pending = local()
 
 __all__ = ["SoonValue"]
 
 
 class SoonValue(Generic[ValueT_co]):
+    """will get value soon"""
+
     def __init__(self) -> None:
         self._value: ValueT_co | local = Pending
 
     def __repr__(self) -> str:
         status = "pending" if self._value is Pending else "done"
         return f"<SoonValue: status={status}>"
```

### Comparing `async_wrapper-0.4.4/PKG-INFO` & `async_wrapper-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-wrapper
-Version: 0.4.4
+Version: 0.4.5
 Summary: async wrapper
 Home-page: https://github.com/phi-friday/async-wrapper
 License: MIT
 Author: phi
 Author-email: phi.friday@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

