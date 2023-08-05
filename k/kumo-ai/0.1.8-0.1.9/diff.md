# Comparing `tmp/kumo-ai-0.1.8.tar.gz` & `tmp/kumo-ai-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kumo-ai-0.1.8.tar", last modified: Fri Jun 23 03:33:46 2023, max compression
+gzip compressed data, was "kumo-ai-0.1.9.tar", last modified: Fri Aug  4 16:18:00 2023, max compression
```

## Comparing `kumo-ai-0.1.8.tar` & `kumo-ai-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-06-23 03:33:46.696894 kumo-ai-0.1.8/
--rw-r--r--   0 siyang     (501) staff       (20)     1800 2023-02-27 18:06:46.000000 kumo-ai-0.1.8/.gitignore
--rw-r--r--   0 siyang     (501) staff       (20)      933 2023-03-17 21:55:08.000000 kumo-ai-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 siyang     (501) staff       (20)     1061 2023-02-23 21:09:43.000000 kumo-ai-0.1.8/LICENSE
--rw-r--r--   0 siyang     (501) staff       (20)      194 2023-05-25 20:14:27.000000 kumo-ai-0.1.8/Makefile
--rw-r--r--   0 siyang     (501) staff       (20)      482 2023-06-23 03:33:46.696755 kumo-ai-0.1.8/PKG-INFO
--rw-r--r--   0 siyang     (501) staff       (20)       39 2023-02-23 21:09:43.000000 kumo-ai-0.1.8/README.md
-drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-06-23 03:33:46.694876 kumo-ai-0.1.8/kumo_ai.egg-info/
--rw-r--r--   0 siyang     (501) staff       (20)      482 2023-06-23 03:33:46.000000 kumo-ai-0.1.8/kumo_ai.egg-info/PKG-INFO
--rw-r--r--   0 siyang     (501) staff       (20)      722 2023-06-23 03:33:46.000000 kumo-ai-0.1.8/kumo_ai.egg-info/SOURCES.txt
--rw-r--r--   0 siyang     (501) staff       (20)        1 2023-06-23 03:33:46.000000 kumo-ai-0.1.8/kumo_ai.egg-info/dependency_links.txt
--rw-r--r--   0 siyang     (501) staff       (20)       34 2023-06-23 03:33:46.000000 kumo-ai-0.1.8/kumo_ai.egg-info/requires.txt
--rw-r--r--   0 siyang     (501) staff       (20)        7 2023-06-23 03:33:46.000000 kumo-ai-0.1.8/kumo_ai.egg-info/top_level.txt
-drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-06-23 03:33:46.695115 kumo-ai-0.1.8/kumoai/
--rw-r--r--   0 siyang     (501) staff       (20)        0 2023-02-27 18:06:46.000000 kumo-ai-0.1.8/kumoai/__init__.py
--rw-r--r--   0 siyang     (501) staff       (20)    15118 2023-05-25 17:33:50.000000 kumo-ai-0.1.8/kumoai/client.py
-drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-06-23 03:33:46.695719 kumo-ai-0.1.8/kumoai/datamodel/
--rw-r--r--   0 siyang     (501) staff       (20)        0 2023-02-27 18:06:46.000000 kumo-ai-0.1.8/kumoai/datamodel/__init__.py
--rw-r--r--   0 siyang     (501) staff       (20)      974 2023-04-03 17:42:04.000000 kumo-ai-0.1.8/kumoai/datamodel/data_source.py
--rw-r--r--   0 siyang     (501) staff       (20)     6537 2023-05-25 20:37:19.000000 kumo-ai-0.1.8/kumoai/datamodel/jobs.py
--rw-r--r--   0 siyang     (501) staff       (20)      561 2023-04-05 16:11:01.000000 kumo-ai-0.1.8/kumoai/datamodel/json_serde.py
--rw-r--r--   0 siyang     (501) staff       (20)     6473 2023-06-23 03:31:27.000000 kumo-ai-0.1.8/kumoai/datamodel/pquery.py
-drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-06-23 03:33:46.696582 kumo-ai-0.1.8/kumoai/examples/
--rw-r--r--   0 siyang     (501) staff       (20)        0 2023-03-29 16:49:40.000000 kumo-ai-0.1.8/kumoai/examples/__init__.py
--rw-r--r--   0 siyang     (501) staff       (20)     4836 2023-06-23 03:32:38.000000 kumo-ai-0.1.8/kumoai/examples/financial.py
--rw-r--r--   0 siyang     (501) staff       (20)     8952 2023-06-23 03:32:04.000000 kumo-ai-0.1.8/kumoai/examples/financial_binary_classify_S3.json
--rw-r--r--   0 siyang     (501) staff       (20)     9341 2023-06-23 03:32:04.000000 kumo-ai-0.1.8/kumoai/examples/financial_binary_classify_SNOWFLAKE.json
--rw-r--r--   0 siyang     (501) staff       (20)     5375 2023-06-23 03:32:04.000000 kumo-ai-0.1.8/kumoai/examples/hm_churn.json
--rw-r--r--   0 siyang     (501) staff       (20)     3080 2023-05-18 17:13:05.000000 kumo-ai-0.1.8/kumoai/examples/orchestration.py
--rw-r--r--   0 siyang     (501) staff       (20)     3436 2023-06-23 03:31:27.000000 kumo-ai-0.1.8/kumoai/examples/save_load_modify_pquery.py
--rw-r--r--   0 siyang     (501) staff       (20)      967 2023-05-18 17:51:43.000000 kumo-ai-0.1.8/precommit-pyrightconfig.json
--rw-r--r--   0 siyang     (501) staff       (20)      924 2023-05-18 17:52:10.000000 kumo-ai-0.1.8/pyrightconfig.json
--rw-r--r--   0 siyang     (501) staff       (20)       38 2023-06-23 03:33:46.696942 kumo-ai-0.1.8/setup.cfg
--rw-r--r--   0 siyang     (501) staff       (20)      885 2023-06-23 03:33:15.000000 kumo-ai-0.1.8/setup.py
+drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-08-04 16:18:00.604829 kumo-ai-0.1.9/
+-rw-r--r--   0 siyang     (501) staff       (20)     1800 2023-02-27 18:06:46.000000 kumo-ai-0.1.9/.gitignore
+-rw-r--r--   0 siyang     (501) staff       (20)      933 2023-03-17 21:55:08.000000 kumo-ai-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 siyang     (501) staff       (20)     1061 2023-02-23 21:09:43.000000 kumo-ai-0.1.9/LICENSE
+-rw-r--r--   0 siyang     (501) staff       (20)      194 2023-05-25 20:14:27.000000 kumo-ai-0.1.9/Makefile
+-rw-r--r--   0 siyang     (501) staff       (20)      482 2023-08-04 16:18:00.604679 kumo-ai-0.1.9/PKG-INFO
+-rw-r--r--   0 siyang     (501) staff       (20)       39 2023-02-23 21:09:43.000000 kumo-ai-0.1.9/README.md
+drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-08-04 16:18:00.602767 kumo-ai-0.1.9/kumo_ai.egg-info/
+-rw-r--r--   0 siyang     (501) staff       (20)      482 2023-08-04 16:18:00.000000 kumo-ai-0.1.9/kumo_ai.egg-info/PKG-INFO
+-rw-r--r--   0 siyang     (501) staff       (20)      722 2023-08-04 16:18:00.000000 kumo-ai-0.1.9/kumo_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 siyang     (501) staff       (20)        1 2023-08-04 16:18:00.000000 kumo-ai-0.1.9/kumo_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 siyang     (501) staff       (20)       34 2023-08-04 16:18:00.000000 kumo-ai-0.1.9/kumo_ai.egg-info/requires.txt
+-rw-r--r--   0 siyang     (501) staff       (20)        7 2023-08-04 16:18:00.000000 kumo-ai-0.1.9/kumo_ai.egg-info/top_level.txt
+drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-08-04 16:18:00.602962 kumo-ai-0.1.9/kumoai/
+-rw-r--r--   0 siyang     (501) staff       (20)        0 2023-02-27 18:06:46.000000 kumo-ai-0.1.9/kumoai/__init__.py
+-rw-r--r--   0 siyang     (501) staff       (20)    15118 2023-05-25 17:33:50.000000 kumo-ai-0.1.9/kumoai/client.py
+drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-08-04 16:18:00.603589 kumo-ai-0.1.9/kumoai/datamodel/
+-rw-r--r--   0 siyang     (501) staff       (20)        0 2023-02-27 18:06:46.000000 kumo-ai-0.1.9/kumoai/datamodel/__init__.py
+-rw-r--r--   0 siyang     (501) staff       (20)      974 2023-04-03 17:42:04.000000 kumo-ai-0.1.9/kumoai/datamodel/data_source.py
+-rw-r--r--   0 siyang     (501) staff       (20)     6537 2023-05-25 20:37:19.000000 kumo-ai-0.1.9/kumoai/datamodel/jobs.py
+-rw-r--r--   0 siyang     (501) staff       (20)      561 2023-04-05 16:11:01.000000 kumo-ai-0.1.9/kumoai/datamodel/json_serde.py
+-rw-r--r--   0 siyang     (501) staff       (20)     6473 2023-06-23 03:31:27.000000 kumo-ai-0.1.9/kumoai/datamodel/pquery.py
+drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-08-04 16:18:00.604497 kumo-ai-0.1.9/kumoai/examples/
+-rw-r--r--   0 siyang     (501) staff       (20)        0 2023-03-29 16:49:40.000000 kumo-ai-0.1.9/kumoai/examples/__init__.py
+-rw-r--r--   0 siyang     (501) staff       (20)     5033 2023-08-03 17:45:01.000000 kumo-ai-0.1.9/kumoai/examples/financial.py
+-rw-r--r--   0 siyang     (501) staff       (20)     9202 2023-08-03 17:48:01.000000 kumo-ai-0.1.9/kumoai/examples/financial_binary_classify_S3.json
+-rw-r--r--   0 siyang     (501) staff       (20)     9593 2023-08-03 17:50:51.000000 kumo-ai-0.1.9/kumoai/examples/financial_binary_classify_SNOWFLAKE.json
+-rw-r--r--   0 siyang     (501) staff       (20)     5375 2023-06-23 03:32:04.000000 kumo-ai-0.1.9/kumoai/examples/hm_churn.json
+-rw-r--r--   0 siyang     (501) staff       (20)     3253 2023-08-04 16:16:55.000000 kumo-ai-0.1.9/kumoai/examples/orchestration.py
+-rw-r--r--   0 siyang     (501) staff       (20)     3436 2023-06-23 03:31:27.000000 kumo-ai-0.1.9/kumoai/examples/save_load_modify_pquery.py
+-rw-r--r--   0 siyang     (501) staff       (20)      967 2023-05-18 17:51:43.000000 kumo-ai-0.1.9/precommit-pyrightconfig.json
+-rw-r--r--   0 siyang     (501) staff       (20)      924 2023-05-18 17:52:10.000000 kumo-ai-0.1.9/pyrightconfig.json
+-rw-r--r--   0 siyang     (501) staff       (20)       38 2023-08-04 16:18:00.604873 kumo-ai-0.1.9/setup.cfg
+-rw-r--r--   0 siyang     (501) staff       (20)      885 2023-08-04 16:17:11.000000 kumo-ai-0.1.9/setup.py
```

### Comparing `kumo-ai-0.1.8/.gitignore` & `kumo-ai-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.8/.pre-commit-config.yaml` & `kumo-ai-0.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.8/LICENSE` & `kumo-ai-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.8/kumo_ai.egg-info/SOURCES.txt` & `kumo-ai-0.1.9/kumo_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.8/kumoai/client.py` & `kumo-ai-0.1.9/kumoai/client.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.8/kumoai/datamodel/data_source.py` & `kumo-ai-0.1.9/kumoai/datamodel/data_source.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.8/kumoai/datamodel/jobs.py` & `kumo-ai-0.1.9/kumoai/datamodel/jobs.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.8/kumoai/datamodel/json_serde.py` & `kumo-ai-0.1.9/kumoai/datamodel/json_serde.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.8/kumoai/datamodel/pquery.py` & `kumo-ai-0.1.9/kumoai/datamodel/pquery.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.8/kumoai/examples/financial.py` & `kumo-ai-0.1.9/kumoai/examples/financial.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,19 @@
         ColumnKeyGroup(columns=[
             ColumnKey(table_name='DISTRICT', col_name='DISTRICT_ID'),
             ColumnKey(table_name='ACCOUNT', col_name='DISTRICT_ID'),
             ColumnKey(table_name='CLIENT', col_name='DISTRICT_ID')
         ]))
     graph.col_groups.append(
         ColumnKeyGroup(columns=[
+            ColumnKey(table_name='DISP', col_name='DISP_ID'),
+            ColumnKey(table_name='CARD', col_name='DISP_ID')
+        ]))
+    graph.col_groups.append(
+        ColumnKeyGroup(columns=[
             ColumnKey(table_name='CLIENT', col_name='CLIENT_ID'),
             ColumnKey(table_name='DISP', col_name='CLIENT_ID')
         ]))
     graph.col_groups.append(
         ColumnKeyGroup(columns=[
             ColumnKey(table_name='ACCOUNT', col_name='ACCOUNT_ID'),
             ColumnKey(table_name='DISP', col_name='ACCOUNT_ID'),
```

### Comparing `kumo-ai-0.1.8/kumoai/examples/financial_binary_classify_S3.json` & `kumo-ai-0.1.9/kumoai/examples/financial_binary_classify_S3.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7937312825520834%*

 * *Differences: {"'advanced_options_yaml'": 'None',*

 * * "'graph'": "{'tables': {'DISTRICT': {'cols': {4: {'stype': 'numerical'}, 5: {'stype': "*

 * *            "'numerical'}, 6: {'stype': 'numerical'}, 7: {'stype': 'numerical'}, 8: {'stype': "*

 * *            "'numerical'}, 13: {'stype': 'numerical'}}}, 'TRANS': {'cols': {5: {'stype': "*

 * *            "'numerical'}, 9: {'stype': 'numerical'}}}}, 'col_groups': {insert: [(1, "*

 * *            "OrderedDict([('columns', [OrderedDict([('table_name', 'DISP'), ('col_name', "*

 * *            "'DISP_ID' […]*

```diff
@@ -1,8 +1,9 @@
 {
+    "advanced_options_yaml": null,
     "graph": {
         "col_groups": [
             {
                 "columns": [
                     {
                         "col_name": "DISTRICT_ID",
                         "table_name": "DISTRICT"
@@ -16,14 +17,26 @@
                         "table_name": "CLIENT"
                     }
                 ]
             },
             {
                 "columns": [
                     {
+                        "col_name": "DISP_ID",
+                        "table_name": "DISP"
+                    },
+                    {
+                        "col_name": "DISP_ID",
+                        "table_name": "CARD"
+                    }
+                ]
+            },
+            {
+                "columns": [
+                    {
                         "col_name": "CLIENT_ID",
                         "table_name": "CLIENT"
                     },
                     {
                         "col_name": "CLIENT_ID",
                         "table_name": "DISP"
                     }
@@ -187,31 +200,31 @@
                     },
                     {
                         "name": "A4",
                         "stype": "numerical"
                     },
                     {
                         "name": "A5",
-                        "stype": "categorical"
+                        "stype": "numerical"
                     },
                     {
                         "name": "A6",
-                        "stype": "categorical"
+                        "stype": "numerical"
                     },
                     {
                         "name": "A7",
-                        "stype": "categorical"
+                        "stype": "numerical"
                     },
                     {
                         "name": "A8",
-                        "stype": "categorical"
+                        "stype": "numerical"
                     },
                     {
                         "name": "A9",
-                        "stype": "categorical"
+                        "stype": "numerical"
                     },
                     {
                         "name": "A10",
                         "stype": "numerical"
                     },
                     {
                         "name": "A11",
@@ -223,15 +236,15 @@
                     },
                     {
                         "name": "A13",
                         "stype": "numerical"
                     },
                     {
                         "name": "A14",
-                        "stype": "categorical"
+                        "stype": "numerical"
                     },
                     {
                         "name": "A15",
                         "stype": "numerical"
                     },
                     {
                         "name": "A16",
@@ -346,15 +359,15 @@
                     },
                     {
                         "name": "OPERATION",
                         "stype": "categorical"
                     },
                     {
                         "name": "AMOUNT",
-                        "stype": "categorical"
+                        "stype": "numerical"
                     },
                     {
                         "name": "BALANCE",
                         "stype": "numerical"
                     },
                     {
                         "name": "K_SYMBOL",
@@ -362,15 +375,15 @@
                     },
                     {
                         "name": "BANK",
                         "stype": "categorical"
                     },
                     {
                         "name": "ACCOUNT",
-                        "stype": "categorical"
+                        "stype": "numerical"
                     }
                 ],
                 "pkey": "TRANS_ID",
                 "source_table": {
                     "data_source_type": "S3",
                     "file_type": "PARQUET",
                     "s3_path": "s3://kumo-public-datasets/financial/parquet/TRANS/"
```

### Comparing `kumo-ai-0.1.8/kumoai/examples/financial_binary_classify_SNOWFLAKE.json` & `kumo-ai-0.1.9/kumoai/examples/financial_binary_classify_SNOWFLAKE.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7937345377604167%*

 * *Differences: {"'advanced_options_yaml'": 'None',*

 * * "'graph'": "{'tables': {'DISTRICT': {'cols': {4: {'stype': 'numerical'}, 5: {'stype': "*

 * *            "'numerical'}, 6: {'stype': 'numerical'}, 7: {'stype': 'numerical'}, 8: {'stype': "*

 * *            "'numerical'}, 13: {'stype': 'numerical'}}}, 'TRANS': {'cols': {4: {'stype': "*

 * *            "'numerical'}}}}, 'col_groups': {insert: [(1, OrderedDict([('columns', "*

 * *            "[OrderedDict([('table_name', 'DISP'), ('col_name', 'DISP_ID')]), "*

 * *            "OrderedDict([('table_n […]*

```diff
@@ -1,8 +1,9 @@
 {
+    "advanced_options_yaml": null,
     "graph": {
         "col_groups": [
             {
                 "columns": [
                     {
                         "col_name": "DISTRICT_ID",
                         "table_name": "DISTRICT"
@@ -16,14 +17,26 @@
                         "table_name": "CLIENT"
                     }
                 ]
             },
             {
                 "columns": [
                     {
+                        "col_name": "DISP_ID",
+                        "table_name": "DISP"
+                    },
+                    {
+                        "col_name": "DISP_ID",
+                        "table_name": "CARD"
+                    }
+                ]
+            },
+            {
+                "columns": [
+                    {
                         "col_name": "CLIENT_ID",
                         "table_name": "CLIENT"
                     },
                     {
                         "col_name": "CLIENT_ID",
                         "table_name": "DISP"
                     }
@@ -195,31 +208,31 @@
                     },
                     {
                         "name": "A4",
                         "stype": "numerical"
                     },
                     {
                         "name": "A5",
-                        "stype": "categorical"
+                        "stype": "numerical"
                     },
                     {
                         "name": "A6",
-                        "stype": "categorical"
+                        "stype": "numerical"
                     },
                     {
                         "name": "A7",
-                        "stype": "categorical"
+                        "stype": "numerical"
                     },
                     {
                         "name": "A8",
-                        "stype": "categorical"
+                        "stype": "numerical"
                     },
                     {
                         "name": "A9",
-                        "stype": "categorical"
+                        "stype": "numerical"
                     },
                     {
                         "name": "A10",
                         "stype": "numerical"
                     },
                     {
                         "name": "A11",
@@ -231,15 +244,15 @@
                     },
                     {
                         "name": "A13",
                         "stype": "numerical"
                     },
                     {
                         "name": "A14",
-                        "stype": "categorical"
+                        "stype": "numerical"
                     },
                     {
                         "name": "A15",
                         "stype": "numerical"
                     },
                     {
                         "name": "A16",
@@ -356,15 +369,15 @@
                     },
                     {
                         "name": "OPERATION",
                         "stype": "categorical"
                     },
                     {
                         "name": "AMOUNT",
-                        "stype": "categorical"
+                        "stype": "numerical"
                     },
                     {
                         "name": "BALANCE",
                         "stype": "numerical"
                     },
                     {
                         "name": "K_SYMBOL",
```

### Comparing `kumo-ai-0.1.8/kumoai/examples/hm_churn.json` & `kumo-ai-0.1.9/kumoai/examples/hm_churn.json`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.8/kumoai/examples/orchestration.py` & `kumo-ai-0.1.9/kumoai/examples/orchestration.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,72 @@
 import logging
 import sys
 from time import sleep
+from typing import TypeVar
 
 from kumoai.client import KumoClient
-from kumoai.datamodel.jobs import (JobStatus, MetadataField,
-                                   PredictionArtifactType,
-                                   PredictionStorageType, S3PredictionOutput)
+from kumoai.datamodel.jobs import (BatchPredictionJobResource,
+                                   BatchPredictionOptions, JobStatus,
+                                   MetadataField, PredictionArtifactType,
+                                   PredictionStorageType, S3PredictionOutput,
+                                   TrainingJobResource)
 
 logging.basicConfig(format='%(asctime)s | %(levelname)s : %(message)s',
                     level=logging.INFO,
                     stream=sys.stdout)
 
 logger = logging.getLogger(__name__)
 
 kumo_client = KumoClient.from_env()
 
+JobResource = TypeVar('JobResource', TrainingJobResource,
+                      BatchPredictionJobResource)
+
+
+def wait_job_to_complete(
+    job: JobResource,
+    *,
+    poll_interval_seconds: float = 10.0,
+    raise_if_failed: bool = True,
+) -> JobResource:
+    # Poll job status every 10 seconds and log job status/progress.
+    while job.job_status_report.status == JobStatus.RUNNING:
+        logger.info('Job status: %s', job.job_status_report)
+        sleep(poll_interval_seconds)
+        if isinstance(job, TrainingJobResource):
+            job = kumo_client.get_training_job(job.job_id)
+        elif isinstance(job, BatchPredictionJobResource):
+            job = kumo_client.get_batch_prediction_job(job.job_id)
+
+    # Check if job is successful.
+    if job.job_status_report.status != JobStatus.DONE:
+        if raise_if_failed:
+            raise RuntimeError(f'Job did not complete successfully: {job}')
+        else:
+            logger.error('Job did not complete successfully: %s', job)
+
+    return job
+
 
 def run_training_job(pquery_name: str, poll_interval_seconds: float = 10.0):
     """
     This example demonstrates how to start a query (re)training job, and wait
     until it finishes by polling the job status every `poll_interval_seconds`.
     """
     # Kick off a training job.
     training_job = kumo_client.create_training_job(pquery_id=pquery_name)
-
-    # Poll job status every 10 seconds and log job status/progress.
-    while training_job.job_status_report.status == JobStatus.RUNNING:
-        logger.info('Job status: %s', training_job.job_status_report)
-        sleep(poll_interval_seconds)
-        training_job = kumo_client.get_training_job(training_job.job_id)
-
-    # Check if job is successful.
-    if training_job.job_status_report.status == JobStatus.DONE:
-        logger.info('Query %s training job %s succeeded! Result:\n%s',
-                    training_job.predictive_query_id, training_job.job_id,
-                    training_job.result)
-    else:
-        raise RuntimeError(f'Training failed: {training_job}')
+    wait_job_to_complete(training_job,
+                         poll_interval_seconds=poll_interval_seconds,
+                         raise_if_failed=True)
 
 
-def run_prediction_job(s3_prediction_file_path: str,
-                       poll_interval_seconds: float = 10.0):
+def run_prediction_job(
+        s3_prediction_file_path: str,
+        options: BatchPredictionOptions = BatchPredictionOptions(),
+        poll_interval_seconds: float = 10.0):
     """
     This example demonstrates how to start a batch prediction job, and wait
     until it finishes by polling the job status every `poll_interval_seconds`.
     """
     # Kick off a batch prediction job.
     prediction_job = kumo_client.create_batch_prediction_job(
         pquery_id='my_predictive_query',
@@ -53,24 +75,13 @@
                 storage_type=PredictionStorageType.S3,
                 artifact_type=PredictionArtifactType.PREDICTIONS,
                 file_path=s3_prediction_file_path,
                 extra_fields=[
                     MetadataField.JOB_TIMESTAMP, MetadataField.ANCHOR_TIMESTAMP
                 ])
         ],
+        options=options,
     )
 
-    # Poll job status every 10 seconds and log job status/progress.
-    while prediction_job.job_status_report.status == JobStatus.RUNNING:
-        logger.info('Job status: %s', prediction_job.job_status_report)
-        sleep(poll_interval_seconds)
-        prediction_job = kumo_client.get_batch_prediction_job(
-            prediction_job.job_id)
-
-    # Check if job is successful.
-    if prediction_job.job_status_report.status == JobStatus.DONE:
-        logger.info(
-            'Query %s batch prediction job=%s succeeded! Job summary:\n%s',
-            prediction_job.predictive_query_id, prediction_job.job_id,
-            prediction_job.result)
-    else:
-        raise RuntimeError(f'Batch prediction failed: {prediction_job}')
+    wait_job_to_complete(prediction_job,
+                         poll_interval_seconds=poll_interval_seconds,
+                         raise_if_failed=True)
```

### Comparing `kumo-ai-0.1.8/kumoai/examples/save_load_modify_pquery.py` & `kumo-ai-0.1.9/kumoai/examples/save_load_modify_pquery.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.8/precommit-pyrightconfig.json` & `kumo-ai-0.1.9/precommit-pyrightconfig.json`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.8/pyrightconfig.json` & `kumo-ai-0.1.9/pyrightconfig.json`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.8/setup.py` & `kumo-ai-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 DESCRIPTION = 'Kumo.ai Client SDK'
 LONG_DESCRIPTION = """
 SDK/API for Kumo.ai clients to allow programmatic access to Kumo.ai
 """
 
 install_requires = [
     "pydantic==1.10.4",
```

