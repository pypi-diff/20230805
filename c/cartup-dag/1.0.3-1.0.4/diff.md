# Comparing `tmp/cartup_dag-1.0.3.tar.gz` & `tmp/cartup_dag-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cartup_dag-1.0.3.tar", last modified: Thu Jul 27 03:00:23 2023, max compression
+gzip compressed data, was "cartup_dag-1.0.4.tar", last modified: Sat Aug  5 00:30:41 2023, max compression
```

## Comparing `cartup_dag-1.0.3.tar` & `cartup_dag-1.0.4.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.433517 cartup_dag-1.0.3/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)       55 2023-07-26 06:42:37.000000 cartup_dag-1.0.3/MANIFEST.in
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      566 2023-07-27 03:00:23.433323 cartup_dag-1.0.3/PKG-INFO
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.426824 cartup_dag-1.0.3/cartup_dag/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)       33 2023-07-26 06:24:53.000000 cartup_dag-1.0.3/cartup_dag/__init__.py
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.428077 cartup_dag-1.0.3/cartup_dag/airflow/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2022-05-26 02:28:16.000000 cartup_dag-1.0.3/cartup_dag/airflow/__init__.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     3757 2023-07-27 02:07:48.000000 cartup_dag-1.0.3/cartup_dag/airflow/airflow_service.py
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.428695 cartup_dag-1.0.3/cartup_dag/build/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 06:05:58.000000 cartup_dag-1.0.3/cartup_dag/build/__init__.py
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.429839 cartup_dag-1.0.3/cartup_dag/config/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2022-05-26 02:26:35.000000 cartup_dag-1.0.3/cartup_dag/config/__init__.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1474 2023-07-26 06:06:49.000000 cartup_dag-1.0.3/cartup_dag/config/config.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1270 2023-07-26 06:06:49.000000 cartup_dag-1.0.3/cartup_dag/config/config_local.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1289 2023-07-26 08:17:00.000000 cartup_dag-1.0.3/cartup_dag/config/config_notification.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1026 2023-07-26 06:06:49.000000 cartup_dag-1.0.3/cartup_dag/config/config_prod.py
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.430033 cartup_dag-1.0.3/cartup_dag/jobs/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 06:06:18.000000 cartup_dag-1.0.3/cartup_dag/jobs/__init__.py
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.430138 cartup_dag-1.0.3/cartup_dag/jobs/dashboard/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 06:06:18.000000 cartup_dag-1.0.3/cartup_dag/jobs/dashboard/__init__.py
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.430365 cartup_dag-1.0.3/cartup_dag/jobs/dashboard/dags/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 06:06:18.000000 cartup_dag-1.0.3/cartup_dag/jobs/dashboard/dags/__init__.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1088 2022-07-29 03:12:57.000000 cartup_dag-1.0.3/cartup_dag/jobs/dashboard/dags/dag_dashboard.py
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.430928 cartup_dag-1.0.3/cartup_dag/jobs/search/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 06:06:18.000000 cartup_dag-1.0.3/cartup_dag/jobs/search/__init__.py
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.431180 cartup_dag-1.0.3/cartup_dag/jobs/search/dags/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 06:06:18.000000 cartup_dag-1.0.3/cartup_dag/jobs/search/dags/__init__.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1094 2022-06-02 06:54:22.000000 cartup_dag-1.0.3/cartup_dag/jobs/search/dags/dag_search.py
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.432075 cartup_dag-1.0.3/cartup_dag/server/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2022-05-26 02:28:16.000000 cartup_dag-1.0.3/cartup_dag/server/__init__.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      998 2022-05-26 02:35:43.000000 cartup_dag-1.0.3/cartup_dag/server/response_ws.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     6068 2023-07-27 02:09:30.000000 cartup_dag-1.0.3/cartup_dag/server/server.py
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.432514 cartup_dag-1.0.3/cartup_dag/ssh/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2022-05-26 02:28:16.000000 cartup_dag-1.0.3/cartup_dag/ssh/__init__.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      954 2023-07-26 06:43:24.000000 cartup_dag-1.0.3/cartup_dag/ssh/ssh_client.py
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.433038 cartup_dag-1.0.3/cartup_dag/utils/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2022-05-26 02:28:16.000000 cartup_dag-1.0.3/cartup_dag/utils/__init__.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     2689 2023-07-27 01:36:36.000000 cartup_dag-1.0.3/cartup_dag/utils/utils.py
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.427798 cartup_dag-1.0.3/cartup_dag.egg-info/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      566 2023-07-27 03:00:23.000000 cartup_dag-1.0.3/cartup_dag.egg-info/PKG-INFO
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      969 2023-07-27 03:00:23.000000 cartup_dag-1.0.3/cartup_dag.egg-info/SOURCES.txt
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)        1 2023-07-27 03:00:23.000000 cartup_dag-1.0.3/cartup_dag.egg-info/dependency_links.txt
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      335 2023-07-27 03:00:23.000000 cartup_dag-1.0.3/cartup_dag.egg-info/requires.txt
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)       11 2023-07-27 03:00:23.000000 cartup_dag-1.0.3/cartup_dag.egg-info/top_level.txt
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      334 2023-07-26 06:15:15.000000 cartup_dag-1.0.3/requirements.txt
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)       38 2023-07-27 03:00:23.433567 cartup_dag-1.0.3/setup.cfg
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      936 2023-07-26 06:42:37.000000 cartup_dag-1.0.3/setup.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-08-05 00:30:41.046056 cartup_dag-1.0.4/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)       55 2023-07-26 06:42:37.000000 cartup_dag-1.0.4/MANIFEST.in
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)      566 2023-08-05 00:30:41.045921 cartup_dag-1.0.4/PKG-INFO
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-08-05 00:30:41.041175 cartup_dag-1.0.4/cartup_dag/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)       33 2023-07-26 06:24:53.000000 cartup_dag-1.0.4/cartup_dag/__init__.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-08-05 00:30:41.042187 cartup_dag-1.0.4/cartup_dag/airflow/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2022-05-26 02:28:16.000000 cartup_dag-1.0.4/cartup_dag/airflow/__init__.py
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)     3757 2023-07-27 02:07:48.000000 cartup_dag-1.0.4/cartup_dag/airflow/airflow_service.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-08-05 00:30:41.042309 cartup_dag-1.0.4/cartup_dag/build/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 06:05:58.000000 cartup_dag-1.0.4/cartup_dag/build/__init__.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-08-05 00:30:41.043158 cartup_dag-1.0.4/cartup_dag/config/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2022-05-26 02:26:35.000000 cartup_dag-1.0.4/cartup_dag/config/__init__.py
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1392 2023-08-03 06:57:39.000000 cartup_dag-1.0.4/cartup_dag/config/config.py
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1270 2023-07-26 06:06:49.000000 cartup_dag-1.0.4/cartup_dag/config/config_local.py
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1289 2023-07-26 08:17:00.000000 cartup_dag-1.0.4/cartup_dag/config/config_notification.py
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1026 2023-07-26 06:06:49.000000 cartup_dag-1.0.4/cartup_dag/config/config_prod.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-08-05 00:30:41.043360 cartup_dag-1.0.4/cartup_dag/jobs/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 06:06:18.000000 cartup_dag-1.0.4/cartup_dag/jobs/__init__.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-08-05 00:30:41.043465 cartup_dag-1.0.4/cartup_dag/jobs/dashboard/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 06:06:18.000000 cartup_dag-1.0.4/cartup_dag/jobs/dashboard/__init__.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-08-05 00:30:41.043776 cartup_dag-1.0.4/cartup_dag/jobs/dashboard/dags/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 06:06:18.000000 cartup_dag-1.0.4/cartup_dag/jobs/dashboard/dags/__init__.py
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1088 2022-07-29 03:12:57.000000 cartup_dag-1.0.4/cartup_dag/jobs/dashboard/dags/dag_dashboard.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-08-05 00:30:41.044063 cartup_dag-1.0.4/cartup_dag/jobs/search/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 06:06:18.000000 cartup_dag-1.0.4/cartup_dag/jobs/search/__init__.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-08-05 00:30:41.044265 cartup_dag-1.0.4/cartup_dag/jobs/search/dags/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 06:06:18.000000 cartup_dag-1.0.4/cartup_dag/jobs/search/dags/__init__.py
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1094 2022-06-02 06:54:22.000000 cartup_dag-1.0.4/cartup_dag/jobs/search/dags/dag_search.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-08-05 00:30:41.045040 cartup_dag-1.0.4/cartup_dag/server/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2022-05-26 02:28:16.000000 cartup_dag-1.0.4/cartup_dag/server/__init__.py
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)      998 2022-05-26 02:35:43.000000 cartup_dag-1.0.4/cartup_dag/server/response_ws.py
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)     6322 2023-08-03 05:19:42.000000 cartup_dag-1.0.4/cartup_dag/server/server.py
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)      459 2023-08-03 07:53:08.000000 cartup_dag-1.0.4/cartup_dag/server/test.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-08-05 00:30:41.045405 cartup_dag-1.0.4/cartup_dag/ssh/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2022-05-26 02:28:16.000000 cartup_dag-1.0.4/cartup_dag/ssh/__init__.py
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)      954 2023-07-26 06:43:24.000000 cartup_dag-1.0.4/cartup_dag/ssh/ssh_client.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-08-05 00:30:41.045636 cartup_dag-1.0.4/cartup_dag/utils/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2022-05-26 02:28:16.000000 cartup_dag-1.0.4/cartup_dag/utils/__init__.py
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)     4882 2023-08-05 00:17:05.000000 cartup_dag-1.0.4/cartup_dag/utils/utils.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-08-05 00:30:41.041898 cartup_dag-1.0.4/cartup_dag.egg-info/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)      566 2023-08-05 00:30:41.000000 cartup_dag-1.0.4/cartup_dag.egg-info/PKG-INFO
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)      995 2023-08-05 00:30:41.000000 cartup_dag-1.0.4/cartup_dag.egg-info/SOURCES.txt
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)        1 2023-08-05 00:30:41.000000 cartup_dag-1.0.4/cartup_dag.egg-info/dependency_links.txt
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)      335 2023-08-05 00:30:41.000000 cartup_dag-1.0.4/cartup_dag.egg-info/requires.txt
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)       11 2023-08-05 00:30:41.000000 cartup_dag-1.0.4/cartup_dag.egg-info/top_level.txt
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)      334 2023-07-26 06:15:15.000000 cartup_dag-1.0.4/requirements.txt
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)       38 2023-08-05 00:30:41.046093 cartup_dag-1.0.4/setup.cfg
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)      936 2023-08-05 00:30:37.000000 cartup_dag-1.0.4/setup.py
```

### Comparing `cartup_dag-1.0.3/PKG-INFO` & `cartup_dag-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cartup_dag
-Version: 1.0.3
+Version: 1.0.4
 Summary: DAG Job Library.
 Author: Arvind Rapaka
 Author-email: arvind@cartup.ai
 License: Apache
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `cartup_dag-1.0.3/cartup_dag/airflow/airflow_service.py` & `cartup_dag-1.0.4/cartup_dag/airflow/airflow_service.py`

 * *Files identical despite different names*

