# Comparing `tmp/logger-local-0.0.8.tar.gz` & `tmp/logger-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger-local-0.0.8.tar", last modified: Fri Jul  7 07:40:42 2023, max compression
+gzip compressed data, was "logger-local-0.0.9.tar", last modified: Mon Jul 10 12:59:16 2023, max compression
```

## Comparing `logger-local-0.0.8.tar` & `logger-local-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:40:42.025340 logger-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-07 07:40:32.000000 logger-local-0.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:40:42.025340 logger-local-0.0.8/LoggerLocalPythonPackage/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-07 07:40:32.000000 logger-local-0.0.8/LoggerLocalPythonPackage/LoggerService.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-07 07:40:32.000000 logger-local-0.0.8/LoggerLocalPythonPackage/LoggerServiceSingleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-07 07:40:32.000000 logger-local-0.0.8/LoggerLocalPythonPackage/MessageSeverity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-07 07:40:32.000000 logger-local-0.0.8/LoggerLocalPythonPackage/Writer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:40:32.000000 logger-local-0.0.8/LoggerLocalPythonPackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-07 07:40:42.025340 logger-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-07 07:40:32.000000 logger-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:40:42.025340 logger-local-0.0.8/logger_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-07 07:40:42.000000 logger-local-0.0.8/logger_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-07 07:40:42.000000 logger-local-0.0.8/logger_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 07:40:42.000000 logger-local-0.0.8/logger_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 07:40:42.000000 logger-local-0.0.8/logger_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 07:40:42.029341 logger-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-07 07:40:32.000000 logger-local-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:40:42.025340 logger-local-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-07-07 07:40:32.000000 logger-local-0.0.8/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:59:16.186175 logger-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-10 12:59:06.000000 logger-local-0.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:59:16.186175 logger-local-0.0.9/LoggerLocalPythonPackage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-10 12:59:06.000000 logger-local-0.0.9/LoggerLocalPythonPackage/LoggerService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-10 12:59:06.000000 logger-local-0.0.9/LoggerLocalPythonPackage/LoggerServiceSingleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-10 12:59:06.000000 logger-local-0.0.9/LoggerLocalPythonPackage/MessageSeverity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-10 12:59:06.000000 logger-local-0.0.9/LoggerLocalPythonPackage/Writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 12:59:06.000000 logger-local-0.0.9/LoggerLocalPythonPackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-10 12:59:16.186175 logger-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-10 12:59:06.000000 logger-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:59:16.186175 logger-local-0.0.9/logger_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-10 12:59:16.000000 logger-local-0.0.9/logger_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-10 12:59:16.000000 logger-local-0.0.9/logger_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 12:59:16.000000 logger-local-0.0.9/logger_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 12:59:16.000000 logger-local-0.0.9/logger_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 12:59:16.186175 logger-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-10 12:59:06.000000 logger-local-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:59:16.186175 logger-local-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-10 12:59:06.000000 logger-local-0.0.9/tests/test_writer.py
```

### Comparing `logger-local-0.0.8/LICENSE` & `logger-local-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `logger-local-0.0.8/LoggerLocalPythonPackage/LoggerService.py` & `logger-local-0.0.9/LoggerLocalPythonPackage/LoggerService.py`

 * *Files identical despite different names*

### Comparing `logger-local-0.0.8/LoggerLocalPythonPackage/Writer.py` & `logger-local-0.0.9/LoggerLocalPythonPackage/Writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 import pymysql
 import os
 from dotenv import load_dotenv
 load_dotenv()
 
-debug = os.getenv('DEBUG')
+os_debug = os.getenv('DEBUG')
+if(os_debug=='True' or os_debug=='1'):
+    debug = True
+else:
+    debug = False
+if (debug): print ("Writer.py debug is on debug=", debug)
 
 class Writer:
 
     # TODO: We need to replace this with the database package
     def get_connection(self) -> pymysql.connections.Connection:
         if (debug): print ("get_connection")
         result = pymysql.connect(
             user=os.getenv('RDS_USERNAME'),
             password=os.getenv('RDS_PASSWORD'),
             host=os.getenv('RDS_HOSTNAME'),
             database='logger' # os.getenv('RDS_DB_NAME')
         )
-        if (debug): print(result)
+        #if (debug): print(result)
         return result
 
     def add(self, **kwargs):
