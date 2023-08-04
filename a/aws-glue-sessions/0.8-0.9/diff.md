# Comparing `tmp/aws_glue_sessions-0.8-py3-none-any.whl.zip` & `tmp/aws_glue_sessions-0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 52383 bytes, number of entries: 22
+Zip file size: 52790 bytes, number of entries: 22
 -rw-r--r--  2.0 unx     6148 b- defN 21-Jun-03 01:46 aws_glue_interactive_sessions_kernel/.DS_Store
 -rw-r--r--  2.0 unx       88 b- defN 21-Feb-17 19:30 aws_glue_interactive_sessions_kernel/__init__.py
 -rw-r--r--  2.0 unx      401 b- defN 21-Apr-08 04:17 aws_glue_interactive_sessions_kernel/glue_kernel.py
 -rwxr-xr-x  2.0 unx      754 b- defN 21-Jul-07 23:12 aws_glue_interactive_sessions_kernel/install.sh
 -rwxr-xr-x  2.0 unx      633 b- defN 21-Jul-07 23:12 aws_glue_interactive_sessions_kernel/install_local_mac.sh
--rw-r--r--  2.0 unx   326988 b- defN 21-Apr-12 20:33 aws_glue_interactive_sessions_kernel/service-2.json
+-rw-r--r--  2.0 unx   326988 b- defN 21-Jul-23 14:55 aws_glue_interactive_sessions_kernel/service-2.json
 -rw-r--r--  2.0 unx     2427 b- defN 21-Jul-06 18:44 aws_glue_interactive_sessions_kernel/glue_kernel_utils/GlueSessionsConstants.py
--rw-r--r--  2.0 unx     8362 b- defN 21-Jul-06 18:41 aws_glue_interactive_sessions_kernel/glue_kernel_utils/KernelMagics.py
+-rw-r--r--  2.0 unx     8954 b- defN 21-Jul-18 05:52 aws_glue_interactive_sessions_kernel/glue_kernel_utils/KernelMagics.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Feb-17 19:57 aws_glue_interactive_sessions_kernel/glue_kernel_utils/__init__.py
--rw-r--r--  2.0 unx    26960 b- defN 21-Jul-07 04:41 aws_glue_interactive_sessions_kernel/glue_python_kernel/GlueKernel.py
+-rw-r--r--  2.0 unx    27791 b- defN 21-Jul-18 05:50 aws_glue_interactive_sessions_kernel/glue_python_kernel/GlueKernel.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Feb-24 06:41 aws_glue_interactive_sessions_kernel/glue_python_kernel/__init__.py
 -rw-r--r--  2.0 unx      210 b- defN 21-May-05 22:50 aws_glue_interactive_sessions_kernel/glue_python_kernel/kernel.json
--rw-r--r--  2.0 unx    26966 b- defN 21-Jul-07 04:41 aws_glue_interactive_sessions_kernel/glue_scala_kernel/GlueKernel.py
+-rw-r--r--  2.0 unx    27798 b- defN 21-Jul-18 05:48 aws_glue_interactive_sessions_kernel/glue_scala_kernel/GlueKernel.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Feb-17 19:57 aws_glue_interactive_sessions_kernel/glue_scala_kernel/__init__.py
 -rw-r--r--  2.0 unx      206 b- defN 21-May-05 23:18 aws_glue_interactive_sessions_kernel/glue_scala_kernel/kernel.json
