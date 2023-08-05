# Comparing `tmp/pulumi_splunk-1.3.0a1691044717.tar.gz` & `tmp/pulumi_splunk-1.3.0a1691216102.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_splunk-1.3.0a1691044717.tar", last modified: Thu Aug  3 06:48:34 2023, max compression
+gzip compressed data, was "pulumi_splunk-1.3.0a1691216102.tar", last modified: Sat Aug  5 06:19:11 2023, max compression
```

## Comparing `pulumi_splunk-1.3.0a1691044717.tar` & `pulumi_splunk-1.3.0a1691216102.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:48:34.608621 pulumi_splunk-1.3.0a1691044717/
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-08-03 06:48:34.608621 pulumi_splunk-1.3.0a1691044717/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:48:34.608621 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    90731 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/admin_saml_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    38600 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/apps_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    21845 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/authentication_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    45752 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/authorization_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:48:34.608621 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/configs_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    14301 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/data_ui_views.py
--rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/generic_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/global_http_event_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)   154784 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)    22396 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/inputs_http_event_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    42002 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/inputs_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    29483 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/inputs_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    18863 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/inputs_tcp_cooked.py
--rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/inputs_tcp_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/inputs_tcp_splunk_tcp_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    13939 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/inputs_tcp_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    34193 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/inputs_udp.py
--rw-r--r--   0 runner    (1001) docker     (123)    73136 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43975 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/outputs_tcp_default.py
--rw-r--r--   0 runner    (1001) docker     (123)    43421 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/outputs_tcp_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    31871 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/outputs_tcp_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    27807 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/outputs_tcp_syslog.py
--rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   514411 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/saved_searches.py
--rw-r--r--   0 runner    (1001) docker     (123)    16950 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk/sh_indexes_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:48:34.608621 pulumi_splunk-1.3.0a1691044717/pulumi_splunk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/pulumi_splunk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 06:48:34.608621 pulumi_splunk-1.3.0a1691044717/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-08-03 06:48:34.000000 pulumi_splunk-1.3.0a1691044717/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:19:11.093613 pulumi_splunk-1.3.0a1691216102/
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-08-05 06:19:11.093613 pulumi_splunk-1.3.0a1691216102/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:19:11.093613 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90731 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/admin_saml_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38600 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/apps_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21845 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/authentication_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45752 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/authorization_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:19:11.093613 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/configs_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14301 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/data_ui_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/generic_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/global_http_event_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154784 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22396 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/inputs_http_event_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42002 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/inputs_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29483 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/inputs_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18863 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/inputs_tcp_cooked.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/inputs_tcp_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/inputs_tcp_splunk_tcp_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13939 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/inputs_tcp_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34193 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/inputs_udp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73136 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43975 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/outputs_tcp_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43421 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/outputs_tcp_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31871 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/outputs_tcp_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27807 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/outputs_tcp_syslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   514411 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/saved_searches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16950 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk/sh_indexes_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:19:11.093613 pulumi_splunk-1.3.0a1691216102/pulumi_splunk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-08-05 06:19:11.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-05 06:19:11.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 06:19:11.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 06:19:11.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-05 06:19:11.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-05 06:19:11.000000 pulumi_splunk-1.3.0a1691216102/pulumi_splunk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 06:19:11.093613 pulumi_splunk-1.3.0a1691216102/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-08-05 06:19:10.000000 pulumi_splunk-1.3.0a1691216102/setup.py
```

### Comparing `pulumi_splunk-1.3.0a1691044717/PKG-INFO` & `pulumi_splunk-1.3.0a1691216102/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_splunk
-Version: 1.3.0a1691044717
+Version: 1.3.0a1691216102
 Summary: A Pulumi package for creating and managing splunk cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-splunk
 Keywords: pulumi splunk
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_splunk-1.3.0a1691044717/README.md` & `pulumi_splunk-1.3.0a1691216102/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/__init__.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/_inputs.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/_utilities.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/admin_saml_groups.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/admin_saml_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/apps_local.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/apps_local.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/authentication_users.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/authentication_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/authorization_roles.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/authorization_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/config/vars.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/configs_conf.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/configs_conf.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/data_ui_views.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/data_ui_views.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/generic_acl.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/generic_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/global_http_event_collector.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/global_http_event_collector.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/indexes.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/indexes.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/inputs_http_event_collector.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/inputs_http_event_collector.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/inputs_monitor.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/inputs_monitor.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/inputs_script.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/inputs_script.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/inputs_tcp_cooked.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/inputs_tcp_cooked.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/inputs_tcp_raw.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/inputs_tcp_raw.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/inputs_tcp_splunk_tcp_token.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/inputs_tcp_splunk_tcp_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/inputs_tcp_ssl.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/inputs_tcp_ssl.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/inputs_udp.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/inputs_udp.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/outputs.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/outputs_tcp_default.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/outputs_tcp_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/outputs_tcp_group.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/outputs_tcp_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/outputs_tcp_server.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/outputs_tcp_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/outputs_tcp_syslog.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/outputs_tcp_syslog.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/provider.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/saved_searches.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/saved_searches.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk/sh_indexes_manager.py` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk/sh_indexes_manager.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk.egg-info/PKG-INFO` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-splunk
-Version: 1.3.0a1691044717
+Version: 1.3.0a1691216102
 Summary: A Pulumi package for creating and managing splunk cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-splunk
 Keywords: pulumi splunk
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_splunk-1.3.0a1691044717/pulumi_splunk.egg-info/SOURCES.txt` & `pulumi_splunk-1.3.0a1691216102/pulumi_splunk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1691044717/setup.py` & `pulumi_splunk-1.3.0a1691216102/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.3.0a1691044717"
-PLUGIN_VERSION = "1.3.0-alpha.1691044717+3660794a"
+VERSION = "1.3.0a1691216102"
+PLUGIN_VERSION = "1.3.0-alpha.1691216102+acff7038"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'splunk', PLUGIN_VERSION])
         except OSError as error:
```

