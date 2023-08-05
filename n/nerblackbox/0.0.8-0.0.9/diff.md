# Comparing `tmp/nerblackbox-0.0.8.tar.gz` & `tmp/nerblackbox-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nerblackbox-0.0.8.tar", last modified: Sun Jan 24 17:47:25 2021, max compression
+gzip compressed data, was "dist/nerblackbox-0.0.9.tar", last modified: Mon Apr  5 20:02:59 2021, max compression
```

## Comparing `nerblackbox-0.0.8.tar` & `nerblackbox-0.0.9.tar`

### file list

```diff
@@ -1,86 +1,94 @@
-drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/
--rw-r--r--   0 stofe      (502) staff       (20)      234 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/MANIFEST.in
--rw-r--r--   0 stofe      (502) staff       (20)     4637 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/PKG-INFO
--rw-r--r--   0 stofe      (502) staff       (20)     2888 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/README.rst
-drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/nerblackbox/
--rw-r--r--   0 stofe      (502) staff       (20)      994 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/MLproject
--rw-r--r--   0 stofe      (502) staff       (20)      110 2021-01-24 17:04:34.000000 nerblackbox-0.0.8/nerblackbox/__about__.py
--rw-r--r--   0 stofe      (502) staff       (20)      343 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/__init__.py
--rw-r--r--   0 stofe      (502) staff       (20)     6677 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/api.py
--rw-r--r--   0 stofe      (502) staff       (20)     6683 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/cli.py
-drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/nerblackbox/modules/
--rw-r--r--   0 stofe      (502) staff       (20)        0 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/__init__.py
-drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/nerblackbox/modules/data/
--rw-r--r--   0 stofe      (502) staff       (20)        0 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/data/__init__.py
-drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/nerblackbox/modules/data/datasets/
--rw-r--r--   0 stofe      (502) staff       (20)        0 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/data/datasets/.gitignore
-drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/nerblackbox/modules/data/experiment_configs/
--rw-r--r--   0 stofe      (502) staff       (20)        0 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/data/experiment_configs/.gitignore
--rw-r--r--   0 stofe      (502) staff       (20)      274 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/data/experiment_configs/default.ini
--rw-r--r--   0 stofe      (502) staff       (20)      455 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/data/experiment_configs/exp_test.ini
-drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/nerblackbox/modules/data/pretrained_models/
--rw-r--r--   0 stofe      (502) staff       (20)        0 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/data/pretrained_models/.gitignore
-drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/nerblackbox/modules/datasets/
--rw-r--r--   0 stofe      (502) staff       (20)        0 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/datasets/__init__.py
-drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/nerblackbox/modules/datasets/formatter/
--rw-r--r--   0 stofe      (502) staff       (20)        0 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/datasets/formatter/__init__.py
--rw-r--r--   0 stofe      (502) staff       (20)      797 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/datasets/formatter/auto_formatter.py
--rw-r--r--   0 stofe      (502) staff       (20)    13278 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/datasets/formatter/base_formatter.py
--rw-r--r--   0 stofe      (502) staff       (20)     3832 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/datasets/formatter/conll2003_formatter.py
--rw-r--r--   0 stofe      (502) staff       (20)     3867 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/datasets/formatter/suc_formatter.py
--rw-r--r--   0 stofe      (502) staff       (20)     3673 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/datasets/formatter/swedish_ner_corpus_formatter.py
--rw-r--r--   0 stofe      (502) staff       (20)      711 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/datasets/formatter/util_functions.py
--rw-r--r--   0 stofe      (502) staff       (20)     5016 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/datasets/plots.py
-drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/nerblackbox/modules/experiment_config/
--rw-r--r--   0 stofe      (502) staff       (20)        0 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/experiment_config/__init__.py
--rw-r--r--   0 stofe      (502) staff       (20)     9387 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/experiment_config/experiment_config.py
--rw-r--r--   0 stofe      (502) staff       (20)     1447 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/experiment_results.py
--rw-r--r--   0 stofe      (502) staff       (20)      557 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/experiments_results.py
--rw-r--r--   0 stofe      (502) staff       (20)    35013 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/main.py
-drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/nerblackbox/modules/ner_training/
--rw-r--r--   0 stofe      (502) staff       (20)        0 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/ner_training/__init__.py
--rw-r--r--   0 stofe      (502) staff       (20)    13805 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/ner_training/bert_ner_single.py
-drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/nerblackbox/modules/ner_training/data_preprocessing/
--rw-r--r--   0 stofe      (502) staff       (20)        0 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/ner_training/data_preprocessing/__init__.py
--rw-r--r--   0 stofe      (502) staff       (20)     6009 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/ner_training/data_preprocessing/data_preprocessor.py
-drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/nerblackbox/modules/ner_training/data_preprocessing/tools/
--rw-r--r--   0 stofe      (502) staff       (20)        0 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/ner_training/data_preprocessing/tools/__init__.py
--rw-r--r--   0 stofe      (502) staff       (20)      851 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/ner_training/data_preprocessing/tools/bert_dataset.py
--rw-r--r--   0 stofe      (502) staff       (20)     4238 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/ner_training/data_preprocessing/tools/csv_reader.py
--rw-r--r--   0 stofe      (502) staff       (20)      730 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/ner_training/data_preprocessing/tools/input_example.py
--rw-r--r--   0 stofe      (502) staff       (20)     7846 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/ner_training/data_preprocessing/tools/input_example_to_tensors.py
-drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/nerblackbox/modules/ner_training/logging/
--rw-r--r--   0 stofe      (502) staff       (20)        0 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/ner_training/logging/__init__.py
--rw-r--r--   0 stofe      (502) staff       (20)     2869 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/ner_training/logging/default_logger.py
--rw-r--r--   0 stofe      (502) staff       (20)     4714 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/ner_training/logging/mlflow_client.py
-drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/nerblackbox/modules/ner_training/metrics/
--rw-r--r--   0 stofe      (502) staff       (20)        0 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/ner_training/metrics/__init__.py
--rw-r--r--   0 stofe      (502) staff       (20)     3848 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/ner_training/metrics/logged_metrics.py
--rw-r--r--   0 stofe      (502) staff       (20)     9055 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/ner_training/metrics/ner_metrics.py
--rw-r--r--   0 stofe      (502) staff       (20)    31798 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/ner_training/ner_model.py
--rw-r--r--   0 stofe      (502) staff       (20)    11065 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/ner_training/ner_model_predict.py
--rw-r--r--   0 stofe      (502) staff       (20)     5831 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/ner_training/ner_model_train.py
-drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/nerblackbox/modules/scripts/
--rw-r--r--   0 stofe      (502) staff       (20)        0 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/scripts/__init__.py
--rw-r--r--   0 stofe      (502) staff       (20)      856 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/scripts/script_analyze_data.py
--rw-r--r--   0 stofe      (502) staff       (20)     4607 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/scripts/script_run_experiment.py
--rw-r--r--   0 stofe      (502) staff       (20)     1404 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/scripts/script_set_up_dataset.py
-drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/nerblackbox/modules/utils/
--rw-r--r--   0 stofe      (502) staff       (20)        0 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/utils/__init__.py
--rw-r--r--   0 stofe      (502) staff       (20)      712 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/utils/env_variable.py
--rw-r--r--   0 stofe      (502) staff       (20)     6463 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/modules/utils/util_functions.py
-drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/nerblackbox/tests/
--rw-r--r--   0 stofe      (502) staff       (20)        0 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/tests/__init__.py
--rw-r--r--   0 stofe      (502) staff       (20)     5977 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/nerblackbox/tests/test_ner_metrics.py
-drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/nerblackbox.egg-info/
--rw-r--r--   0 stofe      (502) staff       (20)     4637 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/nerblackbox.egg-info/PKG-INFO
--rw-r--r--   0 stofe      (502) staff       (20)     2972 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/nerblackbox.egg-info/SOURCES.txt
--rw-r--r--   0 stofe      (502) staff       (20)        1 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/nerblackbox.egg-info/dependency_links.txt
--rw-r--r--   0 stofe      (502) staff       (20)       79 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/nerblackbox.egg-info/entry_points.txt
--rw-r--r--   0 stofe      (502) staff       (20)        1 2020-10-23 17:20:04.000000 nerblackbox-0.0.8/nerblackbox.egg-info/not-zip-safe
--rw-r--r--   0 stofe      (502) staff       (20)      271 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/nerblackbox.egg-info/requires.txt
--rw-r--r--   0 stofe      (502) staff       (20)       12 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/nerblackbox.egg-info/top_level.txt
--rw-r--r--   0 stofe      (502) staff       (20)      174 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/requirements.txt
--rw-r--r--   0 stofe      (502) staff       (20)       88 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/requirements_dev.txt
--rw-r--r--   0 stofe      (502) staff       (20)       63 2021-01-24 17:47:25.000000 nerblackbox-0.0.8/setup.cfg
--rw-r--r--   0 stofe      (502) staff       (20)     2444 2021-01-24 17:02:30.000000 nerblackbox-0.0.8/setup.py
+drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-04-05 20:02:59.000000 nerblackbox-0.0.9/
+-rw-r--r--   0 stofe      (502) staff       (20)      234 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/MANIFEST.in
+-rw-r--r--   0 stofe      (502) staff       (20)     3595 2021-04-05 20:02:59.000000 nerblackbox-0.0.9/PKG-INFO
+-rw-r--r--   0 stofe      (502) staff       (20)     2011 2021-04-05 19:21:35.000000 nerblackbox-0.0.9/README.rst
+drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-04-05 20:02:59.000000 nerblackbox-0.0.9/data/
+-rw-r--r--   0 stofe      (502) staff       (20)        0 2021-01-24 17:02:30.000000 nerblackbox-0.0.9/data/__init__.py
+drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-04-05 20:02:59.000000 nerblackbox-0.0.9/dataX/
+-rw-r--r--   0 stofe      (502) staff       (20)        0 2021-01-24 17:02:30.000000 nerblackbox-0.0.9/dataX/__init__.py
+drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-04-05 20:02:59.000000 nerblackbox-0.0.9/nerblackbox/
+-rw-r--r--   0 stofe      (502) staff       (20)      994 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/MLproject
+-rw-r--r--   0 stofe      (502) staff       (20)      110 2021-04-05 19:21:35.000000 nerblackbox-0.0.9/nerblackbox/__about__.py
+-rw-r--r--   0 stofe      (502) staff       (20)      343 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/__init__.py
+-rw-r--r--   0 stofe      (502) staff       (20)     6677 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/api.py
+-rw-r--r--   0 stofe      (502) staff       (20)     6941 2021-04-05 19:21:35.000000 nerblackbox-0.0.9/nerblackbox/cli.py
+drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-04-05 20:02:59.000000 nerblackbox-0.0.9/nerblackbox/modules/
+-rw-r--r--   0 stofe      (502) staff       (20)        0 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/__init__.py
+drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-04-05 20:02:59.000000 nerblackbox-0.0.9/nerblackbox/modules/data/
+drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-04-05 20:02:59.000000 nerblackbox-0.0.9/nerblackbox/modules/data/datasets/
+-rw-r--r--   0 stofe      (502) staff       (20)        0 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/data/datasets/.gitignore
+drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-04-05 20:02:59.000000 nerblackbox-0.0.9/nerblackbox/modules/data/experiment_configs/
+-rw-r--r--   0 stofe      (502) staff       (20)        0 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/data/experiment_configs/.gitignore
+-rw-r--r--   0 stofe      (502) staff       (20)      274 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/data/experiment_configs/default.ini
+-rw-r--r--   0 stofe      (502) staff       (20)      455 2021-04-05 19:21:35.000000 nerblackbox-0.0.9/nerblackbox/modules/data/experiment_configs/my_experiment.ini
+-rw-r--r--   0 stofe      (502) staff       (20)      320 2021-04-05 19:21:35.000000 nerblackbox-0.0.9/nerblackbox/modules/data/experiment_configs/my_experiment_conll2003.ini
+-rw-r--r--   0 stofe      (502) staff       (20)      322 2021-04-05 19:21:35.000000 nerblackbox-0.0.9/nerblackbox/modules/data/experiment_configs/my_experiment_sic.ini
+-rw-r--r--   0 stofe      (502) staff       (20)      322 2021-04-05 19:21:35.000000 nerblackbox-0.0.9/nerblackbox/modules/data/experiment_configs/my_experiment_suc.ini
+-rw-r--r--   0 stofe      (502) staff       (20)      339 2021-04-05 19:21:35.000000 nerblackbox-0.0.9/nerblackbox/modules/data/experiment_configs/my_experiment_swedish_ner_corpus.ini
+drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-04-05 20:02:59.000000 nerblackbox-0.0.9/nerblackbox/modules/data/pretrained_models/
+-rw-r--r--   0 stofe      (502) staff       (20)        0 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/data/pretrained_models/.gitignore
+drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-04-05 20:02:59.000000 nerblackbox-0.0.9/nerblackbox/modules/datasets/
+-rw-r--r--   0 stofe      (502) staff       (20)        0 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/datasets/__init__.py
+drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-04-05 20:02:59.000000 nerblackbox-0.0.9/nerblackbox/modules/datasets/formatter/
+-rw-r--r--   0 stofe      (502) staff       (20)        0 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/datasets/formatter/__init__.py
+-rw-r--r--   0 stofe      (502) staff       (20)      944 2021-04-05 19:21:35.000000 nerblackbox-0.0.9/nerblackbox/modules/datasets/formatter/auto_formatter.py
+-rw-r--r--   0 stofe      (502) staff       (20)    13278 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/datasets/formatter/base_formatter.py
+-rw-r--r--   0 stofe      (502) staff       (20)     3832 2021-04-05 19:21:35.000000 nerblackbox-0.0.9/nerblackbox/modules/datasets/formatter/conll2003_formatter.py
+-rw-r--r--   0 stofe      (502) staff       (20)     4854 2021-04-05 19:21:35.000000 nerblackbox-0.0.9/nerblackbox/modules/datasets/formatter/sic_formatter.py
+-rw-r--r--   0 stofe      (502) staff       (20)     3867 2021-04-05 19:21:35.000000 nerblackbox-0.0.9/nerblackbox/modules/datasets/formatter/suc_formatter.py
+-rw-r--r--   0 stofe      (502) staff       (20)     3672 2021-04-05 19:21:35.000000 nerblackbox-0.0.9/nerblackbox/modules/datasets/formatter/swedish_ner_corpus_formatter.py
+-rw-r--r--   0 stofe      (502) staff       (20)      711 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/datasets/formatter/util_functions.py
+-rw-r--r--   0 stofe      (502) staff       (20)     5016 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/datasets/plots.py
+drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-04-05 20:02:59.000000 nerblackbox-0.0.9/nerblackbox/modules/experiment_config/
+-rw-r--r--   0 stofe      (502) staff       (20)        0 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/experiment_config/__init__.py
+-rw-r--r--   0 stofe      (502) staff       (20)     9387 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/experiment_config/experiment_config.py
+-rw-r--r--   0 stofe      (502) staff       (20)     1447 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/experiment_results.py
+-rw-r--r--   0 stofe      (502) staff       (20)      557 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/experiments_results.py
+-rw-r--r--   0 stofe      (502) staff       (20)    34973 2021-04-05 19:21:35.000000 nerblackbox-0.0.9/nerblackbox/modules/main.py
+drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-04-05 20:02:59.000000 nerblackbox-0.0.9/nerblackbox/modules/ner_training/
+-rw-r--r--   0 stofe      (502) staff       (20)        0 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/ner_training/__init__.py
+-rw-r--r--   0 stofe      (502) staff       (20)    13805 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/ner_training/bert_ner_single.py
+drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-04-05 20:02:59.000000 nerblackbox-0.0.9/nerblackbox/modules/ner_training/data_preprocessing/
+-rw-r--r--   0 stofe      (502) staff       (20)        0 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/ner_training/data_preprocessing/__init__.py
+-rw-r--r--   0 stofe      (502) staff       (20)     6806 2021-04-05 19:21:35.000000 nerblackbox-0.0.9/nerblackbox/modules/ner_training/data_preprocessing/data_preprocessor.py
+drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-04-05 20:02:59.000000 nerblackbox-0.0.9/nerblackbox/modules/ner_training/data_preprocessing/tools/
+-rw-r--r--   0 stofe      (502) staff       (20)        0 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/ner_training/data_preprocessing/tools/__init__.py
+-rw-r--r--   0 stofe      (502) staff       (20)      851 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/ner_training/data_preprocessing/tools/bert_dataset.py
+-rw-r--r--   0 stofe      (502) staff       (20)     4238 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/ner_training/data_preprocessing/tools/csv_reader.py
+-rw-r--r--   0 stofe      (502) staff       (20)      730 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/ner_training/data_preprocessing/tools/input_example.py
+-rw-r--r--   0 stofe      (502) staff       (20)     7846 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/ner_training/data_preprocessing/tools/input_example_to_tensors.py
+drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-04-05 20:02:59.000000 nerblackbox-0.0.9/nerblackbox/modules/ner_training/logging/
+-rw-r--r--   0 stofe      (502) staff       (20)        0 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/ner_training/logging/__init__.py
+-rw-r--r--   0 stofe      (502) staff       (20)     2869 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/ner_training/logging/default_logger.py
+-rw-r--r--   0 stofe      (502) staff       (20)     4714 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/ner_training/logging/mlflow_client.py
+drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-04-05 20:02:59.000000 nerblackbox-0.0.9/nerblackbox/modules/ner_training/metrics/
+-rw-r--r--   0 stofe      (502) staff       (20)        0 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/ner_training/metrics/__init__.py
+-rw-r--r--   0 stofe      (502) staff       (20)     3848 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/ner_training/metrics/logged_metrics.py
+-rw-r--r--   0 stofe      (502) staff       (20)     9055 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/ner_training/metrics/ner_metrics.py
+-rw-r--r--   0 stofe      (502) staff       (20)    31798 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/ner_training/ner_model.py
+-rw-r--r--   0 stofe      (502) staff       (20)    11047 2021-04-05 19:21:35.000000 nerblackbox-0.0.9/nerblackbox/modules/ner_training/ner_model_predict.py
+-rw-r--r--   0 stofe      (502) staff       (20)     5831 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/ner_training/ner_model_train.py
+drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-04-05 20:02:59.000000 nerblackbox-0.0.9/nerblackbox/modules/scripts/
+-rw-r--r--   0 stofe      (502) staff       (20)        0 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/scripts/__init__.py
+-rw-r--r--   0 stofe      (502) staff       (20)      856 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/scripts/script_analyze_data.py
+-rw-r--r--   0 stofe      (502) staff       (20)     4607 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/scripts/script_run_experiment.py
+-rw-r--r--   0 stofe      (502) staff       (20)     1404 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/scripts/script_set_up_dataset.py
+drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-04-05 20:02:59.000000 nerblackbox-0.0.9/nerblackbox/modules/utils/
+-rw-r--r--   0 stofe      (502) staff       (20)        0 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/utils/__init__.py
+-rw-r--r--   0 stofe      (502) staff       (20)      712 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/utils/env_variable.py
+-rw-r--r--   0 stofe      (502) staff       (20)     6463 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/modules/utils/util_functions.py
+drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-04-05 20:02:59.000000 nerblackbox-0.0.9/nerblackbox/tests/
+-rw-r--r--   0 stofe      (502) staff       (20)        0 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/tests/__init__.py
+-rw-r--r--   0 stofe      (502) staff       (20)     5977 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/nerblackbox/tests/test_ner_metrics.py
+drwxr-xr-x   0 stofe      (502) staff       (20)        0 2021-04-05 20:02:59.000000 nerblackbox-0.0.9/nerblackbox.egg-info/
+-rw-r--r--   0 stofe      (502) staff       (20)     3595 2021-04-05 20:02:58.000000 nerblackbox-0.0.9/nerblackbox.egg-info/PKG-INFO
+-rw-r--r--   0 stofe      (502) staff       (20)     3316 2021-04-05 20:02:58.000000 nerblackbox-0.0.9/nerblackbox.egg-info/SOURCES.txt
+-rw-r--r--   0 stofe      (502) staff       (20)        1 2021-04-05 20:02:58.000000 nerblackbox-0.0.9/nerblackbox.egg-info/dependency_links.txt
+-rw-r--r--   0 stofe      (502) staff       (20)       79 2021-04-05 20:02:58.000000 nerblackbox-0.0.9/nerblackbox.egg-info/entry_points.txt
+-rw-r--r--   0 stofe      (502) staff       (20)        1 2020-10-23 17:20:04.000000 nerblackbox-0.0.9/nerblackbox.egg-info/not-zip-safe
+-rw-r--r--   0 stofe      (502) staff       (20)      264 2021-04-05 20:02:58.000000 nerblackbox-0.0.9/nerblackbox.egg-info/requires.txt
+-rw-r--r--   0 stofe      (502) staff       (20)       23 2021-04-05 20:02:58.000000 nerblackbox-0.0.9/nerblackbox.egg-info/top_level.txt
+-rw-r--r--   0 stofe      (502) staff       (20)      167 2021-04-05 19:21:35.000000 nerblackbox-0.0.9/requirements.txt
+-rw-r--r--   0 stofe      (502) staff       (20)       88 2021-04-05 18:42:30.000000 nerblackbox-0.0.9/requirements_dev.txt
+-rw-r--r--   0 stofe      (502) staff       (20)       63 2021-04-05 20:02:59.000000 nerblackbox-0.0.9/setup.cfg
+-rw-r--r--   0 stofe      (502) staff       (20)     2502 2021-04-05 19:21:35.000000 nerblackbox-0.0.9/setup.py
```

### Comparing `nerblackbox-0.0.8/PKG-INFO` & `nerblackbox-0.0.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: nerblackbox
-Version: 0.0.8
-Summary: fine-tune transformer-based models for named entity recognition
+Version: 0.0.9
+Summary: fine-tune transformer-based language models for named entity recognition
 Home-page: https://pypi.org/project/nerblackbox
 Author: Felix Stollenwerk
 Author-email: felix.stollenwerk@arbetsformedlingen.se
 License: Apache 2.0
