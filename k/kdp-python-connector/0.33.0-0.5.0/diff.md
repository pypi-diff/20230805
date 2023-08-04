# Comparing `tmp/kdp-python-connector-0.33.0.tar.gz` & `tmp/kdp-python-connector-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kdp-python-connector-0.33.0.tar", last modified: Fri Aug  4 22:02:56 2023, max compression
+gzip compressed data, was "kdp-python-connector-0.5.0.tar", last modified: Tue Jul 12 19:49:47 2022, max compression
```

## Comparing `kdp-python-connector-0.33.0.tar` & `kdp-python-connector-0.5.0.tar`

### file list

```diff
@@ -1,36 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 22:02:56.815770 kdp-python-connector-0.33.0/
--rw-r--r--   0 runner    (1001) docker     (122)      292 2023-08-04 22:02:56.815770 kdp-python-connector-0.33.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      272 2023-08-04 22:02:40.000000 kdp-python-connector-0.33.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 22:02:56.811770 kdp-python-connector-0.33.0/kdp_connector/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-08-04 22:02:40.000000 kdp-python-connector-0.33.0/kdp_connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 22:02:56.811770 kdp-python-connector-0.33.0/kdp_connector/configuration/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 22:02:40.000000 kdp-python-connector-0.33.0/kdp_connector/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3103 2023-08-04 22:02:40.000000 kdp-python-connector-0.33.0/kdp_connector/configuration/authenticationUtil.py
--rw-r--r--   0 runner    (1001) docker     (122)     1978 2023-08-04 22:02:40.000000 kdp-python-connector-0.33.0/kdp_connector/configuration/configurationUtil.py
--rw-r--r--   0 runner    (1001) docker     (122)     1587 2023-08-04 22:02:40.000000 kdp-python-connector-0.33.0/kdp_connector/configuration/keycloak_authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)      548 2023-08-04 22:02:40.000000 kdp-python-connector-0.33.0/kdp_connector/configuration/proxy_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 22:02:56.811770 kdp-python-connector-0.33.0/kdp_connector/connectors/
--rw-r--r--   0 runner    (1001) docker     (122)      648 2023-08-04 22:02:40.000000 kdp-python-connector-0.33.0/kdp_connector/connectors/Storage.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 22:02:40.000000 kdp-python-connector-0.33.0/kdp_connector/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1580 2023-08-04 22:02:40.000000 kdp-python-connector-0.33.0/kdp_connector/connectors/audit_log.py
--rw-r--r--   0 runner    (1001) docker     (122)     3721 2023-08-04 22:02:40.000000 kdp-python-connector-0.33.0/kdp_connector/connectors/audit_log_configs.py
--rw-r--r--   0 runner    (1001) docker     (122)     7467 2023-08-04 22:02:40.000000 kdp-python-connector-0.33.0/kdp_connector/connectors/batch_write.py
--rw-r--r--   0 runner    (1001) docker     (122)     2205 2023-08-04 22:02:40.000000 kdp-python-connector-0.33.0/kdp_connector/connectors/index_management.py
--rw-r--r--   0 runner    (1001) docker     (122)     2333 2023-08-04 22:02:40.000000 kdp-python-connector-0.33.0/kdp_connector/connectors/ingest_job_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     8744 2023-08-04 22:02:40.000000 kdp-python-connector-0.33.0/kdp_connector/connectors/kdp_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2260 2023-08-04 22:02:40.000000 kdp-python-connector-0.33.0/kdp_connector/connectors/query.py
--rw-r--r--   0 runner    (1001) docker     (122)     4696 2023-08-04 22:02:40.000000 kdp-python-connector-0.33.0/kdp_connector/connectors/read.py
--rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-08-04 22:02:40.000000 kdp-python-connector-0.33.0/kdp_connector/connectors/upload.py
--rw-r--r--   0 runner    (1001) docker     (122)    24816 2023-08-04 22:02:40.000000 kdp-python-connector-0.33.0/kdp_connector/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 22:02:56.815770 kdp-python-connector-0.33.0/kdp_python_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      292 2023-08-04 22:02:56.000000 kdp-python-connector-0.33.0/kdp_python_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-08-04 22:02:56.000000 kdp-python-connector-0.33.0/kdp_python_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-04 22:02:56.000000 kdp-python-connector-0.33.0/kdp_python_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-08-04 22:02:56.000000 kdp-python-connector-0.33.0/kdp_python_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-08-04 22:02:56.000000 kdp-python-connector-0.33.0/kdp_python_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-04 22:02:56.815770 kdp-python-connector-0.33.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1372 2023-08-04 22:02:40.000000 kdp-python-connector-0.33.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 22:02:56.815770 kdp-python-connector-0.33.0/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4014 2023-08-04 22:02:40.000000 kdp-python-connector-0.33.0/test/test_ingest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1216 2023-08-04 22:02:40.000000 kdp-python-connector-0.33.0/test/test_keycloak.py
--rw-r--r--   0 runner    (1001) docker     (122)     4925 2023-08-04 22:02:40.000000 kdp-python-connector-0.33.0/test/test_read.py
+drwxr-xr-x   0 emily      (501) staff       (20)        0 2022-07-12 19:49:47.696629 kdp-python-connector-0.5.0/
+-rw-r--r--   0 emily      (501) staff       (20)      357 2022-07-12 19:49:47.696381 kdp-python-connector-0.5.0/PKG-INFO
+-rw-r--r--   0 emily      (501) staff       (20)     1112 2022-07-12 19:07:05.000000 kdp-python-connector-0.5.0/README.md
+drwxr-xr-x   0 emily      (501) staff       (20)        0 2022-07-12 19:49:47.684094 kdp-python-connector-0.5.0/kdp_connector/
+-rw-r--r--   0 emily      (501) staff       (20)       80 2022-07-12 19:07:05.000000 kdp-python-connector-0.5.0/kdp_connector/__init__.py
+drwxr-xr-x   0 emily      (501) staff       (20)        0 2022-07-12 19:49:47.685242 kdp-python-connector-0.5.0/kdp_connector/configuration/
+-rw-r--r--   0 emily      (501) staff       (20)        0 2022-07-12 19:07:05.000000 kdp-python-connector-0.5.0/kdp_connector/configuration/__init__.py
+-rw-r--r--   0 emily      (501) staff       (20)      622 2022-07-12 19:07:05.000000 kdp-python-connector-0.5.0/kdp_connector/configuration/authenticationUtil.py
+-rw-r--r--   0 emily      (501) staff       (20)     1552 2022-07-12 19:07:05.000000 kdp-python-connector-0.5.0/kdp_connector/configuration/configurationUtil.py
+drwxr-xr-x   0 emily      (501) staff       (20)        0 2022-07-12 19:49:47.688751 kdp-python-connector-0.5.0/kdp_connector/connectors/
+-rw-r--r--   0 emily      (501) staff       (20)        0 2022-07-12 19:07:05.000000 kdp-python-connector-0.5.0/kdp_connector/connectors/__init__.py
+-rw-r--r--   0 emily      (501) staff       (20)     1723 2022-07-12 19:07:05.000000 kdp-python-connector-0.5.0/kdp_connector/connectors/index_management.py
+-rw-r--r--   0 emily      (501) staff       (20)     1219 2022-07-12 19:07:05.000000 kdp-python-connector-0.5.0/kdp_connector/connectors/ingest.py
+-rw-r--r--   0 emily      (501) staff       (20)     1941 2022-07-12 19:07:05.000000 kdp-python-connector-0.5.0/kdp_connector/connectors/ingest_job_api.py
+-rw-r--r--   0 emily      (501) staff       (20)     3536 2022-07-12 19:07:05.000000 kdp-python-connector-0.5.0/kdp_connector/connectors/kdp_api.py
+-rw-r--r--   0 emily      (501) staff       (20)      562 2022-07-12 19:07:05.000000 kdp-python-connector-0.5.0/kdp_connector/connectors/query.py
+-rw-r--r--   0 emily      (501) staff       (20)     3294 2022-07-12 19:07:05.000000 kdp-python-connector-0.5.0/kdp_connector/connectors/read.py
+-rw-r--r--   0 emily      (501) staff       (20)      901 2022-07-12 19:07:05.000000 kdp-python-connector-0.5.0/kdp_connector/connectors/upload.py
+-rw-r--r--   0 emily      (501) staff       (20)     6746 2022-07-12 19:07:05.000000 kdp-python-connector-0.5.0/kdp_connector/main.py
+drwxr-xr-x   0 emily      (501) staff       (20)        0 2022-07-12 19:49:47.695445 kdp-python-connector-0.5.0/kdp_python_connector.egg-info/
+-rw-r--r--   0 emily      (501) staff       (20)      357 2022-07-12 19:49:47.000000 kdp-python-connector-0.5.0/kdp_python_connector.egg-info/PKG-INFO
+-rw-r--r--   0 emily      (501) staff       (20)      760 2022-07-12 19:49:47.000000 kdp-python-connector-0.5.0/kdp_python_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 emily      (501) staff       (20)        1 2022-07-12 19:49:47.000000 kdp-python-connector-0.5.0/kdp_python_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 emily      (501) staff       (20)       13 2022-07-12 19:49:47.000000 kdp-python-connector-0.5.0/kdp_python_connector.egg-info/requires.txt
+-rw-r--r--   0 emily      (501) staff       (20)       14 2022-07-12 19:49:47.000000 kdp-python-connector-0.5.0/kdp_python_connector.egg-info/top_level.txt
+-rw-r--r--   0 emily      (501) staff       (20)       38 2022-07-12 19:49:47.696683 kdp-python-connector-0.5.0/setup.cfg
+-rw-r--r--   0 emily      (501) staff       (20)     1073 2022-07-12 19:07:05.000000 kdp-python-connector-0.5.0/setup.py
+drwxr-xr-x   0 emily      (501) staff       (20)        0 2022-07-12 19:49:47.696077 kdp-python-connector-0.5.0/test/
+-rw-r--r--   0 emily      (501) staff       (20)     3982 2022-07-12 19:07:05.000000 kdp-python-connector-0.5.0/test/test_ingest.py
+-rw-r--r--   0 emily      (501) staff       (20)     4925 2022-07-12 19:07:05.000000 kdp-python-connector-0.5.0/test/test_read.py
```

### Comparing `kdp-python-connector-0.33.0/kdp_connector/configuration/configurationUtil.py` & `kdp-python-connector-0.5.0/kdp_connector/configuration/configurationUtil.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,15 @@
 import kdp_api
 
 
 class ConfigurationUtil(object):
 
     @staticmethod
     def create_configuration(host: str, jwt: str, path_to_ca_file: str = '', discard_unknown_keys: bool = True):
