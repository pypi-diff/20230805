# Comparing `tmp/graia-broadcast-0.8.9.tar.gz` & `tmp/graia-broadcast-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graia-broadcast-0.8.9.tar", last modified: Mon Apr  5 04:18:33 2021, max compression
+gzip compressed data, was "graia-broadcast-0.9.0.tar", max compression
```

## Comparing `graia-broadcast-0.8.9.tar` & `graia-broadcast-0.9.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      578 2021-04-05 04:16:00.000000 graia-broadcast-0.8.9/pyproject.toml
--rw-r--r--   0        0        0    14051 2021-04-05 01:59:16.000000 graia-broadcast-0.8.9/src/graia/broadcast/__init__.py
--rw-r--r--   0        0        0        0 2020-10-17 09:30:46.000000 graia-broadcast-0.8.9/src/graia/broadcast/builtin/__init__.py
--rw-r--r--   0        0        0     2071 2021-03-21 04:01:24.000000 graia-broadcast-0.8.9/src/graia/broadcast/builtin/decorators.py
--rw-r--r--   0        0        0      642 2021-03-13 16:30:38.000000 graia-broadcast-0.8.9/src/graia/broadcast/builtin/event.py
--rw-r--r--   0        0        0     4780 2021-04-05 04:16:14.000000 graia-broadcast-0.8.9/src/graia/broadcast/builtin/factory.py
--rw-r--r--   0        0        0        0 2020-10-17 09:30:46.000000 graia-broadcast-0.8.9/src/graia/broadcast/entities/__init__.py
--rw-r--r--   0        0        0     1370 2021-03-13 19:04:42.000000 graia-broadcast-0.8.9/src/graia/broadcast/entities/context.py
--rw-r--r--   0        0        0      113 2021-03-21 03:40:32.000000 graia-broadcast-0.8.9/src/graia/broadcast/entities/decorator.py
--rw-r--r--   0        0        0     5737 2021-04-04 17:25:38.000000 graia-broadcast-0.8.9/src/graia/broadcast/entities/dispatcher.py
--rw-r--r--   0        0        0     1289 2020-12-20 08:03:58.000000 graia-broadcast-0.8.9/src/graia/broadcast/entities/event.py
--rw-r--r--   0        0        0     1021 2021-03-13 19:04:42.000000 graia-broadcast-0.8.9/src/graia/broadcast/entities/exectarget.py
--rw-r--r--   0        0        0      942 2021-02-05 04:37:40.000000 graia-broadcast-0.8.9/src/graia/broadcast/entities/listener.py
--rw-r--r--   0        0        0      406 2020-12-06 04:31:00.000000 graia-broadcast-0.8.9/src/graia/broadcast/entities/namespace.py
--rw-r--r--   0        0        0      926 2020-12-06 04:31:00.000000 graia-broadcast-0.8.9/src/graia/broadcast/entities/signatures/__init__.py
--rw-r--r--   0        0        0      510 2021-03-20 12:40:56.000000 graia-broadcast-0.8.9/src/graia/broadcast/entities/track_log.py
--rw-r--r--   0        0        0      565 2020-12-06 04:31:00.000000 graia-broadcast-0.8.9/src/graia/broadcast/exceptions.py
--rw-r--r--   0        0        0        0 2020-10-17 09:30:46.000000 graia-broadcast-0.8.9/src/graia/broadcast/interfaces/__init__.py
--rw-r--r--   0        0        0     1649 2021-03-13 19:04:42.000000 graia-broadcast-0.8.9/src/graia/broadcast/interfaces/decorator.py
--rw-r--r--   0        0        0    11862 2021-03-20 11:57:38.000000 graia-broadcast-0.8.9/src/graia/broadcast/interfaces/dispatcher.py
--rw-r--r--   0        0        0     4355 2021-02-05 04:37:32.000000 graia-broadcast-0.8.9/src/graia/broadcast/interrupt/__init__.py
--rw-r--r--   0        0        0     2464 2021-02-05 04:37:40.000000 graia-broadcast-0.8.9/src/graia/broadcast/interrupt/waiter.py
--rw-r--r--   0        0        0      134 2020-12-06 04:31:02.000000 graia-broadcast-0.8.9/src/graia/broadcast/priority.py
--rw-r--r--   0        0        0      404 2021-03-13 19:04:42.000000 graia-broadcast-0.8.9/src/graia/broadcast/typing.py
--rw-r--r--   0        0        0     5287 2021-03-13 19:04:42.000000 graia-broadcast-0.8.9/src/graia/broadcast/utilles.py
--rw-r--r--   0        0        0      924 2021-04-05 04:18:34.088955 graia-broadcast-0.8.9/setup.py
--rw-r--r--   0        0        0      614 2021-04-05 04:18:34.089955 graia-broadcast-0.8.9/PKG-INFO
+-rwxr-xr-x   0        0        0      553 2021-05-22 16:23:31.000000 graia-broadcast-0.9.0/pyproject.toml
+-rwxr-xr-x   0        0        0    14072 2021-05-22 14:52:49.000000 graia-broadcast-0.9.0/src/graia/broadcast/__init__.py
+-rwxr-xr-x   0        0        0        0 2020-10-17 09:30:46.000000 graia-broadcast-0.9.0/src/graia/broadcast/builtin/__init__.py
+-rwxr-xr-x   0        0        0     2071 2021-03-21 04:01:24.000000 graia-broadcast-0.9.0/src/graia/broadcast/builtin/decorators.py
+-rwxr-xr-x   0        0        0      651 2021-05-22 11:55:34.000000 graia-broadcast-0.9.0/src/graia/broadcast/builtin/event.py
+-rwxr-xr-x   0        0        0     5036 2021-04-05 05:39:34.000000 graia-broadcast-0.9.0/src/graia/broadcast/builtin/factory.py
+-rwxr-xr-x   0        0        0        0 2020-10-17 09:30:46.000000 graia-broadcast-0.9.0/src/graia/broadcast/entities/__init__.py
+-rwxr-xr-x   0        0        0     2265 2021-05-22 16:23:39.000000 graia-broadcast-0.9.0/src/graia/broadcast/entities/context.py
+-rwxr-xr-x   0        0        0      113 2021-03-21 03:40:32.000000 graia-broadcast-0.9.0/src/graia/broadcast/entities/decorator.py
+-rwxr-xr-x   0        0        0     5737 2021-05-22 13:36:18.000000 graia-broadcast-0.9.0/src/graia/broadcast/entities/dispatcher.py
+-rwxr-xr-x   0        0        0      727 2021-05-22 16:23:39.000000 graia-broadcast-0.9.0/src/graia/broadcast/entities/event.py
+-rwxr-xr-x   0        0        0      960 2021-05-22 16:23:39.000000 graia-broadcast-0.9.0/src/graia/broadcast/entities/exectarget.py
+-rwxr-xr-x   0        0        0      948 2021-05-22 16:23:39.000000 graia-broadcast-0.9.0/src/graia/broadcast/entities/listener.py
+-rwxr-xr-x   0        0        0      344 2021-05-22 16:23:39.000000 graia-broadcast-0.9.0/src/graia/broadcast/entities/namespace.py
+-rwxr-xr-x   0        0        0      844 2021-05-22 11:58:34.000000 graia-broadcast-0.9.0/src/graia/broadcast/entities/signatures/__init__.py
+-rwxr-xr-x   0        0        0      455 2021-05-22 16:14:31.000000 graia-broadcast-0.9.0/src/graia/broadcast/entities/track_log.py
+-rwxr-xr-x   0        0        0      565 2020-12-06 04:31:00.000000 graia-broadcast-0.9.0/src/graia/broadcast/exceptions.py
+-rwxr-xr-x   0        0        0        0 2020-10-17 09:30:46.000000 graia-broadcast-0.9.0/src/graia/broadcast/interfaces/__init__.py
+-rwxr-xr-x   0        0        0     1649 2021-03-13 19:04:42.000000 graia-broadcast-0.9.0/src/graia/broadcast/interfaces/decorator.py
+-rwxr-xr-x   0        0        0    11106 2021-05-22 16:23:39.000000 graia-broadcast-0.9.0/src/graia/broadcast/interfaces/dispatcher.py
+-rwxr-xr-x   0        0        0     3496 2021-05-22 16:23:39.000000 graia-broadcast-0.9.0/src/graia/broadcast/interrupt/__init__.py
+-rwxr-xr-x   0        0        0     2476 2021-05-22 11:55:34.000000 graia-broadcast-0.9.0/src/graia/broadcast/interrupt/waiter.py
+-rwxr-xr-x   0        0        0      134 2020-12-06 04:31:02.000000 graia-broadcast-0.9.0/src/graia/broadcast/priority.py
+-rwxr-xr-x   0        0        0      579 2021-05-22 15:11:56.000000 graia-broadcast-0.9.0/src/graia/broadcast/typing.py
+-rwxr-xr-x   0        0        0     4408 2021-05-22 16:23:39.000000 graia-broadcast-0.9.0/src/graia/broadcast/utilles.py
+-rw-r--r--   0        0        0      924 2021-05-22 16:23:53.258006 graia-broadcast-0.9.0/setup.py
+-rw-r--r--   0        0        0      614 2021-05-22 16:23:53.258413 graia-broadcast-0.9.0/PKG-INFO
```

### Comparing `graia-broadcast-0.8.9/src/graia/broadcast/__init__.py` & `graia-broadcast-0.9.0/src/graia/broadcast/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from .typing import T_Dispatcher
 
 from .entities.exectarget import ExecTarget
 
 from .interfaces.dispatcher import DispatcherInterface
 from .entities.decorator import Decorator
 from .entities.dispatcher import BaseDispatcher
