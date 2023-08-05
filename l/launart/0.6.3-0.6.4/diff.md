# Comparing `tmp/launart-0.6.3.tar.gz` & `tmp/launart-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "launart-0.6.3.tar", last modified: Wed Jan  4 10:11:16 2023, max compression
+gzip compressed data, was "launart-0.6.4.tar", last modified: Sat Aug  5 12:55:11 2023, max compression
```

## Comparing `launart-0.6.3.tar` & `launart-0.6.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-04 10:10:33.705308 launart-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-01-04 10:10:33.705308 launart-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-01-04 10:10:33.705308 launart-0.6.3/launart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-01-04 10:10:33.705308 launart-0.6.3/launart/_sideload.py
--rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-01-04 10:10:33.705308 launart-0.6.3/launart/component.py
--rw-r--r--   0 runner    (1001) docker     (123)    21517 2023-01-04 10:10:33.705308 launart-0.6.3/launart/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-01-04 10:10:33.705308 launart-0.6.3/launart/saya.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-01-04 10:10:33.705308 launart-0.6.3/launart/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-01-04 10:10:33.705308 launart-0.6.3/launart/utilles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-01-04 10:10:33.705308 launart-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-01-04 10:10:33.705308 launart-0.6.3/tests/_saya_mod/empty_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-01-04 10:10:33.705308 launart-0.6.3/tests/_saya_mod/fail_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-01-04 10:10:33.705308 launart-0.6.3/tests/_saya_mod/ok_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-01-04 10:10:33.705308 launart-0.6.3/tests/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-01-04 10:10:33.705308 launart-0.6.3/tests/launchable.py
--rw-r--r--   0 runner    (1001) docker     (123)    10517 2023-01-04 10:10:33.705308 launart-0.6.3/tests/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-04 10:10:33.709308 launart-0.6.3/tests/saya.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-01-04 10:10:33.709308 launart-0.6.3/tests/sideload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-01-04 10:10:33.709308 launart-0.6.3/tests/utils.py
--rw-------   0 runner    (1001) docker     (123)     1178 2023-01-04 10:11:16.244109 launart-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-05 12:54:59.880786 launart-0.6.4/LICENSE
+-rw-r--r--   0        0        0      929 2023-08-05 12:54:59.880786 launart-0.6.4/README.md
+-rw-r--r--   0        0        0      591 2023-08-05 12:54:59.880786 launart-0.6.4/launart/__init__.py
+-rw-r--r--   0        0        0     1099 2023-08-05 12:54:59.880786 launart-0.6.4/launart/_sideload.py
+-rw-r--r--   0        0        0     7195 2023-08-05 12:54:59.880786 launart-0.6.4/launart/component.py
+-rw-r--r--   0        0        0    21879 2023-08-05 12:54:59.880786 launart-0.6.4/launart/manager.py
+-rw-r--r--   0        0        0     1020 2023-08-05 12:54:59.880786 launart-0.6.4/launart/saya.py
+-rw-r--r--   0        0        0      713 2023-08-05 12:54:59.880786 launart-0.6.4/launart/service.py
+-rw-r--r--   0        0        0     3722 2023-08-05 12:54:59.880786 launart-0.6.4/launart/utilles.py
+-rw-r--r--   0        0        0     1552 2023-08-05 12:55:11.857344 launart-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-08-05 12:54:59.880786 launart-0.6.4/tests/_saya_mod/empty_sub.py
+-rw-r--r--   0        0        0      135 2023-08-05 12:54:59.880786 launart-0.6.4/tests/_saya_mod/fail_sub.py
+-rw-r--r--   0        0        0      947 2023-08-05 12:54:59.880786 launart-0.6.4/tests/_saya_mod/ok_sub.py
+-rw-r--r--   0        0        0     2062 2023-08-05 12:54:59.880786 launart-0.6.4/tests/fixture.py
+-rw-r--r--   0        0        0     4269 2023-08-05 12:54:59.880786 launart-0.6.4/tests/launchable.py
+-rw-r--r--   0        0        0    10571 2023-08-05 12:54:59.880786 launart-0.6.4/tests/manager.py
+-rw-r--r--   0        0        0     1106 2023-08-05 12:54:59.880786 launart-0.6.4/tests/saya.py
+-rw-r--r--   0        0        0     2416 2023-08-05 12:54:59.880786 launart-0.6.4/tests/sideload.py
+-rw-r--r--   0        0        0     3033 2023-08-05 12:54:59.880786 launart-0.6.4/tests/utils.py
+-rw-r--r--   0        0        0     1314 1970-01-01 00:00:00.000000 launart-0.6.4/PKG-INFO
```

### Comparing `launart-0.6.3/LICENSE` & `launart-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `launart-0.6.3/README.md` & `launart-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `launart-0.6.3/launart/__init__.py` & `launart-0.6.4/launart/__init__.py`

 * *Files identical despite different names*

### Comparing `launart-0.6.3/launart/_sideload.py` & `launart-0.6.4/launart/_sideload.py`

 * *Files identical despite different names*

### Comparing `launart-0.6.3/launart/component.py` & `launart-0.6.4/launart/component.py`

 * *Files identical despite different names*

### Comparing `launart-0.6.3/launart/manager.py` & `launart-0.6.4/launart/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     Literal,
     Optional,
     Type,
     TypeVar,
     cast,
 )
 
