# Comparing `tmp/torchtnt-nightly-2023.8.3.tar.gz` & `tmp/torchtnt-nightly-2023.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchtnt-nightly-2023.8.3.tar", last modified: Thu Aug  3 11:26:33 2023, max compression
+gzip compressed data, was "torchtnt-nightly-2023.8.4.tar", last modified: Fri Aug  4 11:25:59 2023, max compression
```

## Comparing `torchtnt-nightly-2023.8.3.tar` & `torchtnt-nightly-2023.8.4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:26:33.606840 torchtnt-nightly-2023.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-08-03 11:26:33.606840 torchtnt-nightly-2023.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 11:26:33.606840 torchtnt-nightly-2023.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:26:33.570840 torchtnt-nightly-2023.8.3/torchtnt/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:26:33.578840 torchtnt-nightly-2023.8.3/torchtnt/framework/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/framework/_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/framework/_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    37488 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/framework/auto_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/framework/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:26:33.586840 torchtnt-nightly-2023.8.3/torchtnt/framework/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/framework/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/framework/callbacks/base_csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/framework/callbacks/garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/framework/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/framework/callbacks/learning_rate_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/framework/callbacks/module_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/framework/callbacks/pytorch_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/framework/callbacks/system_resources_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15752 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/framework/callbacks/torchsnapshot_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/framework/callbacks/tqdm_progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/framework/callbacks/train_progress_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/framework/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/framework/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/framework/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/framework/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/framework/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    16174 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/framework/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:26:33.598840 torchtnt-nightly-2023.8.3/torchtnt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:26:33.598840 torchtnt-nightly-2023.8.3/torchtnt/utils/data/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/data/data_prefetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/data/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/data/multi_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/data/profile_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    19008 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/early_stop_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/flops.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/fsspec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:26:33.606840 torchtnt-nightly-2023.8.3/torchtnt/utils/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/loggers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/loggers/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/loggers/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/loggers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/loggers/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/loggers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27731 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/module_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/oom.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/prepare_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/rank_zero_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/stateful.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-08-03 11:23:07.000000 torchtnt-nightly-2023.8.3/torchtnt/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:26:33.606840 torchtnt-nightly-2023.8.3/torchtnt_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-08-03 11:26:33.000000 torchtnt-nightly-2023.8.3/torchtnt_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-08-03 11:26:33.000000 torchtnt-nightly-2023.8.3/torchtnt_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:26:33.000000 torchtnt-nightly-2023.8.3/torchtnt_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-03 11:26:33.000000 torchtnt-nightly-2023.8.3/torchtnt_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 11:26:33.000000 torchtnt-nightly-2023.8.3/torchtnt_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:26:33.000000 torchtnt-nightly-2023.8.3/torchtnt_nightly.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:25:59.196450 torchtnt-nightly-2023.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-08-04 11:25:59.196450 torchtnt-nightly-2023.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 11:25:59.196450 torchtnt-nightly-2023.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:25:59.168450 torchtnt-nightly-2023.8.4/torchtnt/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:25:59.172450 torchtnt-nightly-2023.8.4/torchtnt/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37488 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/auto_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:25:59.176450 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/base_csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/learning_rate_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/module_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/pytorch_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/system_resources_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15752 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/torchsnapshot_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/tqdm_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/train_progress_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16174 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:25:59.188450 torchtnt-nightly-2023.8.4/torchtnt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:25:59.192450 torchtnt-nightly-2023.8.4/torchtnt/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/data/data_prefetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/data/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/data/multi_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/data/profile_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19008 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/early_stop_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/flops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/fsspec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:25:59.192450 torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27731 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/module_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/oom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/prepare_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/rank_zero_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:25:59.196450 torchtnt-nightly-2023.8.4/torchtnt_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-08-04 11:25:59.000000 torchtnt-nightly-2023.8.4/torchtnt_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-08-04 11:25:59.000000 torchtnt-nightly-2023.8.4/torchtnt_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 11:25:59.000000 torchtnt-nightly-2023.8.4/torchtnt_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-04 11:25:59.000000 torchtnt-nightly-2023.8.4/torchtnt_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-04 11:25:59.000000 torchtnt-nightly-2023.8.4/torchtnt_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 11:25:59.000000 torchtnt-nightly-2023.8.4/torchtnt_nightly.egg-info/zip-safe
```

### Comparing `torchtnt-nightly-2023.8.3/LICENSE` & `torchtnt-nightly-2023.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/PKG-INFO` & `torchtnt-nightly-2023.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt-nightly
-Version: 2023.8.3
+Version: 2023.8.4
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.8.3 Summary: A
+Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.8.4 Summary: A
 lightweight library for PyTorch training tools and utilities Home-page: https:/
 /github.com/pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com
 License: BSD-3 Keywords: pytorch,torch,training,tools,utilities Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