-from .entities.event import BaseEvent
+from .entities.event import Dispatchable
 from .entities.listener import Listener
 from .entities.namespace import Namespace
 from .entities.signatures import Force, RemoveMe
 from .exceptions import (
     DisabledNamespace,
     ExecutionStop,
     ExistedNamespace,
@@ -91,38 +91,38 @@
             .filter(lambda x: not x.namespace.hide)  # filter for hide
             .filter(lambda x: not x.namespace.disabled)  # filter for disabled
             .filter(lambda x: event_class in x.listening_events)
             # .collect(list)  # collect to a whole list
         )
 
     async def layered_scheduler(
-        self, listener_generator: Generator[Listener, None, None], event: BaseEvent
+        self, listener_generator: Generator[Listener, None, None], event: Dispatchable
     ):
         grouped: Dict[int, List[Listener]] = group_dict(
             listener_generator, lambda x: x.priority
         )
         for _, current_group in sorted(grouped.items(), key=lambda x: x[0]):
             coros = [self.Executor(target=i, event=event) for i in current_group]
             done_tasks, _ = await asyncio.wait(coros)
             for task in done_tasks:
                 if task.exception().__class__ is PropagationCancelled:
                     break
 
     async def Executor(
         self,
         target: Union[Callable, ExecTarget],
-        event: BaseEvent,
+        event: Dispatchable,
         dispatchers: List[
             Union[
                 Type[BaseDispatcher],
                 Callable,
                 BaseDispatcher,
             ]
         ] = None,
-        post_exception_event: bool = False,
+        post_exception_event: bool = True,
         print_exception: bool = True,
         enableInternalAccess: bool = False,
     ):
         from .builtin.event import ExceptionThrowed
 
         is_exectarget = cached_isinstance(target, ExecTarget)
         is_listener = cached_isinstance(target, Listener)