--rw-r--r--  2.0 unx       61 b- defN 21-Feb-17 19:30 aws_glue_sessions-0.8.data/data/aws_lambda/handlers.py
--rw-r--r--  2.0 unx       90 b- defN 21-Feb-17 19:30 aws_glue_sessions-0.8.data/data/aws_lambda/lambda-transform.yml
--rw-r--r--  2.0 unx      572 b- defN 21-Jul-07 23:20 aws_glue_sessions-0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Jul-07 23:20 aws_glue_sessions-0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx      119 b- defN 21-Jul-07 23:20 aws_glue_sessions-0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       37 b- defN 21-Jul-07 23:20 aws_glue_sessions-0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2421 b- defN 21-Jul-07 23:20 aws_glue_sessions-0.8.dist-info/RECORD
-22 files, 403535 bytes uncompressed, 48203 bytes compressed:  88.1%
+-rw-r--r--  2.0 unx       61 b- defN 21-Feb-17 19:30 aws_glue_sessions-0.9.data/data/aws_lambda/handlers.py
+-rw-r--r--  2.0 unx       90 b- defN 21-Feb-17 19:30 aws_glue_sessions-0.9.data/data/aws_lambda/lambda-transform.yml
+-rw-r--r--  2.0 unx      572 b- defN 21-Jul-23 15:23 aws_glue_sessions-0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Jul-23 15:23 aws_glue_sessions-0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx      119 b- defN 21-Jul-23 15:23 aws_glue_sessions-0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       37 b- defN 21-Jul-23 15:23 aws_glue_sessions-0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2421 b- defN 21-Jul-23 15:23 aws_glue_sessions-0.9.dist-info/RECORD
+22 files, 405790 bytes uncompressed, 48610 bytes compressed:  88.0%
```

## zipnote {}

```diff
@@ -39,29 +39,29 @@
 
 Filename: aws_glue_interactive_sessions_kernel/glue_scala_kernel/__init__.py
 Comment: 
 
 Filename: aws_glue_interactive_sessions_kernel/glue_scala_kernel/kernel.json
 Comment: 
 
-Filename: aws_glue_sessions-0.8.data/data/aws_lambda/handlers.py
+Filename: aws_glue_sessions-0.9.data/data/aws_lambda/handlers.py
 Comment: 
 
-Filename: aws_glue_sessions-0.8.data/data/aws_lambda/lambda-transform.yml
+Filename: aws_glue_sessions-0.9.data/data/aws_lambda/lambda-transform.yml
 Comment: 
 
-Filename: aws_glue_sessions-0.8.dist-info/METADATA
+Filename: aws_glue_sessions-0.9.dist-info/METADATA
 Comment: 
 
-Filename: aws_glue_sessions-0.8.dist-info/WHEEL
+Filename: aws_glue_sessions-0.9.dist-info/WHEEL
 Comment: 
 
-Filename: aws_glue_sessions-0.8.dist-info/entry_points.txt
+Filename: aws_glue_sessions-0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: aws_glue_sessions-0.8.dist-info/top_level.txt
+Filename: aws_glue_sessions-0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: aws_glue_sessions-0.8.dist-info/RECORD
+Filename: aws_glue_sessions-0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aws_glue_interactive_sessions_kernel/glue_kernel_utils/KernelMagics.py

```diff
@@ -12,15 +12,22 @@
         self.kernel = kernel
 
     @line_magic('iam_role')
     def set_iam_role(self, glue_role_arn):
         self._validate_magic()
         self.kernel._send_output(f'Current glue_role_arn is {self.kernel.get_glue_role_arn()}')
         self.kernel.set_glue_role_arn(glue_role_arn)
-        self.kernel._send_output(f'IAM role has been set to {glue_role_arn}.')
+        self.kernel._send_output(f'glue_role_arn has been set to {glue_role_arn}.')
+
+    @line_magic('idle_timeout')
+    def set_idle_timeout(self, idle_timeout=None):
+        self._validate_magic()
+        self.kernel._send_output(f'Current idle_timeout is {self.kernel.get_idle_timeout()}')
+        self.kernel.set_idle_timeout = idle_timeout
+        self.kernel._send_output(f'idle_timeout has been set to {idle_timeout} minutes.')
 
     @line_magic('reauthenticate')
     def reauthenticate(self, line=None):
         glue_role_arn = self.kernel.get_glue_role_arn()
         if line:
             glue_role_arn = line
         self.kernel._send_output(f'IAM role has been set to {glue_role_arn}. Reauthenticating.')
@@ -74,19 +81,22 @@
         if not self.kernel.get_session_id():
             self.kernel._send_output('There is no current session.')
             return
         self.kernel.delete_session()
         self.kernel._send_output(f'Deleted session.')
 
     @line_magic('session_id')
-    def get_session_id(self, line=None):
+    def set_session_id(self, line=None):
         if not self.kernel.get_session_id():
             self.kernel._send_output('There is no current session.')
-            return
-        self.kernel._send_output(f'Current Session ID: {self.kernel.get_session_id()}')
+        else:
+            self.kernel._send_output(f'Current active Session ID: {self.kernel.get_session_id()}')
+        self.kernel.set_new_session_id(line)
+        self.kernel._send_output(f'Setting session ID to {self.kernel.get_new_session_id()}. You must connect to a session with this ID before this ID becomes the active Session ID.')
+
 
     @line_magic('enable_glue_datacatalog')
     def set_enable_glue_datacatalog(self, line=None):
         self._validate_magic()
         self.kernel._send_output("Enabling Glue DataCatalog")
         self.kernel.set_enable_glue_datacatalog()
```

