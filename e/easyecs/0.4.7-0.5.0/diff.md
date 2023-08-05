# Comparing `tmp/easyecs-0.4.7.tar.gz` & `tmp/easyecs-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyecs-0.4.7.tar", max compression
+gzip compressed data, was "easyecs-0.5.0.tar", max compression
```

## Comparing `easyecs-0.4.7.tar` & `easyecs-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     2230 2023-08-05 13:13:21.640137 easyecs-0.4.7/README.md
--rw-r--r--   0        0        0        0 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/__init__.py
--rwxr-xr-x   0        0        0     8332 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/cli.py
--rw-r--r--   0        0        0        0 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/cloudformation/__init__.py
--rw-r--r--   0        0        0       90 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/cloudformation/client.py
--rw-r--r--   0        0        0     3522 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/cloudformation/fetch.py
--rw-r--r--   0        0        0        0 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/cloudformation/stack/__init__.py
--rw-r--r--   0        0        0     1921 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/cloudformation/stack/create.py
--rw-r--r--   0        0        0     1131 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/cloudformation/stack/delete.py
--rw-r--r--   0        0        0     3274 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/cloudformation/stack/update.py
--rw-r--r--   0        0        0     8573 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/cloudformation/template/__init__.py
--rw-r--r--   0        0        0    12373 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/command/__init__.py
--rw-r--r--   0        0        0     1393 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/docker/__init__.py
--rw-r--r--   0        0        0        0 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/helpers/__init__.py
--rw-r--r--   0        0        0      264 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/helpers/color.py
--rw-r--r--   0        0        0     2292 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/helpers/common.py
--rw-r--r--   0        0        0     1895 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/helpers/loader.py
--rw-r--r--   0        0        0      531 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/helpers/selector.py
--rw-r--r--   0        0        0     3272 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/helpers/settings.py
--rw-r--r--   0        0        0       42 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/helpers/signal.py
--rw-r--r--   0        0        0     2804 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/model/ecs.py
--rw-r--r--   0        0        0      607 2023-08-05 13:13:21.664137 easyecs-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 easyecs-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     2230 2023-08-05 13:23:54.112800 easyecs-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-08-05 13:23:54.128800 easyecs-0.5.0/easyecs/__init__.py
+-rwxr-xr-x   0        0        0     9052 2023-08-05 13:23:54.128800 easyecs-0.5.0/easyecs/cli.py
+-rw-r--r--   0        0        0        0 2023-08-05 13:23:54.128800 easyecs-0.5.0/easyecs/cloudformation/__init__.py
+-rw-r--r--   0        0        0       90 2023-08-05 13:23:54.128800 easyecs-0.5.0/easyecs/cloudformation/client.py
+-rw-r--r--   0        0        0     3522 2023-08-05 13:23:54.128800 easyecs-0.5.0/easyecs/cloudformation/fetch.py
+-rw-r--r--   0        0        0        0 2023-08-05 13:23:54.128800 easyecs-0.5.0/easyecs/cloudformation/stack/__init__.py
+-rw-r--r--   0        0        0     1921 2023-08-05 13:23:54.128800 easyecs-0.5.0/easyecs/cloudformation/stack/create.py
+-rw-r--r--   0        0        0     1131 2023-08-05 13:23:54.128800 easyecs-0.5.0/easyecs/cloudformation/stack/delete.py
+-rw-r--r--   0        0        0     3274 2023-08-05 13:23:54.128800 easyecs-0.5.0/easyecs/cloudformation/stack/update.py
+-rw-r--r--   0        0        0     8573 2023-08-05 13:23:54.128800 easyecs-0.5.0/easyecs/cloudformation/template/__init__.py
+-rw-r--r--   0        0        0    12373 2023-08-05 13:23:54.128800 easyecs-0.5.0/easyecs/command/__init__.py
+-rw-r--r--   0        0        0     1897 2023-08-05 13:23:54.128800 easyecs-0.5.0/easyecs/docker/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 13:23:54.128800 easyecs-0.5.0/easyecs/helpers/__init__.py
+-rw-r--r--   0        0        0      264 2023-08-05 13:23:54.128800 easyecs-0.5.0/easyecs/helpers/color.py
+-rw-r--r--   0        0        0     2292 2023-08-05 13:23:54.128800 easyecs-0.5.0/easyecs/helpers/common.py
+-rw-r--r--   0        0        0     1895 2023-08-05 13:23:54.128800 easyecs-0.5.0/easyecs/helpers/loader.py
+-rw-r--r--   0        0        0      531 2023-08-05 13:23:54.128800 easyecs-0.5.0/easyecs/helpers/selector.py
+-rw-r--r--   0        0        0     3272 2023-08-05 13:23:54.128800 easyecs-0.5.0/easyecs/helpers/settings.py
+-rw-r--r--   0        0        0       42 2023-08-05 13:23:54.128800 easyecs-0.5.0/easyecs/helpers/signal.py
+-rw-r--r--   0        0        0     2804 2023-08-05 13:23:54.128800 easyecs-0.5.0/easyecs/model/ecs.py
+-rw-r--r--   0        0        0      607 2023-08-05 13:23:54.128800 easyecs-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 easyecs-0.5.0/PKG-INFO
```

### Comparing `easyecs-0.4.7/README.md` & `easyecs-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.7/easyecs/cli.py` & `easyecs-0.5.0/easyecs/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,25 +53,26 @@
     ecs_manifest,
     stack_name,
     aws_account_id,
     aws_region,
     vpc_id,
     subnet_ids,
     azs,