+from creart import it
 from loguru import logger
 from statv import Stats, Statv
 
 from launart._sideload import FutureMark, override
 from launart.component import Launchable, resolve_requirements
 from launart.service import ExportInterface, Service, TInterface
 from launart.utilles import FlexibleTaskGroup, priority_strategy
@@ -470,15 +471,24 @@
         loop: Optional[asyncio.AbstractEventLoop] = None,
         stop_signal: Iterable[signal.Signals] = (signal.SIGINT,),
     ):
         import contextlib
         import functools
         import threading
 
-        loop = loop or asyncio.new_event_loop()
+        if loop is not None:
+            from warnings import warn
+
+            warn(
+                "The loop argument is deprecated since launart 0.6.4, " "and scheduled for removal in launart 0.7.0.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+
+        loop = it(asyncio.AbstractEventLoop)
 
         logger.info("Starting launart main task...", style="green bold")
 
         launch_task = loop.create_task(self.launch(), name="amnesia-launch")
         handled_signals: Dict[signal.Signals, Any] = {}
         signal_handler = functools.partial(self._on_sys_signal, main_task=launch_task)
         if threading.current_thread() is threading.main_thread():  # pragma: worst case
@@ -498,16 +508,17 @@
                 signal.signal(sig, handler)
 
         try:
             self._cancel_tasks(loop)
             loop.run_until_complete(loop.shutdown_asyncgens())
             with contextlib.suppress(RuntimeError, AttributeError):
                 # LINK: https://docs.python.org/3.10/library/asyncio-eventloop.html#asyncio.loop.shutdown_default_executor
-                loop.run_until_complete(loop.shutdown_default_executor())
+                loop.run_until_complete(loop.shutdown_default_executor())  # type: ignore
         finally:
+            asyncio.set_event_loop(None)
             logger.success("asyncio shutdown complete.", style="green bold")
 
     def _on_sys_signal(self, _, __, main_task: asyncio.Task):
         self.status.exiting = True
         if self.task_group is not None:
             self.task_group.stop = True
             if self.task_group.blocking_task is not None:  # pragma: worst case
```

### Comparing `launart-0.6.3/launart/saya.py` & `launart-0.6.4/launart/saya.py`

 * *Files identical despite different names*

### Comparing `launart-0.6.3/launart/service.py` & `launart-0.6.4/launart/service.py`

 * *Files identical despite different names*

### Comparing `launart-0.6.3/launart/utilles.py` & `launart-0.6.4/launart/utilles.py`

 * *Files identical despite different names*

### Comparing `launart-0.6.3/pyproject.toml` & `launart-0.6.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,30 @@
 [project]
 name = "launart"
-version = "0.6.3"
+version = "0.6.4"
 description = "Component lifetime manager for runtime."
 authors = [
     { name = "GreyElaina", email = "GreyElaina@outlook.com" },
 ]
 dependencies = [
     "statv>=0.2.2",
     "loguru>=0.6.0",
+    "creart>=0.3.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 saya = [
     "graia-saya>=0.0.16",
 ]
 
-[tool.pdm.scripts.test]
-composite = [
-    "coverage run -m pytest",
-    "coverage xml",
-    "coverage report",
-]
-
-[tool.pdm.dev-dependencies]
-dev = [
-    "richuru>=0.1.0",
-    "black>=22.6.0",
-    "isort>=5.10.1",
-    "graia-saya~=0.0",
-    "coverage~=6.4",
-    "pytest~=7.1",
-    "pytest-asyncio~=0.19",
-]
-
 [tool.black]
 line-length = 120
 
 [tool.isort]
 profile = "black"
 
 [tool.coverage.run]
@@ -70,22 +53,41 @@
     "except ImportError:",
 ]
 partial_branches = [
     "pragma: worst case",
 ]
 precision = 2
 