## aws_glue_interactive_sessions_kernel/glue_python_kernel/GlueKernel.py

```diff
@@ -22,14 +22,15 @@
 from IPython import get_ipython
 from ..glue_kernel_utils.KernelMagics import KernelMagics
 
 
 class GlueKernel(IPythonKernel):
     time_out = float('inf')
     session_id = None
+    new_session_id = None
     glue_client = None
     implementation = 'Python Glue Session'
     implementation_version = '1.0'
     language = 'no-op'
     language_version = '0.1'
     language_info = {
         'name': 'Python_Glue_Session',
@@ -58,14 +59,15 @@
         self.security_config = None
         self.session_name = "AssumeRoleSession"
         self.max_capacity = None
         self.number_of_workers = 5
         self.worker_type ='G.1X'
         self.temp_dir = None
         self.job_type = "glueetl"
+        self.idle_timeout = None
 
         if not self.ipython_display:
             self.ipython_display = IpythonDisplay()
 
         self._register_magics()
 
     def do_execute(self, code: str, silent: bool, store_history=True, user_expressions=None, allow_stdin=False):
@@ -234,14 +236,17 @@
                 updated_configs['endpoint'] = configs.get('endpoint')
             if 'region' in configs:
                 self.set_region(configs.get('region'))
                 updated_configs['region'] = configs.get('region')
             if 'iam_role' in configs:
                 self.set_glue_role_arn(configs.get('iam_role'))
                 updated_configs['iam_role'] = configs.get('iam_role')
+            if 'session_id' in configs:
+                self.set_new_session_id(configs.get('session_id'))
+                updated_configs['session_id'] = configs.get('session_id')
             if 'max_capacity' in configs:
                 self.set_max_capacity(configs.get('max_capacity'))
                 updated_configs['max_capacity'] = configs.get('max_capacity')
             if 'number_of_workers' in configs:
                 self.set_number_of_workers(configs.get('number_of_workers'))
                 updated_configs['number_of_workers'] = configs.get('number_of_workers')
             if 'worker_type' in configs:
@@ -299,17 +304,23 @@
 
     def get_sessions(self):
         return self.glue_client.list_sessions()
 
     def get_session_id(self):
         return self.session_id
 
+    def get_new_session_id(self):
+        return self.new_session_id
+
     def set_session_id(self, session_id):
         self.session_id = session_id
 
+    def set_new_session_id(self, new_session_id):
+        self.new_session_id = new_session_id
+
     def set_endpoint_url(self, endpoint_url):
         self.endpoint_url = endpoint_url
 
     def get_endpoint_url(self):
         return self.endpoint_url
 
     def set_region(self, region):
@@ -405,14 +416,20 @@
 
     def get_temp_dir(self):
         return self.temp_dir
 
     def set_temp_dir(self, temp_dir):
         self.temp_dir = temp_dir
 
+    def get_idle_timeout(self):
+        return self.idle_timeout
+
+    def set_idle_timeout(self, idle_timeout):
+        self.idle_timeout = idle_timeout
+
     def disconnect(self):
         if self.get_session_id():
             session_id = self.get_session_id()
             self.set_session_id(None)
             self._send_output(f'Disconnected from session {session_id}')
         else:
             self.ipython_display.send_error(f'Not currently connected to a session. \n')
@@ -462,20 +479,24 @@
     def create_session(self):
         self._send_output("Trying to create a Glue session for the kernel.")
         self._send_output(f"Worker Type: {self.get_worker_type()}")
         self._send_output(f"Number of Workers: {self.get_number_of_workers()}")
         if self.get_max_capacity() and (self.get_number_of_workers() and self.get_worker_type()):
             raise ValueError(f'Either max_capacity or worker_type and number_of_workers must be set, but not both.')
 
+        if not self.get_new_session_id():
+            raise ValueError(f'session_id must be set to create a new session.')
+
         additional_args = self._get_additional_arguments()
 
         self.session_id = self.glue_client.create_session(
             Role=self.get_glue_role_arn(),
             DefaultArguments=self.get_default_arguments(),
             Connections=self.get_connections(),
+            Id=self.get_new_session_id(),
             Command={
                 "Name": self.get_job_type(),
                 "PythonVersion": "3"
             },
         **additional_args)["Session"]["Id"]
 
         self._send_output(f'Waiting for session {self.session_id} to get into ready status...')
@@ -497,14 +518,16 @@
             additional_args['MaxCapacity'] = self.get_max_capacity()
         if self.get_number_of_workers():
             additional_args['NumberOfWorkers'] = self.get_number_of_workers()
         if self.get_worker_type():
             additional_args['WorkerType'] = self.get_worker_type()
         if self.get_security_config():
             additional_args['SecurityConfiguration'] = self.get_security_config()
+        if self.get_idle_timeout():
+            additional_args['IdleTimeout'] = self.get_idle_timeout()
         return additional_args
 
     def delete_session(self):
         if self.session_id:
             try:
                 self._send_output(f'Terminating session: {self.session_id}')
                 # TODO: how do we delete session if our security token expires?
```

