# Comparing `tmp/grafana-api-sdk-0.2.0.tar.gz` & `tmp/grafana-api-sdk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grafana-api-sdk-0.2.0.tar", last modified: Wed Jun 28 18:49:37 2023, max compression
+gzip compressed data, was "grafana-api-sdk-0.3.0.tar", last modified: Sat Aug  5 20:15:53 2023, max compression
```

## Comparing `grafana-api-sdk-0.2.0.tar` & `grafana-api-sdk-0.3.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:49:37.338922 grafana-api-sdk-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-06-28 18:49:37.338922 grafana-api-sdk-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:49:37.338922 grafana-api-sdk-0.2.0/grafana_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19022 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    41670 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/alerting.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/alerting_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)    34167 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/alerting_provisioning.py
--rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/correlations.py
--rw-r--r--   0 runner    (1001) docker     (123)    22349 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    28697 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/external_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/legacy_alerting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/legacy_playlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/library.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/licensing.py
--rw-r--r--   0 runner    (1001) docker     (123)    26267 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    19500 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/organisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/other_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/playlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/query_history.py
--rw-r--r--   0 runner    (1001) docker     (123)    46835 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/rbac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/search.py
--rw-r--r--   0 runner    (1001) docker     (123)    15748 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/short_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/team.py
--rw-r--r--   0 runner    (1001) docker     (123)    17682 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/grafana_api/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 18:49:37.338922 grafana-api-sdk-0.2.0/grafana_api_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-06-28 18:49:37.000000 grafana-api-sdk-0.2.0/grafana_api_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-28 18:49:37.000000 grafana-api-sdk-0.2.0/grafana_api_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 18:49:37.000000 grafana-api-sdk-0.2.0/grafana_api_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-28 18:49:37.000000 grafana-api-sdk-0.2.0/grafana_api_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-28 18:49:37.000000 grafana-api-sdk-0.2.0/grafana_api_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 18:49:37.338922 grafana-api-sdk-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-28 18:49:02.000000 grafana-api-sdk-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 20:15:53.578186 grafana-api-sdk-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-08-05 20:15:53.578186 grafana-api-sdk-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11977 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 20:15:53.574186 grafana-api-sdk-0.3.0/grafana_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19025 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41838 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/alerting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/alerting_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34379 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/alerting_provisioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13172 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/correlations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22354 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28742 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/external_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11388 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/legacy_alerting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/legacy_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/licensing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26393 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19500 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/organisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/other_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/query_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46835 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/rbac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/short_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17682 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/grafana_api/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 20:15:53.578186 grafana-api-sdk-0.3.0/grafana_api_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-08-05 20:15:53.000000 grafana-api-sdk-0.3.0/grafana_api_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-05 20:15:53.000000 grafana-api-sdk-0.3.0/grafana_api_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 20:15:53.000000 grafana-api-sdk-0.3.0/grafana_api_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-05 20:15:53.000000 grafana-api-sdk-0.3.0/grafana_api_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-05 20:15:53.000000 grafana-api-sdk-0.3.0/grafana_api_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 20:15:53.578186 grafana-api-sdk-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-08-05 20:15:30.000000 grafana-api-sdk-0.3.0/setup.py
```

### Comparing `grafana-api-sdk-0.2.0/LICENSE` & `grafana-api-sdk-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.2.0/PKG-INFO` & `grafana-api-sdk-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: grafana-api-sdk
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Grafana API SDK
 Home-page: https://github.com/ZPascal/grafana_api_sdk
 Author: Pascal Zimmermann
 Author-email: info@theiotstudio.com
 Project-URL: Source, https://github.com/ZPascal/grafana_api_sdk
 Project-URL: Bug Tracker, https://github.com/ZPascal/grafana_api_sdk/issues
 Project-URL: Documentation, https://zpascal.github.io/grafana_api_sdk/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: http2
 License-File: LICENSE
 
 # Grafana API SDK 
-The repository includes a Python SDK for the Grafana API. It's possible to communicate with the Grafana API endpoints. Another feature of the SDK is the possibility to specify the used folder for the dashboard.
+The repository includes an SDK for the Grafana API. It's possible to interact with all public available Grafana HTTP API endpoints.
 
 ## Differences between [grafana-client](https://github.com/panodata/grafana-client), [grafana_api](https://github.com/m0nhawk/grafana_api/) and the [grafana_api_sdk](https://github.com/ZPascal/grafana_api_sdk)
 The grafana-client is only a fork of the non-maintained grafana_api repository. In general, the grafana-client project started at the same time, as I started this project. The corresponding SDK is a completely new project and based on non-other project and include a few features that are currently not implemented inside the grafana-client.
 
-The main feature that is implemented inside this library:
+The core features that are implemented inside this library:
 
-- Grafana V8 Alerting API support (possibility to communicate (currently read only) with the attached Prometheus and Alertmanager)
+- All public Grafana API (HTTP) endpoints are supported
+- Full API support for Grafana legacy alerting, current alerting, alerting channels and alert provisioning
+- Possibility to specify custom and self-signed certificates
+- HTTP/2 support
 
 In general my focus inside this project is to implement and deliver old and new features from the Grafana API, to document all features and functionality clear and to increase the overall test coverage of the project.
 
 ## Currently, supported features
 
 ### Dashboard
 - Create/ Update a dashboard 
@@ -243,14 +247,15 @@
 - Unstar a query inside the history
 
 ### Other HTTP
 - Get frontend settings
 - Renew login session 
 - Get health status
 - Get metrics
+- Get Plugin metrics
 
 ### Licensing
 - Check license availability
 - Manually force license refresh
 - Remove the license from the database
 
 ### Annotation
@@ -303,14 +308,18 @@
 - Search service accounts
 - Create a service account
 - Get service account by id
 - Update a service account
 - Get service account token by id
 - Create service account token by id
 - Delete service account by id
+- Migrate API token to service account by token id
+- Revert the generated service account to API token
+- Get service account migration status
+- Hide the API keys tab inside the UI
 
 ### RBAC
 - Get status
 - Get all roles
 - Get role
 - Create role
 - Update role
```

### Comparing `grafana-api-sdk-0.2.0/README.md` & `grafana-api-sdk-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # Grafana API SDK ![Coverage report](https://github.com/ZPascal/grafana_api_sdk/blob/main/docs/coverage.svg)
-The repository includes a Python SDK for the Grafana API. It's possible to communicate with the Grafana API endpoints. Another feature of the SDK is the possibility to specify the used folder for the dashboard.
+The repository includes an SDK for the Grafana API. It's possible to interact with all public available Grafana HTTP API endpoints.
 
 ## Differences between [grafana-client](https://github.com/panodata/grafana-client), [grafana_api](https://github.com/m0nhawk/grafana_api/) and the [grafana_api_sdk](https://github.com/ZPascal/grafana_api_sdk)
 The grafana-client is only a fork of the non-maintained grafana_api repository. In general, the grafana-client project started at the same time, as I started this project. The corresponding SDK is a completely new project and based on non-other project and include a few features that are currently not implemented inside the grafana-client.
 
-The main feature that is implemented inside this library:
+The core features that are implemented inside this library:
 
