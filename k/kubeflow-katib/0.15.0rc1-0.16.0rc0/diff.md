# Comparing `tmp/kubeflow-katib-0.15.0rc1.tar.gz` & `tmp/kubeflow-katib-0.16.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubeflow-katib-0.15.0rc1.tar", last modified: Wed Feb 15 15:24:03 2023, max compression
+gzip compressed data, was "kubeflow-katib-0.16.0rc0.tar", last modified: Sat Aug  5 19:13:29 2023, max compression
```

## Comparing `kubeflow-katib-0.15.0rc1.tar` & `kubeflow-katib-0.16.0rc0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2023-02-15 15:24:03.925317 kubeflow-katib-0.15.0rc1/
--rw-r--r--   0 avelichk   (501) staff       (20)     1193 2023-02-15 15:24:03.925072 kubeflow-katib-0.15.0rc1/PKG-INFO
--rw-r--r--   0 avelichk   (501) staff       (20)     5474 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/README.md
-drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2023-02-15 15:24:03.917489 kubeflow-katib-0.15.0rc1/kubeflow/
--rw-r--r--   0 avelichk   (501) staff       (20)       65 2023-02-15 15:23:23.000000 kubeflow-katib-0.15.0rc1/kubeflow/__init__.py
-drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2023-02-15 15:24:03.918275 kubeflow-katib-0.15.0rc1/kubeflow/katib/
--rw-r--r--   0 avelichk   (501) staff       (20)     4402 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/__init__.py
-drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2023-02-15 15:24:03.918634 kubeflow-katib-0.15.0rc1/kubeflow/katib/api/
--rw-r--r--   0 avelichk   (501) staff       (20)       87 2023-02-15 15:23:23.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/api/__init__.py
--rw-r--r--   0 avelichk   (501) staff       (20)    44722 2023-02-15 15:23:23.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/api/katib_client.py
--rw-r--r--   0 avelichk   (501) staff       (20)     1998 2023-02-15 15:23:23.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/api/search.py
--rw-r--r--   0 avelichk   (501) staff       (20)    26164 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/api_client.py
--rw-r--r--   0 avelichk   (501) staff       (20)    12364 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/configuration.py
-drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2023-02-15 15:24:03.918850 kubeflow-katib-0.15.0rc1/kubeflow/katib/constants/
--rw-r--r--   0 avelichk   (501) staff       (20)        0 2023-02-15 15:23:23.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/constants/__init__.py
--rw-r--r--   0 avelichk   (501) staff       (20)     2094 2023-02-15 15:23:23.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/constants/constants.py
--rw-r--r--   0 avelichk   (501) staff       (20)     3711 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/exceptions.py
--rw-r--r--   0 avelichk   (501) staff       (20)   113357 2023-02-15 15:24:03.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/katib_api_pb2.py
-drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2023-02-15 15:24:03.923699 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/
--rw-r--r--   0 avelichk   (501) staff       (20)     3803 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/__init__.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4099 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_algorithm_setting.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4681 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_algorithm_spec.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4118 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_collector_spec.py
--rw-r--r--   0 avelichk   (501) staff       (20)     5659 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_config_map_source.py
--rw-r--r--   0 avelichk   (501) staff       (20)     6208 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_early_stopping_rule.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4155 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_early_stopping_setting.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4757 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_early_stopping_spec.py
--rw-r--r--   0 avelichk   (501) staff       (20)     7260 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_experiment.py
--rw-r--r--   0 avelichk   (501) staff       (20)     8063 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_experiment_condition.py
--rw-r--r--   0 avelichk   (501) staff       (20)     6818 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_experiment_list.py
--rw-r--r--   0 avelichk   (501) staff       (20)    12877 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_experiment_spec.py
--rw-r--r--   0 avelichk   (501) staff       (20)    22676 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_experiment_status.py
--rw-r--r--   0 avelichk   (501) staff       (20)     5051 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_feasible_space.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4520 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_file_system_path.py
--rw-r--r--   0 avelichk   (501) staff       (20)     3821 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_filter_spec.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4885 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_graph_config.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4933 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_metric.py
--rw-r--r--   0 avelichk   (501) staff       (20)     3887 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_metric_strategy.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4172 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_metrics_collector_spec.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4188 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_nas_config.py
--rw-r--r--   0 avelichk   (501) staff       (20)     8263 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_objective_spec.py
--rw-r--r--   0 avelichk   (501) staff       (20)     3470 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_observation.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4195 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_operation.py
--rw-r--r--   0 avelichk   (501) staff       (20)     5573 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_optimal_trial.py
--rw-r--r--   0 avelichk   (501) staff       (20)     3947 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_parameter_assignment.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4913 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_parameter_spec.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4905 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_source_spec.py
--rw-r--r--   0 avelichk   (501) staff       (20)     7260 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_suggestion.py
--rw-r--r--   0 avelichk   (501) staff       (20)     8063 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_suggestion_condition.py
--rw-r--r--   0 avelichk   (501) staff       (20)     6818 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_suggestion_list.py
--rw-r--r--   0 avelichk   (501) staff       (20)     6155 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_suggestion_spec.py
--rw-r--r--   0 avelichk   (501) staff       (20)     9515 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_suggestion_status.py
--rw-r--r--   0 avelichk   (501) staff       (20)     7110 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_trial.py
--rw-r--r--   0 avelichk   (501) staff       (20)     6577 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_trial_assignment.py
--rw-r--r--   0 avelichk   (501) staff       (20)     7913 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_trial_condition.py
--rw-r--r--   0 avelichk   (501) staff       (20)     6703 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_trial_list.py
--rw-r--r--   0 avelichk   (501) staff       (20)     5184 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_trial_parameter_spec.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4135 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_trial_source.py
--rw-r--r--   0 avelichk   (501) staff       (20)    13953 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_trial_spec.py
--rw-r--r--   0 avelichk   (501) staff       (20)     6840 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_trial_status.py
--rw-r--r--   0 avelichk   (501) staff       (20)    11124 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_trial_template.py
--rw-r--r--   0 avelichk   (501) staff       (20)    12243 2023-02-15 15:23:47.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/rest.py
-drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2023-02-15 15:24:03.923906 kubeflow-katib-0.15.0rc1/kubeflow/katib/utils/
--rw-r--r--   0 avelichk   (501) staff       (20)        0 2023-02-15 15:23:23.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/utils/__init__.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4090 2023-02-15 15:23:23.000000 kubeflow-katib-0.15.0rc1/kubeflow/katib/utils/utils.py
-drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2023-02-15 15:24:03.924561 kubeflow-katib-0.15.0rc1/kubeflow_katib.egg-info/
--rw-r--r--   0 avelichk   (501) staff       (20)     1193 2023-02-15 15:24:03.000000 kubeflow-katib-0.15.0rc1/kubeflow_katib.egg-info/PKG-INFO
--rw-r--r--   0 avelichk   (501) staff       (20)     2686 2023-02-15 15:24:03.000000 kubeflow-katib-0.15.0rc1/kubeflow_katib.egg-info/SOURCES.txt
--rw-r--r--   0 avelichk   (501) staff       (20)        1 2023-02-15 15:24:03.000000 kubeflow-katib-0.15.0rc1/kubeflow_katib.egg-info/dependency_links.txt
--rw-r--r--   0 avelichk   (501) staff       (20)        1 2023-02-15 15:24:03.000000 kubeflow-katib-0.15.0rc1/kubeflow_katib.egg-info/not-zip-safe
--rw-r--r--   0 avelichk   (501) staff       (20)      114 2023-02-15 15:24:03.000000 kubeflow-katib-0.15.0rc1/kubeflow_katib.egg-info/requires.txt
--rw-r--r--   0 avelichk   (501) staff       (20)        9 2023-02-15 15:24:03.000000 kubeflow-katib-0.15.0rc1/kubeflow_katib.egg-info/top_level.txt
--rw-r--r--   0 avelichk   (501) staff       (20)       38 2023-02-15 15:24:03.925415 kubeflow-katib-0.15.0rc1/setup.cfg
--rw-r--r--   0 avelichk   (501) staff       (20)     2574 2023-02-15 15:24:03.000000 kubeflow-katib-0.15.0rc1/setup.py
+drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2023-08-05 19:13:29.304454 kubeflow-katib-0.16.0rc0/
+-rw-r--r--   0 avelichk   (501) staff       (20)     1193 2023-08-05 19:13:29.304345 kubeflow-katib-0.16.0rc0/PKG-INFO
+-rw-r--r--   0 avelichk   (501) staff       (20)     5474 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/README.md
+drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2023-08-05 19:13:29.297154 kubeflow-katib-0.16.0rc0/kubeflow/
+-rw-r--r--   0 avelichk   (501) staff       (20)       65 2023-08-05 19:13:09.000000 kubeflow-katib-0.16.0rc0/kubeflow/__init__.py
+drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2023-08-05 19:13:29.297932 kubeflow-katib-0.16.0rc0/kubeflow/katib/
+-rw-r--r--   0 avelichk   (501) staff       (20)     4402 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/__init__.py
+drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2023-08-05 19:13:29.298291 kubeflow-katib-0.16.0rc0/kubeflow/katib/api/
+-rw-r--r--   0 avelichk   (501) staff       (20)       87 2023-08-05 19:13:09.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/api/__init__.py
+-rw-r--r--   0 avelichk   (501) staff       (20)    47097 2023-08-05 19:13:09.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/api/katib_client.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     1998 2023-08-05 19:13:09.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/api/search.py
+-rw-r--r--   0 avelichk   (501) staff       (20)    26164 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/api_client.py
+-rw-r--r--   0 avelichk   (501) staff       (20)    12364 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/configuration.py
+drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2023-08-05 19:13:29.298505 kubeflow-katib-0.16.0rc0/kubeflow/katib/constants/
+-rw-r--r--   0 avelichk   (501) staff       (20)        0 2023-08-05 19:13:09.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/constants/__init__.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     2094 2023-08-05 19:13:09.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/constants/constants.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     3711 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/exceptions.py
+-rw-r--r--   0 avelichk   (501) staff       (20)   113357 2023-08-05 19:13:29.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/katib_api_pb2.py
+drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2023-08-05 19:13:29.303316 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/
+-rw-r--r--   0 avelichk   (501) staff       (20)     3565 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/__init__.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4099 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_algorithm_setting.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4681 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_algorithm_spec.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4118 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_collector_spec.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     5659 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_config_map_source.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     6208 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_early_stopping_rule.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4155 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_early_stopping_setting.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4757 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_early_stopping_spec.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     7260 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_experiment.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     8063 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_experiment_condition.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     6818 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_experiment_list.py
+-rw-r--r--   0 avelichk   (501) staff       (20)    12877 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_experiment_spec.py
+-rw-r--r--   0 avelichk   (501) staff       (20)    22676 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_experiment_status.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     5051 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_feasible_space.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4520 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_file_system_path.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     3821 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_filter_spec.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4885 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_graph_config.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4933 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_metric.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     3887 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_metric_strategy.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4172 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_metrics_collector_spec.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4188 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_nas_config.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     8263 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_objective_spec.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     3470 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_observation.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4195 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_operation.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     5573 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_optimal_trial.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     3947 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_parameter_assignment.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4913 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_parameter_spec.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4905 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_source_spec.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     7260 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_suggestion.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     8063 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_suggestion_condition.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     6818 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_suggestion_list.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     6155 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_suggestion_spec.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     9515 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_suggestion_status.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     7110 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_trial.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     6577 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_trial_assignment.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     7913 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_trial_condition.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     6703 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_trial_list.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     5184 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_trial_parameter_spec.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4135 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_trial_source.py
+-rw-r--r--   0 avelichk   (501) staff       (20)    13953 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_trial_spec.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     6840 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_trial_status.py
+-rw-r--r--   0 avelichk   (501) staff       (20)    11124 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_trial_template.py
+-rw-r--r--   0 avelichk   (501) staff       (20)    12243 2023-08-05 19:13:14.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/rest.py
+drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2023-08-05 19:13:29.303529 kubeflow-katib-0.16.0rc0/kubeflow/katib/utils/
+-rw-r--r--   0 avelichk   (501) staff       (20)        0 2023-08-05 19:13:09.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/utils/__init__.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4090 2023-08-05 19:13:09.000000 kubeflow-katib-0.16.0rc0/kubeflow/katib/utils/utils.py
+drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2023-08-05 19:13:29.304186 kubeflow-katib-0.16.0rc0/kubeflow_katib.egg-info/
+-rw-r--r--   0 avelichk   (501) staff       (20)     1193 2023-08-05 19:13:29.000000 kubeflow-katib-0.16.0rc0/kubeflow_katib.egg-info/PKG-INFO
+-rw-r--r--   0 avelichk   (501) staff       (20)     2686 2023-08-05 19:13:29.000000 kubeflow-katib-0.16.0rc0/kubeflow_katib.egg-info/SOURCES.txt
+-rw-r--r--   0 avelichk   (501) staff       (20)        1 2023-08-05 19:13:29.000000 kubeflow-katib-0.16.0rc0/kubeflow_katib.egg-info/dependency_links.txt
+-rw-r--r--   0 avelichk   (501) staff       (20)        1 2023-08-05 19:13:29.000000 kubeflow-katib-0.16.0rc0/kubeflow_katib.egg-info/not-zip-safe
+-rw-r--r--   0 avelichk   (501) staff       (20)      123 2023-08-05 19:13:29.000000 kubeflow-katib-0.16.0rc0/kubeflow_katib.egg-info/requires.txt
+-rw-r--r--   0 avelichk   (501) staff       (20)        9 2023-08-05 19:13:29.000000 kubeflow-katib-0.16.0rc0/kubeflow_katib.egg-info/top_level.txt
+-rw-r--r--   0 avelichk   (501) staff       (20)       38 2023-08-05 19:13:29.304491 kubeflow-katib-0.16.0rc0/setup.cfg
+-rw-r--r--   0 avelichk   (501) staff       (20)     2584 2023-08-05 19:13:29.000000 kubeflow-katib-0.16.0rc0/setup.py
```

### Comparing `kubeflow-katib-0.15.0rc1/PKG-INFO` & `kubeflow-katib-0.16.0rc0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kubeflow-katib
-Version: 0.15.0rc1
+Version: 0.16.0rc0
 Summary: Katib Python SDK for APIVersion v1beta1
 Home-page: https://github.com/kubeflow/katib/tree/master/sdk/python/v1beta1
 Author: Kubeflow Authors
 Author-email: premnath.vel@gmail.com
 License: Apache License Version 2.0
 Description: Katib Python SDK for APIVersion v1beta1
 Platform: UNKNOWN