## aws_glue_interactive_sessions_kernel/glue_scala_kernel/GlueKernel.py

```diff
@@ -22,14 +22,15 @@
 from IPython import get_ipython
 from ..glue_kernel_utils.KernelMagics import KernelMagics
 
 
 class GlueKernel(IPythonKernel):
     time_out = float('inf')
     session_id = None
+    new_session_id = None
     glue_client = None
     implementation = 'Scala Glue Session'
     implementation_version = '1.0'
     language = 'no-op'
     language_version = '0.1'
     language_info = {
         'name': 'scala',
@@ -58,14 +59,15 @@
         self.security_config = None
         self.session_name = "AssumeRoleSession"
         self.max_capacity = None
         self.number_of_workers = 5
         self.worker_type = 'G.1X'
         self.temp_dir = None
         self.job_type = "glueetl"
+        self.idle_timeout = None
 
         if not self.ipython_display:
             self.ipython_display = IpythonDisplay()
 
         self._register_magics()
 
     def do_execute(self, code: str, silent: bool, store_history=True, user_expressions=None, allow_stdin=False):
@@ -235,14 +237,17 @@
                 updated_configs['endpoint'] = configs.get('endpoint')
             if 'region' in configs:
                 self.set_region(configs.get('region'))
                 updated_configs['region'] = configs.get('region')
             if 'iam_role' in configs:
                 self.set_glue_role_arn(configs.get('iam_role'))
                 updated_configs['iam_role'] = configs.get('iam_role')
+            if 'session_id' in configs:
+                self.set_new_session_id(configs.get('session_id'))
+                updated_configs['session_id'] = configs.get('session_id')
             if 'max_capacity' in configs:
                 self.set_max_capacity(configs.get('max_capacity'))
                 updated_configs['max_capacity'] = configs.get('max_capacity')
             if 'number_of_workers' in configs:
                 self.set_number_of_workers(configs.get('number_of_workers'))
                 updated_configs['number_of_workers'] = configs.get('number_of_workers')
             if 'worker_type' in configs:
@@ -300,17 +305,23 @@
 
     def get_sessions(self):
         return self.glue_client.list_sessions()
 
     def get_session_id(self):
         return self.session_id
 
+    def get_new_session_id(self):
+        return self.new_session_id
+
     def set_session_id(self, session_id):
         self.session_id = session_id
 
+    def set_new_session_id(self, new_session_id):
+        self.new_session_id = new_session_id
+
     def set_endpoint_url(self, endpoint_url):
         self.endpoint_url = endpoint_url
 
     def get_endpoint_url(self):
         return self.endpoint_url
 
     def set_region(self, region):
@@ -406,14 +417,20 @@
 
     def get_temp_dir(self):
         return self.temp_dir
 
     def set_temp_dir(self, temp_dir):
         self.temp_dir = temp_dir
 
+    def get_idle_timeout(self):
+        return self.idle_timeout
+
+    def set_idle_timeout(self, idle_timeout):
+        self.idle_timeout = idle_timeout
+
     def disconnect(self):
         if self.get_session_id():
             session_id = self.get_session_id()
             self.set_session_id(None)
             self._send_output(f'Disconnected from session {session_id}')
         else:
             self.ipython_display.send_error(f'Not currently connected to a session. \n')
@@ -462,20 +479,25 @@
 
     def create_session(self):
         self._send_output("Trying to create a Glue session for the kernel.")
         self._send_output(f"Worker Type: {self.get_worker_type()}")
         self._send_output(f"Number of Workers: {self.get_number_of_workers()}")
         if self.get_max_capacity() and (self.get_number_of_workers() and self.get_worker_type()):
             raise ValueError(f'Either max_capacity or worker_type and number_of_workers must be set, but not both.')
+
+        if not self.get_new_session_id():
+            raise ValueError(f'session_id must be set to create a new session.')
+
         additional_args = self._get_additional_arguments()
 
         self.session_id = self.glue_client.create_session(
             Role=self.get_glue_role_arn(),
             DefaultArguments=self.get_default_arguments(),
             Connections=self.get_connections(),
+            Id=self.get_new_session_id(),
             Command={
                 "Name": self.get_job_type(),
                 "PythonVersion": "3"
             },
             **additional_args)["Session"]["Id"]
 
         self._send_output(f'Waiting for session {self.session_id} to get into ready status...')
@@ -497,14 +519,16 @@
             additional_args['MaxCapacity'] = self.get_max_capacity()
         if self.get_number_of_workers():
             additional_args['NumberOfWorkers'] = self.get_number_of_workers()
         if self.get_worker_type():
             additional_args['WorkerType'] = self.get_worker_type()
         if self.get_security_config():
             additional_args['SecurityConfiguration'] = self.get_security_config()
+        if self.get_idle_timeout():
+            additional_args['IdleTimeout'] = self.get_idle_timeout()
         return additional_args
 
     def delete_session(self):
         if self.session_id:
             try:
                 self._send_output(f'Terminating session: {self.session_id}')
                 # TODO: how do we delete session if our security token expires?
```