-- Grafana V8 Alerting API support (possibility to communicate (currently read only) with the attached Prometheus and Alertmanager)
+- All public Grafana API (HTTP) endpoints are supported
+- Full API support for Grafana legacy alerting, current alerting, alerting channels and alert provisioning
+- Possibility to specify custom and self-signed certificates
+- HTTP/2 support
 
 In general my focus inside this project is to implement and deliver old and new features from the Grafana API, to document all features and functionality clear and to increase the overall test coverage of the project.
 
 ## Currently, supported features
 
 ### Dashboard
 - Create/ Update a dashboard 
@@ -226,14 +229,15 @@
 - Unstar a query inside the history
 
 ### Other HTTP
 - Get frontend settings
 - Renew login session 
 - Get health status
 - Get metrics
+- Get Plugin metrics
 
 ### Licensing
 - Check license availability
 - Manually force license refresh
 - Remove the license from the database
 
 ### Annotation
@@ -286,14 +290,18 @@
 - Search service accounts
 - Create a service account
 - Get service account by id
 - Update a service account
 - Get service account token by id
 - Create service account token by id
 - Delete service account by id
+- Migrate API token to service account by token id
+- Revert the generated service account to API token
+- Get service account migration status
+- Hide the API keys tab inside the UI
 
 ### RBAC
 - Get status
 - Get all roles
 - Get role
 - Create role
 - Update role
```

### Comparing `grafana-api-sdk-0.2.0/grafana_api/admin.py` & `grafana-api-sdk-0.3.0/grafana_api/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import logging
-from urllib3 import response
+from httpx import Response
 
 from .model import (
     APIModel,
     APIEndpoints,
     RequestsMethods,
     GlobalUser,
 )
@@ -540,18 +540,18 @@
         Raises:
             Exception: Unspecified error by executing the API call
 
         Returns:
             None
         """
 
-        api_call: response = Api(self.grafana_api_model).call_the_api(
+        api_call: Response = Api(self.grafana_api_model).call_the_api(
             f"{APIEndpoints.ADMIN.value}/encryption/rotate-data-keys",
             RequestsMethods.POST,
             json.dumps(dict()),
         )
 
-        if api_call.status != 204:
+        if api_call.status_code != 204:
             logging.error(f"Please, check the error: {api_call}.")
             raise Exception
         else:
             logging.info("You successfully rotated the data keys.")
```

### Comparing `grafana-api-sdk-0.2.0/grafana_api/alerting.py` & `grafana-api-sdk-0.3.0/grafana_api/alerting.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,16 +35,16 @@
             ValueError: Missed specifying a necessary value
             Exception: Unspecified error by executing the API call
 
         Returns:
             api_call (list): Returns the list of Alertmanager alerts
         """
 
-        if (type(recipient) == int and recipient != 0) or (
-            type(recipient) == str and len(recipient) != 0
+        if (isinstance(recipient, int) and recipient != 0) or (
+            isinstance(recipient, str) and len(recipient) != 0
         ):
             api_call: list = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.ALERTS_ALERTMANAGER.value}/{recipient}/api/v2/alerts",
             )
 
             if api_call == list() or api_call[0].get("receivers") is None:
                 logging.error(f"Please, check the error: {api_call}.")
@@ -69,16 +69,16 @@
             Exception: Unspecified error by executing the API call
 
         Returns:
             None
         """
 
         if (
-            (type(recipient) == int and recipient != 0)
-            or (type(recipient) == str and len(recipient) != 0)
+            (isinstance(recipient, int) and recipient != 0)
+            or (isinstance(recipient, str) and len(recipient) != 0)
         ) and alerts != list():
             alerts_json_list: list = list()
 
             for alert in alerts:
                 alert_json_dict: dict = dict(
                     {
                         "startsAt": alert.starts_at,
@@ -115,16 +115,16 @@
             ValueError: Missed specifying a necessary value
             Exception: Unspecified error by executing the API call
 
         Returns:
             api_call (list): Returns the list of Alertmanager group alerts
         """
 
-        if (type(recipient) == int and recipient != 0) or (
-            type(recipient) == str and len(recipient) != 0
+        if (isinstance(recipient, int) and recipient != 0) or (
+            isinstance(recipient, str) and len(recipient) != 0
         ):
             api_call: list = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.ALERTS_ALERTMANAGER.value}/{recipient}/api/v2/alerts",
             )
 
             if api_call == list() or api_call[0].get("alerts") is None:
                 logging.error(f"Please, check the error: {api_call}.")
@@ -149,16 +149,16 @@
             Exception: Unspecified error by executing the API call
 
         Returns:
             None
         """
 
         if (
-            (type(recipient) == int and recipient != 0)
-            or (type(recipient) == str and len(recipient) != 0)
+            (isinstance(recipient, int) and recipient != 0)
+            or (isinstance(recipient, str) and len(recipient) != 0)
         ) and len(silence_id) != 0:
             api_call: dict = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.ALERTS_ALERTMANAGER.value}/{recipient}/api/v2/silence/{silence_id}",
                 RequestsMethods.DELETE,
             )
 
             if api_call != dict():
@@ -184,16 +184,16 @@
             Exception: Unspecified error by executing the API call
 
         Returns:
             api_call (dict): Returns the dict of Alertmanager silence alert
         """
 
         if (
-            (type(recipient) == int and recipient != 0)
-            or (type(recipient) == str and len(recipient) != 0)
+            (isinstance(recipient, int) and recipient != 0)
+            or (isinstance(recipient, str) and len(recipient) != 0)
         ) and len(silence_id) != 0:
             api_call: dict = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.ALERTS_ALERTMANAGER.value}/{recipient}/api/v2/silence/{silence_id}",
             )
 
             if api_call == dict() or api_call.get("id") is None:
                 logging.error(f"Check the error: {api_call}.")
