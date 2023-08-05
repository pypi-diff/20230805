# Comparing `tmp/async_wrapper-0.4.5.tar.gz` & `tmp/async_wrapper-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_wrapper-0.4.5.tar", max compression
+gzip compressed data, was "async_wrapper-0.4.6.tar", max compression
```

## Comparing `async_wrapper-0.4.5.tar` & `async_wrapper-0.4.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1070 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/LICENSE
--rw-r--r--   0        0        0     1681 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/README.md
--rw-r--r--   0        0        0     3449 2023-08-05 08:43:52.787309 async_wrapper-0.4.5/pyproject.toml
--rw-r--r--   0        0        0      419 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/__init__.py
--rw-r--r--   0        0        0       63 2023-08-05 08:43:52.819309 async_wrapper-0.4.5/src/async_wrapper/_version.py
--rw-r--r--   0        0        0      157 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/convert/__init__.py
--rw-r--r--   0        0        0      595 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/convert/_async.py
--rw-r--r--   0        0        0     1186 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/convert/_sync.py
--rw-r--r--   0        0        0     1407 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/convert/abc.py
--rw-r--r--   0        0        0     1101 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/convert/main.py
--rw-r--r--   0        0        0      551 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/exception.py
--rw-r--r--   0        0        0        0 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/py.typed
--rw-r--r--   0        0        0     8007 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/queue.py
--rw-r--r--   0        0        0      151 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/task_group/__init__.py
--rw-r--r--   0        0        0     6794 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/task_group/task_group.py
--rw-r--r--   0        0        0      837 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/task_group/value.py
--rw-r--r--   0        0        0    10749 2023-08-05 08:43:41.379218 async_wrapper-0.4.5/src/async_wrapper/wait.py
--rw-r--r--   0        0        0     2593 1970-01-01 00:00:00.000000 async_wrapper-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-05 12:04:15.257181 async_wrapper-0.4.6/LICENSE
+-rw-r--r--   0        0        0     1681 2023-08-05 12:04:15.257181 async_wrapper-0.4.6/README.md
+-rw-r--r--   0        0        0     3467 2023-08-05 12:04:31.509246 async_wrapper-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0      479 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/__init__.py
+-rw-r--r--   0        0        0       63 2023-08-05 12:04:31.549247 async_wrapper-0.4.6/src/async_wrapper/_version.py
+-rw-r--r--   0        0        0      157 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/convert/__init__.py
+-rw-r--r--   0        0        0      595 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/convert/_async.py
+-rw-r--r--   0        0        0     2462 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/convert/_sync.py
+-rw-r--r--   0        0        0     1407 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/convert/abc.py
+-rw-r--r--   0        0        0     1101 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/convert/main.py
+-rw-r--r--   0        0        0      551 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/exception.py
+-rw-r--r--   0        0        0        0 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/py.typed
+-rw-r--r--   0        0        0     8007 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/queue.py
+-rw-r--r--   0        0        0      207 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/task_group/__init__.py
+-rw-r--r--   0        0        0     6984 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/task_group/task_group.py
+-rw-r--r--   0        0        0      837 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/task_group/value.py
+-rw-r--r--   0        0        0    10697 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/wait.py
+-rw-r--r--   0        0        0     2626 1970-01-01 00:00:00.000000 async_wrapper-0.4.6/PKG-INFO
```

### Comparing `async_wrapper-0.4.5/LICENSE` & `async_wrapper-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.5/README.md` & `async_wrapper-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.5/pyproject.toml` & `async_wrapper-0.4.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "async-wrapper"
-version = "0.4.5"
+version = "0.4.6"
 description = "async wrapper"
 authors = ["phi <phi.friday@gmail.com>"]
 readme = "README.md"
 license = "MIT License"
 homepage = "https://github.com/phi-friday/async-wrapper"
 repository = "https://github.com/phi-friday/async-wrapper"
 packages = [{ include = "async_wrapper", from = 'src' }]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 typing-extensions = "^4.6.3"
 anyio = "^3.7.0"