## Comparing `aws_glue_sessions-0.8.dist-info/METADATA` & `aws_glue_sessions-0.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: aws-glue-sessions
-Version: 0.8
+Version: 0.9
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Dist: hdijupyterutils (>=0.6)
 Requires-Dist: autovizwidget (>=0.6)
 Requires-Dist: ipython (>=4.0.2)
 Requires-Dist: nose
 Requires-Dist: requests
-Requires-Dist: ipykernel (>=4.2.2)
+Requires-Dist: ipykernel (==5.3.4)
 Requires-Dist: ipywidgets (>5.0.0)
 Requires-Dist: notebook (>=4.2)
 Requires-Dist: tornado (>=4)
 Requires-Dist: requests-kerberos (>=0.8.0)
 Requires-Dist: boto3
 Requires-Dist: botocore
 Requires-Dist: Click
```

## Comparing `aws_glue_sessions-0.8.dist-info/RECORD` & `aws_glue_sessions-0.9.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 aws_glue_interactive_sessions_kernel/.DS_Store,sha256=ANDyl8Z-0lDs5Zn9fBAeK3aWigbNIUCxswebXvpyO78,6148
 aws_glue_interactive_sessions_kernel/__init__.py,sha256=S85vAcKBjjnNFwiSNB-50dx947iZuAXKKiaZLLtus2c,88
 aws_glue_interactive_sessions_kernel/glue_kernel.py,sha256=vorXd7yUjNwhV7ReEAQBMDv8bAb_0z9tlKa74JUBdCI,401
 aws_glue_interactive_sessions_kernel/install.sh,sha256=O0682O5dqoplEMeIQ3TNGqrvYYgKk6diEw31AQ9H52U,754
 aws_glue_interactive_sessions_kernel/install_local_mac.sh,sha256=BOtyqUG8w0qKeiouIlgUvgz0sTrPDef-s5wACXn873k,633
 aws_glue_interactive_sessions_kernel/service-2.json,sha256=8ZJtqh0MKUdd5jzaO8jGDXqPw168BYi0zQCZCmkDMeY,326988
 aws_glue_interactive_sessions_kernel/glue_kernel_utils/GlueSessionsConstants.py,sha256=OmhB7fNYZ23IlGPUBigLk1FREHEDqRekkhYoOgDrelk,2427