@@ -214,16 +214,16 @@
             ValueError: Missed specifying a necessary value
             Exception: Unspecified error by executing the API call
 
         Returns:
             api_call (list): Returns the list of Alertmanager silence alerts
         """
 
-        if (type(recipient) == int and recipient != 0) or (
-            type(recipient) == str and len(recipient) != 0
+        if (isinstance(recipient, int) and recipient != 0) or (
+            isinstance(recipient, str) and len(recipient) != 0
         ):
             api_call: list = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.ALERTS_ALERTMANAGER.value}/{recipient}/api/v2/silences",
             )
 
             if api_call == list() or api_call[0].get("id") is None:
                 logging.error(f"Check the error: {api_call}.")
@@ -248,16 +248,16 @@
             Exception: Unspecified error by executing the API call
 
         Returns:
             api_call (dict): Returns the dict of newly created silence alert
         """
 
         if (
-            (type(recipient) == int and recipient != 0)
-            or (type(recipient) == str and len(recipient) != 0)
+            (isinstance(recipient, int) and recipient != 0)
+            or (isinstance(recipient, str) and len(recipient) != 0)
         ) or silence is not None:
             silence_json_dict: dict = dict(
                 {
                     "comment": silence.comment,
                     "createdBy": silence.created_by,
                     "endsAt": silence.ends_at,
                     "id": silence.id,
@@ -291,16 +291,16 @@
             ValueError: Missed specifying a necessary value
             Exception: Unspecified error by executing the API call
 
         Returns:
             api_call (dict): Returns the dict of the Alertmanager status
         """
 
-        if (type(recipient) == int and recipient != 0) or (
-            type(recipient) == str and len(recipient) != 0
+        if (isinstance(recipient, int) and recipient != 0) or (
+            isinstance(recipient, str) and len(recipient) != 0
         ):
             api_call: dict = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.ALERTS_ALERTMANAGER.value}/{recipient}/api/v2/status",
             )
 
             if api_call == dict() or api_call.get("config") is None:
                 logging.error(f"Check the error: {api_call}.")
@@ -321,16 +321,16 @@
             ValueError: Missed specifying a necessary value
             Exception: Unspecified error by executing the API call
 
         Returns:
             None
         """
 
-        if (type(recipient) == int and recipient != 0) or (
-            type(recipient) == str and len(recipient) != 0
+        if (isinstance(recipient, int) and recipient != 0) or (
+            isinstance(recipient, str) and len(recipient) != 0
         ):
             api_call: dict = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.ALERTS_ALERTMANAGER.value}/{recipient}/config/api/v1/alerts",
                 RequestsMethods.DELETE,
             )
 
             if (
@@ -355,16 +355,16 @@
             ValueError: Missed specifying a necessary value
             Exception: Unspecified error by executing the API call
 
         Returns:
             api_call (dict): Returns the dict of the Alertmanager config
         """
 
-        if (type(recipient) == int and recipient != 0) or (
-            type(recipient) == str and len(recipient) != 0
+        if (isinstance(recipient, int) and recipient != 0) or (
+            isinstance(recipient, str) and len(recipient) != 0
         ):
             api_call: dict = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.ALERTS_ALERTMANAGER.value}/{recipient}/config/api/v1/alerts",
             )
 
             if api_call == dict() or api_call.get("alertmanager_config") is None:
                 logging.error(f"Check the error: {api_call}.")
@@ -393,16 +393,16 @@
             Exception: Unspecified error by executing the API call
 
         Returns:
             None
         """
 
         if (
-            (type(recipient) == int and recipient != 0)
-            or (type(recipient) == str and len(recipient) != 0)
+            (isinstance(recipient, int) and recipient != 0)
+            or (isinstance(recipient, str) and len(recipient) != 0)
         ) and alertmanager_config is not None:
             alertmanager_configuration_json_dict: dict = dict()
 
             alertmanager_configuration_json_dict["alertmanager_config"] = dict(
                 {
                     "global": alertmanager_config.global_config,
                     "inhibit_rules": alertmanager_config.inhibit_rules,
@@ -451,16 +451,16 @@
 
         Returns:
             None
         """
 
         if (
             (
-                (type(recipient) == int and recipient != 0)
-                or (type(recipient) == str and len(recipient) != 0)
+                (isinstance(recipient, int) and recipient != 0)
+                or (isinstance(recipient, str) and len(recipient) != 0)
             )
             and alert != dict()
             and receivers is not None
         ):
             alertmanager_receivers_json_dict: dict = dict()
             receivers_list: list = list()
 
@@ -531,16 +531,16 @@
             ValueError: Missed specifying a necessary value
             Exception: Unspecified error by executing the API call
 
         Returns:
             api_call (dict): Returns the dict of the prometheus alerts
         """
 
-        if (type(recipient) == int and recipient != 0) or (
-            type(recipient) == str and len(recipient) != 0
+        if (isinstance(recipient, int) and recipient != 0) or (
+            isinstance(recipient, str) and len(recipient) != 0
         ):
             api_call: dict = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.ALERTS_PROMETHEUS.value}/{recipient}/api/v1/alerts",
             )
 
             if api_call == dict() or api_call.get("data") is None:
                 logging.error(f"Check the error: {api_call}.")
@@ -561,16 +561,16 @@
             ValueError: Missed specifying a necessary value
             Exception: Unspecified error by executing the API call
 
         Returns:
             api_call (dict): Returns the dict of the prometheus rules
         """
 
-        if (type(recipient) == int and recipient != 0) or (
-            type(recipient) == str and len(recipient) != 0
+        if (isinstance(recipient, int) and recipient != 0) or (
+            isinstance(recipient, str) and len(recipient) != 0
         ):
             api_call: dict = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.ALERTS_PROMETHEUS.value}/{recipient}/api/v1/rules",
             )
 
             if api_call == dict() or api_call.get("data") is None:
                 logging.error(f"Check the error: {api_call}.")
@@ -591,16 +591,16 @@
             ValueError: Missed specifying a necessary value
             Exception: Unspecified error by executing the API call
 
         Returns:
             api_call (dict): Returns the dict of the ruler rules
         """
 
-        if (type(recipient) == int and recipient != 0) or (
-            type(recipient) == str and len(recipient) != 0
+        if (isinstance(recipient, int) and recipient != 0) or (
+            isinstance(recipient, str) and len(recipient) != 0
         ):
             api_call: dict = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.ALERTS_RULER.value}/{recipient}/api/v1/rules",
             )
 
             if api_call == dict():
                 logging.error(f"Check the error: {api_call}.")
@@ -623,16 +623,16 @@
             Exception: Unspecified error by executing the API call
 
         Returns:
             None
         """
 
         if (
-            (type(recipient) == int and recipient != 0)
-            or (type(recipient) == str and len(recipient) != 0)
+            (isinstance(recipient, int) and recipient != 0)
+            or (isinstance(recipient, str) and len(recipient) != 0)
         ) and len(namespace) != 0:
             api_call: dict = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.ALERTS_RULER.value}/{recipient}/api/v1/rules/{namespace}",
                 RequestsMethods.DELETE,
             )
 
             if api_call != dict():
@@ -658,16 +658,16 @@
             Exception: Unspecified error by executing the API call
 
         Returns:
             api_call (dict): Returns the dict of the ruler groups
         """
 
         if (
-            (type(recipient) == int and recipient != 0)
-            or (type(recipient) == str and len(recipient) != 0)
+            (isinstance(recipient, int) and recipient != 0)
+            or (isinstance(recipient, str) and len(recipient) != 0)
         ) and len(namespace) != 0:
             api_call: dict = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.ALERTS_RULER.value}/{recipient}/api/v1/rules/{namespace}",
             )
 
             if api_call == dict():
                 logging.error(f"Check the error: {api_call}.")
@@ -701,16 +701,16 @@
 
         Returns:
             None
         """
 
         if (
             (
-                (type(recipient) == int and recipient != 0)
-                or (type(recipient) == str and len(recipient) != 0)
+                (isinstance(recipient, int) and recipient != 0)
+                or (isinstance(recipient, str) and len(recipient) != 0)
             )
             and len(namespace) != 0
             and len(group_name) != 0
             and rules != list()
         ):
             rules_json_list: list = list()
 
@@ -765,16 +765,16 @@
 
         Returns:
             None
         """
 
         if (
             (
-                (type(recipient) == int and recipient != 0)
-                or (type(recipient) == str and len(recipient) != 0)
+                (isinstance(recipient, int) and recipient != 0)
+                or (isinstance(recipient, str) and len(recipient) != 0)
             )
             and len(namespace) != 0
             and len(group_name) != 0
         ):
             api_call: dict = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.ALERTS_RULER.value}/{recipient}/api/v1/rules/{namespace}/{group_name}",
                 RequestsMethods.DELETE,
