# Comparing `tmp/kedro-prefect-oliver-0.1.8.tar.gz` & `tmp/kedro-prefect-oliver-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-prefect-oliver-0.1.8.tar", last modified: Wed Jun  7 20:55:59 2023, max compression
+gzip compressed data, was "kedro-prefect-oliver-0.1.9.tar", last modified: Thu Jun 22 01:00:20 2023, max compression
```

## Comparing `kedro-prefect-oliver-0.1.8.tar` & `kedro-prefect-oliver-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-07 20:55:59.212405 kedro-prefect-oliver-0.1.8/
--rw-rw-rw-   0 root         (0) root         (0)     1140 2023-06-07 20:55:43.000000 kedro-prefect-oliver-0.1.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      577 2023-06-07 20:55:59.212405 kedro-prefect-oliver-0.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4582 2023-06-07 20:55:43.000000 kedro-prefect-oliver-0.1.8/README
--rw-rw-rw-   0 root         (0) root         (0)     5684 2023-06-07 20:55:43.000000 kedro-prefect-oliver-0.1.8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-07 20:55:59.212405 kedro-prefect-oliver-0.1.8/setup.cfg
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-07 20:55:59.212405 kedro-prefect-oliver-0.1.8/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-07 20:55:59.212405 kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver/
--rw-rw-rw-   0 root         (0) root         (0)      122 2023-06-07 20:55:43.000000 kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1979 2023-06-07 20:55:43.000000 kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver/infrastructure.py
--rw-rw-rw-   0 root         (0) root         (0)    14741 2023-06-07 20:55:43.000000 kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver/register.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-07 20:55:59.212405 kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)      577 2023-06-07 20:55:59.000000 kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-06-07 20:55:59.000000 kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-07 20:55:59.000000 kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      366 2023-06-07 20:55:59.000000 kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-07 20:55:59.000000 kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 01:00:20.593423 kedro-prefect-oliver-0.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1140 2023-06-22 01:00:00.000000 kedro-prefect-oliver-0.1.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      577 2023-06-22 01:00:20.593423 kedro-prefect-oliver-0.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4582 2023-06-22 01:00:00.000000 kedro-prefect-oliver-0.1.9/README
+-rw-rw-rw-   0 root         (0) root         (0)     5684 2023-06-22 01:00:00.000000 kedro-prefect-oliver-0.1.9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-22 01:00:20.593423 kedro-prefect-oliver-0.1.9/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 01:00:20.589422 kedro-prefect-oliver-0.1.9/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 01:00:20.593423 kedro-prefect-oliver-0.1.9/src/kedro_prefect_oliver/
+-rw-rw-rw-   0 root         (0) root         (0)      122 2023-06-22 01:00:00.000000 kedro-prefect-oliver-0.1.9/src/kedro_prefect_oliver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1979 2023-06-22 01:00:00.000000 kedro-prefect-oliver-0.1.9/src/kedro_prefect_oliver/infrastructure.py
+-rw-rw-rw-   0 root         (0) root         (0)    14945 2023-06-22 01:00:00.000000 kedro-prefect-oliver-0.1.9/src/kedro_prefect_oliver/register.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 01:00:20.593423 kedro-prefect-oliver-0.1.9/src/kedro_prefect_oliver.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)      577 2023-06-22 01:00:20.000000 kedro-prefect-oliver-0.1.9/src/kedro_prefect_oliver.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-06-22 01:00:20.000000 kedro-prefect-oliver-0.1.9/src/kedro_prefect_oliver.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-22 01:00:20.000000 kedro-prefect-oliver-0.1.9/src/kedro_prefect_oliver.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      366 2023-06-22 01:00:20.000000 kedro-prefect-oliver-0.1.9/src/kedro_prefect_oliver.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-22 01:00:20.000000 kedro-prefect-oliver-0.1.9/src/kedro_prefect_oliver.egg-info/top_level.txt
```

### Comparing `kedro-prefect-oliver-0.1.8/LICENSE` & `kedro-prefect-oliver-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kedro-prefect-oliver-0.1.8/PKG-INFO` & `kedro-prefect-oliver-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-prefect-oliver
-Version: 0.1.8
+Version: 0.1.9
 Summary: Kedro-Prefect integration library
 Author-email: Oliver OTL <dev@olivetreeholdings.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `kedro-prefect-oliver-0.1.8/README` & `kedro-prefect-oliver-0.1.9/README`

 * *Files identical despite different names*

### Comparing `kedro-prefect-oliver-0.1.8/pyproject.toml` & `kedro-prefect-oliver-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name =  "kedro-prefect-oliver"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
     {name = "Oliver OTL", email = "dev@olivetreeholdings.com"},
 ]
 description = "Kedro-Prefect integration library"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver/infrastructure.py` & `kedro-prefect-oliver-0.1.9/src/kedro_prefect_oliver/infrastructure.py`

 * *Files identical despite different names*

### Comparing `kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver/register.py` & `kedro-prefect-oliver-0.1.9/src/kedro_prefect_oliver/register.py`

 * *Files 10% similar despite different names*

```diff
@@ -118,27 +118,21 @@
 
     # return tasks as it is mutated. We want to make this obvious to the user.
     return node_task, tasks  # type: ignore[return-value]
 
 
 @task
 def run_kedro_task(
-    kedro_task: Union[KedroInitTask, KedroTask],
+    kedro_task: KedroTask,
     task_dict: Union[None, Dict[str, Union[DataCatalog, str]]] = None,
-) -> Union[Dict[str, Union[DataCatalog, str]], None]:
+) -> Union[Dict[str, Union[DataCatalog, str]], bool]:
     """Run a Kedro node as a Prefect task."""