-aws_glue_interactive_sessions_kernel/glue_kernel_utils/KernelMagics.py,sha256=LPNrW7Yb3IT7NXNflE2I0PLf36E4js1axagOXeIA6ec,8362
+aws_glue_interactive_sessions_kernel/glue_kernel_utils/KernelMagics.py,sha256=yMxqi7LG4DKg9kLle3g32EYUlTd0v-Wlt338QXba0fQ,8954
 aws_glue_interactive_sessions_kernel/glue_kernel_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aws_glue_interactive_sessions_kernel/glue_python_kernel/GlueKernel.py,sha256=WWs9JZdH_mqqlNZD8SEjIwAinhVCugGs64Agu-ygX_s,26960
+aws_glue_interactive_sessions_kernel/glue_python_kernel/GlueKernel.py,sha256=xVlyi-yts-rqt09h0tnJrE6Dsybg8keTNYPXRwfe6EI,27791
 aws_glue_interactive_sessions_kernel/glue_python_kernel/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 aws_glue_interactive_sessions_kernel/glue_python_kernel/kernel.json,sha256=rImd4SMW8D0xqFLMD9VNDpevo7ebBMgA8raVIvHpzUM,210
-aws_glue_interactive_sessions_kernel/glue_scala_kernel/GlueKernel.py,sha256=yr2s_qgQ75JkpmgHTZL9r8-1HwZowxTKTowbMoACDu8,26966
+aws_glue_interactive_sessions_kernel/glue_scala_kernel/GlueKernel.py,sha256=1J3diDBXfNzP2BE2INVPzwxLOdYeR7OVEDHds_KlCmg,27798
 aws_glue_interactive_sessions_kernel/glue_scala_kernel/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 aws_glue_interactive_sessions_kernel/glue_scala_kernel/kernel.json,sha256=hom8cC8-6MgQ9H3lk9w5FgukWp_tD1KzH48U1P736W0,206
-aws_glue_sessions-0.8.data/data/aws_lambda/handlers.py,sha256=DOAphixCXcmIHxF503wiaOiItEcBtOZO-8wQ1TmaTC0,61
-aws_glue_sessions-0.8.data/data/aws_lambda/lambda-transform.yml,sha256=L1jP9znEQ-zla0Ges5uzqdP7ZOk1o1AJAUG7DcCSA8A,90
-aws_glue_sessions-0.8.dist-info/METADATA,sha256=4M6lnxKDMRS03FVK9mbI7Lgt6X7X1mbchgFEn-hHrqE,572
-aws_glue_sessions-0.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-aws_glue_sessions-0.8.dist-info/entry_points.txt,sha256=ekeAgfZvrGiXt-MWsaJgjL7E9Th_TSUqaAAYnt0vhzg,119
-aws_glue_sessions-0.8.dist-info/top_level.txt,sha256=lFIZhHsFozM6TjppXBg_NKehCa9qxH7MXEbO1C8HgAw,37
-aws_glue_sessions-0.8.dist-info/RECORD,,
+aws_glue_sessions-0.9.data/data/aws_lambda/handlers.py,sha256=DOAphixCXcmIHxF503wiaOiItEcBtOZO-8wQ1TmaTC0,61
+aws_glue_sessions-0.9.data/data/aws_lambda/lambda-transform.yml,sha256=L1jP9znEQ-zla0Ges5uzqdP7ZOk1o1AJAUG7DcCSA8A,90
+aws_glue_sessions-0.9.dist-info/METADATA,sha256=aXNzQ5UD4s3P_SoZCkovWZMvD81Hg6PJ3PGN3del-8g,572
+aws_glue_sessions-0.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+aws_glue_sessions-0.9.dist-info/entry_points.txt,sha256=ekeAgfZvrGiXt-MWsaJgjL7E9Th_TSUqaAAYnt0vhzg,119
+aws_glue_sessions-0.9.dist-info/top_level.txt,sha256=lFIZhHsFozM6TjppXBg_NKehCa9qxH7MXEbO1C8HgAw,37
+aws_glue_sessions-0.9.dist-info/RECORD,,
```