@@ -805,16 +805,16 @@
 
         Returns:
             api_call (dict): Returns the dict of all ruler groups
         """
 
         if (
             (
-                (type(recipient) == int and recipient != 0)
-                or (type(recipient) == str and len(recipient) != 0)
+                (isinstance(recipient, int) and recipient != 0)
+                or (isinstance(recipient, str) and len(recipient) != 0)
             )
             and len(namespace) != 0
             and len(group_name) != 0
         ):
             api_call: dict = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.ALERTS_RULER.value}/{recipient}/api/v1/rules/{namespace}/{group_name}",
             )
@@ -903,16 +903,16 @@
 
         Returns:
             api_call (dict): Returns the result of the specified recipient rule
         """
 
         if (
             (
-                (type(recipient) == int and recipient != 0)
-                or (type(recipient) == str and len(recipient) != 0)
+                (isinstance(recipient, int) and recipient != 0)
+                or (isinstance(recipient, str) and len(recipient) != 0)
             )
             and len(expr) != 0
             and len(condition) != 0
             and data_query != list()
         ):
             datasource_rule_query_objects_json: list = list()
             datasource_rule_query_object_json: dict = dict()
```

### Comparing `grafana-api-sdk-0.2.0/grafana_api/alerting_notifications.py` & `grafana-api-sdk-0.3.0/grafana_api/alerting_notifications.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.2.0/grafana_api/alerting_provisioning.py` & `grafana-api-sdk-0.3.0/grafana_api/alerting_provisioning.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,17 @@
                 raise Exception
             else:
                 logging.info("You successfully created the corresponding alert rule.")
         else:
             logging.error("There is no alert_rule defined.")
             raise ValueError
 
-    def update_alert_rule(self, uid: str, alert_rule: AlertRule, disable_provenance: bool = False):
+    def update_alert_rule(
+        self, uid: str, alert_rule: AlertRule, disable_provenance: bool = False
+    ):
         """The method includes a functionality to update an existing alert rule
 
         Args:
             uid (str): Specify the alert rule uid
             alert_rule (AlertRule): Specify the alert rule
             disable_provenance (bool): Specify if the provenance header should be set or not (default False)
 
@@ -125,15 +127,19 @@
             else:
                 logging.info("You successfully updated the corresponding alert rule.")
         else:
             logging.error("There is no uid or alert_rule defined.")
             raise ValueError
 
     def update_the_interval_of_a_alert_rule_group(
-        self, folder_uid: str, group: str, alert_rule_group_interval: int, disable_provenance: bool = False
+        self,
+        folder_uid: str,
+        group: str,
+        alert_rule_group_interval: int,
+        disable_provenance: bool = False,
     ):
         """The method includes a functionality to update the interval of a alert rule group
 
         Args:
             folder_uid (str): Specify the folder uid
             group (str): Specify the group
             alert_rule_group_interval (int): Specify the alert rule group interval
@@ -216,15 +222,19 @@
 
         if api_call == list():
             logging.error(f"Check the error: {api_call}.")
             raise Exception
         else:
             return api_call
 
-    def add_contact_point(self, embedded_contact_point: EmbeddedContactPoint, disable_provenance: bool = False):
+    def add_contact_point(
+        self,
+        embedded_contact_point: EmbeddedContactPoint,
+        disable_provenance: bool = False,
+    ):
         """The method includes a functionality to create a contact point
 
         Args:
             embedded_contact_point (EmbeddedContactPoint): Specify the embedded contact point
             disable_provenance (bool): Specify if the provenance header should be set or not (default False)
 
         Raises:
@@ -259,15 +269,18 @@
             else:
                 logging.info("You successfully created a new contact point.")
         else:
             logging.error("There is no embedded_contact_point defined.")
             raise ValueError
 
     def update_contact_point(
-        self, uid: str, embedded_contact_point: EmbeddedContactPoint, disable_provenance: bool = False
+        self,
+        uid: str,
+        embedded_contact_point: EmbeddedContactPoint,
+        disable_provenance: bool = False,
     ):
         """The method includes a functionality to update a contact point
 
         Args:
             uid (str): Specify the uid of the contact point
             embedded_contact_point (EmbeddedContactPoint): Specify the embedded contact point
             disable_provenance (bool): Specify if the provenance header should be set or not (default False)
@@ -401,15 +414,15 @@
             api_call (list): Returns all mute timings
         """
 
         api_call: list = Api(self.grafana_api_model).call_the_api(
             f"{APIEndpoints.ALERTING_PROVISIONING.value}/mute-timings",
         )
 
-        if type(api_call) != list:
+        if isinstance(api_call, list) is False:
             logging.error(f"Check the error: {api_call}.")
             raise Exception
         else:
             return api_call
 
     def get_mute_timing(self, name: str) -> dict:
         """The method includes a functionality to get a mute timings specified by the name
@@ -435,15 +448,17 @@
                 raise Exception
             else:
                 return api_call
         else:
             logging.error("There is no name defined.")
             raise ValueError
 
-    def add_mute_timing(self, mute_time_interval: MuteTimeInterval, disable_provenance: bool = False):
+    def add_mute_timing(
+        self, mute_time_interval: MuteTimeInterval, disable_provenance: bool = False
+    ):
         """The method includes a functionality to create a mute timing
 
         Args:
             mute_time_interval (MuteTimeInterval): Specify the mute time interval
             disable_provenance (bool): Specify if the provenance header should be set or not (default False)
 
         Raises:
@@ -468,15 +483,20 @@
                 raise Exception
             else:
                 logging.info("You successfully added the mute timing.")
         else:
             logging.error("There is no mute_time_interval defined.")
             raise ValueError
 
-    def update_mute_timing(self, name: str, mute_time_interval: MuteTimeInterval, disable_provenance: bool = False):
+    def update_mute_timing(
+        self,
+        name: str,
+        mute_time_interval: MuteTimeInterval,
+        disable_provenance: bool = False,
+    ):
         """The method includes a functionality to update an existing mute timing
 
         Args:
             name (str): Specify the mute timing name
             mute_time_interval (MuteTimeInterval): Specify the mute time interval
             disable_provenance (bool): Specify if the provenance header should be set or not (default False)
 
@@ -546,15 +566,15 @@
             api_call (list): Returns all message templates
         """
 
         api_call: list = Api(self.grafana_api_model).call_the_api(
             f"{APIEndpoints.ALERTING_PROVISIONING.value}/templates",
         )
 
-        if type(api_call) != list:
+        if isinstance(api_call, list) is False:
             logging.error(f"Check the error: {api_call}.")
             raise Exception
         else:
             return api_call
 
     def get_message_template(self, name: str) -> dict:
         """The method includes a functionality to get a message template specified by the name
@@ -581,15 +601,17 @@
                 raise Exception
             else:
                 return api_call
         else:
             logging.error("There is no name defined.")
             raise ValueError
 
-    def create_or_update_message_template(self, name: str, message_template: str, disable_provenance: bool = False):
+    def create_or_update_message_template(
+        self, name: str, message_template: str, disable_provenance: bool = False
+    ):
         """The method includes a functionality to create or update a message template
 
         Args:
             name (str): Specify the message template name
             message_template (str): Specify the message template
             disable_provenance (bool): Specify if the provenance header should be set or not (default False)
 
@@ -680,15 +702,15 @@
 
         Returns:
             result (list, None): Returns the mute time interval list or None
         """
 
         mute_timing_interval_list: list = list()
 