+[tool.pdm.scripts.test]
+composite = [
+    "coverage run -m pytest",
+    "coverage xml",
+    "coverage report",
+]
+
+[tool.pdm.dev-dependencies]
+dev = [
+    "richuru>=0.1.0",
+    "black>=22.6.0",
+    "isort>=5.10.1",
+    "graia-saya~=0.0",
+    "coverage~=6.4",
+    "pytest~=7.1",
+    "pytest-asyncio~=0.19",
+    "graia-broadcast>=0.22.1",
+]
+
 [tool.pyright]
 exclude = [
     "__pypackages__",
 ]
 
 [tool.pytest.ini_options]
 python_files = "tests/*"
 asyncio_mode = "strict"
 norecursedirs = "_saya_mod"
 
 [build-system]
 requires = [
-    "pdm-pep517>=0.12.0",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
```

### Comparing `launart-0.6.3/tests/_saya_mod/ok_sub.py` & `launart-0.6.4/tests/_saya_mod/ok_sub.py`

 * *Files identical despite different names*

### Comparing `launart-0.6.3/tests/fixture.py` & `launart-0.6.4/tests/fixture.py`

 * *Files identical despite different names*

### Comparing `launart-0.6.3/tests/launchable.py` & `launart-0.6.4/tests/launchable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import asyncio
 
 import pytest
 
 from launart import Launart
 from launart.component import Launchable, LaunchableStatus
 from tests.fixture import EmptyLaunchable, component, interface, service
```

### Comparing `launart-0.6.3/tests/manager.py` & `launart-0.6.4/tests/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+from __future__ import annotations
+
 import asyncio
 from signal import SIGINT, default_int_handler, signal
 
 import pytest
+from creart import it
 
 from launart import Launart
 from launart.component import Launchable
 from launart.service import ExportInterface, Service
 from tests.fixture import EmptyLaunchable, component, interface, service
 
 
@@ -23,19 +26,19 @@
     lc = EmptyLaunchable()
     mgr.add_launchable(lc)
     mgr.launch_blocking()
     assert lc.triggered
 
     # set SIGINT and do again
     lc.triggered = False
-    loop = asyncio.new_event_loop()
+    loop = it(asyncio.AbstractEventLoop)
     tsk = loop.create_task(asyncio.sleep(2.0))
     tsk2 = loop.create_task(asyncio.sleep(0))
     signal(SIGINT, lambda *_: None)
-    mgr.launch_blocking(loop=loop)
+    mgr.launch_blocking()
     assert tsk.cancelled()
     assert tsk.done()
     assert tsk2.done()
     assert lc.triggered
     signal(SIGINT, default_int_handler)
```

### Comparing `launart-0.6.3/tests/saya.py` & `launart-0.6.4/tests/saya.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pytest
 from graia.saya import Saya
 from graia.saya.behaviour.entity import Behaviour
 from graia.saya.schema import BaseSchema
 
 from launart.manager import Launart
 from launart.saya import LaunartBehaviour
```

### Comparing `launart-0.6.3/tests/sideload.py` & `launart-0.6.4/tests/sideload.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import asyncio
 
 import pytest
 
 from launart import Launart
 from launart.component import Launchable
 from tests.fixture import component
```

### Comparing `launart-0.6.3/tests/utils.py` & `launart-0.6.4/tests/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import asyncio
 from typing import Any, cast
 
 import pytest
 
 from launart._sideload import Override, override
 from launart.component import RequirementResolveFailed, resolve_requirements
```

### Comparing `launart-0.6.3/PKG-INFO` & `launart-0.6.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: launart
-Version: 0.6.3
+Version: 0.6.4
 Summary: Component lifetime manager for runtime.
+Author-Email: GreyElaina <GreyElaina@outlook.com>
 License: MIT
-Author-email: GreyElaina <GreyElaina@outlook.com>
 Requires-Python: >=3.8
+Requires-Dist: statv>=0.2.2
+Requires-Dist: loguru>=0.6.0
+Requires-Dist: creart>=0.3.0
+Requires-Dist: graia-saya>=0.0.16; extra == "saya"
 Provides-Extra: saya
 Description-Content-Type: text/markdown
 
 # Launart - Launch for Graia Project
 
 [![PyPI](https://img.shields.io/pypi/v/launart)](https://pypi.org/project/launart)
 [![Docs](https://img.shields.io/badge/文档-here-blue)](https://graia.readthedocs.io/other/launart/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![codecov](https://codecov.io/gh/GraiaProject/launart/branch/master/graph/badge.svg?token=MW5U3JYXRA)](https://codecov.io/gh/GraiaProject/launart)
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 
 `Launart` 是实际实现了 `Launch API`, 即统一的应用实例启动时部件管理; 本部件为 Graia Project 内部使用.
 
-在应用实例装载 `richuru` 后可获得更加缤纷多彩的控制台输出.
+在应用实例装载 `richuru` 后可获得更加缤纷多彩的控制台输出.
```

