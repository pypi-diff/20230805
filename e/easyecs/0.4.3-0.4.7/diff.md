# Comparing `tmp/easyecs-0.4.3.tar.gz` & `tmp/easyecs-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyecs-0.4.3.tar", max compression
+gzip compressed data, was "easyecs-0.4.7.tar", max compression
```

## Comparing `easyecs-0.4.3.tar` & `easyecs-0.4.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     2230 2023-08-03 11:55:08.399009 easyecs-0.4.3/README.md
--rw-r--r--   0        0        0        0 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/__init__.py
--rwxr-xr-x   0        0        0     8332 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/cli.py
--rw-r--r--   0        0        0        0 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/cloudformation/__init__.py
--rw-r--r--   0        0        0       90 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/cloudformation/client.py
--rw-r--r--   0        0        0     3522 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/cloudformation/fetch.py
--rw-r--r--   0        0        0        0 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/cloudformation/stack/__init__.py
--rw-r--r--   0        0        0     1921 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/cloudformation/stack/create.py
--rw-r--r--   0        0        0     1131 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/cloudformation/stack/delete.py
--rw-r--r--   0        0        0     3274 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/cloudformation/stack/update.py
--rw-r--r--   0        0        0     8573 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/cloudformation/template/__init__.py
--rw-r--r--   0        0        0    12418 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/command/__init__.py
--rw-r--r--   0        0        0     1386 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/docker/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/helpers/__init__.py
--rw-r--r--   0        0        0      264 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/helpers/color.py
--rw-r--r--   0        0        0     2292 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/helpers/common.py
--rw-r--r--   0        0        0     1895 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/helpers/loader.py
--rw-r--r--   0        0        0      531 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/helpers/selector.py
--rw-r--r--   0        0        0     3272 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/helpers/settings.py
--rw-r--r--   0        0        0       42 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/helpers/signal.py
--rw-r--r--   0        0        0     2804 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/model/ecs.py
--rw-r--r--   0        0        0      607 2023-08-03 11:55:08.423010 easyecs-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 easyecs-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     2230 2023-08-05 13:13:21.640137 easyecs-0.4.7/README.md
+-rw-r--r--   0        0        0        0 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/__init__.py
+-rwxr-xr-x   0        0        0     8332 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/cli.py
+-rw-r--r--   0        0        0        0 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/cloudformation/__init__.py
+-rw-r--r--   0        0        0       90 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/cloudformation/client.py
+-rw-r--r--   0        0        0     3522 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/cloudformation/fetch.py
+-rw-r--r--   0        0        0        0 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/cloudformation/stack/__init__.py
+-rw-r--r--   0        0        0     1921 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/cloudformation/stack/create.py
+-rw-r--r--   0        0        0     1131 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/cloudformation/stack/delete.py
+-rw-r--r--   0        0        0     3274 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/cloudformation/stack/update.py
+-rw-r--r--   0        0        0     8573 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/cloudformation/template/__init__.py
+-rw-r--r--   0        0        0    12373 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/command/__init__.py
+-rw-r--r--   0        0        0     1393 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/docker/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/helpers/__init__.py
+-rw-r--r--   0        0        0      264 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/helpers/color.py
+-rw-r--r--   0        0        0     2292 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/helpers/common.py
+-rw-r--r--   0        0        0     1895 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/helpers/loader.py
+-rw-r--r--   0        0        0      531 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/helpers/selector.py
+-rw-r--r--   0        0        0     3272 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/helpers/settings.py
+-rw-r--r--   0        0        0       42 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/helpers/signal.py
+-rw-r--r--   0        0        0     2804 2023-08-05 13:13:21.660137 easyecs-0.4.7/easyecs/model/ecs.py
+-rw-r--r--   0        0        0      607 2023-08-05 13:13:21.664137 easyecs-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 easyecs-0.4.7/PKG-INFO
```

### Comparing `easyecs-0.4.3/README.md` & `easyecs-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.3/easyecs/cli.py` & `easyecs-0.4.7/easyecs/cli.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.3/easyecs/cloudformation/fetch.py` & `easyecs-0.4.7/easyecs/cloudformation/fetch.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.3/easyecs/cloudformation/stack/create.py` & `easyecs-0.4.7/easyecs/cloudformation/stack/create.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.3/easyecs/cloudformation/stack/delete.py` & `easyecs-0.4.7/easyecs/cloudformation/stack/delete.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.3/easyecs/cloudformation/stack/update.py` & `easyecs-0.4.7/easyecs/cloudformation/stack/update.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.3/easyecs/cloudformation/template/__init__.py` & `easyecs-0.4.7/easyecs/cloudformation/template/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.3/easyecs/command/__init__.py` & `easyecs-0.4.7/easyecs/command/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,23 +69,15 @@
                 "host": ["localhost"],
                 "portNumber": [port_number],
                 "localPortNumber": [local_port_number],
             },
         )
         # It has to be done like that, in a new session.
         # Otherwise a CTRL+C would kill all port forwards.
