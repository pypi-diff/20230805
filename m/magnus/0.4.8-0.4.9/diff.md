# Comparing `tmp/magnus-0.4.8.tar.gz` & `tmp/magnus-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnus-0.4.8.tar", max compression
+gzip compressed data, was "magnus-0.4.9.tar", max compression
```

## Comparing `magnus-0.4.8.tar` & `magnus-0.4.9.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0    11357 2023-03-01 22:08:18.076084 magnus-0.4.8/LICENSE
--rw-r--r--   0        0        0    10940 2023-03-01 22:08:18.076084 magnus-0.4.8/README.md
--rw-r--r--   0        0        0     1048 2023-03-01 22:08:18.088084 magnus-0.4.8/magnus/__init__.py
--rw-r--r--   0        0        0    13407 2023-03-01 22:08:18.088084 magnus-0.4.8/magnus/catalog.py
--rw-r--r--   0        0        0    13623 2023-03-01 22:08:18.088084 magnus-0.4.8/magnus/cli.py
--rw-r--r--   0        0        0    47471 2023-03-01 22:08:18.088084 magnus-0.4.8/magnus/datastore.py
--rw-r--r--   0        0        0     2318 2023-03-01 22:08:18.088084 magnus-0.4.8/magnus/defaults.py
--rw-r--r--   0        0        0     2539 2023-03-01 22:08:18.088084 magnus-0.4.8/magnus/docker_utils.py
--rw-r--r--   0        0        0     2369 2023-03-01 22:08:18.088084 magnus-0.4.8/magnus/exceptions.py
--rw-r--r--   0        0        0    41016 2023-03-01 22:08:18.088084 magnus-0.4.8/magnus/executor.py
--rw-r--r--   0        0        0     5021 2023-03-01 22:08:18.088084 magnus-0.4.8/magnus/experiment_tracker.py
--rw-r--r--   0        0        0    15493 2023-03-01 22:08:18.088084 magnus-0.4.8/magnus/graph.py
--rw-r--r--   0        0        0    12226 2023-03-01 22:08:18.088084 magnus-0.4.8/magnus/integration.py
--rw-r--r--   0        0        0     7446 2023-03-01 22:08:18.088084 magnus-0.4.8/magnus/interaction.py
--rw-r--r--   0        0        0      473 2023-03-01 22:08:18.088084 magnus-0.4.8/magnus/log_config.ini
--rw-r--r--   0        0        0    33663 2023-03-01 22:08:18.088084 magnus-0.4.8/magnus/names.py
--rw-r--r--   0        0        0    40956 2023-03-01 22:08:18.088084 magnus-0.4.8/magnus/nodes.py
--rw-r--r--   0        0        0     1730 2023-03-01 22:08:18.088084 magnus-0.4.8/magnus/pickler.py
--rw-r--r--   0        0        0    18030 2023-03-01 22:08:18.088084 magnus-0.4.8/magnus/pipeline.py
--rw-r--r--   0        0        0     9204 2023-03-01 22:08:18.088084 magnus-0.4.8/magnus/sdk.py
--rw-r--r--   0        0        0     5588 2023-03-01 22:08:18.088084 magnus-0.4.8/magnus/secrets.py
--rw-r--r--   0        0        0    10033 2023-03-01 22:08:18.088084 magnus-0.4.8/magnus/tasks.py
--rw-r--r--   0        0        0    21264 2023-03-01 22:08:18.088084 magnus-0.4.8/magnus/utils.py
--rw-r--r--   0        0        0     4195 2023-03-01 22:08:32.520126 magnus-0.4.8/pyproject.toml
--rw-r--r--   0        0        0    12081 1970-01-01 00:00:00.000000 magnus-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-06 13:04:25.150597 magnus-0.4.9/LICENSE
+-rw-r--r--   0        0        0    10940 2023-03-06 13:04:25.150597 magnus-0.4.9/README.md
+-rw-r--r--   0        0        0     1158 2023-03-06 13:04:25.166597 magnus-0.4.9/magnus/__init__.py
+-rw-r--r--   0        0        0    13338 2023-03-06 13:04:25.166597 magnus-0.4.9/magnus/catalog.py
+-rw-r--r--   0        0        0    13623 2023-03-06 13:04:25.166597 magnus-0.4.9/magnus/cli.py
+-rw-r--r--   0        0        0      111 2023-03-06 13:04:25.166597 magnus-0.4.9/magnus/context.py
+-rw-r--r--   0        0        0    47471 2023-03-06 13:04:25.166597 magnus-0.4.9/magnus/datastore.py
+-rw-r--r--   0        0        0     2383 2023-03-06 13:04:25.166597 magnus-0.4.9/magnus/defaults.py
+-rw-r--r--   0        0        0     2539 2023-03-06 13:04:25.166597 magnus-0.4.9/magnus/docker_utils.py
+-rw-r--r--   0        0        0     2369 2023-03-06 13:04:25.166597 magnus-0.4.9/magnus/exceptions.py
+-rw-r--r--   0        0        0    41016 2023-03-06 13:04:25.166597 magnus-0.4.9/magnus/executor.py
+-rw-r--r--   0        0        0     5021 2023-03-06 13:04:25.166597 magnus-0.4.9/magnus/experiment_tracker.py
+-rw-r--r--   0        0        0    15493 2023-03-06 13:04:25.166597 magnus-0.4.9/magnus/graph.py
+-rw-r--r--   0        0        0    12226 2023-03-06 13:04:25.166597 magnus-0.4.9/magnus/integration.py
+-rw-r--r--   0        0        0    11712 2023-03-06 13:04:25.166597 magnus-0.4.9/magnus/interaction.py
+-rw-r--r--   0        0        0      473 2023-03-06 13:04:25.166597 magnus-0.4.9/magnus/log_config.ini
+-rw-r--r--   0        0        0    33663 2023-03-06 13:04:25.166597 magnus-0.4.9/magnus/names.py
+-rw-r--r--   0        0        0    40956 2023-03-06 13:04:25.166597 magnus-0.4.9/magnus/nodes.py
+-rw-r--r--   0        0        0     1730 2023-03-06 13:04:25.166597 magnus-0.4.9/magnus/pickler.py
+-rw-r--r--   0        0        0    17940 2023-03-06 13:04:25.166597 magnus-0.4.9/magnus/pipeline.py
+-rw-r--r--   0        0        0     9350 2023-03-06 13:04:25.166597 magnus-0.4.9/magnus/sdk.py
+-rw-r--r--   0        0        0     5588 2023-03-06 13:04:25.166597 magnus-0.4.9/magnus/secrets.py
+-rw-r--r--   0        0        0    10033 2023-03-06 13:04:25.166597 magnus-0.4.9/magnus/tasks.py
+-rw-r--r--   0        0        0    21264 2023-03-06 13:04:25.166597 magnus-0.4.9/magnus/utils.py
+-rw-r--r--   0        0        0     4217 2023-03-06 13:04:43.310767 magnus-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0    12081 1970-01-01 00:00:00.000000 magnus-0.4.9/PKG-INFO
```

### Comparing `magnus-0.4.8/LICENSE` & `magnus-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `magnus-0.4.8/README.md` & `magnus-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `magnus-0.4.8/magnus/__init__.py` & `magnus-0.4.9/magnus/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import logging
 
 from yachalk import chalk
 