-        if time_intervals is not None and type(time_intervals) == list:
+        if time_intervals is not None and isinstance(time_intervals, list):
             for time_interval in time_intervals:
                 mute_timing_interval_list.append(
                     {
                         "days_of_month": time_interval.days_of_month,
                         "months": time_interval.months,
                         "times": self.__create_time_range_list(time_interval.times),
                         "weekdays": time_interval.weekdays,
@@ -709,15 +731,15 @@
 
         Returns:
             timing_list (list): Returns the time list
         """
 
         timing_list: list = list()
 
-        if timing is not None and type(timing) == list:
+        if timing is not None and isinstance(timing, list):
             for time in timing:
                 timing_list.append(
                     {"start_time": time.start_time, "end_time": time.end_time}
                 )
 
             return timing_list
         else:
@@ -758,15 +780,15 @@
 
         Returns:
             result (list, None): Returns the alert routes list or None
         """
 
         routes_list: list = list()
 
-        if routes is not None and type(routes) == list:
+        if routes is not None and isinstance(routes, list):
             for route in routes:
                 routes_list.append(self.__create_alert_route_dictionary(route))
 
             return routes_list
         else:
             return routes
 
@@ -779,15 +801,15 @@
 
         Returns:
             route_matchers_list (list): Returns the list of object matchers
         """
 
         route_matchers_list: list = list()
 
-        if matchers is not None and type(matchers) == list:
+        if matchers is not None and isinstance(matchers, list):
             for matcher in matchers:
                 route_matcher_dict: dict = dict(
                     {
                         "name": matcher.name,
                         "type": matcher.type.value,
                         "value": matcher.value,
                     }
```

### Comparing `grafana-api-sdk-0.2.0/grafana_api/annotations.py` & `grafana-api-sdk-0.3.0/grafana_api/annotations.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.2.0/grafana_api/api.py` & `grafana-api-sdk-0.3.0/grafana_api/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import logging
 import json
 import base64
+from typing import Union
 
-import urllib3
-from urllib3 import exceptions
+import httpx
+from httpx import ConnectError
+import asyncio
 
 from .model import RequestsMethods, ERROR_MESSAGES, APIModel
 
 
 class Api:
     """The class includes all necessary methods to make API calls to the Grafana API endpoints
 
@@ -62,73 +64,174 @@
                 )
             ).decode("utf-8")
             headers.update({"Authorization": f"Basic {credentials}"})
 
         headers["Content-Type"] = "application/json"
         headers["Accept"] = "application/json"
 
-        if org_id_header is not None and type(org_id_header) == int:
+        if org_id_header is not None and isinstance(org_id_header, int):
             headers["X-Grafana-Org-Id"] = org_id_header
 
-        if type(disable_provenance_header) == bool and disable_provenance_header:
+        if isinstance(disable_provenance_header, bool) and disable_provenance_header:
             headers["X-Disable-Provenance"] = f"{disable_provenance_header}"
 