```

### Comparing `kubeflow-katib-0.15.0rc1/README.md` & `kubeflow-katib-0.16.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/__init__.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/__init__.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/api/katib_client.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/api/katib_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,45 +8,47 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import multiprocessing
-from typing import Callable, List, Dict, Any
 import inspect
+import multiprocessing
 import textwrap
-import grpc
 import time
+from typing import Any, Callable, Dict, List, Optional, Union
 
-from kubernetes import client, config
+import grpc
+import kubeflow.katib.katib_api_pb2 as katib_api_pb2
 from kubeflow.katib import models
 from kubeflow.katib.api_client import ApiClient
 from kubeflow.katib.constants import constants
 from kubeflow.katib.utils import utils
-import kubeflow.katib.katib_api_pb2 as katib_api_pb2
+from kubernetes import client, config
 
 
 class KatibClient(object):
     def __init__(
         self,
         config_file: str = None,
         context: str = None,
         client_configuration: client.Configuration = None,
+        namespace: str = utils.get_default_target_namespace(),
     ):
         """KatibClient constructor.
 
         Args:
             config_file: Path to the kube-config file. Defaults to ~/.kube/config.
             context: Set the active context. Defaults to current_context from the kube-config.
             client_configuration: Client configuration for cluster authentication.
                 You have to provide valid configuration with Bearer token or
                 with username and password.
                 You can find an example here: https://github.com/kubernetes-client/python/blob/67f9c7a97081b4526470cad53576bc3b71fa6fcc/examples/remote_cluster.py#L31
+            namespace: Target Kubernetes namespace. Can be overridden during method invocations.
         """
 
         self.in_cluster = False
         # If client configuration is not set, use kube-config to access Kubernetes APIs.
         if client_configuration is None:
             # Load kube-config or in-cluster config.
             if config_file or not utils.is_running_in_k8s():