-from magnus.interaction import (get_experiment_tracker_context,
+from magnus.interaction import (end_interactive_session,
+                                get_experiment_tracker_context,
                                 get_from_catalog, get_object, get_parameter,
                                 get_run_id, get_secret, put_in_catalog,
-                                put_object, store_parameter, track_this)
-from magnus.sdk import AsIs, Pipeline, Task, step
+                                put_object, start_interactive_session,
+                                store_parameter, track_this)
+from magnus.sdk import AsIs, Pipeline, Task
 
 chalk_colors = {
     'debug': chalk.grey,
     'info': chalk.green,
     'warning': chalk.yellow_bright,
     'error': chalk.bold.red
 }
```

### Comparing `magnus-0.4.8/magnus/catalog.py` & `magnus-0.4.9/magnus/catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,17 +16,16 @@
     This method should be called after the executor module has been populated with all the systems.
 
     This method retrieves the run log store from the global executor.
 
     Returns:
         object: The run log store
     """
-    from magnus.pipeline import \
-        global_executor  # pylint: disable=import-outside-toplevel
-    return global_executor.run_log_store
+    from magnus import context
+    return context.executor.run_log_store
 
 
 def is_catalog_out_of_sync(catalog, synced_catalogs=None) -> bool:
     """
     Check if the catalog items are out of sync from already cataloged objects.
     If they are, return False.
     If the object does not exist or synced catalog does not exist, return True
