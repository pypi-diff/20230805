# Comparing `tmp/graia-scheduler-0.1.5.tar.gz` & `tmp/graia_scheduler-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graia-scheduler-0.1.5.tar", last modified: Sun Jun 11 07:23:10 2023, max compression
+gzip compressed data, was "graia_scheduler-0.2.0.tar", last modified: Sat Aug  5 13:20:46 2023, max compression
```

## Comparing `graia-scheduler-0.1.5.tar` & `graia_scheduler-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1273 2023-06-11 07:22:51.068739 graia-scheduler-0.1.5/README.md
--rw-r--r--   0        0        0      991 2023-06-11 07:22:51.068739 graia-scheduler-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2521 2023-06-11 07:22:51.068739 graia-scheduler-0.1.5/src/graia/scheduler/__init__.py
--rw-r--r--   0        0        0       91 2023-06-11 07:22:51.068739 graia-scheduler-0.1.5/src/graia/scheduler/exception.py
--rw-r--r--   0        0        0      129 2023-06-11 07:22:51.068739 graia-scheduler-0.1.5/src/graia/scheduler/saya/__init__.py
--rw-r--r--   0        0        0     1329 2023-06-11 07:22:51.068739 graia-scheduler-0.1.5/src/graia/scheduler/saya/behaviour.py
--rw-r--r--   0        0        0      471 2023-06-11 07:22:51.072739 graia-scheduler-0.1.5/src/graia/scheduler/saya/schema.py
--rw-r--r--   0        0        0     1113 2023-06-11 07:22:51.072739 graia-scheduler-0.1.5/src/graia/scheduler/service.py
--rw-r--r--   0        0        0     4760 2023-06-11 07:22:51.072739 graia-scheduler-0.1.5/src/graia/scheduler/task.py
--rw-r--r--   0        0        0     3679 2023-06-11 07:22:51.072739 graia-scheduler-0.1.5/src/graia/scheduler/timers.py
--rw-r--r--   0        0        0     1524 2023-06-11 07:22:51.072739 graia-scheduler-0.1.5/src/graia/scheduler/utilles.py
--rw-r--r--   0        0        0     1549 1970-01-01 00:00:00.000000 graia-scheduler-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1273 2023-08-05 13:20:29.729066 graia_scheduler-0.2.0/README.md
+-rw-r--r--   0        0        0     1151 2023-08-05 13:20:46.945672 graia_scheduler-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2521 2023-08-05 13:20:29.733066 graia_scheduler-0.2.0/src/graia/scheduler/__init__.py
+-rw-r--r--   0        0        0     1692 2023-08-05 13:20:29.733066 graia_scheduler-0.2.0/src/graia/scheduler/creator.py
+-rw-r--r--   0        0        0       91 2023-08-05 13:20:29.733066 graia_scheduler-0.2.0/src/graia/scheduler/exception.py
+-rw-r--r--   0        0        0      129 2023-08-05 13:20:29.733066 graia_scheduler-0.2.0/src/graia/scheduler/saya/__init__.py
+-rw-r--r--   0        0        0     1330 2023-08-05 13:20:29.733066 graia_scheduler-0.2.0/src/graia/scheduler/saya/behaviour.py
+-rw-r--r--   0        0        0      471 2023-08-05 13:20:29.733066 graia_scheduler-0.2.0/src/graia/scheduler/saya/schema.py
+-rw-r--r--   0        0        0     1113 2023-08-05 13:20:29.733066 graia_scheduler-0.2.0/src/graia/scheduler/service.py
+-rw-r--r--   0        0        0     4760 2023-08-05 13:20:29.733066 graia_scheduler-0.2.0/src/graia/scheduler/task.py
+-rw-r--r--   0        0        0     3679 2023-08-05 13:20:29.733066 graia_scheduler-0.2.0/src/graia/scheduler/timers.py
+-rw-r--r--   0        0        0     1524 2023-08-05 13:20:29.733066 graia_scheduler-0.2.0/src/graia/scheduler/utilles.py
+-rw-r--r--   0        0        0     1740 1970-01-01 00:00:00.000000 graia_scheduler-0.2.0/PKG-INFO
```

### Comparing `graia-scheduler-0.1.5/README.md` & `graia_scheduler-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `graia-scheduler-0.1.5/src/graia/scheduler/__init__.py` & `graia_scheduler-0.2.0/src/graia/scheduler/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from datetime import datetime
 from typing import Iterable, List, Optional
 
 from graia.broadcast.typing import T_Dispatcher
 
 Timer = Iterable[datetime]
 
-from asyncio import AbstractEventLoop
 import asyncio
+from asyncio import AbstractEventLoop
+from typing import Callable, TypeVar
 
 from graia.broadcast import Broadcast
 from graia.broadcast.entities.decorator import Decorator
 
 from .task import SchedulerTask
-from typing import Callable, TypeVar
 
 T_Callable = TypeVar("T_Callable", bound=Callable)
 
 
 class GraiaScheduler:
     """任务计划器"""
```

### Comparing `graia-scheduler-0.1.5/src/graia/scheduler/saya/behaviour.py` & `graia_scheduler-0.2.0/src/graia/scheduler/saya/behaviour.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -39,8 +39,8 @@
                 target.stop()
                 self.scheduler.schedule_tasks.remove(target)
         else:
             return
 
         return True
 
-    uninstall = release
+    uninstall = release
```

### Comparing `graia-scheduler-0.1.5/src/graia/scheduler/service.py` & `graia_scheduler-0.2.0/src/graia/scheduler/service.py`

 * *Files identical despite different names*

### Comparing `graia-scheduler-0.1.5/src/graia/scheduler/task.py` & `graia_scheduler-0.2.0/src/graia/scheduler/task.py`

 * *Files identical despite different names*

### Comparing `graia-scheduler-0.1.5/src/graia/scheduler/timers.py` & `graia_scheduler-0.2.0/src/graia/scheduler/timers.py`

 * *Files identical despite different names*

### Comparing `graia-scheduler-0.1.5/src/graia/scheduler/utilles.py` & `graia_scheduler-0.2.0/src/graia/scheduler/utilles.py`

 * *Files identical despite different names*

### Comparing `graia-scheduler-0.1.5/PKG-INFO` & `graia_scheduler-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 Metadata-Version: 2.1
 Name: graia-scheduler
-Version: 0.1.5
+Version: 0.2.0
 Summary: a scheduler for graia framework
+Author-Email: GreyElaina <31543961+GreyElaina@users.noreply.github.com>
 License: MIT
-Author-email: GreyElaina <31543961+GreyElaina@users.noreply.github.com>
-Requires-Python: >=3.8,<4.0
+Requires-Python: <4.0,>=3.8
+Requires-Dist: graia-broadcast~=0.23.0
+Requires-Dist: croniter<2.0.0,>=1.0.0
+Requires-Dist: launart~=0.6.4
+Requires-Dist: creart~=0.3.0
+Requires-Dist: graia-saya<0.1,>=0.0.16; extra == "saya"
 Provides-Extra: saya
 Description-Content-Type: text/markdown
 
 # Graia Scheduler
 
 一个基于 `asyncio`, 设计简洁, 代码简单的计划任务库, 使用 `loop.create_task` 创建计划任务;  
 同时使用生成器特性与 `croniter` 的定时设计, 轻盈而强大.
@@ -64,8 +69,7 @@
     print("print every second.")
 
 
 loop.run_until_complete(scheduler.run())
 ```
 
 因为基于 `BroadcastControl`, 你可以享受使用 `Dispatcher`, `Interrupt`, `Decorator` 的开发体验.
-
```