+    show_docker_logs,
     run,
 ):
     if not no_docker_build:
         loader_docker = Loader(
             "Building and pushing docker images:",
             "Building and pushing docker images: \u2705",
             "Building and pushing docker images: \u274c",
             0.05,
         )
         loader_docker.start()
-        build_docker_image(ecs_manifest)
+        build_docker_image(ecs_manifest, show_docker_logs)
         loader_docker.stop()
 
     loader = Loader(
         "Creating CloudFormation template:",
         "Creating CloudFormation template: \u2705",
         "Creating CloudFormation template: \u274c",
         0.05,
@@ -132,39 +133,42 @@
     aws_account_id,
     aws_region,
     vpc_id,
     subnet_ids,
     azs,
     force_redeployment,
     aws_account,
+    show_docker_logs,
     run,
 ):
     print()
     if has_ecs_file_changed(cache_settings) or force_redeployment:
         step_import_aws_cdk()
         step_docker_build_and_push(
             no_docker_build,
             ecs_manifest,
             stack_name,
             aws_account_id,
             aws_region,
             vpc_id,
             subnet_ids,
             azs,
+            show_docker_logs,
             run,
         )
         step_create_or_update_stack(stack_name, force_redeployment)
         save_hash(aws_account)
     else:
         print(f"{Color.YELLOW}No updates are to be performed.{Color.END}")
 
 
 def action_run(ctx):
     no_docker_build = ctx.obj["no_docker_build"]
     force_redeployment = ctx.obj["force_redeployment"]
+    show_docker_logs = ctx.obj["show_docker_logs"]
     aws_account = fetch_aws_account()
     cache_settings = load_settings(aws_account)
     ecs_manifest = read_ecs_file()
     app_name = ecs_manifest.metadata.appname
     user = ecs_manifest.metadata.user
     aws_region = cache_settings["aws_region"]
     aws_account_id = cache_settings["aws_account_id"]
@@ -181,14 +185,15 @@
         aws_account_id,
         aws_region,
         vpc_id,
         subnet_ids,
         azs,
         force_redeployment,
         aws_account,
+        show_docker_logs,
         run=True,
     )
     parsed_containers = fetch_containers(user, app_name)
     print()
     create_port_forwards(ecs_manifest, aws_region, aws_account, parsed_containers)
     step_idle_keyboard()
 
@@ -196,14 +201,15 @@
 
     exit(0)
 
 
 def action_dev(ctx):
     no_docker_build = ctx.obj["no_docker_build"]
     force_redeployment = ctx.obj["force_redeployment"]
+    show_docker_logs = ctx.obj["show_docker_logs"]
     aws_account = fetch_aws_account()
     cache_settings = load_settings(aws_account)
     ecs_manifest = read_ecs_file()
     app_name = ecs_manifest.metadata.appname
     user = ecs_manifest.metadata.user
     aws_region = cache_settings["aws_region"]
     aws_account_id = cache_settings["aws_account_id"]