@@ -54,43 +56,47 @@
             else:
                 config.load_incluster_config()
                 self.in_cluster = True
 
         k8s_client = client.ApiClient(client_configuration)
         self.custom_api = client.CustomObjectsApi(k8s_client)
         self.api_client = ApiClient()
+        self.namespace = namespace
 
     def _is_ipython(self):
         """Returns whether we are running in notebook."""
+
         try:
             import IPython
 
             ipy = IPython.get_ipython()
             if ipy is None:
                 return False
         except ImportError:
             return False
         return True
 
     def create_experiment(
         self,
         experiment: models.V1beta1Experiment,
-        namespace: str = utils.get_default_target_namespace(),
+        namespace: Optional[str] = None,
     ):
         """Create the Katib Experiment.
 
         Args:
             experiment: Experiment object of type V1beta1Experiment.
             namespace: Namespace for the Experiment.
 
         Raises:
             TimeoutError: Timeout to create Katib Experiment.
             RuntimeError: Failed to create Katib Experiment.
         """
 
+        namespace = namespace or self.namespace
+
         try:
             self.custom_api.create_namespaced_custom_object(
                 constants.KUBEFLOW_GROUP,
                 constants.KATIB_VERSION,
                 namespace,
                 constants.EXPERIMENT_PLURAL,
                 experiment,
@@ -125,23 +131,24 @@
     def tune(
         self,
         # TODO (andreyvelich): How to be consistent with other APIs (name) ?
         name: str,
         objective: Callable,
         parameters: Dict[str, Any],
         base_image: str = constants.BASE_IMAGE_TENSORFLOW,
-        namespace: str = utils.get_default_target_namespace(),
+        namespace: Optional[str] = None,
         algorithm_name: str = "random",
         objective_metric_name: str = None,
         additional_metric_names: List[str] = [],
         objective_type: str = "maximize",
         objective_goal: float = None,
         max_trial_count: int = None,
         parallel_trial_count: int = None,
         max_failed_trial_count: int = None,
+        resources_per_trial: Union[dict, client.V1ResourceRequirements, None] = None,
         retain_trials: bool = False,
         packages_to_install: List[str] = None,
         pip_index_url: str = "https://pypi.org/simple",
     ):
         """Create HyperParameter Tuning Katib Experiment from the objective function.
 
         Args:
@@ -167,26 +174,46 @@
             objective_type: Type for the Experiment optimization for the objective metric.
                 Must be one of `minimize` or `maximize`.
             objective_goal: Objective goal that Experiment should reach to be Succeeded.
             max_trial_count: Maximum number of Trials to run. For the default
                 values check this doc: https://www.kubeflow.org/docs/components/katib/experiment/#configuration-spec.
             parallel_trial_count: Number of Trials that Experiment runs in parallel.
             max_failed_trial_count: Maximum number of Trials allowed to fail.
+            resources_per_trial: A parameter that lets you specify how much
+            resources each trial container should have. You can either specify a
+            kubernetes.client.V1ResourceRequirements object (documented here:
+            https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1ResourceRequirements.md)
+            or a dictionary that includes one or more of the following keys:
+            `cpu`, `memory`, or `gpu` (other keys will be ignored). Appropriate
+            values for these keys are documented here:
+            https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/.
+            For example:
+                {
+                    "cpu": "1",
+                    "gpu": "1",
+                    "memory": "2Gi",
+                }
+            Please note, `gpu` specifies a resource request with a key of
+            `nvidia.com/gpu`, i.e. an NVIDIA GPU. If you need a different type
+            of GPU, pass in a V1ResourceRequirement instance instead, since it's
+            more flexible. This parameter is optional and defaults to None.
             retain_trials: Whether Trials' resources (e.g. pods) are deleted after Succeeded state.
             packages_to_install: List of Python packages to install in addition
                 to the base image packages. These packages are installed before
                 executing the objective function.
             pip_index_url: The PyPI url from which to install Python packages.
 
         Raises:
             ValueError: Objective function has invalid arguments.
             TimeoutError: Timeout to create Katib Experiment.
             RuntimeError: Failed to create Katib Experiment.
         """
 
+        namespace = namespace or self.namespace
+
         # Create Katib Experiment template.
         experiment = models.V1beta1Experiment(
             api_version=f"{constants.KUBEFLOW_GROUP}/{constants.KATIB_VERSION}",
             kind=constants.EXPERIMENT_KIND,
             metadata=models.V1ObjectMeta(name=name, namespace=namespace),
             spec=models.V1beta1ExperimentSpec(),
         )
@@ -268,14 +295,23 @@
         # Install Python packages if that is required.
         if packages_to_install is not None:
             exec_script = (
                 utils.get_script_for_python_packages(packages_to_install, pip_index_url)
                 + exec_script
             )
 
+        if isinstance(resources_per_trial, dict):
+            if "gpu" in resources_per_trial:
+                resources_per_trial["nvidia.com/gpu"] = resources_per_trial.pop("gpu")
+
+            resources_per_trial = client.V1ResourceRequirements(
+                requests=resources_per_trial,
+                limits=resources_per_trial,
+            )
+
         # Create Trial specification.
         trial_spec = client.V1Job(
             api_version="batch/v1",
             kind="Job",
             spec=client.V1JobSpec(
                 template=client.V1PodTemplateSpec(
                     metadata=models.V1ObjectMeta(
@@ -285,14 +321,15 @@
                         restart_policy="Never",
                         containers=[
                             client.V1Container(
                                 name=constants.DEFAULT_PRIMARY_CONTAINER_NAME,
                                 image=base_image,
                                 command=["bash", "-c"],
                                 args=[exec_script],
+                                resources=resources_per_trial,
                             )
                         ],
                     ),
                 )
             ),
         )
 
@@ -312,15 +349,15 @@
 
         # Create the Katib Experiment.
         self.create_experiment(experiment, namespace)
 
     def get_experiment(
         self,
         name: str,
-        namespace: str = utils.get_default_target_namespace(),
+        namespace: Optional[str] = None,
         timeout: int = constants.DEFAULT_TIMEOUT,
     ):
         """Get the Katib Experiment.
 
         Args:
             name: Name for the Experiment.
             namespace: Namespace for the Experiment.
@@ -331,14 +368,16 @@
             V1beta1Experiment: Katib Experiment object.
 
         Raises:
             TimeoutError: Timeout to get Katib Experiment.
             RuntimeError: Failed to get Katib Experiment.
         """
 
+        namespace = namespace or self.namespace
+
         try:
             thread = self.custom_api.get_namespaced_custom_object(
                 constants.KUBEFLOW_GROUP,
                 constants.KATIB_VERSION,
                 namespace,
                 constants.EXPERIMENT_PLURAL,
                 name,
@@ -351,15 +390,15 @@
         except multiprocessing.TimeoutError:
             raise TimeoutError(f"Timeout to get Katib Experiment: {namespace}/{name}")
         except Exception:
             raise RuntimeError(f"Failed to get Katib Experiment: {namespace}/{name}")
 
     def list_experiments(
         self,
-        namespace: str = utils.get_default_target_namespace(),
+        namespace: Optional[str] = None,
         timeout: int = constants.DEFAULT_TIMEOUT,
     ):
         """List of all Katib Experiments in namespace.
 
         Args:
             namespace: Namespace to list the Experiments.
             timeout: Optional, Kubernetes API server timeout in seconds
@@ -370,14 +409,16 @@
             empty list if Experiments cannot be found.
 
         Raises:
             TimeoutError: Timeout to list Katib Experiments.
             RuntimeError: Failed to list Katib Experiments.
         """
 
+        namespace = namespace or self.namespace
+
         result = []
         try:
             thread = self.custom_api.list_namespaced_custom_object(
                 constants.KUBEFLOW_GROUP,
                 constants.KATIB_VERSION,
                 namespace=namespace,
                 plural=constants.EXPERIMENT_PLURAL,
@@ -399,15 +440,15 @@
                 f"Failed to list Katib Experiments in namespace: {namespace}"
             )
         return result
 
     def get_experiment_conditions(
         self,
         name: str,
-        namespace: str = utils.get_default_target_namespace(),
+        namespace: Optional[str] = None,
         experiment: models.V1beta1Experiment = None,
         timeout: int = constants.DEFAULT_TIMEOUT,
     ):
         """Get the Experiment conditions. Experiment is in the condition when
         `status` is True for the appropriate condition `type`.
 
         Args:
@@ -424,14 +465,16 @@
                 conditions yet.
 
         Raises:
             TimeoutError: Timeout to get Katib Experiment.
             RuntimeError: Failed to get Katib Experiment.
         """
 
+        namespace = namespace or self.namespace
+
         if experiment is None:
             experiment = self.get_experiment(name, namespace, timeout)
 
         if (
             experiment.status
             and experiment.status.conditions
             and len(experiment.status.conditions) > 0
@@ -439,15 +482,15 @@
             return experiment.status.conditions
 
         return []
 
     def is_experiment_created(
         self,
         name: str,
-        namespace: str = utils.get_default_target_namespace(),
+        namespace: Optional[str] = None,
         experiment: models.V1beta1Experiment = None,
         timeout: int = constants.DEFAULT_TIMEOUT,
     ):
         """Check if Experiment is Created.
 
         Args:
             name: Name for the Experiment.
@@ -460,23 +503,25 @@
             bool: True is Experiment is Created, else False.
 
         Raises:
             TimeoutError: Timeout to get Katib Experiment.
             RuntimeError: Failed to get Katib Experiment.
         """
 
+        namespace = namespace or self.namespace
+
         return utils.has_condition(
             self.get_experiment_conditions(name, namespace, experiment, timeout),
             constants.EXPERIMENT_CONDITION_CREATED,
         )
 
     def is_experiment_running(
         self,
         name: str,
-        namespace: str = utils.get_default_target_namespace(),
+        namespace: Optional[str] = None,
         experiment: models.V1beta1Experiment = None,
         timeout: int = constants.DEFAULT_TIMEOUT,
     ):
         """Check if Experiment is Running.
 
         Args:
             name: Name for the Experiment.
@@ -489,23 +534,25 @@
             bool: True is Experiment is Running, else False.
 
         Raises:
             TimeoutError: Timeout to get Katib Experiment.
             RuntimeError: Failed to get Katib Experiment.
         """
 
+        namespace = namespace or self.namespace
+
         return utils.has_condition(
             self.get_experiment_conditions(name, namespace, experiment, timeout),
             constants.EXPERIMENT_CONDITION_RUNNING,
         )
 
     def is_experiment_restarting(
         self,
         name: str,
-        namespace: str = utils.get_default_target_namespace(),
+        namespace: Optional[str] = None,
         experiment: models.V1beta1Experiment = None,
         timeout: int = constants.DEFAULT_TIMEOUT,
     ):
         """Check if Experiment is Restarting.
         Args:
             name: Name for the Experiment.
             namespace: Namespace for the Experiment.
@@ -517,23 +564,25 @@
             bool: True is Experiment is Resting, else False.
 
         Raises:
             TimeoutError: Timeout to get Katib Experiment.
             RuntimeError: Failed to get Katib Experiment.
         """
 
+        namespace = namespace or self.namespace
+
         return utils.has_condition(
             self.get_experiment_conditions(name, namespace, experiment, timeout),
             constants.EXPERIMENT_CONDITION_RESTARTING,
         )
 
     def is_experiment_succeeded(
         self,
         name: str,
-        namespace: str = utils.get_default_target_namespace(),
+        namespace: Optional[str] = None,
         experiment: models.V1beta1Experiment = None,
         timeout: int = constants.DEFAULT_TIMEOUT,
     ):
         """Check if Experiment is Succeeded.
         Args:
             name: Name for the Experiment.
             namespace: Namespace for the Experiment.
@@ -545,23 +594,25 @@
             bool: True is Experiment is Succeeded, else False.
 
         Raises:
             TimeoutError: Timeout to get Katib Experiment.
             RuntimeError: Failed to get Katib Experiment.
         """
 
+        namespace = namespace or self.namespace
+
         return utils.has_condition(
             self.get_experiment_conditions(name, namespace, experiment, timeout),
             constants.EXPERIMENT_CONDITION_SUCCEEDED,
         )
 
     def is_experiment_failed(
         self,
         name: str,
-        namespace: str = utils.get_default_target_namespace(),
+        namespace: Optional[str] = None,
         experiment: models.V1beta1Experiment = None,
         timeout: int = constants.DEFAULT_TIMEOUT,
     ):
         """Check if Experiment is Failed.
         Args:
             name: Name for the Experiment.
             namespace: Namespace for the Experiment.
@@ -573,23 +624,25 @@
             bool: True is Experiment is Failed, else False.
 
         Raises:
             TimeoutError: Timeout to get Katib Experiment.
             RuntimeError: Failed to get Katib Experiment.
         """
 
+        namespace = namespace or self.namespace
+
         return utils.has_condition(
             self.get_experiment_conditions(name, namespace, experiment, timeout),
             constants.EXPERIMENT_CONDITION_FAILED,
         )
 
     def wait_for_experiment_condition(
         self,
         name: str,
-        namespace: str = utils.get_default_target_namespace(),
+        namespace: Optional[str] = None,
         expected_condition: str = constants.EXPERIMENT_CONDITION_SUCCEEDED,
         timeout: int = 600,
         polling_interval: int = 15,
         apiserver_timeout: int = constants.DEFAULT_TIMEOUT,
     ):
         """Wait until Experiment reaches specific condition. By default it waits
         for the Succeeded condition.
@@ -609,16 +662,17 @@
         Raises:
             RuntimeError: Failed to get Katib Experiment or Experiment reaches
                 Failed state if it does not wait for this condition.
             TimeoutError: Timeout waiting for Experiment to reach required condition
                 or timeout to get Katib Experiment.
         """
 
-        for _ in range(round(timeout / polling_interval)):
+        namespace = namespace or self.namespace
 
+        for _ in range(round(timeout / polling_interval)):
             # We should get Experiment only once per cycle and check the statuses.
             experiment = self.get_experiment(name, namespace, apiserver_timeout)
 
             # Wait for Failed condition.
             if (
                 expected_condition == constants.EXPERIMENT_CONDITION_FAILED
                 and self.is_experiment_failed(
@@ -692,15 +746,15 @@
         raise TimeoutError(
             f"Timeout waiting for Experiment: {namespace}/{name} to reach {expected_condition} state"
         )
 
     def edit_experiment_budget(
         self,
         name: str,
-        namespace: str = utils.get_default_target_namespace(),
+        namespace: Optional[str] = None,
         max_trial_count: int = None,
         parallel_trial_count: int = None,
         max_failed_trial_count: int = None,
         timeout: int = constants.DEFAULT_TIMEOUT,
     ):
         """Update Experiment budget for the running Trials. You can modify Trial
         budget to resume Succeeded Experiments with `LongRunning` and `FromVolume`
@@ -721,14 +775,16 @@
             ValueError: The new Trial budget is not set.
             TimeoutError: Timeout to edit/get Katib Experiment or timeout to wait
                 until Experiment reaches Restarting condition.
             RuntimeError: Failed to edit/get Katib Experiment or Experiment
                 reaches Failed condition.
         """
 
+        namespace = namespace or self.namespace
+
         # The new Trial budget must be set.
         if (
             max_trial_count is None
             and parallel_trial_count is None
             and max_failed_trial_count is None
         ):
             raise ValueError(
@@ -762,15 +818,15 @@
             raise RuntimeError(f"Failed to edit Katib Experiment: {namespace}/{name}")
 
         print(f"Experiment {namespace}/{name} has been updated")
 
     def delete_experiment(
         self,
         name: str,
-        namespace: str = utils.get_default_target_namespace(),
+        namespace: Optional[str] = None,
         delete_options: client.V1DeleteOptions = None,
     ):
         """Delete the Katib Experiment.
 
         Args:
             name: Name for the Experiment.
             namespace: Namespace for the Experiment.
@@ -778,14 +834,16 @@
                 Katib Experiment. For example, grace period seconds.
 
         Raises:
             TimeoutError: Timeout to delete Katib Experiment.
             RuntimeError: Failed to delete Katib Experiment.
         """
 
+        namespace = namespace or self.namespace
+
         try:
             self.custom_api.delete_namespaced_custom_object(
                 constants.KUBEFLOW_GROUP,
                 constants.KATIB_VERSION,
                 namespace,
                 constants.EXPERIMENT_PLURAL,
                 name,
@@ -800,15 +858,15 @@
 
         # TODO (andreyvelich): Use proper logger.
         print(f"Experiment {namespace}/{name} has been deleted")
 
     def get_suggestion(
         self,
         name: str,
-        namespace: str = utils.get_default_target_namespace(),
+        namespace: Optional[str] = None,
         timeout: int = constants.DEFAULT_TIMEOUT,
     ):
         """Get the Katib Suggestion.
 
         Args:
             name: Name for the Suggestion.
             namespace: Namespace for the Suggestion.
@@ -819,14 +877,16 @@
             V1beta1Suggestion: Katib Suggestion object.
 
         Raises:
             TimeoutError: Timeout to get Katib Suggestion.
             RuntimeError: Failed to get Katib Suggestion.
         """
 
+        namespace = namespace or self.namespace
+
         try:
             thread = self.custom_api.get_namespaced_custom_object(
                 constants.KUBEFLOW_GROUP,
                 constants.KATIB_VERSION,
                 namespace,
                 constants.SUGGESTION_PLURAL,
                 name,
@@ -839,15 +899,15 @@
         except multiprocessing.TimeoutError:
             raise TimeoutError(f"Timeout to get Katib Suggestion: {namespace}/{name}")
         except Exception:
             raise RuntimeError(f"Failed to get Katib Suggestion: {namespace}/{name}")
 
     def list_suggestions(
         self,
-        namespace: str = utils.get_default_target_namespace(),
+        namespace: Optional[str] = None,
         timeout: int = constants.DEFAULT_TIMEOUT,
     ):
         """List of all Katib Suggestion in namespace.
 
         Args:
             namespace: Namespace to list the Suggestions.
             timeout: Optional, Kubernetes API server timeout in seconds
@@ -858,14 +918,16 @@
             empty list if Suggestions cannot be found.
 
         Raises:
             TimeoutError: Timeout to list Katib Suggestions.
             RuntimeError: Failed to list Katib Suggestions.
         """
 
+        namespace = namespace or self.namespace
+
         result = []
         try:
             thread = self.custom_api.list_namespaced_custom_object(
                 constants.KUBEFLOW_GROUP,
                 constants.KATIB_VERSION,
                 namespace=namespace,
                 plural=constants.EXPERIMENT_PLURAL,
@@ -887,15 +949,15 @@
                 f"Failed to list Katib Suggestions in namespace: {namespace}"
             )
         return result
 
     def get_trial(
         self,
         name: str,
-        namespace: str = utils.get_default_target_namespace(),
+        namespace: Optional[str] = None,
         timeout: int = constants.DEFAULT_TIMEOUT,
     ):
         """Get the Katib Trial.
 
         Args:
             name: Name for the Trial.
             namespace: Namespace for the Trial.
@@ -906,14 +968,16 @@
             V1beta1Trial: Katib Trial object.
 
         Raises:
             TimeoutError: Timeout to get Katib Trial.
             RuntimeError: Failed to get Katib Trial.
         """
 
+        namespace = namespace or self.namespace
+
         try:
             thread = self.custom_api.get_namespaced_custom_object(
                 constants.KUBEFLOW_GROUP,
                 constants.KATIB_VERSION,
                 namespace,
                 constants.TRIAL_PLURAL,
                 name,
@@ -927,15 +991,15 @@
             raise TimeoutError(f"Timeout to get Katib Trial: {namespace}/{name}")
         except Exception:
             raise RuntimeError(f"Failed to get Katib Trial: {namespace}/{name}")
 
     def list_trials(
         self,
         experiment_name: str = None,
-        namespace: str = utils.get_default_target_namespace(),
+        namespace: Optional[str] = None,
         timeout: int = constants.DEFAULT_TIMEOUT,
     ):
         """List of all Trials in namespace. If Experiment name is set,
         it returns all Trials belong to the Experiment.
 
         Args:
             experiment_name: Optional name for the Experiment.
@@ -948,14 +1012,16 @@
             empty list if Trials cannot be found.
 
         Raises:
             TimeoutError: Timeout to list Katib Trials.
             RuntimeError: Failed to list Katib Trials.
         """
 
+        namespace = namespace or self.namespace
+
         result = []
         try:
             if experiment_name is None:
                 thread = self.custom_api.list_namespaced_custom_object(
                     constants.KUBEFLOW_GROUP,
                     constants.KATIB_VERSION,
                     namespace=namespace,
@@ -985,15 +1051,15 @@
         except Exception:
             raise RuntimeError(f"Failed to list Katib Trials in namespace: {namespace}")
         return result
 
     def get_success_trial_details(
         self,
         experiment_name: str = None,
-        namespace: str = utils.get_default_target_namespace(),
+        namespace: Optional[str] = None,
         timeout: int = constants.DEFAULT_TIMEOUT,
     ):
         """Get the Succeeded Trial details. If Experiment name is set,
         it returns Succeeded Trials details belong to the Experiment.
 
         Args:
             experiment_name: Optional name for the Experiment.
@@ -1006,14 +1072,16 @@
             It returns empty list if Succeeded Trials cannot be found.
 
         Raises:
             TimeoutError: Timeout to list Katib Trials.
             RuntimeError: Failed to list Katib Trials.
         """
 
+        namespace = namespace or self.namespace
+
         result = []
         try:
             if experiment_name is None:
                 thread = self.custom_api.list_namespaced_custom_object(
                     constants.KUBEFLOW_GROUP,
                     constants.KATIB_VERSION,
                     namespace=namespace,
@@ -1056,15 +1124,15 @@
         except Exception:
             raise RuntimeError(f"Failed to list Katib Trials in namespace: {namespace}")
         return result
 
     def get_optimal_hyperparameters(
         self,
         name: str,
-        namespace: str = utils.get_default_target_namespace(),
+        namespace: Optional[str] = None,
         timeout: int = constants.DEFAULT_TIMEOUT,
     ):
         """Get the current optimal Trial from the Experiment.
 
         Args:
             name: Name for the Experiment.
             namespace: Namespace for the Experiment.
@@ -1076,28 +1144,30 @@
             It returns `None` if Experiment does not have optimal Trial yet.
 
         Raises:
             TimeoutError: Timeout to get Katib Experiment.
             RuntimeError: Failed to get Katib Experiment.
         """
 
+        namespace = namespace or self.namespace
+
         experiment = self.get_experiment(name, namespace, timeout)
         if (
             experiment.status
             and experiment.status.current_optimal_trial
             and experiment.status.current_optimal_trial.observation.metrics
         ):
             return experiment.status.current_optimal_trial
         else:
             return None
 
     def get_trial_metrics(
         self,
         name: str,
-        namespace: str = utils.get_default_target_namespace(),
+        namespace: Optional[str] = None,
         db_manager_address: str = constants.DEFAULT_DB_MANAGER_ADDRESS,
         timeout: str = constants.DEFAULT_TIMEOUT,
     ):
         """Get the Trial Metric Results from the Katib DB.
         Katib DB Manager service should be accessible while calling this API.
 
         If you run this API in-cluster (e.g. from the Kubeflow Notebook) you can
@@ -1121,21 +1191,22 @@
             For example, to get the first metric value run the following:
             `get_trial_metrics(...)[0].metric.value
 
         Raises:
             RuntimeError: Unable to get Trial metrics.
         """
 
+        namespace = namespace or self.namespace
+
         db_manager_address = db_manager_address.split(":")
         channel = grpc.beta.implementations.insecure_channel(
             db_manager_address[0], int(db_manager_address[1])
         )
 
         with katib_api_pb2.beta_create_DBManager_stub(channel) as client:
-
             try:
                 # When metric name is empty, we select all logs from the Katib DB.
                 observation_logs = client.GetObservationLog(
                     katib_api_pb2.GetObservationLogRequest(trial_name=name),
                     timeout=timeout,
                 )
             except Exception as e:
```

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/api/search.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/api/search.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/api_client.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/api_client.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/configuration.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/configuration.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/constants/constants.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/constants/constants.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/exceptions.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/exceptions.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/katib_api_pb2.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/katib_api_pb2.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/__init__.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,13 +53,8 @@
 from kubeflow.katib.models.v1beta1_trial_parameter_spec import V1beta1TrialParameterSpec
 from kubeflow.katib.models.v1beta1_trial_source import V1beta1TrialSource
 from kubeflow.katib.models.v1beta1_trial_spec import V1beta1TrialSpec
 from kubeflow.katib.models.v1beta1_trial_status import V1beta1TrialStatus
 from kubeflow.katib.models.v1beta1_trial_template import V1beta1TrialTemplate
 
 # Import Kubernetes models.
-from kubernetes.client import V1ObjectMeta
-from kubernetes.client import V1ListMeta
-from kubernetes.client import V1Container
-from kubernetes.client import V1HTTPGetAction
-from kubernetes.client import V1ManagedFieldsEntry
-from kubernetes.client import V1OwnerReference
+from kubernetes.client import *
```

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_algorithm_setting.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_algorithm_setting.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_algorithm_spec.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_algorithm_spec.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_collector_spec.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_collector_spec.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_config_map_source.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_config_map_source.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_early_stopping_rule.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_early_stopping_rule.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_early_stopping_setting.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_early_stopping_setting.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_early_stopping_spec.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_early_stopping_spec.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_experiment.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_experiment.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_experiment_condition.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_experiment_condition.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_experiment_list.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_experiment_list.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_experiment_spec.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_experiment_spec.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_experiment_status.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_experiment_status.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_feasible_space.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_feasible_space.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_file_system_path.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_file_system_path.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_filter_spec.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_filter_spec.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_graph_config.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_graph_config.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_metric.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_metric.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_metric_strategy.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_metric_strategy.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_metrics_collector_spec.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_metrics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_nas_config.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_nas_config.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_objective_spec.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_objective_spec.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_observation.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_observation.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_operation.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_operation.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_optimal_trial.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_optimal_trial.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_parameter_assignment.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_parameter_assignment.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_parameter_spec.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_parameter_spec.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_source_spec.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_source_spec.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_suggestion.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_suggestion.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_suggestion_condition.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_suggestion_condition.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_suggestion_list.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_suggestion_list.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_suggestion_spec.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_suggestion_spec.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_suggestion_status.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_suggestion_status.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_trial.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_trial.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_trial_assignment.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_trial_assignment.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_trial_condition.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_trial_condition.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_trial_list.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_trial_list.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_trial_parameter_spec.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_trial_parameter_spec.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_trial_source.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_trial_source.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_trial_spec.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_trial_spec.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_trial_status.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_trial_status.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/models/v1beta1_trial_template.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/models/v1beta1_trial_template.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/rest.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/rest.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow/katib/utils/utils.py` & `kubeflow-katib-0.16.0rc0/kubeflow/katib/utils/utils.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow_katib.egg-info/PKG-INFO` & `kubeflow-katib-0.16.0rc0/kubeflow_katib.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kubeflow-katib
-Version: 0.15.0rc1
+Version: 0.16.0rc0
 Summary: Katib Python SDK for APIVersion v1beta1
 Home-page: https://github.com/kubeflow/katib/tree/master/sdk/python/v1beta1
 Author: Kubeflow Authors
 Author-email: premnath.vel@gmail.com
 License: Apache License Version 2.0
 Description: Katib Python SDK for APIVersion v1beta1
 Platform: UNKNOWN
```

### Comparing `kubeflow-katib-0.15.0rc1/kubeflow_katib.egg-info/SOURCES.txt` & `kubeflow-katib-0.16.0rc0/kubeflow_katib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.15.0rc1/setup.py` & `kubeflow-katib-0.16.0rc0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,30 +18,30 @@
 
 REQUIRES = [
     "certifi>=14.05.14",
     "six>=1.10",
     "setuptools>=21.0.0",
     "urllib3>=1.15.1",
     "kubernetes>=23.6.0",
-    "grpcio==1.41.1",
-    "protobuf==3.19.5",
+    "grpcio>=1.41.1",
+    "protobuf>=3.19.5, <=3.20.3",
 ]
 
 katib_grpc_api_file = "../../../pkg/apis/manager/v1beta1/python/api_pb2.py"
 
 # Copy Katib gRPC Python APIs to use it in the Katib SDK Client.
 # We need to always copy this file only on the SDK building stage, not on SDK installation stage.
 if os.path.exists(katib_grpc_api_file):
     shutil.copy(
         katib_grpc_api_file, "kubeflow/katib/katib_api_pb2.py",
     )
 
 setuptools.setup(
     name="kubeflow-katib",
-    version="0.15.0rc1",
+    version="0.16.0rc0",
     author="Kubeflow Authors",
     author_email="premnath.vel@gmail.com",
     license="Apache License Version 2.0",
     url="https://github.com/kubeflow/katib/tree/master/sdk/python/v1beta1",
     description="Katib Python SDK for APIVersion v1beta1",
     long_description="Katib Python SDK for APIVersion v1beta1",
     packages=setuptools.find_packages(include=("kubeflow*")),
```