-        ssm_cmd = [
-            "session-manager-plugin",
-            json.dumps(ssm_response),
-            aws_region,
-            "StartSession",
-            aws_account,
-            json.dumps(dict(Target=target)),
-            "https://ssm.eu-west-1.amazonaws.com",
-        ]
+        ssm_cmd = generate_ssm_cmd(ssm_response, aws_region, aws_account, target)
         process = subprocess.Popen(
             ssm_cmd,
             start_new_session=True,
             stdin=subprocess.PIPE,
             stdout=subprocess.DEVNULL,
         )
         popen_procs_port_forward.append(process)
@@ -235,14 +227,26 @@
             if not proc_nc_server.poll():
                 proc_nc_server.wait()
                 break
             time.sleep(0.1)
     return found_tty
 
 
+def generate_ssm_cmd(ssm_nc_server, aws_region, aws_account, target):
+    return [
+        "session-manager-plugin",
+        json.dumps(ssm_nc_server),
+        aws_region,
+        "StartSession",
+        aws_account,
+        json.dumps(dict(Target=target)),
+        f"https://ssm.{aws_region}.amazonaws.com",
+    ]
+
+
 def run_nc_command(parsed_containers, aws_region, aws_account, container_name):
     random_port = generate_random_port()
     parsed_containers[container_name]["netcat_port"] = random_port
     port_forward(
         parsed_containers,
         container_name,
         random_port,
@@ -258,23 +262,15 @@
     ]
     parameters_nc_server = {"command": command_server}
     ssm_nc_server = client.start_session(
         Target=target,
         DocumentName="AWS-StartInteractiveCommand",
         Parameters=parameters_nc_server,
     )
-    cmd_nc_server = [
-        "session-manager-plugin",
-        json.dumps(ssm_nc_server),
-        aws_region,
-        "StartSession",
-        aws_account,
-        json.dumps(dict(Target=target)),
-        "https://ssm.eu-west-1.amazonaws.com",
-    ]
+    cmd_nc_server = generate_ssm_cmd(ssm_nc_server, aws_region, aws_account, target)
     proc_nc_server = subprocess.Popen(
         cmd_nc_server,
         start_new_session=True,
         stdin=subprocess.PIPE,
         stdout=subprocess.DEVNULL,
     )
     popen_procs_port_forward.append(proc_nc_server)
```

### Comparing `easyecs-0.4.3/easyecs/docker/__init__.py` & `easyecs-0.4.7/easyecs/docker/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 import subprocess
 from easyecs.helpers.common import parse_dict_with_env_var
 
 
+def docker_build_cmd(build, image_name):
+    dockerfile = build.dockerfile
+    target = build.target
+    if target:
+        target = f"--target {target}"
+    build_args = build.args
+    build_args = parse_dict_with_env_var(build_args)
+    build_args_str = " ".join(
+        [f'--build-arg {key}="{value}"' for key, value in build_args.items()]
+    )
+    build_cmd = f"docker build -t {image_name}"
+    if dockerfile:
+        build_cmd += f" -f {dockerfile}"
+    if target:
+        build_cmd += f" {target}"
+    if build.args:
+        build_cmd += f" {build_args_str}"
+    build_cmd += " ."
+    return build_cmd
+
+
 def build_docker_image(ecs_manifest):
     containers = ecs_manifest.task_definition.containers
     for container in containers:
         image_name = container.image
         build = container.build
         if build:
-            dockerfile = build.dockerfile
-            if dockerfile:
-                dockerfile = f"-f {dockerfile}"
-            target = build.target
-            if target:
-                target = f"--target {target}"
-            build_args = build.args
-            build_args = parse_dict_with_env_var(build_args)
-            build_args_str = " ".join(
-                [f'--build-arg {key}="{value}"' for key, value in build_args.items()]
-            )
-            build_cmd = f"docker build -t {image_name} {dockerfile}"
-            if target:
-                build_cmd += f" {target}"
-            build_cmd += f" {build_args_str}"
-            build_cmd += " ."
+            build_cmd = docker_build_cmd(build, image_name)
             res = subprocess.Popen(
                 build_cmd,
                 shell=True,
             )
             res.wait()
             if res.poll() != 0:
                 raise Exception("There was an issue building the docker image")
```

### Comparing `easyecs-0.4.3/easyecs/helpers/common.py` & `easyecs-0.4.7/easyecs/helpers/common.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.3/easyecs/helpers/loader.py` & `easyecs-0.4.7/easyecs/helpers/loader.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.3/easyecs/helpers/selector.py` & `easyecs-0.4.7/easyecs/helpers/selector.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.3/easyecs/helpers/settings.py` & `easyecs-0.4.7/easyecs/helpers/settings.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.3/easyecs/model/ecs.py` & `easyecs-0.4.7/easyecs/model/ecs.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.3/pyproject.toml` & `easyecs-0.4.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easyecs"
-version = "0.4.3"
+version = "0.4.7"
 description = ""
 authors = ["BONVARLET Benjamin <benjaminbonvarlet96@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.6"
```

### Comparing `easyecs-0.4.3/PKG-INFO` & `easyecs-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyecs
-Version: 0.4.3
+Version: 0.4.7
 Summary: 
 Author: BONVARLET Benjamin
 Author-email: benjaminbonvarlet96@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

