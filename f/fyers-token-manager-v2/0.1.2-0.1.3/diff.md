# Comparing `tmp/fyers_token_manager_v2-0.1.2.tar.gz` & `tmp/fyers_token_manager_v2-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers_token_manager_v2-0.1.2.tar", last modified: Fri May 19 05:05:21 2023, max compression
+gzip compressed data, was "fyers_token_manager_v2-0.1.3.tar", last modified: Sat Aug  5 13:58:03 2023, max compression
```

## Comparing `fyers_token_manager_v2-0.1.2.tar` & `fyers_token_manager_v2-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-19 05:05:21.773408 fyers_token_manager_v2-0.1.2/
--rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)       11 2022-10-12 11:09:01.000000 fyers_token_manager_v2-0.1.2/LICENSE
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-19 05:05:21.773408 fyers_token_manager_v2-0.1.2/PKG-INFO
--rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)      786 2023-05-10 05:26:39.000000 fyers_token_manager_v2-0.1.2/README.md
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-19 05:05:21.769408 fyers_token_manager_v2-0.1.2/fyers_token_manager_v2/
--rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)     4840 2023-05-19 05:03:48.000000 fyers_token_manager_v2-0.1.2/fyers_token_manager_v2/__init__.py
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-19 05:05:21.773408 fyers_token_manager_v2-0.1.2/fyers_token_manager_v2.egg-info/
--rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-19 05:05:21.000000 fyers_token_manager_v2-0.1.2/fyers_token_manager_v2.egg-info/PKG-INFO
--rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)      290 2023-05-19 05:05:21.000000 fyers_token_manager_v2-0.1.2/fyers_token_manager_v2.egg-info/SOURCES.txt
--rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)        1 2023-05-19 05:05:21.000000 fyers_token_manager_v2-0.1.2/fyers_token_manager_v2.egg-info/dependency_links.txt
--rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)       15 2023-05-19 05:05:21.000000 fyers_token_manager_v2-0.1.2/fyers_token_manager_v2.egg-info/requires.txt
--rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)       23 2023-05-19 05:05:21.000000 fyers_token_manager_v2-0.1.2/fyers_token_manager_v2.egg-info/top_level.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       38 2023-05-19 05:05:21.773408 fyers_token_manager_v2-0.1.2/setup.cfg
--rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)      682 2023-05-19 05:04:36.000000 fyers_token_manager_v2-0.1.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-05 13:58:03.951595 fyers_token_manager_v2-0.1.3/
+-rwxrwxrwx   0 root         (0) root         (0)       11 2023-08-05 13:54:25.000000 fyers_token_manager_v2-0.1.3/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     1157 2023-08-05 13:58:03.951399 fyers_token_manager_v2-0.1.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      786 2023-08-05 13:54:25.000000 fyers_token_manager_v2-0.1.3/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-05 13:58:03.948923 fyers_token_manager_v2-0.1.3/fyers_token_manager_v2/
+-rwxrwxrwx   0 root         (0) root         (0)     4941 2023-08-05 13:56:31.000000 fyers_token_manager_v2-0.1.3/fyers_token_manager_v2/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-05 13:58:03.950897 fyers_token_manager_v2-0.1.3/fyers_token_manager_v2.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     1157 2023-08-05 13:58:03.000000 fyers_token_manager_v2-0.1.3/fyers_token_manager_v2.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      290 2023-08-05 13:58:03.000000 fyers_token_manager_v2-0.1.3/fyers_token_manager_v2.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-08-05 13:58:03.000000 fyers_token_manager_v2-0.1.3/fyers_token_manager_v2.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-08-05 13:58:03.000000 fyers_token_manager_v2-0.1.3/fyers_token_manager_v2.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       23 2023-08-05 13:58:03.000000 fyers_token_manager_v2-0.1.3/fyers_token_manager_v2.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-08-05 13:58:03.951674 fyers_token_manager_v2-0.1.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      682 2023-08-05 13:57:55.000000 fyers_token_manager_v2-0.1.3/setup.py
```

### Comparing `fyers_token_manager_v2-0.1.2/PKG-INFO` & `fyers_token_manager_v2-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: fyers_token_manager_v2
-Version: 0.1.2
+Version: 0.1.3
 Summary: Fyers Token Manager
 Home-page: https://github.com/krunaldodiya/fyers_token_manager
 Author: Krunal Dodiya
 Author-email: kunal.dodiya1@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ```
 config = {
@@ -48,7 +50,9 @@
 #### HTTP Client
 
 - fyersTokenManager.http_client.get_profile()
 
 #### WebSocket Client
 
 - fyersTokenManager.ws_client.subscribe(payload)
+
+
```