```

### Comparing `magnus-0.4.8/magnus/cli.py` & `magnus-0.4.9/magnus/cli.py`

 * *Files identical despite different names*

### Comparing `magnus-0.4.8/magnus/datastore.py` & `magnus-0.4.9/magnus/datastore.py`

 * *Files identical despite different names*

### Comparing `magnus-0.4.8/magnus/defaults.py` & `magnus-0.4.9/magnus/defaults.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 LOG_LEVEL = 'WARNING'
 
 
 class EXECUTION_PLAN(Enum):
     # execution_plans
     CHAINED = 'chained'  #  121 relationship between run log and the dag.
     UNCHAINED = 'unchained'  # Only captures execution of steps, no relation.
+    INTERACTIVE = 'interactive'  # used for interactive sessions
 
 
 # Config file environment variable
 MAGNUS_CONFIG_FILE = 'MAGNUS_CONFIG_FILE'
 MAGNUS_RUN_TAG = 'MAGNUS_RUN_TAG'
 
 # Interaction settings
```

### Comparing `magnus-0.4.8/magnus/docker_utils.py` & `magnus-0.4.9/magnus/docker_utils.py`

 * *Files identical despite different names*

### Comparing `magnus-0.4.8/magnus/exceptions.py` & `magnus-0.4.9/magnus/exceptions.py`

 * *Files identical despite different names*

### Comparing `magnus-0.4.8/magnus/executor.py` & `magnus-0.4.9/magnus/executor.py`

 * *Files identical despite different names*

### Comparing `magnus-0.4.8/magnus/experiment_tracker.py` & `magnus-0.4.9/magnus/experiment_tracker.py`

 * *Files identical despite different names*

### Comparing `magnus-0.4.8/magnus/graph.py` & `magnus-0.4.9/magnus/graph.py`

 * *Files identical despite different names*

### Comparing `magnus-0.4.8/magnus/integration.py` & `magnus-0.4.9/magnus/integration.py`

 * *Files identical despite different names*

### Comparing `magnus-0.4.8/magnus/names.py` & `magnus-0.4.9/magnus/names.py`

 * *Files identical despite different names*

### Comparing `magnus-0.4.8/magnus/nodes.py` & `magnus-0.4.9/magnus/nodes.py`

 * *Files identical despite different names*

### Comparing `magnus-0.4.8/magnus/pickler.py` & `magnus-0.4.9/magnus/pickler.py`

 * *Files identical despite different names*

### Comparing `magnus-0.4.8/magnus/pipeline.py` & `magnus-0.4.9/magnus/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import json
 import logging
-from typing import Optional, Union
+from typing import Union
 
-from magnus import defaults, exceptions, graph, utils
+from magnus import context, defaults, exceptions, graph, utils
 
 logger = logging.getLogger(defaults.NAME)
 