+sniffio = "1.3.0"
 uvloop = { version = "^0.17.0", optional = true, markers = "platform_system != 'Windows'" }
 exceptiongroup = { version = "^1.1.2", markers = "python_version < '3.11'" }
 
 [tool.poetry.extras]
 uvloop = ['uvloop']
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `async_wrapper-0.4.5/src/async_wrapper/convert/_async.py` & `async_wrapper-0.4.6/src/async_wrapper/convert/_async.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.5/src/async_wrapper/convert/_sync.py` & `async_wrapper-0.4.6/src/async_wrapper/convert/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 from __future__ import annotations
 
-from concurrent.futures import ThreadPoolExecutor, wait
-from functools import partial, wraps
-from typing import Awaitable, Callable, TypeVar
+from inspect import iscoroutinefunction
+from typing import Any, Callable, Coroutine, TypeVar, overload
 
-import anyio
 from typing_extensions import ParamSpec
 
-ValueT_co = TypeVar("ValueT_co", covariant=True)
-ParamT = ParamSpec("ParamT")
-
-__all__ = ["async_to_sync"]
-
-
-def async_to_sync(
-    func: Callable[ParamT, Awaitable[ValueT_co]],
-) -> Callable[ParamT, ValueT_co]:
-    sync_func = _as_sync(func)
+from ._async import sync_to_async
+from ._sync import async_to_sync
 
-    @wraps(func)
-    def inner(*args: ParamT.args, **kwargs: ParamT.kwargs) -> ValueT_co:
-        with ThreadPoolExecutor(1) as pool:
-            future = pool.submit(sync_func, *args, **kwargs)
-            wait([future])
-            return future.result()
-
-    return inner
-
-
-def _as_sync(
-    func: Callable[ParamT, Awaitable[ValueT_co]],
-) -> Callable[ParamT, ValueT_co]:
-    @wraps(func)
-    def inner(*args: ParamT.args, **kwargs: ParamT.kwargs) -> ValueT_co:
-        return _run(func, *args, **kwargs)
+ValueT = TypeVar("ValueT")
+ParamT = ParamSpec("ParamT")
 
-    return inner
+__all__ = ["toggle_func", "async_to_sync", "sync_to_async"]
 
 
-def _run(
-    func: Callable[ParamT, Awaitable[ValueT_co]],
-    *args: ParamT.args,
-    **kwargs: ParamT.kwargs,
-) -> ValueT_co:
-    return anyio.run(partial(func, *args, **kwargs))
+@overload
+def toggle_func(
+    func: Callable[ParamT, Coroutine[Any, Any, ValueT]],
+) -> Callable[ParamT, ValueT]:
+    ...
+
+
+@overload
+def toggle_func(
+    func: Callable[ParamT, ValueT],
+) -> Callable[ParamT, Coroutine[Any, Any, ValueT]]:
+    ...
+
+
+def toggle_func(
+    func: Callable[ParamT, ValueT] | Callable[ParamT, Coroutine[Any, Any, ValueT]],
+) -> Callable[ParamT, ValueT] | Callable[ParamT, Coroutine[Any, Any, ValueT]]:
+    """sync to async, async to sync
+
+    Args:
+        func: sync or async func
+        backend: sync or async backend. Defaults to None.
+
+    Returns:
+        async or sync func
+    """
+    if iscoroutinefunction(func):
+        return async_to_sync(func)
+    return sync_to_async(func)  # type: ignore
```

### Comparing `async_wrapper-0.4.5/src/async_wrapper/convert/abc.py` & `async_wrapper-0.4.6/src/async_wrapper/convert/abc.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.5/src/async_wrapper/exception.py` & `async_wrapper-0.4.6/src/async_wrapper/exception.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.5/src/async_wrapper/queue.py` & `async_wrapper-0.4.6/src/async_wrapper/queue.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.5/src/async_wrapper/task_group/task_group.py` & `async_wrapper-0.4.6/src/async_wrapper/task_group/task_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from contextlib import AsyncExitStack
 from functools import partial, wraps
 from typing import TYPE_CHECKING, Any, Awaitable, Callable, Coroutine, Generic, TypeVar
 
+from anyio import create_task_group as _create_task_group
 from anyio.abc import TaskGroup as _TaskGroup
 from typing_extensions import Concatenate, ParamSpec, Self, override
 
 from async_wrapper.task_group.value import SoonValue
 
 if TYPE_CHECKING:
     from types import TracebackType
@@ -15,14 +16,16 @@
     from anyio.abc import CancelScope, CapacityLimiter, Lock, Semaphore
 
 ValueT_co = TypeVar("ValueT_co", covariant=True)
 OtherValueT_co = TypeVar("OtherValueT_co", covariant=True)
 ParamT = ParamSpec("ParamT")
 OtherParamT = ParamSpec("OtherParamT")
 