-
+        connection=None
         try:
             params_to_insert = kwargs['object']
             # creating connection
             connection = self.get_connection()
             # connection = self._pool.get_connection()
             cursor = connection.cursor()
 
@@ -51,27 +56,30 @@
             sql = f"""INSERT INTO logger_table ({joined_keys})
                         VALUES ({generate_values_pattern});
             """
             cursor.execute(sql,listed_values)
         except Exception as e:
             print("catched " + str(e))
         finally:
-            connection.commit()
-            cursor.close()
-            connection.close()
+            if(connection):
+                connection.commit()
+                cursor.close()
+                connection.close()
 
     def add_message(self, message, log_level):
-        if (debug): print ("add_message" + message+ ' ' + log_level)
+        connection=None
+        if (debug): print ("add_message" + message+ ' ' + str(log_level))
         try:
             # creating connection
             connection = self.get_connection()
             # connection = self._pool.get_connection()
             cursor = connection.cursor()
             sql = f"INSERT INTO logger.logger_table (payload, severity_id) VALUES ('{message}', {log_level})"
             cursor.execute(sql)
 
         except Exception as e:
             print("Writer.py Writer.add_message catched" + str(e))
         finally:
-            connection.commit()
-            cursor.close()
-            connection.close()
+            if(connection):
+                connection.commit()
+                cursor.close()
+                connection.close()
```

### Comparing `logger-local-0.0.8/PKG-INFO` & `logger-local-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles Logger Python Local
 Home-page: https://github.com/circles-zone/logger-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `logger-local-0.0.8/README.md` & `logger-local-0.0.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -46,8 +46,12 @@
 replace the x with the latest version in pypi.org/project/logger-local
 logger-local==0.0.x
 
 Please includ at least two Logger calls in each method:
 "Start " + class.method names "( "+ parameters + ")";
 "Start " + class.method names + " returned " + return values;
 
-TOOD: We nee to add tests
+TOOD: We nee to add Unit Tests so this command will work
+python -m unittest .\tests\test_writer.py
+
+
+pip install -r .\requirements.txt
```

### Comparing `logger-local-0.0.8/logger_local.egg-info/PKG-INFO` & `logger-local-0.0.9/logger_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles Logger Python Local
 Home-page: https://github.com/circles-zone/logger-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `logger-local-0.0.8/setup.py` & `logger-local-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='logger-local',
-    version='0.0.8',
+    version='0.0.9',
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles Logger Python Local",
     long_description="This is a package for sharing common Logger function used in different repositories",
     long_description_content_type="text/markdown",
     url="https://github.com/circles-zone/logger-local-python-package",
     packages=setuptools.find_packages(),
```

### Comparing `logger-local-0.0.8/tests/test_writer.py` & `logger-local-0.0.9/tests/test_writer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,36 @@
+# TODO: Should convert this file to Python Unit Test
 import pymysql
 import os
-from LoggerLocalPythonPackage.MessageSeverity import MessageSeverity
-from LoggerLocalPythonPackage.LoggerServiceSingleton import locallgr
 
+import sys
+package_dir = "."
+sys.path.append(package_dir)
+
+# TODO: This is too long, let's shorten it.
+from LoggerLocalPythonPackage.MessageSeverity import MessageSeverity
+from Local_Logger import Local_Logger
+import pytest
+locallgr=Local_Logger()
 ID = 5000001
 # ID = 1
 
+# Connect to the datbaase to validat that the log was inserted
 def get_connection() -> pymysql.connections.Connection:
     return pymysql.connect(
         user=os.getenv('RDS_USERNAME'),
         password=os.getenv('RDS_PASSWORD'),
         host=os.getenv('RDS_HOSTNAME'),
-        database=os.getenv('RDS_DB_NAME')
+        database='logger' #os.getenv('RDS_DB_NAME')
     )