-Description: 
-        .. .. include:: ./docs_source/source/shared/main1.rst
-        
-        ===========
+Description: ===========
         nerblackbox
         ===========
         
-        A python package to fine-tune transformer-based models for Named Entity Recognition (NER).
+        A python package to fine-tune transformer-based language models for Named Entity Recognition (NER).
         
         .. image:: https://img.shields.io/pypi/v/nerblackbox
             :target: https://pypi.org/project/nerblackbox
             :alt: PyPI
         
         .. image:: https://img.shields.io/pypi/pyversions/nerblackbox
             :target: https://www.python.org/doc/versions/
@@ -40,25 +37,23 @@
         - Source Code: https://github.com/af-ai-center/nerblackbox
         - Documentation: https://af-ai-center.github.io/nerblackbox
         - PyPI: https://pypi.org/project/nerblackbox
         
         About
         =====
         
-        `Transformer-based models <https://arxiv.org/abs/1706.03762>`_ like `BERT <https://arxiv.org/abs/1810.04805>`_ have had a `game-changing impact <https://paperswithcode.com/task/language-modelling>`_ on Natural Language Processing.
+        `Transformer-based language models <https://arxiv.org/abs/1706.03762>`_ like `BERT <https://arxiv.org/abs/1810.04805>`_ have had a `game-changing impact <https://paperswithcode.com/task/language-modelling>`_ on Natural Language Processing.
         