+__all__ = ["TaskGroupWrapper", "create_task_group_wrapper"]
+
 
 class TaskGroupWrapper(_TaskGroup):
     """wrap anyio.TaskGroup
 
     how to use:
     >>> import anyio
     >>>
@@ -72,15 +75,15 @@
     @override
     def start_soon(
         self,
         func: Callable[..., Awaitable[Any]],
         *args: Any,
         name: Any = None,
     ) -> None:
-        return self._task_group.start_soon(_as_coro, func, *args, name=name)
+        return self._task_group.start_soon(func, *args, name=name)
 
     @override
     async def start(
         self,
         func: Callable[..., Awaitable[Any]],
         *args: Any,
         name: Any = None,
@@ -99,15 +102,18 @@
     async def __aexit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> bool | None:
         if self._active_self:
-            return await self._task_group.__aexit__(exc_type, exc_val, exc_tb)
+            try:
+                return await self._task_group.__aexit__(exc_type, exc_val, exc_tb)
+            finally:
+                self._active_self = False
         return None
 
     def wrap(
         self,
         func: Callable[ParamT, Awaitable[ValueT_co]],
         semaphore: Semaphore | None = None,
         limiter: CapacityLimiter | None = None,
@@ -144,15 +150,15 @@
         self.task_group = task_group
         self.semaphore = semaphore
         self.limiter = limiter
         self.lock = lock
 
         self._wrapped = None
 
-    def __call__(  # noqa: D102
+    def __call__(
         self,
         *args: ParamT.args,
         **kwargs: ParamT.kwargs,
     ) -> SoonValue[ValueT_co]:
         value: SoonValue[ValueT_co] = SoonValue()
         wrapped = partial(self.wrapped, value, *args, **kwargs)
         self.task_group.start_soon(wrapped)
@@ -224,18 +230,19 @@
             self.task_group,
             semaphore=semaphore,
             limiter=limiter,
             lock=lock,
         )
 
 
-async def _as_coro(
-    func: Callable[ParamT, Awaitable[ValueT_co]],
-    *args: ParamT.args,
-    **kwargs: ParamT.kwargs,
-) -> ValueT_co:
-    return await func(*args, **kwargs)
+def create_task_group_wrapper() -> TaskGroupWrapper:
+    """create new task group wrapper
+
+    Returns:
+        task group wrapper
+    """
+    return TaskGroupWrapper(_create_task_group())
 
 
 def _is_active(task_group: _TaskGroup) -> bool:
     # trio, asyncio
     return task_group._active  # type: ignore # noqa: SLF001
```

### Comparing `async_wrapper-0.4.5/src/async_wrapper/task_group/value.py` & `async_wrapper-0.4.6/src/async_wrapper/task_group/value.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.5/src/async_wrapper/wait.py` & `async_wrapper-0.4.6/src/async_wrapper/wait.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 from __future__ import annotations
 
-import sys
 from functools import partial
 from threading import local
 from typing import TYPE_CHECKING, Any, Awaitable, Callable, Iterable, TypeVar
 
 from anyio import EndOfStream, Event, create_memory_object_stream, create_task_group
 from typing_extensions import ParamSpec, Self, override
 
 from async_wrapper.exception import PendingError
 
-if sys.version_info < (3, 11):
-    pass
-
 if TYPE_CHECKING:
     from types import TracebackType
 
     from anyio import EventStatistics
     from anyio.abc import CancelScope, TaskGroup
     from anyio.streams.memory import MemoryObjectReceiveStream, MemoryObjectSendStream
```

### Comparing `async_wrapper-0.4.5/PKG-INFO` & `async_wrapper-0.4.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-wrapper
-Version: 0.4.5
+Version: 0.4.6
 Summary: async wrapper
 Home-page: https://github.com/phi-friday/async-wrapper
 License: MIT
 Author: phi
 Author-email: phi.friday@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: uvloop
 Requires-Dist: anyio (>=3.7.0,<4.0.0)
 Requires-Dist: exceptiongroup (>=1.1.2,<2.0.0) ; python_version < "3.11"
+Requires-Dist: sniffio (==1.3.0)
 Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
 Requires-Dist: uvloop (>=0.17.0,<0.18.0) ; (platform_system != "Windows") and (extra == "uvloop")
 Project-URL: Repository, https://github.com/phi-friday/async-wrapper
 Description-Content-Type: text/markdown
 
 # async-wrapper
```