@@ -131,15 +131,14 @@
             if target.namespace.disabled:
                 raise DisabledNamespace(
                     "catched a disabled namespace: {0}".format(target.namespace.name)
                 )
 
         target_callable = target.callable if is_exectarget else target
         parameter_compile_result = {}
-        complete_finished = False
 
         track_logs: TrackLog = TrackLog()
         async with self.dispatcher_interface.start_execution(
             event,
             [
                 *(dispatchers or []),
                 *(target.namespace.injected_dispatchers if is_listener else []),
@@ -195,28 +194,26 @@
                     ):
                         parameter_compile_result[
                             name
                         ] = await dii.lookup_param_without_log(
                             name, annotation, default, target.param_paths[name]
                         )
 
-                complete_finished = True
-
                 result = await run_always_await_safely(
                     target_callable, **parameter_compile_result
                 )
             except (ExecutionStop, PropagationCancelled):
                 raise
             except RequirementCrashed:
                 traceback.print_exc()
                 raise
             except Exception as e:
-                if print_exception:
+                if print_exception or event.__class__ is ExceptionThrowed:
                     traceback.print_exc()
-                if post_exception_event:
+                if post_exception_event and event.__class__ is not ExceptionThrowed:
                     self.postEvent(ExceptionThrowed(exception=e, event=event))
                 raise
             finally:
                 _, exception, tb = sys.exc_info()
                 await dii.exec_lifecycle("afterDispatch", exception, tb)
                 await dii.exec_lifecycle("afterTargetExec", exception, tb)
                 await dii.exec_lifecycle("afterExecution", exception, tb)
@@ -251,24 +248,24 @@
             if result.__class__ is RemoveMe:
                 if cached_isinstance(target, Listener):
                     if target in self.listeners:
                         self.listeners.pop(self.listeners.index(target))
 
             return result
 
-    def postEvent(self, event: BaseEvent):
+    def postEvent(self, event: Dispatchable):
         self.loop.create_task(
             self.layered_scheduler(
                 listener_generator=self.default_listener_generator(event.__class__),
                 event=event,
             )
         )
 
     @staticmethod
-    def event_class_generator(target=BaseEvent):
+    def event_class_generator(target=Dispatchable):
         for i in target.__subclasses__():
             yield i
             if i.__subclasses__():
                 yield from Broadcast.event_class_generator(i)
 
     @staticmethod
     def findEvent(name: str):
@@ -340,15 +337,15 @@
                 return i
 
     def removeListener(self, target):
         self.listeners.remove(target)
 
     def receiver(
         self,
-        event: Union[str, Type[BaseEvent]],
+        event: Union[str, Type[Dispatchable]],
         priority: int = 16,
         dispatchers: List[Type[BaseDispatcher]] = [],
         namespace: Namespace = None,
         headless_decorators: List[Decorator] = [],
         enable_internal_access: bool = False,
     ):
         if cached_isinstance(event, str):
```

### Comparing `graia-broadcast-0.8.9/src/graia/broadcast/builtin/decorators.py` & `graia-broadcast-0.9.0/src/graia/broadcast/builtin/decorators.py`

 * *Files identical despite different names*

### Comparing `graia-broadcast-0.8.9/src/graia/broadcast/builtin/event.py` & `graia-broadcast-0.9.0/src/graia/broadcast/builtin/event.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import TYPE_CHECKING
 from ..entities.dispatcher import BaseDispatcher
-from ..entities.event import BaseEvent
+from ..entities.event import Dispatchable
 
 if TYPE_CHECKING:
     from graia.broadcast.interfaces.dispatcher import DispatcherInterface
 
 
-class ExceptionThrowed(BaseEvent):
+class ExceptionThrowed(Dispatchable):
     exception: Exception
-    event: BaseEvent
+    event: Dispatchable
 
     class Dispatcher(BaseDispatcher):
         @staticmethod
         def catch(interface: "DispatcherInterface"):
             if interface.annotation == interface.event.exception.__class__:
                 return interface.event.exception
             if interface.name == "event":
```

### Comparing `graia-broadcast-0.8.9/src/graia/broadcast/builtin/factory.py` & `graia-broadcast-0.9.0/src/graia/broadcast/builtin/factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,36 +49,41 @@
     Union[None, Tuple[StatusCodeEnum, Union[ExcInfo]]],
 ]
 
 
 class DispatcherContextManager(BaseDispatcher):
     generator_factory: Callable[[Any], T_DispatcherContextManager]
     generator: T_DispatcherContextManager