-        In order to utilize the `publicly accessible pretrained models <https://huggingface.co/transformers/pretrained_models.html>`_ for
+        In order to utilize `Hugging Face's publicly accessible pretrained models <https://huggingface.co/transformers/pretrained_models.html>`_ for
         `Named Entity Recognition <https://en.wikipedia.org/wiki/Named-entity_recognition>`_,
         one needs to retrain (or "fine-tune") them using labeled text.
         
         **nerblackbox makes this easy.**
         
-        .. image:: https://raw.githubusercontent.com/af-ai-center/nerblackbox/master/docs/_static/nerblackbox.png
-        
-        .. .. include:: ./docs_source/source/shared/main2.rst
+        .. image:: https://raw.githubusercontent.com/af-ai-center/nerblackbox/master/docs/docs/images/nerblackbox.png
         
         You give it
         
         - a **Dataset** (labeled text)
         - a **Pretrained Model** (transformers)
         
         and you get
@@ -70,46 +65,24 @@
         ============
         
             ``pip install nerblackbox``
         
         Usage
         =====
         
-        .. .. include:: ./docs_source/source/shared/usage.rst
-        
-        Fine-tuning can be done in a few simple steps using an "experiment configuration file"
-        
-        .. code-block:: python
-        
-           # cat <experiment_name>.ini
-           dataset_name = swedish_ner_corpus
-           pretrained_model_name = af-ai-center/bert-base-swedish-uncased
-        
-        and either the Command Line Interface (CLI) or the Python API:
-        
-        .. code-block:: python
-        
-           # CLI
-           nerbb run_experiment <experiment_name>          # fine-tune
-           nerbb get_experiment_results <experiment_name>  # get results/performance
-           nerbb predict <experiment_name> <text_input>    # apply best model
-        
-           # Python API
-           nerbb = NerBlackBox()
-           nerbb.run_experiment(<experiment_name>)         # fine-tune
-           nerbb.get_experiment_results(<experiment_name>) # get results/performance
-           nerbb.predict(<experiment_name>, <text_input>)  # apply best model
+        see documentation: https://af-ai-center.github.io/nerblackbox
         
 Keywords: NLP,NER,named entity recognition,BERT,transformer,pytorch
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: Unix
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.6
```

### Comparing `nerblackbox-0.0.8/nerblackbox/MLproject` & `nerblackbox-0.0.9/nerblackbox/MLproject`

 * *Files identical despite different names*

### Comparing `nerblackbox-0.0.8/nerblackbox/api.py` & `nerblackbox-0.0.9/nerblackbox/api.py`

 * *Files identical despite different names*

### Comparing `nerblackbox-0.0.8/nerblackbox/cli.py` & `nerblackbox-0.0.9/nerblackbox/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,24 @@
     kwargs = {
         "flag": "get_experiment_results",
         "experiment_name": experiment_name,
     }
     _run_nerblackbox_main(ctx.obj, kwargs)
 
 