### Comparing `cartup_dag-1.0.3/cartup_dag/config/config.py` & `cartup_dag-1.0.4/cartup_dag/config/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # Airflow Configs
 AIRFLOW_SERVER = "127.0.0.1"
-AIRFLOW_USER = "airflow"
-AIRFLOW_PASSWD = "airflow"
+AIRFLOW_USER = "admin"
+AIRFLOW_PASSWD = "admin"
 AIRFLOW_DAG_DIR = "/Users/arvind.rapaka/venvs/airflow-2.6.2/airflow/dags"
-AIRFLOW_REST_API_SERVER = "http://127.0.0.14:8080/api/v1"
+AIRFLOW_REST_API_SERVER = "http://127.0.0.1:8080/api/v1"
 AIRFLOW_DAG_DEPLOY_DIR = "/Users/arvind.rapaka/venvs/airflow-2.6.2/airflow/dagfiles/accounts"
 
 # Deploy Directory Configs
 SSH_CERTIFICATE = "/Users/arvind.rapaka/.ssh/id_rsa"
 SSH_SERVER = "127.0.0.1"
 SSH_USER = "arvind.rapaka"
 DEPLOY_DIR = "/Users/arvind.rapaka/venvs/airflow-2.6.2/airflow/dagfiles/accounts"
 
 # Jobs directory. This directory is where template dag files are found.
 JOB_DIR = "/jobs/"
 TEMP_DIR = "/tmp/dag"
 