```

### Comparing `torchtnt-nightly-2023.8.3/README.md` & `torchtnt-nightly-2023.8.4/README.md`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/setup.py` & `torchtnt-nightly-2023.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/framework/__init__.py` & `torchtnt-nightly-2023.8.4/torchtnt/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/framework/_callback_handler.py` & `torchtnt-nightly-2023.8.4/torchtnt/framework/_callback_handler.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/framework/_test_utils.py` & `torchtnt-nightly-2023.8.4/torchtnt/framework/_test_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/framework/auto_unit.py` & `torchtnt-nightly-2023.8.4/torchtnt/framework/auto_unit.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/framework/callback.py` & `torchtnt-nightly-2023.8.4/torchtnt/framework/callback.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/framework/callbacks/__init__.py` & `torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/framework/callbacks/base_csv_writer.py` & `torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/base_csv_writer.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/framework/callbacks/garbage_collector.py` & `torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/framework/callbacks/lambda_callback.py` & `torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/framework/callbacks/learning_rate_monitor.py` & `torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/learning_rate_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/framework/callbacks/module_summary.py` & `torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/module_summary.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/framework/callbacks/pytorch_profiler.py` & `torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/pytorch_profiler.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/framework/callbacks/system_resources_monitor.py` & `torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/system_resources_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py` & `torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/framework/callbacks/torchsnapshot_saver.py` & `torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/torchsnapshot_saver.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/framework/callbacks/tqdm_progress_bar.py` & `torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/tqdm_progress_bar.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/framework/callbacks/train_progress_monitor.py` & `torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/train_progress_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/framework/evaluate.py` & `torchtnt-nightly-2023.8.4/torchtnt/framework/evaluate.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/framework/fit.py` & `torchtnt-nightly-2023.8.4/torchtnt/framework/fit.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/framework/predict.py` & `torchtnt-nightly-2023.8.4/torchtnt/framework/predict.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/framework/state.py` & `torchtnt-nightly-2023.8.4/torchtnt/framework/state.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/framework/train.py` & `torchtnt-nightly-2023.8.4/torchtnt/framework/train.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/framework/unit.py` & `torchtnt-nightly-2023.8.4/torchtnt/framework/unit.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/framework/utils.py` & `torchtnt-nightly-2023.8.4/torchtnt/framework/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,31 +10,21 @@
 import logging
 from contextlib import contextmanager
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 import typing_extensions
-from torch.distributed.fsdp import (
-    FullyShardedDataParallel,
-    FullyShardedDataParallel as FSDP,
-)
 from torch.profiler import record_function
-from torchtnt.utils.version import is_torch_version_geq_2_0
-
-if is_torch_version_geq_2_0():
-    from torch.distributed._composable_state import _get_module_state
-    from torch.distributed.fsdp._common_utils import _FSDPState
-
 from torchtnt.framework.state import State
 from torchtnt.framework.unit import AppStateMixin
 from torchtnt.utils.lr_scheduler import TLRScheduler
+from torchtnt.utils.prepare_module import _is_fsdp_module, FSDPOptimizerWrapper
 from torchtnt.utils.progress import Progress
 
-
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 # Helper functions common across the loops
 def _is_done(
     progress: Progress, max_epochs: Optional[int], max_steps: Optional[int]
 ) -> bool:
@@ -128,86 +118,49 @@
             f"Expected step function to have an annotated argument named ``data``. Found {annotations}."
         )
         return False
     annotated_type = annotations["data"]
     return typing_extensions.get_origin(annotated_type) is collections.abc.Iterator
 
 
-def _is_fsdp_module(module: torch.nn.Module) -> bool:
-    if isinstance(module, FSDP):
-        return True
-
-    if is_torch_version_geq_2_0():
-        # Also check for composable FSDP API
-        maybe_composable_state = _get_module_state(module)
-        if maybe_composable_state is not None:
-            return isinstance(maybe_composable_state, _FSDPState)
-
-    return False
-
-
-class _FSDPOptimizerWrapper:
-    """
-    Wrapper for FSDP optimizer to call specific FSDP optimizer state checkpointing APIs.
-    """
-
-    def __init__(
-        self, module: torch.nn.Module, optimizer: torch.optim.Optimizer
-    ) -> None:
-        self.module = module
-        self.optimizer = optimizer
-
-    def state_dict(self) -> Dict[str, Any]:
-        optim_state_dict = FullyShardedDataParallel.optim_state_dict(
-            self.module, self.optimizer
-        )
-        return optim_state_dict
-
-    def load_state_dict(self, state_dict: Dict[str, Any]) -> None:
-        optim_state_dict = FullyShardedDataParallel.optim_state_dict_to_load(
-            self.module, self.optimizer, state_dict
-        )
-        self.optimizer.load_state_dict(optim_state_dict)
-
-
 def _construct_tracked_optimizers(
     unit: AppStateMixin,
-) -> Dict[str, Union[torch.optim.Optimizer, _FSDPOptimizerWrapper]]:
+) -> Dict[str, Union[torch.optim.Optimizer, FSDPOptimizerWrapper]]:
     """
-    Constructs tracked optimizers. Handles optimizers working on FSDP modules, wrapping them in _FSDPOptimizerWrapper.
+    Constructs tracked optimizers. Handles optimizers working on FSDP modules, wrapping them in FSDPOptimizerWrapper.
     """
-    fsdp_tracked_optimizers: Dict[str, _FSDPOptimizerWrapper] = {}
+    fsdp_tracked_optimizers: Dict[str, FSDPOptimizerWrapper] = {}
     for module in unit.tracked_modules().values():
         if _is_fsdp_module(module):
             # find optimizers for module, if exists
             optimizer_list = _find_optimizers_for_module(
                 module, unit.tracked_optimizers()
             )
             for optim_name, optimizer in optimizer_list:
-                fsdp_tracked_optimizers[optim_name] = _FSDPOptimizerWrapper(
+                fsdp_tracked_optimizers[optim_name] = FSDPOptimizerWrapper(
                     module, optimizer
                 )
 
     # construct custom tracked optimizers with FSDP optimizers
     tracked_optimizers: Dict[
-        str, Union[torch.optim.Optimizer, _FSDPOptimizerWrapper]
+        str, Union[torch.optim.Optimizer, FSDPOptimizerWrapper]
     ] = {
         key: value
         for key, value in unit.tracked_optimizers().items()
         if key not in fsdp_tracked_optimizers
     }
     tracked_optimizers.update(fsdp_tracked_optimizers)
     return tracked_optimizers
 
 
 def _construct_tracked_optimizers_and_schedulers(
     unit: AppStateMixin,
-) -> Dict[str, Union[torch.optim.Optimizer, _FSDPOptimizerWrapper, TLRScheduler]]:
+) -> Dict[str, Union[torch.optim.Optimizer, FSDPOptimizerWrapper, TLRScheduler]]:
     """
-    Combines tracked optimizers and schedulers. Handles optimizers working on FSDP modules, wrapping them in _FSDPOptimizerWrapper.
+    Combines tracked optimizers and schedulers. Handles optimizers working on FSDP modules, wrapping them in FSDPOptimizerWrapper.
     """
     # construct custom tracked optimizers with FSDP optimizers
     tracked_optimizers_and_schedulers = _construct_tracked_optimizers(unit)
 
     # add schedulers
     for lr_scheduler_attrib_name, lr_scheduler in unit.tracked_lr_schedulers().items():
         if lr_scheduler_attrib_name in tracked_optimizers_and_schedulers:
```

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/__init__.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     rank_zero_debug,
     rank_zero_error,
     rank_zero_info,
     rank_zero_print,
     rank_zero_warn,
 )
 from .stateful import Stateful