+@nerbb.command(name="get_experiments_results")
+@click.pass_context
+def get_experiments_results(ctx):
+    """get results for multiple experiments."""
+    kwargs = {
+        "flag": "get_experiments_results",
+    }
+    _run_nerblackbox_main(ctx.obj, kwargs)
+
+
 @nerbb.command(name="init")
 @click.pass_context
 def init(ctx):
     """
     initialize the data_dir directory.
     needs to be called exactly once before any other CLI/API commands of the package are executed.
     """
```

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/datasets/formatter/auto_formatter.py` & `nerblackbox-0.0.9/nerblackbox/modules/datasets/formatter/auto_formatter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from nerblackbox.modules.datasets.formatter.swedish_ner_corpus_formatter import (
     SwedishNerCorpusFormatter,
 )
+from nerblackbox.modules.datasets.formatter.sic_formatter import SICFormatter
 from nerblackbox.modules.datasets.formatter.suc_formatter import SUCFormatter
 from nerblackbox.modules.datasets.formatter.conll2003_formatter import (
     CoNLL2003Formatter,
 )
 from nerblackbox.modules.datasets.formatter.base_formatter import BaseFormatter
 
 
 class AutoFormatter:
     @staticmethod
     def for_dataset(ner_dataset: str) -> BaseFormatter:
         if ner_dataset == "swedish_ner_corpus":
             return SwedishNerCorpusFormatter()
-        elif ner_dataset == "suc":
-            return SUCFormatter()
         elif ner_dataset == "conll2003":
             return CoNLL2003Formatter()
+        elif ner_dataset == "sic":
+            return SICFormatter()
+        elif ner_dataset == "suc":
+            return SUCFormatter()
         else:
             raise Exception(f"ner_dataset = {ner_dataset} unknown.")
```

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/datasets/formatter/base_formatter.py` & `nerblackbox-0.0.9/nerblackbox/modules/datasets/formatter/base_formatter.py`

 * *Files identical despite different names*

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/datasets/formatter/conll2003_formatter.py` & `nerblackbox-0.0.9/nerblackbox/modules/datasets/formatter/conll2003_formatter.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import requests
-
 from os.path import join, isfile
+
 from nerblackbox.modules.datasets.formatter.base_formatter import BaseFormatter
 
 
 class CoNLL2003Formatter(BaseFormatter):
     def __init__(self):
         ner_dataset = "conll2003"
         ner_tag_list = ["PER", "ORG", "LOC", "MISC"]
```

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/datasets/formatter/suc_formatter.py` & `nerblackbox-0.0.9/nerblackbox/modules/datasets/formatter/suc_formatter.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
-
 from os.path import join