-    if task_dict is None:
-        get_run_logger().info("Initializing Kedro session")
-        task_dict = kedro_task.run()
-        return task_dict
-    else:
-        print("Running Kedro node")
-        get_run_logger().info("Running node %s", kedro_task._node.name)
-        kedro_task.run(task_dict)
-        return None
+    get_run_logger().info("Running node %s", kedro_task._node.name)
+    kedro_task.run(task_dict)
+    return True
 
 
 def init_kedro_nodes(
     pipeline_name: str, env: str
 ) -> Dict[
     str,
     Union[
@@ -180,24 +174,24 @@
     )
 
     return {"init_task": init_task, "tasks": tasks}
 
 
 @flow(task_runner=SequentialTaskRunner(), validate_parameters=False, log_prints=False)
 def create_pipeline(
-    pipeline_name: str, env: str, task_retries: int, task_retry_delay: int
+    pipeline_name: str, env: str, task_retries: int, task_retry_delay: int, **kwargs
 ) -> None:
     """Create a Prefect flow from a Kedro pipeline."""
-
+    persist_result = kwargs.get("persist_task_result", None)
     kedro_tasks = init_kedro_nodes(pipeline_name, env)
     init_task = kedro_tasks["init_task"]
     tasks = kedro_tasks["tasks"]
 
-    run_kedro_init_task = run_kedro_task.with_options(name=init_task.name)
-    task_dict = run_kedro_init_task.submit(init_task)
+    get_run_logger().info("Initializing Kedro session")
+    task_dict = init_task.run()
     task_dependencies = {
         kedro_task["task"]: kedro_task["parent_tasks"] for kedro_task in tasks.values()
     }
     todo_nodes = set([kedro_task["task"] for kedro_task in tasks.values()])
     submitted_tasks: Dict[KedroTask, prefect.Task] = {}
     while True:
         ready = {
@@ -207,14 +201,15 @@
         }
         todo_nodes -= ready
         for node in ready:
             run_kedro_node_task = run_kedro_task.with_options(
                 name=node.name,
                 retries=task_retries,
                 retry_delay_seconds=task_retry_delay,
+                persist_result=persist_result,
             )
             future = run_kedro_node_task.submit(
                 node,
                 task_dict,
                 wait_for=[submitted_tasks[t] for t in task_dependencies[node]],
             )
             submitted_tasks[node] = future
@@ -293,14 +288,15 @@
     anchor_date: str = None,
     rrule_string: str = None,
     cron_string: str = None,
     day_or: bool = True,
     timezone: str = "America/New_York",
     task_retries: int = 0,
     task_retry_delay: int = 0,
+    persist_task_result: bool = None,
     env_vars: Dict[str, str] = None,
 ) -> None:
     """Deploy a Kedro pipeline as a Prefect flow."""
 
     kedro_pipeline = kedro_pipeline or "__default__"
     env_vars = env_vars or {}
     # get the dependencies and installs
@@ -330,20 +326,23 @@
     kubernetes_job = KubernetesJob.load(job_name)
 
     parameters = {
         "pipeline_name": kedro_pipeline,
         "env": env,
         "task_retries": task_retries,
         "task_retry_delay": task_retry_delay,
+        "persist_task_result": persist_task_result,
     }
 
     deployment = Deployment.build_from_flow(
         entrypoint=entrypoint,
         flow=create_pipeline.with_options(
-            name=f"{kedro_package}.{kedro_pipeline}", version=version
+            name=f"{kedro_package}.{kedro_pipeline}",
+            version=version,
+            persist_result=persist_task_result,
         ),
         name="kubernetes-job",
         work_queue_name="kubernetes",
         tags=["kubernetes", "kedro"] + tags or [],
         storage=gcs_block,
         infrastructure=kubernetes_job,
         parameters=parameters,
@@ -420,14 +419,20 @@
 @click.option(
     "--task_retry_delay",
     type=int,
     default=0,
     help="Number of seconds to wait between task retries",
 )
 @click.option(
+    "--persist_task_result",
+    type=bool,
+    default=None,
+    help="Persist the result of the task to the Prefect backend",
+)
+@click.option(
     "--env_vars",
     type=str,
     default=None,
     help="A JSON string of environment variables to pass to the Prefect flow",
 )
 def deploy_prefect_flow(
     project: str,
@@ -442,14 +447,15 @@
     anchor_date: str,
     rrule: str,
     cron: str,
     day_or: bool,
     timezone: str,
     task_retries: int,
     task_retry_delay: int,
+    persist_task_result: bool,
     env_vars: str,
 ) -> None:
     deploy_flow(
         project,
         entrypoint,
         bucket,
         kedro_package,
@@ -461,14 +467,15 @@
         anchor_date,
         rrule,
         cron,
         day_or,
         timezone,
         task_retries,
         task_retry_delay,
+        persist_task_result,
         json.loads(env_vars) if env_vars else None,
     )
 
 
 if __name__ == "__main__":
     print("Deploying Prefect flow...")
     # Standalone mode is false to make the function callable from other scripts
```

### Comparing `kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver.egg-info/PKG-INFO` & `kedro-prefect-oliver-0.1.9/src/kedro_prefect_oliver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-prefect-oliver
-Version: 0.1.8
+Version: 0.1.9
 Summary: Kedro-Prefect integration library
 Author-email: Oliver OTL <dev@olivetreeholdings.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