### Comparing `fyers_token_manager_v2-0.1.2/README.md` & `fyers_token_manager_v2-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fyers_token_manager_v2-0.1.2/fyers_token_manager_v2/__init__.py` & `fyers_token_manager_v2-0.1.3/fyers_token_manager_v2/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,24 +14,41 @@
         self.totp_key = config["totp_key"]
         self.pin = config["pin"]
         self.client_id = config["client_id"]
         self.secret_key = config["secret_key"]
         self.redirect_uri = config["redirect_uri"]
 
         self.__accessToken = accessToken
+
         self.__fyersModel = fyersModel
         self.__ws = ws
 
         self.__data_path = None
         self.__logs_path = None
         self.__access_token_file_name = None
 
         self.__set_access_token_file_name()
         self.__initialize()
 
+    @property
+    def http_client(self):
+        return self.__fyersModel.FyersModel(
+            client_id=self.client_id,
+            token=self.http_access_token,
+            log_path=self.__logs_path,
+        )
+
+    @property
+    def ws_client(self):
+        return self.__ws.FyersSocket(
+            access_token=self.ws_access_token,
+            run_background=False,
+            log_path=self.__logs_path,
+        )
+
     def __set_access_token_file_name(self):
         home_directory = os.path.expanduser("~")
 
         self.__data_path = pathlib.Path(
             f"{home_directory}/fyers_token_manager/data/{self.username}"
         )
 
@@ -48,24 +65,14 @@
         )
 
     def __set_initial_values(self, token):
         self.http_access_token = token
 
         self.ws_access_token = f"{self.client_id}:{self.http_access_token}"
 
-        self.http_client = self.__fyersModel.FyersModel(
-            client_id=self.client_id, token=token, log_path=self.__logs_path
-        )
-
-        self.ws_client = self.__ws.FyersSocket(
-            access_token=self.ws_access_token,
-            run_background=False,
-            log_path=self.__logs_path,
-        )
-
     def __initialize(self):
         try:
             token = self.__read_file()
             self.__set_initial_values(token)
         except FileNotFoundError:
             token = self.__setup()
             self.__set_initial_values(token)
```

### Comparing `fyers_token_manager_v2-0.1.2/fyers_token_manager_v2.egg-info/PKG-INFO` & `fyers_token_manager_v2-0.1.3/fyers_token_manager_v2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: fyers-token-manager-v2
-Version: 0.1.2
+Version: 0.1.3
 Summary: Fyers Token Manager
 Home-page: https://github.com/krunaldodiya/fyers_token_manager
 Author: Krunal Dodiya
 Author-email: kunal.dodiya1@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ```
 config = {
@@ -48,7 +50,9 @@
 #### HTTP Client
 
 - fyersTokenManager.http_client.get_profile()
 
 #### WebSocket Client
 
 - fyersTokenManager.ws_client.subscribe(payload)
+
+
```

### Comparing `fyers_token_manager_v2-0.1.2/setup.py` & `fyers_token_manager_v2-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     include_package_data=True,
     name="fyers_token_manager_v2",
-    version="0.1.2",
+    version="0.1.3",
     description="Fyers Token Manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/krunaldodiya/fyers_token_manager",
     author="Krunal Dodiya",
     author_email="kunal.dodiya1@gmail.com",
     packages=setuptools.find_packages(),
```