+
 from nerblackbox.modules.datasets.formatter.base_formatter import BaseFormatter
 
 
 class SUCFormatter(BaseFormatter):
     def __init__(self):
         ner_dataset = "suc"
         ner_tag_list = [
```

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/datasets/formatter/swedish_ner_corpus_formatter.py` & `nerblackbox-0.0.9/nerblackbox/modules/datasets/formatter/swedish_ner_corpus_formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import subprocess
-
 from os.path import join
 
 from nerblackbox.modules.datasets.formatter.base_formatter import BaseFormatter
 from nerblackbox.modules.utils.env_variable import env_variable
 
 
 class SwedishNerCorpusFormatter(BaseFormatter):
```

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/datasets/formatter/util_functions.py` & `nerblackbox-0.0.9/nerblackbox/modules/datasets/formatter/util_functions.py`

 * *Files identical despite different names*

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/datasets/plots.py` & `nerblackbox-0.0.9/nerblackbox/modules/datasets/plots.py`

 * *Files identical despite different names*

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/experiment_config/experiment_config.py` & `nerblackbox-0.0.9/nerblackbox/modules/experiment_config/experiment_config.py`

 * *Files identical despite different names*

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/experiment_results.py` & `nerblackbox-0.0.9/nerblackbox/modules/experiment_results.py`

 * *Files identical despite different names*

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/experiments_results.py` & `nerblackbox-0.0.9/nerblackbox/modules/experiments_results.py`

 * *Files identical despite different names*

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/main.py` & `nerblackbox-0.0.9/nerblackbox/modules/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,48 +15,52 @@
     get_run_name,
     compute_mean_and_dmean,
 )
 from nerblackbox.modules.experiment_results import ExperimentResults
 from typing import Optional, Any, Tuple, Union, Dict, List
 from pandas import DataFrame
 
-DATASETS = ["conll2003", "swedish_ner_corpus"]
+DATASETS_DOWNLOAD = [
+    "conll2003",
+    "swedish_ner_corpus",
+    "sic",
+]
 
 
 class NerBlackBoxMain:
     def __init__(
         self,
         flag: str,
-        usage: Optional[str] = "cli",
+        usage: str = "cli",
         dataset_name: Optional[str] = None,  # analyze_data & set_up_dataset
-        modify: Optional[bool] = True,  # set_up_dataset
-        val_fraction: Optional[float] = 0.3,  # set_up_dataset
-        verbose: Optional[bool] = False,
+        modify: bool = True,  # set_up_dataset
+        val_fraction: float = 0.3,  # set_up_dataset
+        verbose: bool = False,
         experiment_name: Optional[str] = None,
         run_name: Optional[str] = None,  # run_experiment
-        device: Optional[Any] = "gpu",  # run_experiment
-        fp16: Optional[bool] = False,  # run_experiment
+        device: Any = "gpu",  # run_experiment
+        fp16: bool = False,  # run_experiment
         text_input: Optional[str] = None,  # predict
-        ids: Optional[Tuple[str]] = (),  # get_experiments, get_experiments_results
-        as_df: Optional[bool] = True,  # get_experiments, get_experiments_results
-        results: Optional[bool] = False,  # clear_data
+        ids: Tuple[str, ...] = (),  # get_experiments, get_experiments_results
+        as_df: bool = True,  # get_experiments, get_experiments_results
+        results: bool = False,  # clear_data
     ):
         """
         :param flag:            [str], e.g. 'analyze_data', 'set_up_dataset', 'run_experiment', ..
         :param usage:           [str] 'cli' or 'api'
         :param dataset_name     [str] e.g. 'swedish_ner_corpus'
         :param modify           [bool] if True: modify tags as specified in method modify_ner_tag_mapping()
         :param val_fraction     [float] e.g. 0.3
         :param verbose          [bool]
         :param experiment_name: [str], e.g. 'exp0'
         :param run_name:        [str or None], e.g. 'runA'
         :param device:          [torch device]
         :param fp16:            [bool]
         :param text_input:      [str], e.g. 'this is some text that needs to be annotated'
-        :param ids:             [tuple of int], experiment_ids to include
+        :param ids:             [tuple of str], experiment_ids to include
         :param as_df:           [bool] if True, return pandas DataFrame, else return dict
         :param results:         [bool] if True, clear not only checkpoints but also mlflow, tensorboard and logs
         """
         self._assert_flag(flag)
 
         os.environ["MLFLOW_TRACKING_URI"] = env_variable("DIR_MLFLOW")
 
@@ -96,15 +100,15 @@
             self._create_data_directory()
             self._set_client_and_get_experiments()
 
         ################################################################################################################
         # download
         ################################################################################################################
         elif self.flag == "download":
-            for _dataset_name in DATASETS:
+            for _dataset_name in DATASETS_DOWNLOAD:
                 self.set_up_dataset(_dataset_name)
 
         ################################################################################################################
         # analyze_data
         ################################################################################################################
         elif self.flag == "analyze_data":
             self._assert_flag_arg("dataset_name")
@@ -583,15 +587,15 @@
             _best_single_run,
             _best_average_run,
         )
 
     ####################################################################################################################
     # HELPER: ALL EXPERIMENTS
     ####################################################################################################################
-    def _filter_experiments_by_ids(self, _ids: Tuple[str]) -> Dict:
+    def _filter_experiments_by_ids(self, _ids: Tuple[str, ...]) -> Dict:
         r"""
         get _experiments_id2name [dict] with _ids as keys
         -------------------------------------------------
         :param _ids:  [tuple] of [str], e.g. ('4', '5')
         :return: _experiments_id2name [dict] w/ keys = experiment_id [str] & values = experiment_name [str]
         """
         assert (
```

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/ner_training/bert_ner_single.py` & `nerblackbox-0.0.9/nerblackbox/modules/ner_training/bert_ner_single.py`

 * *Files identical despite different names*

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/ner_training/data_preprocessing/data_preprocessor.py` & `nerblackbox-0.0.9/nerblackbox/modules/ner_training/data_preprocessing/data_preprocessor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import List
+
 from nerblackbox.modules.ner_training.data_preprocessing.tools.bert_dataset import (
     BertDataset,
 )
 from nerblackbox.modules.ner_training.data_preprocessing.tools.csv_reader import (
     CsvReader,
 )
 from nerblackbox.modules.ner_training.data_preprocessing.tools.input_example import (
@@ -53,15 +55,17 @@
         for phase in ["train", "val", "test"]:
             # train data
             input_examples_all = csv_reader.get_input_examples(phase)
             input_examples[phase] = self._prune_examples(
                 input_examples_all, phase, ratio=prune_ratio[phase]
             )
 
-        return input_examples, csv_reader.tag_list
+        return input_examples, self._ensure_completeness_in_case_of_bio_tags(
+            csv_reader.tag_list
+        )
 
     def get_input_examples_predict(self, examples):
         """
         get input examples for PREDICT from input argument examples
         -----------------------------------------------------------
         :param examples:         [list] of [str]
         :return: input_examples: [dict] w/ key = 'predict' & value = [list] of [InputExample]
@@ -142,7 +146,22 @@
             return list_of_examples
         else:
             num_examples_old = len(list_of_examples)
             num_examples_new = int(ratio * float(num_examples_old))
             info = f"> {phase.ljust(5)} data: use {num_examples_new} of {num_examples_old} examples"
             self.default_logger.log_info(info)
             return list_of_examples[:num_examples_new]
+
+    @staticmethod
+    def _ensure_completeness_in_case_of_bio_tags(tag_list: List[str]) -> List[str]:
+        """
+        make sure that there is an "I-*" tag for every "B-*" tag in case of BIO-tags
+        ----------------------------------------------------------------------------
+        :param tag_list:             e.g. ["B-person", "B-time", "I-person"]
+        :return: completed_tag_list: e.g. ["B-person", "B-time", "I-person", "I-time"]
+        """
+        b_tags = [tag for tag in tag_list if tag.startswith("B")]
+        for b_tag in b_tags:
+            i_tag = b_tag.replace("B-", "I-")
+            if i_tag not in tag_list:
+                tag_list.append(i_tag)
+        return tag_list
```

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/ner_training/data_preprocessing/tools/bert_dataset.py` & `nerblackbox-0.0.9/nerblackbox/modules/ner_training/data_preprocessing/tools/bert_dataset.py`

 * *Files identical despite different names*

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/ner_training/data_preprocessing/tools/csv_reader.py` & `nerblackbox-0.0.9/nerblackbox/modules/ner_training/data_preprocessing/tools/csv_reader.py`

 * *Files identical despite different names*

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/ner_training/data_preprocessing/tools/input_example.py` & `nerblackbox-0.0.9/nerblackbox/modules/ner_training/data_preprocessing/tools/input_example.py`

 * *Files identical despite different names*

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/ner_training/data_preprocessing/tools/input_example_to_tensors.py` & `nerblackbox-0.0.9/nerblackbox/modules/ner_training/data_preprocessing/tools/input_example_to_tensors.py`

 * *Files identical despite different names*

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/ner_training/logging/default_logger.py` & `nerblackbox-0.0.9/nerblackbox/modules/ner_training/logging/default_logger.py`

 * *Files identical despite different names*

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/ner_training/logging/mlflow_client.py` & `nerblackbox-0.0.9/nerblackbox/modules/ner_training/logging/mlflow_client.py`

 * *Files identical despite different names*

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/ner_training/metrics/logged_metrics.py` & `nerblackbox-0.0.9/nerblackbox/modules/ner_training/metrics/logged_metrics.py`

 * *Files identical despite different names*

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/ner_training/metrics/ner_metrics.py` & `nerblackbox-0.0.9/nerblackbox/modules/ner_training/metrics/ner_metrics.py`

 * *Files identical despite different names*

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/ner_training/ner_model.py` & `nerblackbox-0.0.9/nerblackbox/modules/ner_training/ner_model.py`

 * *Files identical despite different names*

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/ner_training/ner_model_predict.py` & `nerblackbox-0.0.9/nerblackbox/modules/ner_training/ner_model_predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,26 +13,26 @@
     class that predicts tags for given text
     """
 
     @classmethod
     def load_from_checkpoint(
         cls,
         checkpoint_path: str,
-        map_location=None,
-        tags_csv=None,
     ) -> "NerModelPredict":
         """load model in inference mode from checkpoint_path
 
         Args:
             checkpoint_path: path to checkpoint
 
         Returns:
             model loaded from checkpoint
         """
-        model = super().load_from_checkpoint(checkpoint_path, map_location, tags_csv)
+        model = super().load_from_checkpoint(
+            checkpoint_path, map_location=None, tags_csv=None
+        )
         model.freeze()  # for inference mode
         return model
 
     def __init__(self, hparams: Namespace):
         """
         Args:
             hparams: attr experiment_name, run_name, pretrained_model_name, dataset_name, ..
```

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/ner_training/ner_model_train.py` & `nerblackbox-0.0.9/nerblackbox/modules/ner_training/ner_model_train.py`

 * *Files identical despite different names*

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/scripts/script_analyze_data.py` & `nerblackbox-0.0.9/nerblackbox/modules/scripts/script_analyze_data.py`

 * *Files identical despite different names*

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/scripts/script_run_experiment.py` & `nerblackbox-0.0.9/nerblackbox/modules/scripts/script_run_experiment.py`

 * *Files identical despite different names*

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/scripts/script_set_up_dataset.py` & `nerblackbox-0.0.9/nerblackbox/modules/scripts/script_set_up_dataset.py`

 * *Files identical despite different names*

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/utils/env_variable.py` & `nerblackbox-0.0.9/nerblackbox/modules/utils/env_variable.py`

 * *Files identical despite different names*

### Comparing `nerblackbox-0.0.8/nerblackbox/modules/utils/util_functions.py` & `nerblackbox-0.0.9/nerblackbox/modules/utils/util_functions.py`

 * *Files identical despite different names*

### Comparing `nerblackbox-0.0.8/nerblackbox/tests/test_ner_metrics.py` & `nerblackbox-0.0.9/nerblackbox/tests/test_ner_metrics.py`

 * *Files identical despite different names*

### Comparing `nerblackbox-0.0.8/nerblackbox.egg-info/PKG-INFO` & `nerblackbox-0.0.9/nerblackbox.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: nerblackbox
-Version: 0.0.8
-Summary: fine-tune transformer-based models for named entity recognition
+Version: 0.0.9
+Summary: fine-tune transformer-based language models for named entity recognition
 Home-page: https://pypi.org/project/nerblackbox
 Author: Felix Stollenwerk
 Author-email: felix.stollenwerk@arbetsformedlingen.se
 License: Apache 2.0
-Description: 
-        .. .. include:: ./docs_source/source/shared/main1.rst
-        
-        ===========
+Description: ===========
         nerblackbox
         ===========
         
-        A python package to fine-tune transformer-based models for Named Entity Recognition (NER).
+        A python package to fine-tune transformer-based language models for Named Entity Recognition (NER).
         
         .. image:: https://img.shields.io/pypi/v/nerblackbox
             :target: https://pypi.org/project/nerblackbox
             :alt: PyPI
         
         .. image:: https://img.shields.io/pypi/pyversions/nerblackbox
             :target: https://www.python.org/doc/versions/
@@ -40,25 +37,23 @@
         - Source Code: https://github.com/af-ai-center/nerblackbox
         - Documentation: https://af-ai-center.github.io/nerblackbox
         - PyPI: https://pypi.org/project/nerblackbox
         
         About
         =====
         
-        `Transformer-based models <https://arxiv.org/abs/1706.03762>`_ like `BERT <https://arxiv.org/abs/1810.04805>`_ have had a `game-changing impact <https://paperswithcode.com/task/language-modelling>`_ on Natural Language Processing.
+        `Transformer-based language models <https://arxiv.org/abs/1706.03762>`_ like `BERT <https://arxiv.org/abs/1810.04805>`_ have had a `game-changing impact <https://paperswithcode.com/task/language-modelling>`_ on Natural Language Processing.
         
-        In order to utilize the `publicly accessible pretrained models <https://huggingface.co/transformers/pretrained_models.html>`_ for
+        In order to utilize `Hugging Face's publicly accessible pretrained models <https://huggingface.co/transformers/pretrained_models.html>`_ for
         `Named Entity Recognition <https://en.wikipedia.org/wiki/Named-entity_recognition>`_,
         one needs to retrain (or "fine-tune") them using labeled text.
         
         **nerblackbox makes this easy.**
         
-        .. image:: https://raw.githubusercontent.com/af-ai-center/nerblackbox/master/docs/_static/nerblackbox.png
-        
-        .. .. include:: ./docs_source/source/shared/main2.rst
+        .. image:: https://raw.githubusercontent.com/af-ai-center/nerblackbox/master/docs/docs/images/nerblackbox.png
         
         You give it
         
         - a **Dataset** (labeled text)
         - a **Pretrained Model** (transformers)
         
         and you get
@@ -70,46 +65,24 @@
         ============
         
             ``pip install nerblackbox``
         
         Usage
         =====
         
-        .. .. include:: ./docs_source/source/shared/usage.rst
-        
-        Fine-tuning can be done in a few simple steps using an "experiment configuration file"
-        
-        .. code-block:: python
-        
-           # cat <experiment_name>.ini
-           dataset_name = swedish_ner_corpus
-           pretrained_model_name = af-ai-center/bert-base-swedish-uncased
-        
-        and either the Command Line Interface (CLI) or the Python API:
-        
-        .. code-block:: python
-        
-           # CLI
-           nerbb run_experiment <experiment_name>          # fine-tune
-           nerbb get_experiment_results <experiment_name>  # get results/performance
-           nerbb predict <experiment_name> <text_input>    # apply best model
-        
-           # Python API
-           nerbb = NerBlackBox()
-           nerbb.run_experiment(<experiment_name>)         # fine-tune
-           nerbb.get_experiment_results(<experiment_name>) # get results/performance
-           nerbb.predict(<experiment_name>, <text_input>)  # apply best model
+        see documentation: https://af-ai-center.github.io/nerblackbox
         
 Keywords: NLP,NER,named entity recognition,BERT,transformer,pytorch
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: Unix
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.6
```

### Comparing `nerblackbox-0.0.8/nerblackbox.egg-info/SOURCES.txt` & `nerblackbox-0.0.9/nerblackbox.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 MANIFEST.in
 README.rst
 requirements.txt
 requirements_dev.txt
 setup.cfg
 setup.py
+data/__init__.py
+dataX/__init__.py
 nerblackbox/MLproject
 nerblackbox/__about__.py
 nerblackbox/__init__.py
 nerblackbox/api.py
 nerblackbox/cli.py
 nerblackbox.egg-info/PKG-INFO
 nerblackbox.egg-info/SOURCES.txt
@@ -16,26 +18,30 @@
 nerblackbox.egg-info/not-zip-safe
 nerblackbox.egg-info/requires.txt
 nerblackbox.egg-info/top_level.txt
 nerblackbox/modules/__init__.py
 nerblackbox/modules/experiment_results.py
 nerblackbox/modules/experiments_results.py
 nerblackbox/modules/main.py
-nerblackbox/modules/data/__init__.py
 nerblackbox/modules/data/datasets/.gitignore
 nerblackbox/modules/data/experiment_configs/.gitignore
 nerblackbox/modules/data/experiment_configs/default.ini
-nerblackbox/modules/data/experiment_configs/exp_test.ini
+nerblackbox/modules/data/experiment_configs/my_experiment.ini
+nerblackbox/modules/data/experiment_configs/my_experiment_conll2003.ini
+nerblackbox/modules/data/experiment_configs/my_experiment_sic.ini
+nerblackbox/modules/data/experiment_configs/my_experiment_suc.ini
+nerblackbox/modules/data/experiment_configs/my_experiment_swedish_ner_corpus.ini
 nerblackbox/modules/data/pretrained_models/.gitignore
 nerblackbox/modules/datasets/__init__.py
 nerblackbox/modules/datasets/plots.py
 nerblackbox/modules/datasets/formatter/__init__.py
 nerblackbox/modules/datasets/formatter/auto_formatter.py
 nerblackbox/modules/datasets/formatter/base_formatter.py
 nerblackbox/modules/datasets/formatter/conll2003_formatter.py
+nerblackbox/modules/datasets/formatter/sic_formatter.py
 nerblackbox/modules/datasets/formatter/suc_formatter.py
 nerblackbox/modules/datasets/formatter/swedish_ner_corpus_formatter.py
 nerblackbox/modules/datasets/formatter/util_functions.py
 nerblackbox/modules/experiment_config/__init__.py
 nerblackbox/modules/experiment_config/experiment_config.py
 nerblackbox/modules/ner_training/__init__.py
 nerblackbox/modules/ner_training/bert_ner_single.py
```

### Comparing `nerblackbox-0.0.8/setup.py` & `nerblackbox-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 setup(
     name="nerblackbox",
     version=get_package_version("nerblackbox/__about__.py"),
     author="Felix Stollenwerk",
     author_email="felix.stollenwerk@arbetsformedlingen.se",
-    description="fine-tune transformer-based models for named entity recognition",
+    description="fine-tune transformer-based language models for named entity recognition",
     long_description=readme(),
     long_description_content_type="text/x-rst",
     keywords=[
         "NLP",
         "NER",
         "named entity recognition",
         "BERT",
@@ -69,14 +69,15 @@
     zip_safe=False,
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Development Status :: 2 - Pre-Alpha",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Operating System :: Unix",
         "Topic :: Text Processing :: Linguistic",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
     ],
```