-# Set this global executor to the fitted executor for access later
-global_executor = None  # pylint: disable=invalid-name # type: ignore
-
 
 def get_default_configs() -> dict:
     """
     User can provide extensions as part of their code base, magnus-config.yaml provides the place to put them.
     """
     user_configs = {}
     if utils.does_file_exist(defaults.USER_CONFIG_FILE):
@@ -30,15 +27,16 @@
 
 def prepare_configurations(
         configuration_file: str = None,
         pipeline_file: str = None,
         run_id: str = None,
         tag: Union[str, None] = None,
         use_cached: Union[str, None] = '',
-        parameters_file: str = None):
+        parameters_file: str = None,
+        force_local_executor: bool = False):
     # pylint: disable=R0914
     """
     Replace the placeholders in the dag/config against the variables file.
 
     Attach the secrets_handler, run_log_store, catalog_handler to the executor and return it.
 
     Args:
@@ -84,14 +82,17 @@
     tracker_config = configuration.get('experiment_tracking', {})
     if not tracker_config:
         tracker_config = magnus_defaults.get('experiment_tracking', defaults.DEFAULT_EXPERIMENT_TRACKER)
     tracker_handler = utils.get_provider_by_name_and_type('experiment_tracking', tracker_config)
 
     # Mode configurations, configuration over rides everything
     mode_config = configuration.get('mode', {})
+    if force_local_executor:
+        mode_config = {'type': 'local'}
+
     if not mode_config:
         mode_config = magnus_defaults.get('executor', defaults.DEFAULT_EXECUTOR)
     mode_executor = utils.get_provider_by_name_and_type('executor', mode_config)
 
     if pipeline_file:
         # There are use cases where we are only preparing the executor
         pipeline_config = utils.load_yaml(pipeline_file)
@@ -111,16 +112,15 @@
         mode_executor.dag_hash = dag_hash
 
     mode_executor.run_id = run_id
     mode_executor.tag = tag
     mode_executor.use_cached = use_cached
 
     # Set a global executor for inter-module access later
-    global global_executor  # pylint: disable=W0603,invalid-name,
-    global_executor = mode_executor
+    context.executor = mode_executor
 
     mode_executor.run_log_store = run_log_store
     mode_executor.catalog_handler = catalog_handler
     mode_executor.secrets_handler = secrets_handler
     mode_executor.experiment_tracker = tracker_handler
     mode_executor.configuration_file = configuration_file
     mode_executor.parameters_file = parameters_file
```

### Comparing `magnus-0.4.8/magnus/sdk.py` & `magnus-0.4.9/magnus/sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,98 +9,98 @@
 
 from magnus import defaults, exceptions, graph, nodes, pipeline, utils
 from magnus.interaction import get_tag
 
 logger = logging.getLogger(defaults.NAME)
 
 
-class step(object):
+# class step(object):
 
-    def __init__(
-            self, name: Union[str, FunctionType],
-            catalog_config: dict = None, magnus_config: str = None,
-            parameters_file: str = None):
-        """
-        This decorator could be used to make the function within the scope of magnus.
-
-        Since we are not orchestrating, it is expected that resource management happens outside this scope.
-
-        Args:
-            name (str, callable): The name of the step. The step log would have the same name
-            catalog_config (dict): The configuration of the catalog per step.
-            magnus_config (str): The name of the file having the magnus config, defaults to None.
-        """
-        if isinstance(name, FunctionType):
-            name = name()
-
-        self.name = name
-        self.catalog_config = catalog_config
-        self.active = True  # Check if we are executing the function via pipeline
-
-        if pipeline.global_executor \
-                and pipeline.global_executor.execution_plan == defaults.EXECUTION_PLAN.CHAINED.value:
-            self.active = False
-            return
-
-        self.executor = pipeline.prepare_configurations(
-            configuration_file=magnus_config, parameters_file=parameters_file)
-
-        self.executor.execution_plan = defaults.EXECUTION_PLAN.UNCHAINED.value
-        run_id = self.executor.step_decorator_run_id
-        if not run_id:
-            msg = (
-                f'Step decorator expects run id from environment.'
-            )
-            raise Exception(msg)
-
-        self.executor.run_id = run_id
-        utils.set_magnus_environment_variables(run_id=run_id, configuration_file=magnus_config, tag=get_tag())
-
-        try:
-            # Try to get it if previous steps have created it
-            # TODO: Can call the set_up_runlog now.
-            run_log = self.executor.run_log_store.get_run_log_by_id(self.executor.run_id)
-            if run_log.status in [defaults.FAIL, defaults.SUCCESS]:  # TODO: Remove this in preference to defaults
-                """
-                This check is mostly useless as we do not know when the graph ends as they are created dynamically.
-                This only prevents from using a run_id which has reached a final state.
-                #TODO: There is a need to create a status called step_success
-                """
-                msg = (
-                    f'The run_log for run_id: {run_id} already exists and is in {run_log.status} state.'
-                    ' Make sure that this was not run before.'
-                )
-                raise Exception(msg)
-        except exceptions.RunLogNotFoundError:
-            # Create one if they are not created
-            self.executor._set_up_run_log()
-
-    def __call__(self, func):
-        """
-        The function is converted into a node and called via the magnus framework.
-        """
-        @functools.wraps(func)
-        def wrapped_f(*args, **kwargs):
-            if not self.active:
-                # If we are not running via decorator, execute the function
-                return func(*args, **kwargs)
-
-            step_config = {
-                'command': func,
-                'command_type': 'python-function',
-                'type': 'task',
-                'next': 'not defined',
-                'catalog': self.catalog_config
-            }
-            node = graph.create_node(name=self.name, step_config=step_config)
-            self.executor.execute_from_graph(node=node)
-            run_log = self.executor.run_log_store.get_run_log_by_id(run_id=self.executor.run_id, full=False)
-            # TODO: If the previous step succeeded, make the status of the run log step_success
-            print(json.dumps(run_log.dict(), indent=4))
-        return wrapped_f
+#     def __init__(
+#             self, name: Union[str, FunctionType],
+#             catalog_config: dict = None, magnus_config: str = None,
+#             parameters_file: str = None):
+#         """
+#         This decorator could be used to make the function within the scope of magnus.
+
+#         Since we are not orchestrating, it is expected that resource management happens outside this scope.
+
+#         Args:
+#             name (str, callable): The name of the step. The step log would have the same name
+#             catalog_config (dict): The configuration of the catalog per step.
+#             magnus_config (str): The name of the file having the magnus config, defaults to None.
+#         """
+#         if isinstance(name, FunctionType):
+#             name = name()
+
+#         self.name = name
+#         self.catalog_config = catalog_config
+#         self.active = True  # Check if we are executing the function via pipeline
+
+#         if pipeline.global_executor \
+#                 and pipeline.global_executor.execution_plan == defaults.EXECUTION_PLAN.CHAINED.value:
+#             self.active = False
+#             return
+
+#         self.executor = pipeline.prepare_configurations(
+#             configuration_file=magnus_config, parameters_file=parameters_file)
+
+#         self.executor.execution_plan = defaults.EXECUTION_PLAN.UNCHAINED.value
+#         run_id = self.executor.step_decorator_run_id
+#         if not run_id:
+#             msg = (
+#                 f'Step decorator expects run id from environment.'
+#             )
+#             raise Exception(msg)
+
+#         self.executor.run_id = run_id
+#         utils.set_magnus_environment_variables(run_id=run_id, configuration_file=magnus_config, tag=get_tag())
+
+#         try:
+#             # Try to get it if previous steps have created it
+#             # TODO: Can call the set_up_runlog now.
+#             run_log = self.executor.run_log_store.get_run_log_by_id(self.executor.run_id)
+#             if run_log.status in [defaults.FAIL, defaults.SUCCESS]:  # TODO: Remove this in preference to defaults
+#                 """
+#                 This check is mostly useless as we do not know when the graph ends as they are created dynamically.
+#                 This only prevents from using a run_id which has reached a final state.
+#                 #TODO: There is a need to create a status called step_success
+#                 """
+#                 msg = (
+#                     f'The run_log for run_id: {run_id} already exists and is in {run_log.status} state.'
+#                     ' Make sure that this was not run before.'
+#                 )
+#                 raise Exception(msg)
+#         except exceptions.RunLogNotFoundError:
+#             # Create one if they are not created
+#             self.executor._set_up_run_log()
+
+#     def __call__(self, func):
+#         """
+#         The function is converted into a node and called via the magnus framework.
+#         """
+#         @functools.wraps(func)
+#         def wrapped_f(*args, **kwargs):
+#             if not self.active:
+#                 # If we are not running via decorator, execute the function
+#                 return func(*args, **kwargs)
+
+#             step_config = {
+#                 'command': func,
+#                 'command_type': 'python-function',
+#                 'type': 'task',
+#                 'next': 'not defined',
+#                 'catalog': self.catalog_config
+#             }
+#             node = graph.create_node(name=self.name, step_config=step_config)
+#             self.executor.execute_from_graph(node=node)
+#             run_log = self.executor.run_log_store.get_run_log_by_id(run_id=self.executor.run_id, full=False)
+#             # TODO: If the previous step succeeded, make the status of the run log step_success
+#             print(json.dumps(run_log.dict(), indent=4))
+#         return wrapped_f
 
 
 class Task:
     def __init__(self, name: str, command: Union[str, FunctionType], command_type: str = defaults.COMMAND_TYPE,
                  command_config: Optional[dict] = None, catalog: Optional[dict] = None,
                  mode_config: Optional[dict] = None, retry: int = 1, on_failure: str = '',
                  next_node: str = ''):