+    ready: bool = False
 
     def __init__(self, generator_factory: Callable, args=None, kwargs=None) -> None:
         self.generator_factory = generator_factory
         self.args = args or ()
         self.kwargs = kwargs or {}
 
     def beforeExecution(self, interface: "DispatcherInterface"):
         self.generator = self.generator_factory(*self.args, **self.kwargs)
         next(self.generator)
         self.generator.send(interface)
+        self.ready = True
 
     def catch(self, interface: "DispatcherInterface"):
+        if not self.ready:
+            return
         status, value = self.generator.send((StatusCodeEnum.DISPATCHING, None))
         if status is ResponseCodeEnum.VALUE:
             return value
 
     def afterDispatch(
         self,
         interface: "DispatcherInterface",
         exception: Optional[Exception],
         tb: Optional[TracebackType],
     ):
+        self.ready = False
         try:
             if not tb:
                 self.generator.send((StatusCodeEnum.DISPATCH_COMPLETED, None))
             else:
                 self.generator.send(
                     (StatusCodeEnum.DISPATCH_EXCEPTION, ExcInfo(exception, tb))
                 )
@@ -101,36 +106,41 @@
         except StopIteration:
             pass
 
 
 class AsyncDispatcherContextManager(BaseDispatcher):
     generator_factory: Callable[[Any], T_AsyncDispatcherContextManager]
     generator: T_AsyncDispatcherContextManager
+    ready: bool = False
 
     def __init__(self, generator_factory: Callable, args=None, kwargs=None) -> None:
         self.generator_factory = generator_factory
         self.args = args or ()
         self.kwargs = kwargs or {}
 
     async def beforeExecution(self, interface: "DispatcherInterface"):
         self.generator = self.generator_factory(*self.args, **self.kwargs)
         await self.generator.__anext__()
         await self.generator.asend(interface)
+        self.ready = True
 
     async def catch(self, interface: "DispatcherInterface"):
+        if not self.ready:
+            return
         status, value = await self.generator.asend((StatusCodeEnum.DISPATCHING, None))
         if status is ResponseCodeEnum.VALUE:
             return value
 
     async def afterDispatch(
         self,
         interface: "DispatcherInterface",
         exception: Optional[Exception],
         tb: Optional[TracebackType],
     ):
+        self.ready = False
         try:
             if not tb:
                 await self.generator.asend((StatusCodeEnum.DISPATCH_COMPLETED, None))
             else:
                 await self.generator.asend(
                     (StatusCodeEnum.DISPATCH_EXCEPTION, ExcInfo(exception, tb))
                 )
```

### Comparing `graia-broadcast-0.8.9/src/graia/broadcast/entities/context.py` & `graia-broadcast-0.9.0/src/graia/broadcast/interfaces/decorator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,51 @@
-import itertools
+from typing import Any, Dict, TYPE_CHECKING
 
-from typing import Any, Callable, Dict, List
-from graia.broadcast.utilles import NestableIterable
+from graia.broadcast.entities.dispatcher import BaseDispatcher
 