-from .timer import FullSyncPeriodicTimer, get_timer_summary, Timer
+from .timer import FullSyncPeriodicTimer, get_timer_summary, log_elapsed_time, Timer
 from .tqdm import close_progress_bar, create_progress_bar, update_progress_bar
 from .version import (
     get_python_version,
     get_torch_version,
     is_torch_version_ge_1_13_1,
     is_torch_version_geq_1_10,
     is_torch_version_geq_1_11,
@@ -113,14 +113,15 @@
     "rank_zero_error",
     "rank_zero_info",
     "rank_zero_print",
     "rank_zero_warn",
     "Stateful",
     "FullSyncPeriodicTimer",
     "get_timer_summary",
+    "log_elapsed_time",
     "transfer_batch_norm_stats",
     "transfer_weights",
     "get_module_summary",
     "get_summary_table",
     "ModuleSummary",
     "prune_module_summary",
     "Timer",
```

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/data/__init__.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/data/data_prefetcher.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/data/data_prefetcher.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/data/iterators.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/data/iterators.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/data/multi_dataloader.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/data/multi_dataloader.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/data/profile_dataloader.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/data/profile_dataloader.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/device.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/device.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/distributed.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/early_stop_checker.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/early_stop_checker.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/env.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/env.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/flops.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/flops.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/fsspec.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/fsspec.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/loggers/__init__.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/loggers/csv.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/csv.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/loggers/file.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/file.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/loggers/in_memory.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/in_memory.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/loggers/json.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/json.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/loggers/logger.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/loggers/tensorboard.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/loggers/utils.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/memory.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/memory.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/misc.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/misc.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/module_summary.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/module_summary.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/oom.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/oom.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/prepare_module.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/prepare_module.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 from dataclasses import asdict, dataclass
-from typing import Callable, Iterable, Optional, Union
+from typing import Any, Callable, Dict, Iterable, Optional, Union
 
 import torch
 import torch.distributed as dist
 from torch.distributed import ProcessGroup
 from torch.distributed.fsdp import FullyShardedDataParallel as FSDP, StateDictType
 from torch.distributed.fsdp.api import OptimStateDictConfig, StateDictConfig
 from torch.distributed.fsdp.fully_sharded_data_parallel import (
     BackwardPrefetch,
     CPUOffload,
     MixedPrecision,
     ShardingStrategy,
 )
 from torch.nn.parallel import DistributedDataParallel as DDP
 from torchtnt.utils.rank_zero_log import rank_zero_warn
-from torchtnt.utils.version import is_torch_version_geq_1_12
+from torchtnt.utils.version import is_torch_version_geq_1_12, is_torch_version_geq_2_0
+
+if is_torch_version_geq_2_0():
+    from torch.distributed._composable_state import _get_module_state
+    from torch.distributed.fsdp._common_utils import _FSDPState
 
 
 @dataclass
 class Strategy:
     """Dataclass representing a parallelization strategy"""
 
     pass
@@ -177,7 +181,42 @@
     )
 
     if state_dict_type:
         FSDP.set_state_dict_type(
             module, state_dict_type, state_dict_config, optim_state_dict_config
         )
     return module
+
+
+class FSDPOptimizerWrapper:
+    """
+    Wrapper for FSDP optimizer to call specific FSDP optimizer state checkpointing APIs.
+    """
+
+    def __init__(
+        self, module: torch.nn.Module, optimizer: torch.optim.Optimizer
+    ) -> None:
+        self.module = module
+        self.optimizer = optimizer
+
+    def state_dict(self) -> Dict[str, Any]:
+        optim_state_dict = FSDP.optim_state_dict(self.module, self.optimizer)
+        return optim_state_dict
+
+    def load_state_dict(self, state_dict: Dict[str, Any]) -> None:
+        optim_state_dict = FSDP.optim_state_dict_to_load(
+            self.module, self.optimizer, state_dict
+        )
+        self.optimizer.load_state_dict(optim_state_dict)
+
+
+def _is_fsdp_module(module: torch.nn.Module) -> bool:
+    if isinstance(module, FSDP):
+        return True
+
+    if is_torch_version_geq_2_0():
+        # Also check for composable FSDP API
+        maybe_composable_state = _get_module_state(module)
+        if maybe_composable_state is not None:
+            return isinstance(maybe_composable_state, _FSDPState)
+
+    return False
```

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/progress.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/progress.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/rank_zero_log.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/rank_zero_log.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/stateful.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/stateful.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/test_utils.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/timer.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/timer.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,19 +29,50 @@
 import torch.distributed as dist
 from torchtnt.utils.distributed import PGWrapper
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 AsyncOperator = TypeVar("AsyncOperator")
 
+logger: logging.Logger = logging.getLogger(__name__)
 
 _TABLE_ROW = Tuple[str, float, int, float, float]
 _TABLE_DATA = List[_TABLE_ROW]
 
 
+@contextmanager
+def log_elapsed_time(
+    action_name: str, *, cuda_sync: Optional[bool] = None
+) -> Generator[None, None, None]:
+    """Utility to measure and log elapsed time for a given event.
+
+    Args:
+        action_name: the name of the event being timed.
+        cuda_sync: Whether to synchronize the stream in order to measure the most accurate timings on CUDA. Defaults to True if CUDA is available.
+
+    Raises:
+        ValueError: If cuda_sync is set to True but CUDA is not available.
+    """
+    if cuda_sync and not torch.cuda.is_available():
+        raise ValueError(
+            "CUDA must be available in order to enable CUDA synchronization."
+        )
+    cuda_sync = cuda_sync if cuda_sync is not None else torch.cuda.is_available()
+    try:
+        if cuda_sync:
+            torch.cuda.synchronize()
+        start_time: float = perf_counter()
+        yield
+    finally:
+        if cuda_sync:
+            torch.cuda.synchronize()
+        interval_time: float = perf_counter() - start_time
+        logger.info(f"{action_name} took {interval_time} seconds")
+
+
 @runtime_checkable
 class TimerProtocol(Protocol):
     """
     Defines a Timer Protocol with `time` and `reset` methods and an attribute `recorded_durations` for storing timings.
     """
 
     recorded_durations: Dict[str, List[float]]
```

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/tqdm.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/tqdm.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt/utils/version.py` & `torchtnt-nightly-2023.8.4/torchtnt/utils/version.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.3/torchtnt_nightly.egg-info/PKG-INFO` & `torchtnt-nightly-2023.8.4/torchtnt_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt-nightly
-Version: 2023.8.3
+Version: 2023.8.4
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.8.3 Summary: A
+Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.8.4 Summary: A
 lightweight library for PyTorch training tools and utilities Home-page: https:/
 /github.com/pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com
 License: BSD-3 Keywords: pytorch,torch,training,tools,utilities Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
```

### Comparing `torchtnt-nightly-2023.8.3/torchtnt_nightly.egg-info/SOURCES.txt` & `torchtnt-nightly-2023.8.4/torchtnt_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