-        http = urllib3.PoolManager(
-            num_pools=self.grafana_api_model.num_pools,
-            retries=self.grafana_api_model.retries,
-            headers=headers,
-            timeout=self.grafana_api_model.timeout,
-            ssl_context=self.grafana_api_model.ssl_context,
+        http: Union[httpx.Client, httpx.AsyncClient] = self.create_the_http_api_client(
+            headers
         )
 
+        if self.grafana_api_model.http2_support:
+
+            async def _execute_async_api_call():
+                async with http:
+                    return await self._execute_the_async_api_call(
+                        http, method, api_url, response_status_code, json_complete
+                    )
+
+            return asyncio.run(_execute_async_api_call())
+
+        return self._execute_the_api_call(
+            http, method, api_url, response_status_code, json_complete
+        )
+
+    def _execute_the_api_call(
+        self,
+        http: httpx.Client,
+        method: RequestsMethods,
+        api_url: str,
+        response_status_code: bool,
+        json_complete: str,
+    ) -> any:
+        """The method includes a functionality to execute a synchronous api call
+
+        Args:
+            http (httpx.Client): Specify the used synchronous client
+            method (RequestsMethods): Specify the used method
+            api_url (str): Specify the used api url
+            response_status_code (bool): Specify if the response code should be returned
+            json_complete (str): Specify the forwarded json in case of patch, post or put calls
+
+        Raises:
+            Exception: Unspecified error by executing the API call
+
+        Returns:
+            api_call (any): Returns the value of the api call
+        """
+
         try:
             if method.value == RequestsMethods.GET.value:
-                return Api.__check_the_api_call_response(
+                return self._check_the_api_call_response(
                     http.request("GET", api_url),
                     response_status_code,
                 )
             elif method.value == RequestsMethods.PUT.value:
                 if json_complete is not None:
-                    return Api.__check_the_api_call_response(
-                        http.request("PUT", api_url, body=json_complete),
+                    return self._check_the_api_call_response(
+                        http.request("PUT", api_url, content=json_complete),
                         response_status_code,
                     )
                 else:
                     logging.error("Please define the json_complete.")
                     raise Exception
             elif method.value == RequestsMethods.POST.value:
                 if json_complete is not None:
-                    return Api.__check_the_api_call_response(
-                        http.request("POST", api_url, body=json_complete),
+                    return self._check_the_api_call_response(
+                        http.request("POST", api_url, content=json_complete),
                         response_status_code,
                     )
                 else:
                     logging.error("Please define the json_complete.")
                     raise Exception
             elif method.value == RequestsMethods.PATCH.value:
                 if json_complete is not None:
-                    return Api.__check_the_api_call_response(
-                        http.request("PATCH", api_url, body=json_complete),
+                    return self._check_the_api_call_response(
+                        http.request("PATCH", api_url, content=json_complete),
                         response_status_code,
                     )
                 else:
                     logging.error("Please define the json_complete.")
                     raise Exception
             elif method.value == RequestsMethods.DELETE.value:
-                return Api.__check_the_api_call_response(
+                return self._check_the_api_call_response(
                     http.request("DELETE", api_url), response_status_code
                 )
             else:
                 logging.error("Please define a valid method.")
                 raise Exception
         except Exception as e:
             raise e
 
+    async def _execute_the_async_api_call(
+        self,
+        http: httpx.AsyncClient,
+        method: RequestsMethods,
+        api_url: str,
+        response_status_code: bool,
+        json_complete: str,
+    ):
+        """The method includes a functionality to execute an asynchronous api call
+
+        Args:
+            http (httpx.AsyncClient): Specify the used asynchronous client
+            method (RequestsMethods): Specify the used method
+            api_url (str): Specify the used api url
+            response_status_code (bool): Specify if the response code should be returned
+            json_complete (str): Specify the forwarded json in case of patch, post or put calls
+
+        Raises:
+            Exception: Unspecified error by executing the API call
+
+        Returns:
+            api_call (any): Returns the value of the api call
+        """
+
+        try:
+            if method.value == RequestsMethods.GET.value:
+                return self._check_the_api_call_response(
+                    await http.request("GET", api_url),
+                    response_status_code,
+                )
+            elif method.value == RequestsMethods.PUT.value:
+                if json_complete is not None:
+                    return self._check_the_api_call_response(
+                        await http.request("PUT", api_url, content=json_complete),
+                        response_status_code,
+                    )
+                else:
+                    logging.error("Please define the json_complete.")
+                    raise Exception
+            elif method.value == RequestsMethods.POST.value:
+                if json_complete is not None:
+                    return self._check_the_api_call_response(
+                        await http.request("POST", api_url, content=json_complete),
+                        response_status_code,
+                    )
+                else:
+                    logging.error("Please define the json_complete.")
+                    raise Exception
+            elif method.value == RequestsMethods.PATCH.value:
+                if json_complete is not None:
+                    return self._check_the_api_call_response(
+                        await http.request("PATCH", api_url, content=json_complete),
+                        response_status_code,
+                    )
+                else:
+                    logging.error("Please define the json_complete.")
+                    raise Exception
+            elif method.value == RequestsMethods.DELETE.value:
+                return self._check_the_api_call_response(
+                    await http.request("DELETE", api_url), response_status_code
+                )
+            else:
+                logging.error("Please define a valid method.")
+                raise Exception
+        except Exception as e:
+            raise e
+
     @staticmethod
-    def __check_the_api_call_response(
+    def _check_the_api_call_response(
         response: any = None, response_status_code: bool = False
     ) -> any:
         """The method includes a functionality to check the output of API call method for errors
 
         Args:
             response (any): Specify the inserted response
             response_status_code (bool): Specify if the original status code should be attached to the result (default False)
@@ -136,58 +239,105 @@
         Raises:
             Exception: Unspecified error by executing the API call
 
         Returns:
             api_call (any): Returns the value of the api call
         """
 
-        if Api.__check_if_valid_json(response.data.decode("utf-8")):
+        if Api._check_if_valid_json(response.text):
             if (
-                len(json.loads(response.data.decode("utf-8"))) != 0
-                and type(json.loads(response.data.decode("utf-8"))) == dict
+                len(json.loads(response.text)) != 0
+                and type(json.loads(response.text)) == dict
             ):
                 if (
-                    "message" in json.loads(response.data.decode("utf-8")).keys()
-                    and json.loads(response.data.decode("utf-8"))["message"]
-                    in ERROR_MESSAGES
+                    "message" in json.loads(response.text).keys()
+                    and json.loads(response.text)["message"] in ERROR_MESSAGES
                 ):
-                    logging.error(json.loads(response.data.decode("utf-8"))["message"])
-                    raise exceptions.ConnectionError
+                    logging.error(json.loads(response.text)["message"])
+                    raise ConnectError(str(json.loads(response.text)["message"]))
 
-            json_response: (dict | list) = json.loads(response.data.decode("utf-8"))
+            json_response: Union[dict, list] = json.loads(response.text)
 
-            if type(json_response) == dict and response_status_code:
-                json_response.update({"status": response.status})
-            elif type(json_response) == list and response_status_code:
-                json_response[0].update({"status": response.status})
+            if isinstance(json_response, dict) and response_status_code:
+                json_response.update({"status": response.status_code})
+            elif isinstance(json_response, list) and response_status_code:
+                json_response[0].update({"status": response.status_code})
             return json_response
         else:
             if response_status_code:
-                return dict(
-                    {"status": response.status, "data": response.data.decode("utf-8")}
-                )
+                return dict({"status": response.status_code, "data": response.text})
             else:
                 return response
 
     @staticmethod
-    def __check_if_valid_json(response: any) -> bool:
+    def _check_if_valid_json(response: any) -> bool:
         """The method includes a functionality to check if the response json is valid
 
         Args:
             response (any): Specify the inserted response json
 
         Returns:
-            api_call (bool): Returns if the json is valid or not
+            result (bool): Returns if the json is valid or not
         """
 
         try:
             json.loads(response)
         except (TypeError, ValueError):
             return False
         return True
 
     @staticmethod
     def prepare_api_string(query_string: str) -> str:
+        """The method includes a functionality to prepare the api string for the queries
+
+        Args:
+            query_string (str): Specify the corresponding query string
+
+        Returns:
+            query_string (str): Returns the adjusted query string
+        """
+
         if len(query_string) >= 1:
             return f"{query_string}&"
         else:
             return query_string
+
+    def create_the_http_api_client(
+        self, headers: dict = None
+    ) -> Union[httpx.Client, httpx.AsyncClient]:
+        """The method includes a functionality to create the corresponding HTTP client
+
+        Args:
+            headers (dict): Specify the optional inserted headers (Default None)
+
+        Returns:
+            client (Union[httpx.Client, httpx.AsyncClient]): Returns the corresponding client
+        """
+
+        transport: httpx.HTTPTransport = httpx.HTTPTransport(
+            retries=self.grafana_api_model.retries
+        )
+        limits: httpx.Limits = httpx.Limits(
+            max_connections=self.grafana_api_model.num_pools
+        )
+        http2: bool = self.grafana_api_model.http2_support
+
+        if http2:
+            async_transport: httpx.AsyncHTTPTransport = httpx.AsyncHTTPTransport(
+                retries=self.grafana_api_model.retries, http2=http2
+            )
+            return httpx.AsyncClient(
+                http2=True,
+                limits=limits,
+                timeout=self.grafana_api_model.timeout,
+                headers=headers,
+                transport=async_transport,
+                verify=self.grafana_api_model.ssl_context,
+            )
+        else:
+            return httpx.Client(
+                limits=limits,
+                timeout=self.grafana_api_model.timeout,
+                headers=headers,
+                transport=transport,
+                verify=self.grafana_api_model.ssl_context,
+            )
```

### Comparing `grafana-api-sdk-0.2.0/grafana_api/authentication.py` & `grafana-api-sdk-0.3.0/grafana_api/authentication.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.2.0/grafana_api/correlations.py` & `grafana-api-sdk-0.3.0/grafana_api/correlations.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.2.0/grafana_api/dashboard.py` & `grafana-api-sdk-0.3.0/grafana_api/dashboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -563,19 +563,19 @@
 
                 api_call: any = Api(self.grafana_api_model).call_the_api(
                     f"{APIEndpoints.DASHBOARDS.value}/calculate-diff",
                     RequestsMethods.POST,
                     json.dumps(diff_object),
                 )
 
-                if api_call.status != 200:
-                    logging.error(f"Check the error: {api_call.data}.")
+                if api_call.status_code != 200:
+                    logging.error(f"Check the error: {api_call.text}.")
                     raise Exception
                 else:
-                    return api_call.data
+                    return api_call.text
             else:
                 logging.error(
                     "There is no dashboard_uid_and_version_base or dashboard_uid_and_version_new defined."
                 )
                 raise ValueError
         else:
             logging.error(
```

### Comparing `grafana-api-sdk-0.2.0/grafana_api/datasource.py` & `grafana-api-sdk-0.3.0/grafana_api/datasource.py`

 * *Files 0% similar despite different names*

```diff
@@ -708,15 +708,17 @@
                 raise Exception
             else:
                 return api_call
         else:
             logging.error("There is no uid defined.")
             raise ValueError
 
-    def update_datasource_cache(self, uid: str, datasource_cache: DatasourceCache) -> dict:
+    def update_datasource_cache(
+        self, uid: str, datasource_cache: DatasourceCache
+    ) -> dict:
         """The method includes a functionality to update the datasource cache specified by the datasource uid
 
         Args:
             uid (str): Specify the uid of the datasource
             datasource_cache (DatasourceCache): Specif the datasource cache object
 
         Required Permissions:
@@ -751,18 +753,20 @@
                     "ttlResourcesMs": datasource_cache.ttl_resources_ms,
                 }
             )
 
             api_call: dict = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.DATASOURCES.value}/{uid}/cache",
                 RequestsMethods.POST,
-                json.dumps(datasource_cache_object)
+                json.dumps(datasource_cache_object),
             )
 
             if api_call == dict() or api_call.get("dataSourceID") is None:
                 logging.error(f"Check the error: {api_call}.")
                 raise Exception
             else:
                 return api_call
         else:
-            logging.error("There is no uid or the right datasource_cache object defined.")
+            logging.error(
+                "There is no uid or the right datasource_cache object defined."
+            )
             raise ValueError
```

### Comparing `grafana-api-sdk-0.2.0/grafana_api/external_group.py` & `grafana-api-sdk-0.3.0/grafana_api/external_group.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.2.0/grafana_api/folder.py` & `grafana-api-sdk-0.3.0/grafana_api/folder.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 
         if len(uid) != 0:
             api_call = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.FOLDERS.value}/{uid}",
                 RequestsMethods.DELETE,
             )
 
-            if api_call.status != 200:
+            if api_call.status_code != 200:
                 logging.error(f"Please, check the error: {api_call}.")
                 raise Exception
             else:
                 logging.info("You successfully destroyed the folder.")
         else:
             logging.error("There is no folder uid defined.")
             raise ValueError
```

### Comparing `grafana-api-sdk-0.2.0/grafana_api/legacy_alerting.py` & `grafana-api-sdk-0.3.0/grafana_api/legacy_alerting.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             Exception: Unspecified error by executing the API call
 
         Returns:
             api_call (dict): Returns an alert
         """
 
         def _to_camel_case(input_value: str) -> str:
-            content = re.findall('[A-Z][^A-Z]*', input_value)
+            content = re.findall("[A-Z][^A-Z]*", input_value)
             if content != list():
                 if len(content) != 1:
                     return content[0].lower() + "".join(content[1:])
                 else:
                     return content[0].lower()
             return input_value
```

### Comparing `grafana-api-sdk-0.2.0/grafana_api/legacy_playlist.py` & `grafana-api-sdk-0.3.0/grafana_api/legacy_playlist.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.2.0/grafana_api/library.py` & `grafana-api-sdk-0.3.0/grafana_api/library.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.2.0/grafana_api/licensing.py` & `grafana-api-sdk-0.3.0/grafana_api/licensing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from urllib3 import response
+from httpx import Response
 import logging
 
 from .model import (
     APIModel,
     APIEndpoints,
     RequestsMethods,
 )
@@ -35,23 +35,23 @@
         Raises:
             Exception: Unspecified error by executing the API call
 
         Returns:
             api_call (bool): Returns the result if the license is available or not
         """
 
-        api_call: response = Api(self.grafana_api_model).call_the_api(
+        api_call: Response = Api(self.grafana_api_model).call_the_api(
             f"{APIEndpoints.LICENSING.value}/check",
         )
 
-        if api_call.status != 200:
+        if api_call.status_code != 200:
             logging.error(f"Check the error: {api_call}.")
             raise Exception
         else:
-            return json.loads(str(api_call.data.decode("utf-8")))
+            return json.loads(str(api_call.text))
 
     def manually_force_license_refresh(self):
         """The method includes a functionality to manually ask license issuer for a new token
 
         Required Permissions:
             Action: licensing:update
             Scope: N/A
```

### Comparing `grafana-api-sdk-0.2.0/grafana_api/model.py` & `grafana-api-sdk-0.3.0/grafana_api/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import ssl
+import httpx
 from enum import Enum
 from typing import List, TypeVar
 from dataclasses import dataclass, field
 
 Self = TypeVar("Self", bound="Route")
 
 # The constant includes all necessary error messages that can occurs, if you establish a connection to the Grafana API.
@@ -74,25 +75,27 @@
 
     Args:
         host (str): Specify the host of the Grafana system
         token (str): Specify the access token of the Grafana system
         username (str): Specify the username of the Grafana system
         password (str): Specify the password of the Grafana system
         timeout (float): Specify the timeout of the Grafana system
+        http2_support (bool): Specify if you want to use HTTP/2
         ssl_context (ssl.SSLContext): Specify the custom ssl context of the Grafana system
         num_pools (int): Specify the number of the connection pool
         retries (any): Specify the number of the retries. Please use False as parameter to disable the retries
     """
 
     host: str
     token: str = None
     username: str = None
     password: str = None
     timeout: float = 10.0
-    ssl_context: ssl.SSLContext = ssl.create_default_context()
+    http2_support: bool = False
+    ssl_context: ssl.SSLContext = httpx.create_ssl_context(http2=http2_support)
     num_pools: int = 10
     retries: any = 10
 
 
 @dataclass
 class DatasourceQuery:
     """The class includes all necessary variables to specify a query for the datasource search endpoint
```

### Comparing `grafana-api-sdk-0.2.0/grafana_api/organisation.py` & `grafana-api-sdk-0.3.0/grafana_api/organisation.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.2.0/grafana_api/playlist.py` & `grafana-api-sdk-0.3.0/grafana_api/playlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,15 +259,15 @@
 
         if len(playlist_uid) != 0:
             api_call = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.PLAYLISTS.value}/{playlist_uid}",
                 RequestsMethods.DELETE,
             )
 
-            if api_call.status != 200:
-                logging.error(f"Check the error: {api_call.data}.")
+            if api_call.status_code != 200:
+                logging.error(f"Check the error: {api_call.text}.")
                 raise Exception
             else:
                 logging.info("You successfully deleted the corresponding playlist.")
         else:
             logging.error("There is no playlist_uid object defined.")
             raise ValueError
```

### Comparing `grafana-api-sdk-0.2.0/grafana_api/preferences.py` & `grafana-api-sdk-0.3.0/grafana_api/preferences.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             api_call (dict): Returns the current user preferences
         """
 
         api_call: dict = Api(self.grafana_api_model).call_the_api(
             APIEndpoints.USER_PREFERENCES.value,
         )
 
-        if type(api_call) != dict or api_call == dict():
+        if isinstance(api_call, dict) is False or api_call == dict():
             logging.error(f"Check the error: {api_call}.")
             raise Exception
         else:
             return api_call
 
     def update_current_user_preferences(
         self,
@@ -69,15 +69,15 @@
             or timezone is not None
         ):
             modified_values: dict = dict()
 
             if theme is not None:
                 modified_values.update(dict({"theme": theme}))
 
-            if home_dashboard_id != 0 and type(home_dashboard_id) == int:
+            if home_dashboard_id != 0 and isinstance(home_dashboard_id, int):
                 modified_values.update(dict({"homeDashboardId": home_dashboard_id}))
             else:
                 modified_values.update({"homeDashboardUID": home_dashboard_uid})
 
             if timezone is not None:
                 modified_values.update(dict({"timezone": timezone}))
 
@@ -108,15 +108,15 @@
             api_call (dict): Returns the current user preferences
         """
 
         api_call: dict = Api(self.grafana_api_model).call_the_api(
             APIEndpoints.ORG_PREFERENCES.value,
         )
 
-        if type(api_call) != dict or api_call == dict():
+        if isinstance(api_call, dict) is False or api_call == dict():
             logging.error(f"Check the error: {api_call}.")
             raise Exception
         else:
             return api_call
 
     def update_current_org_preferences(
         self,
@@ -147,15 +147,15 @@
             or timezone is not None
         ):
             modified_values: dict = dict()
 
             if theme is not None:
                 modified_values.update(dict({"theme": theme}))
 
-            if home_dashboard_id != 0 and type(home_dashboard_id) == int:
+            if home_dashboard_id != 0 and isinstance(home_dashboard_id, int):
                 modified_values.update(dict({"homeDashboardId": home_dashboard_id}))
             else:
                 modified_values.update({"homeDashboardUID": home_dashboard_uid})
 
             if timezone is not None:
                 modified_values.update(dict({"timezone": timezone}))
```

### Comparing `grafana-api-sdk-0.2.0/grafana_api/query_history.py` & `grafana-api-sdk-0.3.0/grafana_api/query_history.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.2.0/grafana_api/rbac.py` & `grafana-api-sdk-0.3.0/grafana_api/rbac.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.2.0/grafana_api/reporting.py` & `grafana-api-sdk-0.3.0/grafana_api/reporting.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.2.0/grafana_api/search.py` & `grafana-api-sdk-0.3.0/grafana_api/search.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.2.0/grafana_api/service_account.py` & `grafana-api-sdk-0.3.0/grafana_api/service_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,15 +308,18 @@
 
         api_call: dict = Api(self.grafana_api_model).call_the_api(
             f"{APIEndpoints.SERVICE_ACCOUNTS.value}/migrate",
             RequestsMethods.POST,
             json.dumps(dict()),
         )
 
-        if api_call.get("migrated") is None and api_call.get("message") != "API keys migrated to service accounts":
+        if (
+            api_call.get("migrated") is None
+            and api_call.get("message") != "API keys migrated to service accounts"
+        ):
             logging.error(f"Check the error: {api_call}.")
             raise Exception
         else:
             logging.info(
                 "You successfully migrated the API keys to the service accounts."
             )
```

### Comparing `grafana-api-sdk-0.2.0/grafana_api/short_url.py` & `grafana-api-sdk-0.3.0/grafana_api/short_url.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.2.0/grafana_api/snapshot.py` & `grafana-api-sdk-0.3.0/grafana_api/snapshot.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.2.0/grafana_api/team.py` & `grafana-api-sdk-0.3.0/grafana_api/team.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,15 +318,15 @@
         """
 
         if id != 0:
             api_call: dict = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.TEAMS.value}/{id}/preferences",
             )
 
-            if type(api_call) != dict or api_call == dict():
+            if isinstance(api_call, dict) is False or api_call == dict():
                 logging.error(f"Check the error: {api_call}.")
                 raise Exception
             else:
                 return api_call
         else:
             logging.error("There is no id defined.")
             raise ValueError
@@ -366,15 +366,15 @@
             or timezone is not None
         ):
             team_preferences: dict = dict()
 
             if theme is not None:
                 team_preferences.update(dict({"theme": theme}))
 
-            if home_dashboard_id != 0 and type(home_dashboard_id) == int:
+            if home_dashboard_id != 0 and isinstance(home_dashboard_id, int):
                 team_preferences.update(dict({"homeDashboardId": home_dashboard_id}))
             else:
                 team_preferences.update({"homeDashboardUID": home_dashboard_uid})
 
             if timezone is not None:
                 team_preferences.update(dict({"timezone": timezone}))
```

### Comparing `grafana-api-sdk-0.2.0/grafana_api/user.py` & `grafana-api-sdk-0.3.0/grafana_api/user.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.2.0/grafana_api_sdk.egg-info/PKG-INFO` & `grafana-api-sdk-0.3.0/grafana_api_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: grafana-api-sdk
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Grafana API SDK
 Home-page: https://github.com/ZPascal/grafana_api_sdk
 Author: Pascal Zimmermann
 Author-email: info@theiotstudio.com
 Project-URL: Source, https://github.com/ZPascal/grafana_api_sdk
 Project-URL: Bug Tracker, https://github.com/ZPascal/grafana_api_sdk/issues
 Project-URL: Documentation, https://zpascal.github.io/grafana_api_sdk/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: http2
 License-File: LICENSE
 
 # Grafana API SDK 
-The repository includes a Python SDK for the Grafana API. It's possible to communicate with the Grafana API endpoints. Another feature of the SDK is the possibility to specify the used folder for the dashboard.
+The repository includes an SDK for the Grafana API. It's possible to interact with all public available Grafana HTTP API endpoints.
 
 ## Differences between [grafana-client](https://github.com/panodata/grafana-client), [grafana_api](https://github.com/m0nhawk/grafana_api/) and the [grafana_api_sdk](https://github.com/ZPascal/grafana_api_sdk)
 The grafana-client is only a fork of the non-maintained grafana_api repository. In general, the grafana-client project started at the same time, as I started this project. The corresponding SDK is a completely new project and based on non-other project and include a few features that are currently not implemented inside the grafana-client.
 
-The main feature that is implemented inside this library:
+The core features that are implemented inside this library:
 
-- Grafana V8 Alerting API support (possibility to communicate (currently read only) with the attached Prometheus and Alertmanager)
+- All public Grafana API (HTTP) endpoints are supported
+- Full API support for Grafana legacy alerting, current alerting, alerting channels and alert provisioning
+- Possibility to specify custom and self-signed certificates
+- HTTP/2 support
 
 In general my focus inside this project is to implement and deliver old and new features from the Grafana API, to document all features and functionality clear and to increase the overall test coverage of the project.
 
 ## Currently, supported features
 
 ### Dashboard
 - Create/ Update a dashboard 
@@ -243,14 +247,15 @@
 - Unstar a query inside the history
 
 ### Other HTTP
 - Get frontend settings
 - Renew login session 
 - Get health status
 - Get metrics
+- Get Plugin metrics
 
 ### Licensing
 - Check license availability
 - Manually force license refresh
 - Remove the license from the database
 
 ### Annotation
@@ -303,14 +308,18 @@
 - Search service accounts
 - Create a service account
 - Get service account by id
 - Update a service account
 - Get service account token by id
 - Create service account token by id
 - Delete service account by id
+- Migrate API token to service account by token id
+- Revert the generated service account to API token
+- Get service account migration status
+- Hide the API keys tab inside the UI
 
 ### RBAC
 - Get status
 - Get all roles
 - Get role
 - Create role
 - Update role
```

### Comparing `grafana-api-sdk-0.2.0/grafana_api_sdk.egg-info/SOURCES.txt` & `grafana-api-sdk-0.3.0/grafana_api_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.2.0/setup.py` & `grafana-api-sdk-0.3.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     coverage_string: str = "![Coverage report](https://github.com/ZPascal/grafana_api_sdk/blob/main/docs/coverage.svg)"
     long_description: str = fh.read()
 
 long_description = long_description.replace(coverage_string, "")
 
 setuptools.setup(
     name="grafana-api-sdk",
-    version="0.2.0",
+    version="0.3.0",
     author="Pascal Zimmermann",
     author_email="info@theiotstudio.com",
     description="A Grafana API SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ZPascal/grafana_api_sdk",
     project_urls={
@@ -22,10 +22,14 @@
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved",
         "Operating System :: OS Independent",
     ],
     packages=["grafana_api"],
-    install_requires=["urllib3"],
-    python_requires=">=3.6",
+    install_requires=["httpx"],
+    extras_require={
+        "http2": ["httpx[http2]"],
+    },
+    tests_require=["pytest-httpx", "pytest"],
+    python_requires=">=3.8",
 )
```