-from ..typing import T_Dispatcher
-
-
-def path_generator_factory(iterable: List[List["T_Dispatcher"]], start: int):
-    return enumerate(list(itertools.chain(*iterable))[start:])
-
-
-class ExecutionContext:
-    event: "BaseEvent"
-    _index: int
-    lifecycle_refs: Dict[str, List[Callable]]
-    dispatchers: List[T_Dispatcher]
-
-    def __init__(self, dispatchers: List[T_Dispatcher], event: "BaseEvent") -> None:
-        self.event = event
-        self._index = 0
-        self.dispatchers = dispatchers
-
-        self.lifecycle_refs = {}
-
-
-class ParameterContext:
-    name: str
-    annotation: Any
-    default: Any
-
-    dispatchers: List[T_Dispatcher]
-
-    def __init__(self, name, annotation, default, dispatchers, using_path) -> None:
-        self.name = name
-        self.annotation = annotation
-        self.default = default
-        self.dispatchers = dispatchers
-        self.path = NestableIterable(using_path, path_generator_factory)
-
-    def __repr__(self) -> str:
-        return (
-            "<ParameterContext name={0} annotation={1} default={2} locald={3}".format(
-                self.name, self.annotation, self.default, self.dispatchers
-            )
-        )
-
-
-from .event import BaseEvent
+from ..entities.decorator import Decorator
+from ..entities.signatures import Force
+from ..utilles import (
+    run_always_await_safely,
+    cached_isinstance,
+)
+
+if TYPE_CHECKING:
+    from graia.broadcast.interfaces.dispatcher import DispatcherInterface
+
+
+class DecoratorInterface(BaseDispatcher):
+    """Graia Broadcast Control 内部机制 Decorate 的具体管理实现"""
+
+    dispatcher_interface: "DispatcherInterface"
+    local_storage: Dict[Any, Any] = {}
+    return_value: Any = None
+    default = None
+
+    def __init__(self, dispatcher_interface: "DispatcherInterface"):
+        self.dispatcher_interface = dispatcher_interface
+
+    @property
+    def name(self):
+        return self.dispatcher_interface.name
+
+    @property
+    def annotation(self):
+        return self.dispatcher_interface.annotation
+
+    @property
+    def event(self):
+        return self.dispatcher_interface.event
+
+    async def catch(self, interface: "DispatcherInterface"):
+        if cached_isinstance(interface.default, Decorator):
+            decorator: Decorator = interface.default
+            if not decorator.pre:
+                # 作为 装饰
+                self.return_value = await interface.lookup_param(
+                    interface.name, interface.annotation, None
+                )
+            try:
+                return Force(await run_always_await_safely(decorator.target, self))
+            finally:
+                if not decorator.pre:
+                    self.return_value = None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `graia-broadcast-0.8.9/src/graia/broadcast/entities/dispatcher.py` & `graia-broadcast-0.9.0/src/graia/broadcast/entities/dispatcher.py`

 * *Files identical despite different names*

### Comparing `graia-broadcast-0.8.9/src/graia/broadcast/entities/exectarget.py` & `graia-broadcast-0.9.0/src/graia/broadcast/entities/exectarget.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,30 @@
+import inspect
 from typing import Callable, Dict, List, Set
 
-from graia.broadcast.utilles import argument_signature
-
 from ..typing import T_Dispatcher
 from .decorator import Decorator
 
 
 class ExecTarget:
+    callable: Callable
+    inline_dispatchers: List[T_Dispatcher]
+    headless_decorators: List[Decorator]
+    enable_internal_access: bool = False
+
+    param_paths: Dict[str, List[List[T_Dispatcher]]]
+    maybe_failure: Set[str]
+
     def __init__(
         self,
         callable: Callable,
         inline_dispatchers: List[T_Dispatcher] = None,
         headless_decorators: List[Decorator] = None,
         enable_internal_access: bool = False,
-    ) -> None:
+    ):
         self.callable = callable
         self.inline_dispatchers = inline_dispatchers or []
         self.headless_decorators = headless_decorators or []
         self.enable_internal_access = enable_internal_access
 
         self.param_paths = {}
-        self.maybe_failure = set(name for name, _, _ in argument_signature(callable))
-
-    callable: Callable
-    inline_dispatchers: List[T_Dispatcher] = []
-    headless_decorators: List[Decorator] = []
-    enable_internal_access: bool = False
-
-    param_paths: Dict[str, List[List[T_Dispatcher]]]
-    maybe_failure: Set[str]
+        self.maybe_failure = set(inspect.signature(self.callable).parameters.keys())
```

### Comparing `graia-broadcast-0.8.9/src/graia/broadcast/entities/listener.py` & `graia-broadcast-0.9.0/src/graia/broadcast/entities/listener.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from typing import Callable, List, Type
 
 from .dispatcher import BaseDispatcher
-from .event import BaseEvent
+from .event import Dispatchable
 from .namespace import Namespace
 from .decorator import Decorator
 
 from .exectarget import ExecTarget
 
 
 class Listener(ExecTarget):
     def __init__(
         self,
         callable: Callable,
         namespace: Namespace,
-        listening_events: List[Type[BaseEvent]],
+        listening_events: List[Type[Dispatchable]],
         inline_dispatchers: List[BaseDispatcher] = None,
         headless_decorators: List[Decorator] = None,
         priority: int = 16,
         enable_internal_access: bool = False,
     ) -> None:
         super().__init__(
             callable, inline_dispatchers, headless_decorators, enable_internal_access
         )
+
         self.namespace = namespace
         self.listening_events = listening_events
         self.priority = priority
 
     namespace: Namespace