```

### Comparing `magnus-0.4.8/magnus/secrets.py` & `magnus-0.4.9/magnus/secrets.py`

 * *Files identical despite different names*

### Comparing `magnus-0.4.8/magnus/tasks.py` & `magnus-0.4.9/magnus/tasks.py`

 * *Files identical despite different names*

### Comparing `magnus-0.4.8/magnus/utils.py` & `magnus-0.4.9/magnus/utils.py`

 * *Files identical despite different names*

### Comparing `magnus-0.4.8/pyproject.toml` & `magnus-0.4.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magnus"
-version = "0.4.8"
+version = "0.4.9"
 description = "A Compute agnostic pipelining software"
 authors = ["Vijay Vammi <mesanthu@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/AstraZeneca/magnus-core"
 repository = "https://github.com/AstraZeneca/magnus-core"
 documentation = "https://astrazeneca.github.io/magnus-core/"
@@ -35,14 +35,15 @@
 mkdocs = "*"
 mkdocs-material = "*"
 mypy = "^0.931"
 tox = "^3.24.5"
 pre-commit = "*"
 commit-linter = "^1.0.2"
 python-semantic-release = "^7.33.1"
+ipykernel = "^6.21.2"
 
 [tool.poetry.scripts]
 magnus= 'magnus.cli:cli'
 
 # Plugins for Executors
 [tool.poetry.plugins."magnus.executor.BaseExecutor"]
 "local" = "magnus.executor:LocalExecutor"
```

### Comparing `magnus-0.4.8/PKG-INFO` & `magnus-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnus
-Version: 0.4.8
+Version: 0.4.9
 Summary: A Compute agnostic pipelining software
 Home-page: https://github.com/AstraZeneca/magnus-core
 License: Apache-2.0
 Author: Vijay Vammi
 Author-email: mesanthu@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

