# Comparing `tmp/eggella-0.0.8.tar.gz` & `tmp/eggella-0.0.9.tar.gz`

## Comparing `eggella-0.0.8.tar` & `eggella-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/__init__.py
--rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/app.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/exceptions.py
--rw-r--r--   0        0        0     9855 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/manager.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/command/__init__.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/command/abc.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/command/arg_caster.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/command/completer.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/command/handler.py
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/command/objects.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/command/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/events/__init__.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/events/abc.py
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/events/events.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/fsm/__init__.py
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/fsm/fsm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/shortcuts/__init__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/shortcuts/cmd_shortcuts.py
--rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/shortcuts/help_pager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/tools/__init__.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 eggella-0.0.8/eggella/tools/type_caster.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 eggella-0.0.8/.gitignore
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 eggella-0.0.8/README.md
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 eggella-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 eggella-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 eggella-0.0.9/eggella/__init__.py
+-rw-r--r--   0        0        0     9331 2020-02-02 00:00:00.000000 eggella-0.0.9/eggella/app.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 eggella-0.0.9/eggella/exceptions.py
+-rw-r--r--   0        0        0    11265 2020-02-02 00:00:00.000000 eggella-0.0.9/eggella/manager.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 eggella-0.0.9/eggella/command/__init__.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 eggella-0.0.9/eggella/command/abc.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 eggella-0.0.9/eggella/command/arg_caster.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 eggella-0.0.9/eggella/command/completer.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 eggella-0.0.9/eggella/command/handler.py
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 eggella-0.0.9/eggella/command/objects.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 eggella-0.0.9/eggella/command/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.9/eggella/events/__init__.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 eggella-0.0.9/eggella/events/abc.py
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 eggella-0.0.9/eggella/events/events.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 eggella-0.0.9/eggella/fsm/__init__.py
+-rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 eggella-0.0.9/eggella/fsm/fsm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.9/eggella/shortcuts/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 eggella-0.0.9/eggella/shortcuts/cmd_shortcuts.py
+-rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 eggella-0.0.9/eggella/shortcuts/help_pager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.9/eggella/tools/__init__.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 eggella-0.0.9/eggella/tools/type_caster.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 eggella-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 eggella-0.0.9/README.md
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 eggella-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 eggella-0.0.9/PKG-INFO
```

### Comparing `eggella-0.0.8/eggella/manager.py` & `eggella-0.0.9/eggella/manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     List,
     Literal,
     Optional,
+    Set,
     Tuple,
     Type,
 )
 
 from prompt_toolkit.completion.nested import NestedDict
 
 from eggella.command.abc import ABCCommandHandler
@@ -288,7 +289,41 @@
             @wraps(func)
             def wrapper(*args, **kwargs):
                 return func(*args, **kwargs)
 
             return wrapper
 
         return decorator
+
+
+class BlueprintManager:
+    def __init__(self, main_app: "Eggella"):
+        self.app = main_app
+
+        self.blueprints: List["Eggella"] = []
+        self._loaded_blueprints: Set[str] = set()
+
+    def register_blueprints(self, *bp_apps: "Eggella"):
+        for bp_app in bp_apps:
+            self.blueprints.append(bp_app)
+
+    def load_blueprints(self):
+        for blueprint in self.blueprints:
+            if blueprint.app_name in self._loaded_blueprints:
+                continue
+            # register commands to main app
+            for key, command in blueprint.command_manager.commands.items():
+                if self.app.command_manager.commands.get(key) and not self.app.overwrite_commands_from_blueprints:
+                    raise TypeError(f"Command '{key}' already register")
+                self.app.command_manager.commands[key] = command
+            # register FSM groups to main app
+            for key, fsm_state in blueprint.fsm.fsm_storage.items():
+                self.app.fsm.fsm_storage[key] = fsm_state
+
+            # register events
+            for start_ev in blueprint.event_manager.startup_events:
+                self.app.event_manager.startup_events.append(start_ev)
+
+            for close_ev in blueprint.event_manager.close_events:
+                self.app.event_manager.close_events.append(close_ev)
+
+            self._loaded_blueprints.add(blueprint.app_name)
```

### Comparing `eggella-0.0.8/eggella/command/arg_caster.py` & `eggella-0.0.9/eggella/command/arg_caster.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.8/eggella/command/completer.py` & `eggella-0.0.9/eggella/command/completer.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.8/eggella/command/handler.py` & `eggella-0.0.9/eggella/command/handler.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.8/eggella/command/objects.py` & `eggella-0.0.9/eggella/command/objects.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.8/eggella/events/events.py` & `eggella-0.0.9/eggella/events/events.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.8/eggella/fsm/fsm.py` & `eggella-0.0.9/eggella/fsm/fsm.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,18 @@
         self._current_state = state or self._start_state
         return self._exec_state(self._current_state)
 
     def finish(self) -> None:
         self.ctx.clear()
         self._current_state = None
 
+    def actual(self):
+        if self._current_state:
+            return self._exec_state(self._current_state)
+
     def next(self):
         index = self._all_states.index(self._current_state)
         if index < len(self._all_states):
             self._current_state = self._all_states[index + 1]
             return self._exec_state(self._current_state)
         elif index == len(self._all_states) - 1 and self._all_states[index] == self._end_state:
             self.finish()
@@ -125,14 +129,17 @@
             raise RuntimeError(
                 f"State `{state.__class__.__name__}` is not registered in `{self.__app.app_name}`\n"
                 f"Register this state group in application "
                 f"by `register_states({state.__class__.__name__}) method`"
             )
         return self.fsm_storage[state.__class__.__name__].on_state(state)
 
+    def current(self):
+        return self._current_fsm.actual()
+
     def run(self, state: Union[IntStateGroup, Type[IntStateGroup]]):
         if isinstance(state, IntStateGroup):
             self._current_fsm = self.fsm_storage[state.__class__.__name__]
             return self._current_fsm.run(state)
         else:
             self._current_fsm = self.fsm_storage[state.__name__]
             return self._current_fsm.run(state.first())
```

### Comparing `eggella-0.0.8/eggella/shortcuts/cmd_shortcuts.py` & `eggella-0.0.9/eggella/shortcuts/cmd_shortcuts.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.8/eggella/shortcuts/help_pager.py` & `eggella-0.0.9/eggella/shortcuts/help_pager.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.8/eggella/tools/type_caster.py` & `eggella-0.0.9/eggella/tools/type_caster.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.8/.gitignore` & `eggella-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `eggella-0.0.8/README.md` & `eggella-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `eggella-0.0.8/pyproject.toml` & `eggella-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eggella-0.0.8/PKG-INFO` & `eggella-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eggella
-Version: 0.0.8
+Version: 0.0.9
 Summary: Create awesome command line applications with less effort
 Project-URL: Documentation, https://github.com/unknown/eggella#readme
 Project-URL: Issues, https://github.com/unknown/eggella/issues
 Project-URL: Source, https://github.com/unknown/eggella
 Author: georgiy
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
```