-    listening_events: List[Type[BaseEvent]]
-    priority: int = 16
+    listening_events: List[Type[Dispatchable]]
+    priority: int
```

### Comparing `graia-broadcast-0.8.9/src/graia/broadcast/exceptions.py` & `graia-broadcast-0.9.0/src/graia/broadcast/exceptions.py`

 * *Files identical despite different names*

### Comparing `graia-broadcast-0.8.9/src/graia/broadcast/interfaces/dispatcher.py` & `graia-broadcast-0.9.0/src/graia/broadcast/interfaces/dispatcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,39 +8,33 @@
     Generator,
     List,
     Optional,
     TYPE_CHECKING,
     Tuple,
 )
 from graia.broadcast.entities.dispatcher import BaseDispatcher
-from graia.broadcast.entities.event import BaseEvent
+from graia.broadcast.entities.event import Dispatchable
 
 from graia.broadcast.entities.context import ExecutionContext, ParameterContext
 from graia.broadcast.entities.signatures import Force
 from graia.broadcast.entities.track_log import TrackLog, TrackLogType
 from graia.broadcast.exceptions import RequirementCrashed
-from graia.broadcast.typing import T_Dispatcher, T_Dispatcher_Callable
+from graia.broadcast.typing import (
+    T_Dispatcher,
+    T_Dispatcher_Callable,
+    DEFAULT_LIFECYCLE_NAMES,
+)
 
 from ..utilles import NestableIterable, run_always_await_safely, cached_getattr
 
 if TYPE_CHECKING:
     from graia.broadcast import Broadcast
 
 
-DEFAULT_LIFECYCLE_NAMES = (
-    "beforeDispatch",
-    "afterDispatch",
-    "beforeExecution",
-    "afterExecution",
-    "beforeTargetExec",
-    "afterTargetExec",
-)
-
-
-class EmptyEvent(BaseEvent):
+class EmptyEvent(Dispatchable):
     class Dispatcher(BaseDispatcher):
         @staticmethod
         def catch(_):
             pass
 
 
 class DispatcherInterface:
@@ -53,41 +47,25 @@
 
     @property
     def track_log(self):
         return self.track_logs[-1]
 
     @staticmethod
     @lru_cache(None)
-    def get_lifecycle_refs(
-        dispatcher: "T_Dispatcher",
-    ) -> Optional[Dict[str, List]]:
-        from graia.broadcast.entities.dispatcher import BaseDispatcher
-
-        lifecycle_refs: Dict[str, List] = {}
+    def get_lifecycle_refs(dispatcher: "T_Dispatcher", target_dict: Dict[str, List]):
         if not isinstance(dispatcher, (BaseDispatcher, type)):
             return
 
         for name in DEFAULT_LIFECYCLE_NAMES:
-            lifecycle_refs.setdefault(name, [])
-            abstract_lifecycle_func = cached_getattr(BaseDispatcher, name)
-            unbound_attr = getattr(dispatcher, name, None)
+            unbound_attr = cached_getattr(dispatcher, name, None)
 
             if unbound_attr is None:
                 continue
 
-            orig_call = unbound_attr
-            while ismethod(orig_call):
-                orig_call = unbound_attr.__func__
-
-            if orig_call is abstract_lifecycle_func:
-                continue
-
-            lifecycle_refs[name].append(unbound_attr)
-
-        return lifecycle_refs
+            target_dict[name].append(unbound_attr)
 
     def dispatcher_pure_generator(self) -> Generator[None, None, T_Dispatcher]:
         return itertools.chain(
             self.execution_contexts[0].dispatchers,
             self.parameter_contexts[-1].dispatchers,
             self.execution_contexts[-1].dispatchers,
         )
@@ -95,27 +73,25 @@
     def flush_lifecycle_refs(
         self,
         dispatchers: List["T_Dispatcher"] = None,
     ):
         from graia.broadcast.entities.dispatcher import BaseDispatcher
 
         lifecycle_refs = self.execution_contexts[-1].lifecycle_refs
-        if dispatchers is None and lifecycle_refs:  # 已经刷新.
+        if dispatchers is None and lifecycle_refs:
             return
 
         for dispatcher in dispatchers or self.dispatcher_pure_generator():
             if (
                 not isinstance(dispatcher, BaseDispatcher)
                 or dispatcher.__class__ is type
             ):
                 continue
 
-            for name, value in self.get_lifecycle_refs(dispatcher).items():
-                lifecycle_refs.setdefault(name, [])
-                lifecycle_refs[name].extend(value)
+            self.get_lifecycle_refs(dispatcher, lifecycle_refs)
 
     async def exec_lifecycle(self, lifecycle_name: str, *args, **kwargs):
         lifecycle_funcs = self.execution_contexts[-1].lifecycle_refs.get(
             lifecycle_name, []
         )
         if lifecycle_funcs:
             for func in lifecycle_funcs:
@@ -152,15 +128,15 @@
         return self.parameter_contexts[-1].default
 
     @property
     def _index(self) -> int:
         return self.execution_contexts[-1]._index
 
     @property