-        """This method will be used to create the connection configuration
-
-            :param str host: KDP host
-            :param str jwt: JWT token
-            :param str path_to_ca_file: Path to Certificate Authority file
-            :param bool discard_unknown_keys: Whether to discard unknown keys, defaults to True
-
-            :returns: KDP connection configuration
-
-            :rtype: Configuration
-        """
-        # Defining the host is optional and defaults to https://api.app.koverse.com
+        # Defining the host is optional and defaults to https://api.koverse.dev
         # See configurationUtil.py for a list of all supported configuration parameters.
         config = kdp_api.Configuration(
             host=host
         )
 
         # The client must configure the authentication and authorization parameters
         # in accordance with the API server security policy.
```

### Comparing `kdp-python-connector-0.33.0/kdp_connector/connectors/index_management.py` & `kdp-python-connector-0.5.0/kdp_connector/connectors/index_management.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,26 +13,15 @@
 
         self.http = urllib3.HTTPSConnectionPool(host, port=443, cert_reqs='CERT_NONE', assert_hostname=False,
         timeout=Timeout(connect=2.0, read=10.0))
 
 
     def modify_indexes(self, dataset_id: str, create: list, remove: list,
         autoCreateIndexes: bool = False, searchAnyField: bool = False) -> object :
-        """This method will modify existing indexes on a dataset
 
-            :param str dataset_id: ID of dataset
-            :param list create: List of indexes to create
-            :param list remove: List of indexes to delete
-            :param bool autoCreateIndexes: Whether to automatically create indexes when data is written
-            :param bool searchAnyField: Whether to automatically search any field
-
-            :returns: Job ID
-
-            :rtype: str
-       """
         request={}
         request['action']='modifyIndexes'
         request['datasetId']=dataset_id
         request['remove']=remove
         request['create']=create
         request['autoCreateIndexes']=autoCreateIndexes
         request['searchAnyField']=searchAnyField
