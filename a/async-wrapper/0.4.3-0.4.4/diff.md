# Comparing `tmp/async_wrapper-0.4.3.tar.gz` & `tmp/async_wrapper-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_wrapper-0.4.3.tar", max compression
+gzip compressed data, was "async_wrapper-0.4.4.tar", max compression
```

## Comparing `async_wrapper-0.4.3.tar` & `async_wrapper-0.4.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1070 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/LICENSE
--rw-r--r--   0        0        0     1681 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/README.md
--rw-r--r--   0        0        0     3493 2023-08-04 00:24:16.449975 async_wrapper-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      288 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/__init__.py
--rw-r--r--   0        0        0       63 2023-08-04 00:24:16.489975 async_wrapper-0.4.3/src/async_wrapper/_version.py
--rw-r--r--   0        0        0      157 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/convert/__init__.py
--rw-r--r--   0        0        0      595 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/convert/_async.py
--rw-r--r--   0        0        0     1186 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/convert/_sync.py
--rw-r--r--   0        0        0     1261 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/convert/abc.py
--rw-r--r--   0        0        0     1101 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/convert/main.py
--rw-r--r--   0        0        0      551 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/exception.py
--rw-r--r--   0        0        0        0 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/py.typed
--rw-r--r--   0        0        0      151 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/task_group/__init__.py
--rw-r--r--   0        0        0     5976 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/task_group/task_group.py
--rw-r--r--   0        0        0      806 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/task_group/value.py
--rw-r--r--   0        0        0      101 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/utils/__init__.py
--rw-r--r--   0        0        0     7701 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/utils/queue.py
--rw-r--r--   0        0        0     2593 1970-01-01 00:00:00.000000 async_wrapper-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-04 11:43:37.356345 async_wrapper-0.4.4/LICENSE
+-rw-r--r--   0        0        0     1681 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/README.md
+-rw-r--r--   0        0        0     3493 2023-08-04 11:43:56.468479 async_wrapper-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      391 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/__init__.py
+-rw-r--r--   0        0        0       63 2023-08-04 11:43:56.520480 async_wrapper-0.4.4/src/async_wrapper/_version.py
+-rw-r--r--   0        0        0      157 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/convert/__init__.py
+-rw-r--r--   0        0        0      595 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/convert/_async.py
+-rw-r--r--   0        0        0     1186 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/convert/_sync.py
+-rw-r--r--   0        0        0     1261 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/convert/abc.py
+-rw-r--r--   0        0        0     1101 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/convert/main.py
+-rw-r--r--   0        0        0      551 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/exception.py
+-rw-r--r--   0        0        0        0 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/py.typed
+-rw-r--r--   0        0        0     8007 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/queue.py
+-rw-r--r--   0        0        0      151 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/task_group/__init__.py
+-rw-r--r--   0        0        0     5976 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/task_group/task_group.py
+-rw-r--r--   0        0        0      806 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/task_group/value.py
+-rw-r--r--   0        0        0     4267 2023-08-04 11:43:37.360345 async_wrapper-0.4.4/src/async_wrapper/wait.py
+-rw-r--r--   0        0        0     2593 1970-01-01 00:00:00.000000 async_wrapper-0.4.4/PKG-INFO
```

### Comparing `async_wrapper-0.4.3/LICENSE` & `async_wrapper-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.3/README.md` & `async_wrapper-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.3/pyproject.toml` & `async_wrapper-0.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-wrapper"
-version = "0.4.3"
+version = "0.4.4"
 description = "async wrapper"
 authors = ["phi <phi.friday@gmail.com>"]
 readme = "README.md"
 license = "MIT License"
 homepage = "https://github.com/phi-friday/async-wrapper"
 repository = "https://github.com/phi-friday/async-wrapper"
 packages = [{ include = "async_wrapper", from = 'src' }]
```

### Comparing `async_wrapper-0.4.3/src/async_wrapper/convert/_async.py` & `async_wrapper-0.4.4/src/async_wrapper/convert/_async.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.3/src/async_wrapper/convert/_sync.py` & `async_wrapper-0.4.4/src/async_wrapper/convert/_sync.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.3/src/async_wrapper/convert/abc.py` & `async_wrapper-0.4.4/src/async_wrapper/convert/abc.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.3/src/async_wrapper/convert/main.py` & `async_wrapper-0.4.4/src/async_wrapper/convert/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.3/src/async_wrapper/exception.py` & `async_wrapper-0.4.4/src/async_wrapper/exception.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.3/src/async_wrapper/task_group/task_group.py` & `async_wrapper-0.4.4/src/async_wrapper/task_group/task_group.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.3/src/async_wrapper/task_group/value.py` & `async_wrapper-0.4.4/src/async_wrapper/task_group/value.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.3/src/async_wrapper/utils/queue.py` & `async_wrapper-0.4.4/src/async_wrapper/queue.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,38 +26,38 @@
 
 ValueT = TypeVar("ValueT")
 
 
 class Queue(Generic[ValueT]):
     """obtained from asyncio.Queue"""
 
-    _setter: MemoryObjectSendStream[ValueT]
+    _putter: MemoryObjectSendStream[ValueT]
     _getter: MemoryObjectReceiveStream[ValueT]
 
     def __init__(
         self,
         max_size: float | None = None,
         stream: tuple[MemoryObjectSendStream[ValueT], MemoryObjectReceiveStream[ValueT]]
         | None = None,
     ) -> None:
         if stream is None:
-            self._setter, self._getter = create_memory_object_stream(
+            self._putter, self._getter = create_memory_object_stream(
                 max_buffer_size=max_size or math.inf,
             )
         else:
-            setter, getter = stream
-            if setter._closed or getter._closed:  # noqa: SLF001
-                raise QueueBrokenError("setter or getter is closed")
-            if setter._state.buffer is not getter._state.buffer:  # noqa: SLF001
-                raise QueueBrokenError("setter and getter has diff buffer.")
-            self._setter, self._getter = stream
+            putter, getter = stream
+            if putter._closed or getter._closed:  # noqa: SLF001
+                raise QueueBrokenError("putter or getter is closed")
+            if putter._state.buffer is not getter._state.buffer:  # noqa: SLF001
+                raise QueueBrokenError("putter and getter has diff buffer.")
+            self._putter, self._getter = stream
 
     @property
     def _closed(self) -> bool:
-        return self._setter._closed or self._getter._closed  # noqa: SLF001
+        return self._putter._closed or self._getter._closed  # noqa: SLF001
 
     def qsize(self) -> int:
         """number of items in the queue."""
         return len(self._getter._state.buffer)  # noqa: SLF001
 
     @property
     def maxsize(self) -> float:
@@ -97,42 +97,50 @@
             await self._aput(value)
 
     async def _aget(self) -> ValueT:
         """remove and return an item from the queue."""
         try:
             return await self._getter.receive()
         except WouldBlock as exc:
-            raise QueueEmptyError from exc
+            if self.empty():
+                raise QueueEmptyError from exc
+            raise QueueBrokenError from exc
         except (ClosedResourceError, BrokenResourceError) as exc:
             raise QueueBrokenError from exc
 
     async def _aput(self, value: ValueT) -> None:
         """put an item into the queue."""
         try:
-            await self._setter.send(value)
+            await self._putter.send(value)
         except WouldBlock as exc:
-            raise QueueFullError from exc
+            if self.full():
+                raise QueueFullError from exc
+            raise QueueBrokenError from exc
         except (ClosedResourceError, BrokenResourceError) as exc:
             raise QueueBrokenError from exc
 
     def get(self) -> ValueT:
         """remove and return an item from the queue without blocking."""
         try:
             return self._getter.receive_nowait()
         except WouldBlock as exc:
-            raise QueueEmptyError from exc
+            if self.empty():
+                raise QueueEmptyError from exc
+            raise QueueBrokenError from exc
         except (ClosedResourceError, BrokenResourceError) as exc:
             raise QueueBrokenError from exc
 
     def put(self, value: ValueT) -> None:
         """put an item into the queue without blocking."""
         try:
-            self._setter.send_nowait(value)
+            self._putter.send_nowait(value)
         except WouldBlock as exc:
-            raise QueueFullError from exc
+            if self.full():
+                raise QueueFullError from exc
+            raise QueueBrokenError from exc
         except (ClosedResourceError, BrokenResourceError) as exc:
             raise QueueBrokenError from exc
 
     async def aclose(self) -> None:
         """close the stream as async"""
         try:
             await self._aclose()
@@ -153,45 +161,45 @@
         except (ClosedResourceError, BrokenResourceError) as exc:
             raise QueueBrokenError from exc
 
     async def _aclose(self) -> None:
         """close the stream as async"""
         async with create_task_group() as task_group:
             task_group.start_soon(self._getter.aclose)
-            task_group.start_soon(self._setter.aclose)
+            task_group.start_soon(self._putter.aclose)
 
     def _close(self) -> None:
         """close the stream as sync"""
         self._getter.close()
-        self._setter.close()
+        self._putter.close()
 
-    def clone(self, *, setter: bool = False, getter: bool = False) -> Queue[ValueT]:
+    def clone(self, *, putter: bool = False, getter: bool = False) -> Queue[ValueT]:
         """create clone of this queue.
 
         Args:
-            setter: if true, clone setter. Defaults to False.
+            putter: if true, clone putter. Defaults to False.
             getter: if true, clone getter. Defaults to False.
 
         Returns:
             clone
         """
         try:
-            return self._clone(setter=setter, getter=getter)
+            return self._clone(putter=putter, getter=getter)
         except (ClosedResourceError, BrokenResourceError) as exc:
             raise QueueBrokenError from exc
 
-    def _clone(self, *, setter: bool, getter: bool) -> Queue[ValueT]:
+    def _clone(self, *, putter: bool, getter: bool) -> Queue[ValueT]:
         """create clone of this queue"""
         if self._closed:
             raise QueueBrokenError("the queue is already closed")
-        if not setter and not getter:
-            raise ValueError("setter and getter are None.")
-        _setter = self._setter.clone() if setter else self._setter
+        if not putter and not getter:
+            raise ValueError("putter and getter are None.")
+        _putter = self._putter.clone() if putter else self._putter
         _getter = self._getter.clone() if getter else self._getter
-        return Queue(stream=(_setter, _getter))
+        return Queue(stream=(_putter, _getter))
 
     def statistics(self) -> MemoryObjectStreamStatistics:
         """return statstics from stream"""
         return self._getter._state.statistics()  # noqa: SLF001
 
     def __enter__(self) -> Self:
         return self
```

### Comparing `async_wrapper-0.4.3/PKG-INFO` & `async_wrapper-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-wrapper
-Version: 0.4.3
+Version: 0.4.4
 Summary: async wrapper
 Home-page: https://github.com/phi-friday/async-wrapper
 License: MIT
 Author: phi
 Author-email: phi.friday@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