-# config = JOBS[data["jobname"]] + "/dag_template/" + data["jobname"] + "_template"
 JOB_DAG_CONFIG_PATH = {
     "social_videos": "/Users/arvind.rapaka/git/cartup-ml-apis/social_videos/dag_template/social_videos_template",
     "widget_stats_report": ""
 }
 
 # A new way to configure jobs
 replace_conf_params = {"SEARCH_LIBS": "/opt/airflow/dagfiles/dashboard-libs",
                        "ML_LIBS": "/opt/airflow/dagfiles/dashboard-libs",
                        "DASHBOARD_LIB": "/opt/airflow/dagfiles/dashboard-libs",
                        "EMBEDDING_LIB_DIR": "/opt/airflow/dagfiles/dashboard-libs",
                        "SOCIAL_LIB_DIR": "/Users/arvind.rapaka/git/cartup-ml-apis/social_videos",
                        "JOB_DIR": "/opt/airflow/dagfiles/dashboard-libs"}
-JOB_API = "http://localhost:5003/api/v1/jobs"
+JOB_STATUS_API = "http://localhost:5003/api/v1/jobs"
```

### Comparing `cartup_dag-1.0.3/cartup_dag/config/config_local.py` & `cartup_dag-1.0.4/cartup_dag/config/config_local.py`

 * *Files identical despite different names*

### Comparing `cartup_dag-1.0.3/cartup_dag/config/config_notification.py` & `cartup_dag-1.0.4/cartup_dag/config/config_notification.py`

 * *Files identical despite different names*

### Comparing `cartup_dag-1.0.3/cartup_dag/config/config_prod.py` & `cartup_dag-1.0.4/cartup_dag/config/config_prod.py`

 * *Files identical despite different names*

### Comparing `cartup_dag-1.0.3/cartup_dag/jobs/dashboard/dags/dag_dashboard.py` & `cartup_dag-1.0.4/cartup_dag/jobs/dashboard/dags/dag_dashboard.py`

 * *Files identical despite different names*

### Comparing `cartup_dag-1.0.3/cartup_dag/jobs/search/dags/dag_search.py` & `cartup_dag-1.0.4/cartup_dag/jobs/search/dags/dag_search.py`

 * *Files identical despite different names*

### Comparing `cartup_dag-1.0.3/cartup_dag/server/response_ws.py` & `cartup_dag-1.0.4/cartup_dag/server/response_ws.py`

 * *Files identical despite different names*

### Comparing `cartup_dag-1.0.3/cartup_dag/server/server.py` & `cartup_dag-1.0.4/cartup_dag/server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,35 +120,40 @@
 
         for k, v in data.items():
             replace_conf_args_copy[k] = v
 
         #Conf Dir
         replace_conf_args_copy = dict((k.upper(), v) for k, v in replace_conf_args_copy.items())
         replace_conf_args_copy['CONF_DEPLOY_DIR'] = AIRFLOW_DAG_DEPLOY_DIR + "/" + data['org_s'] + "/" + data[
-            "jobname"] + "/config"
+            "jobname"]
         replace_params(replace_conf_args_copy, tmp_dir)
 
 
         # Now SSH the conf and DAG files
         ssh_client.make_remote_dir(remote_dir)
         ssh_client.export_file_directory(remote_dir, tmp_dir)
 
         # Push the DAG files to remote AIRFLOW DAG Folder
         for dag_file in dag_files:
             head, tail = os.path.split(dag_file)