@@ -220,14 +226,15 @@
         aws_account_id,
         aws_region,
         vpc_id,
         subnet_ids,
         azs,
         force_redeployment,
         aws_account,
+        show_docker_logs,
         run=False,
     )
     parsed_containers = fetch_containers(user, app_name)
     print()
     create_port_forwards(ecs_manifest, aws_region, aws_account, parsed_containers)
     run_nc_commands(parsed_containers, aws_region, aws_account, ecs_manifest)
     run_sync_thread(parsed_containers, ecs_manifest)
@@ -280,18 +287,26 @@
     default=False,
     show_default=True,
     help=(
         "If used, and only when there's no update on the cloudformation stack, easyecs"
         " will force a new deployment of the task."
     ),
 )
+@click.option(
+    "--show-docker-logs",
+    is_flag=True,
+    default=False,
+    show_default=True,
+    help="If used, it will show the docker build and push logs",
+)
 @click.pass_context
-def click_run(ctx, no_docker_build, force_redeployment):
+def click_run(ctx, no_docker_build, force_redeployment, show_docker_logs):
     ctx.obj["no_docker_build"] = no_docker_build
     ctx.obj["force_redeployment"] = force_redeployment
+    ctx.obj["show_docker_logs"] = show_docker_logs
     action_run(ctx)
 
 
 @entrypoint.command(name="dev", help="Run a stack in development mode")
 @click.option(
     "--no-docker-build",
     is_flag=True,
@@ -308,18 +323,26 @@
     default=False,
     show_default=True,
     help=(
         "If used, and only when there's no update on the cloudformation stack, easyecs"
         " will force a new deployment of the task."
     ),
 )
+@click.option(
+    "--show-docker-logs",
+    is_flag=True,
+    default=False,
+    show_default=True,
+    help="If used, it will show the docker build and push logs",
+)
 @click.pass_context
-def click_dev(ctx, no_docker_build, force_redeployment):
+def click_dev(ctx, no_docker_build, force_redeployment, show_docker_logs):
     ctx.obj["no_docker_build"] = no_docker_build
     ctx.obj["force_redeployment"] = force_redeployment
+    ctx.obj["show_docker_logs"] = show_docker_logs
     action_dev(ctx)
 
 
 @entrypoint.command(name="delete", help="Delete a stack")
 @click.pass_context
 def click_delete(ctx):
     action_delete(ctx)
```

### Comparing `easyecs-0.4.7/easyecs/cloudformation/fetch.py` & `easyecs-0.5.0/easyecs/cloudformation/fetch.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.7/easyecs/cloudformation/stack/create.py` & `easyecs-0.5.0/easyecs/cloudformation/stack/create.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.7/easyecs/cloudformation/stack/delete.py` & `easyecs-0.5.0/easyecs/cloudformation/stack/delete.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.7/easyecs/cloudformation/stack/update.py` & `easyecs-0.5.0/easyecs/cloudformation/stack/update.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.7/easyecs/cloudformation/template/__init__.py` & `easyecs-0.5.0/easyecs/cloudformation/template/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.7/easyecs/command/__init__.py` & `easyecs-0.5.0/easyecs/command/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.7/easyecs/helpers/common.py` & `easyecs-0.5.0/easyecs/helpers/common.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.7/easyecs/helpers/loader.py` & `easyecs-0.5.0/easyecs/helpers/loader.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.7/easyecs/helpers/selector.py` & `easyecs-0.5.0/easyecs/helpers/selector.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.7/easyecs/helpers/settings.py` & `easyecs-0.5.0/easyecs/helpers/settings.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.7/easyecs/model/ecs.py` & `easyecs-0.5.0/easyecs/model/ecs.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.7/pyproject.toml` & `easyecs-0.5.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easyecs"
-version = "0.4.7"
+version = "0.5.0"
 description = ""
 authors = ["BONVARLET Benjamin <benjaminbonvarlet96@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.6"
```

### Comparing `easyecs-0.4.7/PKG-INFO` & `easyecs-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyecs
-Version: 0.4.7
+Version: 0.5.0
 Summary: 
 Author: BONVARLET Benjamin
 Author-email: benjaminbonvarlet96@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