+@pytest.mark.test
 def test_log():
     object_to_insert_1 = {
-        'ipv4': 'ipv4-py',
-        'ipv6': 'ipv6-py',
+        'client_ip_v4': 'ipv4-py',
+        'client_ip_v6': 'ipv6-py',
         'latitude': 33,
         'longitude': 35,
         'user_id': ID,
         'profile_id': ID,
         'activity': 'test from python',
         'activity_id': ID,
         'payload': 'log from python -object_1',
@@ -34,19 +44,19 @@
     locallgr.info(object=object_to_insert_1)
     conn = get_connection()
     cursor = conn.cursor()
     sql = f"""SELECT severity_id FROM logger.logger_table WHERE payload = '{object_to_insert_1['payload']}' ORDER BY timestamp DESC LIMIT 1;"""
     cursor.execute(sql)
     result = cursor.fetchone()
     assert result[0] == MessageSeverity.Information.value
-
+@pytest.mark.test
 def test_error():
     object_to_insert_2 = {
-        'ipv4': 'ipv4-py',
-        'ipv6': 'ipv6-py',
+        'client_ip_v4': 'ipv4-py',
+        'client_ip_v6': 'ipv6-py',
         'latitude': 33,
         'longitude': 35,
         'user_id': ID,
         'profile_id': ID,
         'activity': 'test from python',
         'activity_id': ID,
         'payload': 'payload from python -object_2',
@@ -55,19 +65,19 @@
     locallgr.error(object=object_to_insert_2)
     conn = get_connection()
     cursor = conn.cursor()
     sql = f"""SELECT severity_id FROM logger.logger_table WHERE payload = '{object_to_insert_2['payload']}' ORDER BY timestamp DESC LIMIT 1;"""
     cursor.execute(sql)
     result = cursor.fetchone()
     assert result[0] == MessageSeverity.Error.value
-
+@pytest.mark.test
 def test_verbose():
     object_to_insert_3 = {
-        'ipv4': 'ipv4-py',
-        'ipv6': 'ipv6-py',
+        'client_ip_v4': 'ipv4-py',
+        'client_ip_v6': 'ipv6-py',
         'latitude': 33,
         'longitude': 35,
         'variable_id': ID,
         'variable_value_old': 'variable_value_old-python-object_3',
         'variable_value_new': 'variable_value_new-python',
         'created_user_id': ID,
         'updated_user_id': ID
@@ -76,18 +86,19 @@
 
     conn = get_connection()
     cursor = conn.cursor()
     sql = f"""SELECT severity_id FROM logger.logger_table WHERE variable_value_old = '{object_to_insert_3['variable_value_old']}' ORDER BY timestamp DESC LIMIT 1;"""
     cursor.execute(sql)
     result = cursor.fetchone()
     assert result[0] == MessageSeverity.Verbose.value
+@pytest.mark.test
 def test_warn():
     object_to_insert_4 = {
-        'ipv4': 'ipv4-py',
-        'ipv6': 'ipv6-py',
+        'client_ip_v4': 'ipv4-py',
+        'client_ip_v6': 'ipv6-py',
         'latitude': 33,
         'longitude': 35,
         'user_id': ID,
         'profile_id': ID,
         'activity': 'test from python',
         'activity_id': ID,
         'payload': 'payload from python -object_4',
@@ -99,26 +110,27 @@
 
     conn = get_connection()
     cursor = conn.cursor()
     sql = f"""SELECT severity_id FROM logger.logger_table WHERE payload = '{object_to_insert_4['payload']}' ORDER BY timestamp DESC LIMIT 1;"""
     cursor.execute(sql)
     result = cursor.fetchone()
     assert result[0] == MessageSeverity.Warning.value
+@pytest.mark.test
 def test_add_message():
     # option to insert only message
     message = 'only message error from python'
     locallgr.error(message)
 
     conn = get_connection()
     cursor = conn.cursor()
     sql = f"""SELECT severity_id FROM logger.logger_table WHERE payload = '{message}' ORDER BY timestamp DESC LIMIT 1;"""
     cursor.execute(sql)
     result = cursor.fetchone()
     assert result[0] == MessageSeverity.Error.value
-
+@pytest.mark.test
 def test_debug():
     object_to_insert_5 = {
         'payload': 'just payload & activity_id - python',
         'activity_id': ID
     }
     locallgr.debug(object=object_to_insert_5)
 
@@ -126,14 +138,18 @@
     cursor = conn.cursor()
     sql = f"""SELECT severity_id FROM logger.logger_table WHERE payload = '{object_to_insert_5['payload']}' ORDER BY timestamp DESC LIMIT 1;"""
     print(sql)
     cursor.execute(sql)
     result = cursor.fetchone()
     assert result[0] == MessageSeverity.Debug.value
 
-
-
-
+if __name__ == "__main__":
+    test_log()
+    test_error()
+    test_verbose()
+    test_add_message()
+    test_warn()
+    test_debug()
```