-            dag_id = data['org_s'] + "_" + tail.rsplit(".", 1)[0]
+            '''dag_id = data['org_s'] + "_" + tail.rsplit(".", 1)[0]
             replace_dag_id = {'DAG_NAME':  dag_id}
-            write_close_file(dag_file, replace_dag_id)
+            write_close_file(dag_file, replace_dag_id)'''
             n_dag_file = head + "/" + data['org_s'] + "_" + tail
             os.rename(dag_file, n_dag_file)
             ssh_client.export_file_directory(AIRFLOW_DAG_DIR, n_dag_file, recursive=False)
             uu_id = str(uuid.uuid4())
-            resp, flag = ("success", True)
-            #resp, flag = airflow_client.run_airflow_cmd(cmd='trigger_dag_run', replace_params={'dag_id': dag_id},
-            #                                data=json.dumps({"conf": {}, "dag_run_id": uu_id}))
+            resp, flag = airflow_client.run_airflow_cmd(req_params={'method': 'GET', 'path': 'dags'})
+            if not flag:
+                logging.error("Not able to trigger the job {} {}".format(n_dag_file, uu_id))
+            else:
+                logging.info(resp.text)
+
+            resp, flag = airflow_client.run_airflow_cmd(cmd='trigger_dag_run', replace_params={'dag_id': data['org_s'] + "_social_videos"},
+                                            data=json.dumps({"conf": {}, "dag_run_id": uu_id}))
             if not flag:
                 logging.error("Not able to trigger the job {} {}".format(n_dag_file, uu_id))
             else:
                 logging.info(resp.text)
 
     except Exception as e:
         logging.error(traceback.print_exc())