```

### Comparing `kdp-python-connector-0.33.0/kdp_connector/connectors/upload.py` & `kdp-python-connector-0.5.0/kdp_connector/connectors/upload.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,24 @@
+
 import json
 import urllib3
 import logging
 from urllib3.util import Timeout
 
-
 class UploadApi(object):
     def __init__(self, configuration=None):
         self.configuration = configuration
-        host = self.configuration.host.replace('https://', '')
+        host=self.configuration.host.replace('https://', '')
 
         self.http = urllib3.HTTPSConnectionPool(host, port=443, cert_reqs='CERT_NONE',
-                                                assert_hostname=False, timeout=Timeout(connect=2.0, read=10.0))
+            assert_hostname=False, timeout=Timeout(connect=2.0, read=10.0))
 
-    def upload(self, dataset_id: str, file_config: object):
-        """This method will upload a file to KDP
 
-            :param str dataset_id: ID of dataset that file will be uploaded to
-            :param object file_config: JSON containing filename and path ex. { "filename": "test.csv", "path": "/path/to/file" }
+    def upload(self, dataset_id:str, file_config: object):
 
-        """
         response = self.http.request(
             'POST',
             self.configuration.host + '/uploads',
             headers={
                 'Authorization': 'Bearer ' + self.configuration.access_token
             },
             fields={
```

### Comparing `kdp-python-connector-0.33.0/kdp_python_connector.egg-info/SOURCES.txt` & `kdp-python-connector-0.5.0/kdp_python_connector.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 README.md
 setup.py
 kdp_connector/__init__.py
 kdp_connector/main.py
 kdp_connector/configuration/__init__.py
 kdp_connector/configuration/authenticationUtil.py
 kdp_connector/configuration/configurationUtil.py
-kdp_connector/configuration/keycloak_authentication.py
-kdp_connector/configuration/proxy_authentication.py
-kdp_connector/connectors/Storage.py
 kdp_connector/connectors/__init__.py
-kdp_connector/connectors/audit_log.py
-kdp_connector/connectors/audit_log_configs.py
-kdp_connector/connectors/batch_write.py
 kdp_connector/connectors/index_management.py
+kdp_connector/connectors/ingest.py
 kdp_connector/connectors/ingest_job_api.py
 kdp_connector/connectors/kdp_api.py
 kdp_connector/connectors/query.py
 kdp_connector/connectors/read.py
 kdp_connector/connectors/upload.py
 kdp_python_connector.egg-info/PKG-INFO
 kdp_python_connector.egg-info/SOURCES.txt
 kdp_python_connector.egg-info/dependency_links.txt
 kdp_python_connector.egg-info/requires.txt
 kdp_python_connector.egg-info/top_level.txt
 test/test_ingest.py
-test/test_keycloak.py
 test/test_read.py
```

### Comparing `kdp-python-connector-0.33.0/setup.py` & `kdp-python-connector-0.5.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,26 @@
-import sys
-
 from setuptools import setup, find_packages
 
-version = '0.0.1'
-if '--version' in sys.argv:
-    index = sys.argv.index('--version')
-    sys.argv.pop(index)
-    version = sys.argv.pop(index)
-
-name = 'kdp-python-connector'
-if '--name' in sys.argv:
-    index = sys.argv.index('--name')
-    sys.argv.pop(index)
-    name = sys.argv.pop(index)
-
+NAME = "kdp-python-connector"
+VERSION = "0.5.0"
 DESCRIPTION = 'Python Connector for KDP Platform'
 LONG_DESCRIPTION = 'Python Connector For Interacting with KDP Platform for various ingestion and retrieval tasks'
 
+
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
-        name=name,
-        version=version,
+        name=NAME,
+        version=VERSION,
         author="Koverse development team",
         author_email="developer@koverse.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=['pandas', 'numpy', 'kdp-api-python-client','python-keycloak'], # add any additional packages that
+        install_requires=['pandas', 'numpy'], # add any additional packages that
         # needs to be installed along with your package. Eg: 'caer'
 
         keywords=['python', 'kdp'],
         # classifiers= [
         #     "Development Status :: 3 - Alpha",
         #     "Intended Audience :: Science/Research",
         #     "Intended Audience :: Developers",
```

### Comparing `kdp-python-connector-0.33.0/test/test_ingest.py` & `kdp-python-connector-0.5.0/test/test_ingest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         self.dataset_id = 'd851a97f-b94a-465a-ae9c-207df0a8260f'
         self.host = 'https://api.koverse.localhost'
         self.input_file = '~/documents/Test documents/WithDates.csv'
         self.write_batch_response = WriteBatchResponse(workspace=self.workspace_id,
                                                        dataset_id=self.dataset_id,
                                                        partitions=[0, 1])
         self.api_instance = Mock()
-        self.api_instance.post_write_id.return_value = self.write_batch_response
+        self.api_instance.write.return_value = self.write_batch_response
 
     @staticmethod
     def getDataframe(size: int):
         data = []
         for x in range(size):
             data.append({'name': 'tom', 'age': 20 + x})
         return pd.DataFrame(data)
@@ -50,17 +50,17 @@
             self.setup()
             mock_api_instance = self.api_instance
 
             with(mock.patch('kdp_api.ApiClient')):
                 with(mock.patch('kdp_api.Configuration')):
                     with(mock.patch('kdp_api.api.write_api.WriteApi', side_effect=[mock_api_instance])):
                         kdp_conn = KdpConn()
-                        partitions_set = kdp_conn.batch_write(self.getDataframe(case.records), self.dataset_id, self.JWT,
-                                                              case.batch_size)
-                        self.assertEqual(len(mock_api_instance.post_write_id.mock_calls), case.expected_batches,
+                        partitions_set = kdp_conn.batch_ingest(self.getDataframe(case.records), self.dataset_id, self.JWT,
+                                                         case.batch_size)
+                        self.assertEqual(len(mock_api_instance.write.mock_calls), case.expected_batches,
                                          'FAILURE: for records=' + str(case.records) +
                                          ' and batch_size=' + str(case.batch_size) +
                                          ' expected_batches did not equal ' + str(case.expected_batches))
 
     def test_ingest_dataframe(self):
         self.setup()
         self.batch_size = 10
@@ -72,17 +72,17 @@
 
         with(mock.patch('kdp_api.ApiClient')):
             with(mock.patch('kdp_api.Configuration')):
                 with(mock.patch('kdp_api.api.write_api.WriteApi', side_effect=[mock_api_instance])):
                     self.setup()
                     self.batch_size = 10
                     kdp_conn = KdpConn()
-                    partitions_set = kdp_conn.batch_write(self.getDataframe(4), self.dataset_id, self.JWT,
-                                                          self.batch_size)
-                    mock_api_instance.post_write_id.assert_has_calls(expected_write_calls)
+                    partitions_set = kdp_conn.batch_ingest(self.getDataframe(4), self.dataset_id, self.JWT,
+                                                     self.batch_size)
+                    mock_api_instance.write.assert_has_calls(expected_write_calls)
 
         expected_partitions_set = {0, 1}
         self.assertEqual(expected_partitions_set, partitions_set)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-python-connector-0.33.0/test/test_read.py` & `kdp-python-connector-0.5.0/test/test_read.py`

 * *Files identical despite different names*