-    def event(self) -> BaseEvent:
+    def event(self) -> Dispatchable:
         return self.execution_contexts[-1].event
 
     @property
     def global_dispatcher(self) -> List[T_Dispatcher]:
         return self.execution_contexts[0].dispatchers
 
     @property
@@ -197,15 +173,15 @@
     async def __aexit__(self, _, exc: Exception, tb):
         await self.exit_current_execution()
         if tb is not None:
             raise exc.with_traceback(tb)
 
     def start_execution(
         self,
-        event: BaseEvent,
+        event: Dispatchable,
         dispatchers: List[T_Dispatcher],
         track_log_receiver: TrackLog = None,
     ) -> "DispatcherInterface":
         self.execution_contexts.append(ExecutionContext(dispatchers, event))
         self.flush_lifecycle_refs()
         self.track_logs.append(track_log_receiver or TrackLog())
         return self
```

### Comparing `graia-broadcast-0.8.9/src/graia/broadcast/interrupt/__init__.py` & `graia-broadcast-0.9.0/src/graia/broadcast/interrupt/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,19 @@
+from asyncio.futures import Future
 from typing import Any, Optional, Type, Union
 from graia.broadcast import Broadcast
 from graia.broadcast.entities.exectarget import ExecTarget
 from graia.broadcast.priority import Priority
-from graia.broadcast.entities.event import BaseEvent
-from abc import ABCMeta, abstractmethod
-from graia.broadcast.utilles import run_always_await
-from graia.broadcast.entities.signatures import Force, RemoveMe
+from graia.broadcast.entities.event import Dispatchable
+from graia.broadcast.entities.signatures import RemoveMe
 from graia.broadcast.exceptions import PropagationCancelled
 import asyncio
 from .waiter import Waiter
 
 
-class ActiveStats:
-    def __init__(self) -> None:
-        self.actived = False
-
-    def get(self) -> bool:
-        return self.actived
-
-    def set(self) -> bool:
-        self.actived = True
-        return True
-
-
-class Value:
-    value: Any
-
-    def __init__(self) -> None:
-        self.value = None
-
-    def getValue(self) -> Any:
-        return self.value
-
-    def setValue(self, value) -> None:
-        self.value = value
-
-
 class InterruptControl:
     """即中断控制, 主要是用于监听器/其他地方进行对符合特定要求的事件的捕获, 并返回事件.
 
     Methods:
         coroutine wait(interrupt: Interrupt) -> Any: 该方法主要用于在当前执行处堵塞当前协程,
             同时将一个一次性使用的监听器挂载, 只要获取到符合条件的事件, 该方法会通过你传入的 `Interrupt` 实例的方法 `trigger`,
             获取处理得到的值并返回; 无论如何, 用于一次性监听使用的监听器总会被销毁.
@@ -60,60 +34,51 @@
             waiter (Waiter): 等待器
             priority (Union[int, Priority]): 中断 inline 监听器的优先级, Defaults to 15.
             **kwargs: 都会直接传入 Broadcast.receiver.
 
         Returns:
             Any: 通常这个值由中断本身定义并返回.
         """
-        local_event = asyncio.Event()
-        value_container = Value()
-        active_stat = ActiveStats()
+        future = asyncio.get_running_loop().create_future()
 
-        listener_callables = []
+        listeners = set()
         for event_type in waiter.listening_events:
             listener_callable = self.leader_listener_generator(
-                local_event, waiter, event_type, value_container, active_stat
+                waiter, event_type, future
             )
             self.broadcast.receiver(
                 event_type, priority=priority or waiter.priority, **kwargs
             )(listener_callable)
-            listener_callables.append(listener_callable)
+            listener = self.broadcast.getListener(listener_callable)
+            listeners.add(listener)
 
         try:
-            await local_event.wait()
+            return await future
         finally:  # 删除 Listener
-            if not local_event.is_set() or not active_stat.get():
-                for i in listener_callables:
-                    self.broadcast.removeListener(self.broadcast.getListener(i))
-        return value_container.getValue()
+            if not future.done():
+                for i in listeners:
+                    self.broadcast.removeListener(i)
 
     def leader_listener_generator(
-        self,
-        event_lock: asyncio.Event,
-        waiter: Waiter,
-        event_type: Type[BaseEvent],
-        value_container: Value,
-        active_stat: ActiveStats,
+        self, waiter: Waiter, event_type: Type[Dispatchable], future: Future
     ):
         async def inside_listener(event: event_type):
-            if active_stat.get():
+            if future.done():
                 return RemoveMe()
 
             result = await self.broadcast.Executor(
                 target=ExecTarget(
                     callable=waiter.detected_event,
                     inline_dispatchers=waiter.using_dispatchers,
                     headless_decorators=waiter.using_decorators,
                     enable_internal_access=waiter.enable_internal_access,
                 ),
                 event=event,
             )
 
             if result is not None:
-                active_stat.set()
-                event_lock.set()
-                value_container.setValue(result)
+                future.set_result(result)
                 if not waiter.block_propagation:
                     return RemoveMe()
                 raise PropagationCancelled()
 
         return inside_listener
```

### Comparing `graia-broadcast-0.8.9/src/graia/broadcast/interrupt/waiter.py` & `graia-broadcast-0.9.0/src/graia/broadcast/interrupt/waiter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Any, List, Type
 from abc import ABCMeta, abstractmethod
 
 from graia.broadcast.entities.decorator import Decorator
-from ..entities.event import BaseEvent
+from ..entities.event import Dispatchable
 from ..typing import T_Dispatcher
 
 
 class Waiter(metaclass=ABCMeta):
-    listening_events: List[Type[BaseEvent]]
+    listening_events: List[Type[Dispatchable]]
     using_dispatchers: List[T_Dispatcher]
     using_decorators: List[Decorator]
     priority: int
     enable_internal_access: bool
     block_propagation: bool
 
     @classmethod
     def create(
         cls,
-        listening_events: List[Type[BaseEvent]],
+        listening_events: List[Type[Dispatchable]],
         using_dispatchers: List[T_Dispatcher] = None,
         using_decorators: List[Decorator] = None,
         priority: int = 15,  # 默认情况下都是需要高于默认 16 的监听吧...
         enable_internal_access: bool = False,
         block_propagation: bool = False,
     ) -> Type["Waiter"]:
         async def detected_event(self) -> Any:
@@ -43,15 +43,15 @@
 
     async def detected_event(self) -> Any:
         pass
 
     @classmethod
     def create_using_function(
         cls,
-        listening_events: List[Type[BaseEvent]],
+        listening_events: List[Type[Dispatchable]],
         using_dispatchers: List[T_Dispatcher] = None,
         using_decorators: List[Decorator] = None,
         priority: int = 15,  # 默认情况下都是需要高于默认 16 的监听吧...
         enable_internal_access: bool = False,
         block_propagation: bool = False,
     ):
         def wrapper(func):
```

### Comparing `graia-broadcast-0.8.9/src/graia/broadcast/utilles.py` & `graia-broadcast-0.9.0/src/graia/broadcast/utilles.py`

 * *Files 15% similar despite different names*

```diff
@@ -110,43 +110,14 @@
             return list(itertools.islice(self.iterable, item, item + 1, None))[0]
 
     def __iter__(self):
         return self.iterable
 
 
 T = TypeVar("T")
-
-"""
-class NestableIterable(Iterable[T]):
-    index_stack: list
-    iterable: Iterable[T]
-
-    def __init__(self, iterable: Iterable[T]) -> None:
-        self.iterable = iterable
-        self.index_stack = [0]
-
-    def __iter__(self):
-        index = self.index_stack[-1]
-        self.index_stack.append(self.index_stack[-1])
-
-        start_offset = index + int(bool(index))
-        try:
-            for self.index_stack[-1], content in enumerate(
-                itertools.islice(self.iterable, start_offset, None, None),
-                start=start_offset,
-            ):
-                yield content
-        finally:
-            self.index_stack.pop()
-
-    def with_new(self, target):
-        self.iterable = target
-        return self
-"""
-
 I = TypeVar("I")
 
 
 class NestableIterable(Generic[I, T]):
     iterable: Iterable[T]
     indexes: List[I]
 
@@ -183,17 +154,14 @@
         current_index = self.indexes[-1]
         self.indexes.append(current_index)
 
         if self.is_index_origin(current_index):
             start_offset = current_index
         else:
             start_offset = self.index_increase_func(current_index, self.iterable)
-        # 0 = 0
-        # <except 0> = index + 1
-        try:
-            for self.indexes[-1], content in self.generator_with_index_factory(
-                self.iterable,
-                start=start_offset,
-            ):
-                yield content
-        finally:
-            self.indexes.pop()
+
+        for self.indexes[-1], content in self.generator_with_index_factory(
+            self.iterable,
+            start=start_offset,
+        ):
+            yield content
+        self.indexes.pop()
```

### Comparing `graia-broadcast-0.8.9/setup.py` & `graia-broadcast-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 {'': ['*']}
 
 install_requires = \
 ['iterwrapper>=0.1.2,<0.2.0', 'pydantic<=1.7.1']
 
 setup_kwargs = {
     'name': 'graia-broadcast',
-    'version': '0.8.9',
+    'version': '0.9.0',
     'description': 'a highly customizable, elegantly designed event system based on asyncio',
     'long_description': None,
     'author': 'GreyElaina',
     'author_email': 'GreyElaina@outlook.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `graia-broadcast-0.8.9/PKG-INFO` & `graia-broadcast-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graia-broadcast
-Version: 0.8.9
+Version: 0.9.0
 Summary: a highly customizable, elegantly designed event system based on asyncio
 License: MIT
 Author: GreyElaina
 Author-email: GreyElaina@outlook.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