@@ -174,13 +179,13 @@
                                                 data=data, req_params=req_params)
     if not flag:
         send_error_response(resp)
     return send_response(resp)
 
 
 def start_server():
-    app.run(debug=True, threaded=True, port=5003)
+    app.run(debug=True, threaded=True, port=5005)
     return app
 
 
 if __name__ == '__main__':
     start_server()
```

### Comparing `cartup_dag-1.0.3/cartup_dag/ssh/ssh_client.py` & `cartup_dag-1.0.4/cartup_dag/ssh/ssh_client.py`

 * *Files identical despite different names*

### Comparing `cartup_dag-1.0.3/cartup_dag.egg-info/PKG-INFO` & `cartup_dag-1.0.4/cartup_dag.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cartup-dag
-Version: 1.0.3
+Version: 1.0.4
 Summary: DAG Job Library.
 Author: Arvind Rapaka
 Author-email: arvind@cartup.ai
 License: Apache
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `cartup_dag-1.0.3/cartup_dag.egg-info/SOURCES.txt` & `cartup_dag-1.0.4/cartup_dag.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -21,11 +21,12 @@
 cartup_dag/jobs/dashboard/dags/dag_dashboard.py
 cartup_dag/jobs/search/__init__.py
 cartup_dag/jobs/search/dags/__init__.py
 cartup_dag/jobs/search/dags/dag_search.py
 cartup_dag/server/__init__.py
 cartup_dag/server/response_ws.py
 cartup_dag/server/server.py
+cartup_dag/server/test.py
 cartup_dag/ssh/__init__.py
 cartup_dag/ssh/ssh_client.py
 cartup_dag/utils/__init__.py
 cartup_dag/utils/utils.py
```

### Comparing `cartup_dag-1.0.3/setup.py` & `cartup_dag-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = f.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='cartup_dag',
-    version='1.0.3',
+    version='1.0.4',
     license='Apache',
     description='DAG Job Library.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email='arvind@cartup.ai',
     author='Arvind Rapaka',
     packages=find_packages(),
```

