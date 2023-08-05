# Comparing `tmp/starwhale-0.5.8.tar.gz` & `tmp/starwhale-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/starwhale-0.5.8.tar", last modified: Wed Jul 26 02:29:34 2023, max compression
+gzip compressed data, was "dist/starwhale-0.5.9.tar", last modified: Mon Jul 31 09:40:17 2023, max compression
```

## Comparing `starwhale-0.5.8.tar` & `starwhale-0.5.9.tar`

### file list

```diff
@@ -1,365 +1,365 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)    20812 2023-07-26 02:29:34.000000 starwhale-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-26 02:18:02.000000 starwhale-0.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-26 02:18:02.000000 starwhale-0.5.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5507 2023-07-26 02:18:02.000000 starwhale-0.5.8/scripts/sw-docker-entrypoint
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 02:29:34.000000 starwhale-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-26 02:18:02.000000 starwhale-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/api/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62504 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/_impl/data_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/api/_impl/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/_impl/dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/api/_impl/dataset/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/_impl/dataset/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/_impl/dataset/builder/mapping_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    13378 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/_impl/dataset/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    51602 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/_impl/dataset/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23177 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/_impl/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/_impl/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12199 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/_impl/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/_impl/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/_impl/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/_impl/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/api/_impl/track/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/_impl/track/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/_impl/track/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/_impl/track/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/_impl/track/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/_impl/track/hooker.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/_impl/track/syncer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19566 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/_impl/track/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/_impl/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/job.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/api/track.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/base/blob/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/base/blob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/base/blob/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/base/blob/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     9138 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/base/bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/base/bundle_copy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/base/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/base/cloud_blob_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/base/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/base/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/base/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/base/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/base/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/base/scheduler/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/base/scheduler/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/base/scheduler/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/base/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/base/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/base/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/base/uri/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/base/uri/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/base/uri/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/base/uri/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/base/uri/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/base/uri/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/base/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/cli/assistance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/cli/assistance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/cli/assistance/broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/cli/assistance/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/cli/assistance/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/cli/assistance/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/cli/assistance/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/cli/assistance/wait_console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/cli/board/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/cli/board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/cli/board/board.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/cli/board/project_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/cli/board/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/cli/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/cli/mngt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/consts/
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/consts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/consts/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/core/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23117 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/dataset/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/dataset/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)    15479 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/dataset/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23851 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/dataset/store.py
--rw-r--r--   0 runner    (1001) docker     (123)    21237 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/dataset/tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)    31788 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/dataset/type.py
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/dataset/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/core/instance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/instance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/instance/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/instance/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/core/job/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/job/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/job/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/job/store.py
--rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/job/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/core/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23670 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/model/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/model/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)    33266 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/model/store.py
--rw-r--r--   0 runner    (1001) docker     (123)    16712 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/model/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/core/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/project/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/project/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/project/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/core/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25082 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/runtime/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    78089 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/runtime/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/runtime/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/runtime/store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/core/runtime/template/
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/runtime/template/Dockerfile.tmpl
--rw-r--r--   0 runner    (1001) docker     (123)    16244 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/runtime/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/core/track/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/core/track/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/integrations/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/integrations/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/integrations/huggingface/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/integrations/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/integrations/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/integrations/pytorch/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/integrations/pytorch/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/integrations/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/integrations/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/integrations/tensorflow/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/mngt/
--rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/mngt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/proto_gen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/proto_gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/proto_gen/model_package_storage_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/utils/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/utils/dict_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/utils/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/utils/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    26882 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/utils/venv.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/utils/venv_pack.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/web/data_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/web/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/web/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/web/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/web/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/web/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/web/ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale/web/ui/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/BlockLabel-cddc2b81.js
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/CarouselItem.svelte_svelte_type_style_lang-08c76e7c.js
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/Column-07457f7d.js
--rw-r--r--   0 runner    (1001) docker     (123)    55885 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/DatasetForm-aac5cbbf.js
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/File-15836fc4.js
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/Image-aea3de20.js
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/Image2-1419ace7.js
--rw-r--r--   0 runner    (1001) docker     (123)   222410 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/LogViewer-b5684b3d.css
--rw-r--r--   0 runner    (1001) docker     (123)   182906 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/LogViewer-f5bb7317.js
--rw-r--r--   0 runner    (1001) docker     (123)    22837 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/Markdown-d8dda0b2.css
--rw-r--r--   0 runner    (1001) docker     (123)   110084 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/Markdown-fdfce605.js
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/Model3D-fba04936.js
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/ModifyUpload-768fe082.js
--rw-r--r--   0 runner    (1001) docker     (123)    36920 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/RedHatDisplay-Bold-44214a55.woff
--rw-r--r--   0 runner    (1001) docker     (123)    29045 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/RedHatDisplay-Bold-ca18645c.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    36532 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/RedHatDisplay-Medium-6ccf2158.woff
--rw-r--r--   0 runner    (1001) docker     (123)    28661 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/RedHatDisplay-Medium-6d3ccc0f.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    36432 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/RedHatDisplay-Regular-1b99a560.woff
--rw-r--r--   0 runner    (1001) docker     (123)    28745 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/RedHatDisplay-Regular-e6fb83d9.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    26372 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/RedHatDisplay-updated-Bold-66d1fc26.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    26532 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/RedHatDisplay-updated-Medium-da0621a9.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    25736 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/RedHatDisplay-updated-Regular-d0b90ff3.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    32012 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/RedHatDisplayVF-updated-ItalicModified-8483eece.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    30784 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/RedHatDisplayVFModified-updated-3a6592a3.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    20932 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/RedHatMono-updated-Regular-1686cd5c.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    29148 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/RedHatMonoVF-updated-4cca9c27.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    32496 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/RedHatMonoVF-updated-Italic-ca135ebd.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    37096 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/RedHatText-Medium-702e86ff.woff
--rw-r--r--   0 runner    (1001) docker     (123)    29049 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/RedHatText-Medium-eb14b046.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    28169 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/RedHatText-Regular-542423d0.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    35980 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/RedHatText-Regular-df36d7d0.woff
--rw-r--r--   0 runner    (1001) docker     (123)    26632 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/RedHatText-updated-Medium-721ddd64.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    25768 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/RedHatText-updated-Regular-2e08dbe8.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    31952 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/RedHatTextVF-updated-ItalicModified-9e1c1004.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    30092 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/RedHatTextVFModified-updated-942d38f7.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/RobotoMono-Regular-5c4ca672.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/Tabs-fc1af0f2.js
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/Upload-0cd7f439.js
--rw-r--r--   0 runner    (1001) docker     (123)    52083 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/Webcam-37a04310.js
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/_commonjsHelpers-23156833.js
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/account2-668f906e.svg
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/bg-1920x1080-8b0d8feb.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/bg-2560x1440-c97cffa5.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/bg-3840x2160-f974f4b1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/color-07ebf074.js
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/csv-17a3ae92.js
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/dsv-62f8cd07.js
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/empty-chart-1e62901a.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/empty-f3091520.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/google-9d1a8b2b.svg
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/iconfont-0a880318.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/iconfont-10b60b11.ttf
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/iconfont-4c4e9d6d.woff
--rw-r--r--   0 runner    (1001) docker     (123)  3421636 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index-3bbbd54b.js
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index-4b525ef6.css
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index-890d4a46.js
--rw-r--r--   0 runner    (1001) docker     (123)  3727911 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index-af425f4b.js
--rw-r--r--   0 runner    (1001) docker     (123)    49490 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index-ddbcf299.css
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index10-4d13164f.js
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index11-13eb176d.js
--rw-r--r--   0 runner    (1001) docker     (123)    21036 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index12-de21ca8a.js
--rw-r--r--   0 runner    (1001) docker     (123)    18562 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index13-0661cc45.js
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index14-e2afac41.js
--rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index15-9ee1eee9.js
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index16-a0351c35.js
--rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index17-a75792cc.js
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index18-0b10ab02.js
--rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index19-ceded876.js
--rw-r--r--   0 runner    (1001) docker     (123)    33614 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index2-d042f67b.js
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index20-d0bcc869.js
--rw-r--r--   0 runner    (1001) docker     (123)    40205 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index21-d2f402e4.js
--rw-r--r--   0 runner    (1001) docker     (123)    17932 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index22-c5e0b0dd.js
--rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index23-e492630c.js
--rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index24-1c64b765.js
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index25-33571440.js
--rw-r--r--   0 runner    (1001) docker     (123)  3544383 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index26-d78d751e.js
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index27-18127a28.js
--rw-r--r--   0 runner    (1001) docker     (123)  4615279 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index28-34a5ed1a.js
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index29-e4ca565e.js
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index3-b8136165.js
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index30-334d010c.js
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index31-1121988e.js
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index32-80223294.js
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index33-a4713f90.js
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index34-69d671c0.js
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index35-91b6f450.js
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index36-6ce81ba8.js
--rw-r--r--   0 runner    (1001) docker     (123)    18675 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index37-f530c08a.js
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index38-fc6af5aa.js
--rw-r--r--   0 runner    (1001) docker     (123)    17339 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index39-671ded20.js
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index4-d076a84c.js
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index5-529df1c0.js
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index6-be007bee.js
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index7-c3badb00.js
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index8-2bbdfede.js
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/index9-0cbe1428.js
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/invalid-file-82d62dec.svg
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/left-8c88a49a.svg
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/left-shadow-e0fdfe32.png
--rw-r--r--   0 runner    (1001) docker     (123)    23111 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/linear-8d973619.js
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/logo_normal_en_blue-18b013e7.png
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/logo_normal_en_gray-163de1a0.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/logo_normal_en_white-ec11283c.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/logo_small_en_white-782559aa.svg
--rw-r--r--   0 runner    (1001) docker     (123)   117896 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/main-99f2bbfd.js
--rw-r--r--   0 runner    (1001) docker     (123)    94147 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/module-ddaca3b9.js
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/module2-74df381a.js
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/module3-49e9a615.js
--rw-r--r--   0 runner    (1001) docker     (123)    42104 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-bold-452a631f.woff
--rw-r--r--   0 runner    (1001) docker     (123)    34752 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-bold-5c4ed5bb.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    37252 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-bold-italic-16cda7ef.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    45068 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-bold-italic-4926428e.woff
--rw-r--r--   0 runner    (1001) docker     (123)    41368 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-extrabold-613313c8.woff
--rw-r--r--   0 runner    (1001) docker     (123)    33808 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-extrabold-648ba0e7.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    44392 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-extrabold-italic-33533562.woff
--rw-r--r--   0 runner    (1001) docker     (123)    36660 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-extrabold-italic-a258578a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    42532 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-extralight-64fbbd3d.woff
--rw-r--r--   0 runner    (1001) docker     (123)    35056 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-extralight-f053be7c.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    44668 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-extralight-italic-6cbe5597.woff
--rw-r--r--   0 runner    (1001) docker     (123)    36800 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-extralight-italic-d23afde2.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    35640 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-heavy-5e0869ee.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    43316 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-heavy-c7e67c68.woff
--rw-r--r--   0 runner    (1001) docker     (123)    37972 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-heavy-italic-8f5fbf20.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    45720 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-heavy-italic-c702fef1.woff
--rw-r--r--   0 runner    (1001) docker     (123)    37368 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-italic-34df3d81.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    45240 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-italic-b81a6146.woff
--rw-r--r--   0 runner    (1001) docker     (123)    41936 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-light-3f8151f4.woff
--rw-r--r--   0 runner    (1001) docker     (123)    34472 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-light-9db6ab0a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    44372 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-light-italic-a1454ca5.woff
--rw-r--r--   0 runner    (1001) docker     (123)    36580 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-light-italic-ec333948.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    51572 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-mono-bold-2bf715ff.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    65060 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-mono-bold-9b29c79a.woff
--rw-r--r--   0 runner    (1001) docker     (123)    50112 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-mono-light-5bae063c.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    63324 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-mono-light-7fbe3706.woff
--rw-r--r--   0 runner    (1001) docker     (123)    65036 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-mono-regular-95881615.woff
--rw-r--r--   0 runner    (1001) docker     (123)    51524 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-mono-regular-a13dec50.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    64944 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-mono-semibold-085fb4a8.woff
--rw-r--r--   0 runner    (1001) docker     (123)    51308 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-mono-semibold-b39c5174.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    42584 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-regular-16b63547.woff
--rw-r--r--   0 runner    (1001) docker     (123)    35128 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-regular-8e2261df.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    33416 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-semibold-3d06895e.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    40620 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-semibold-ec5809e8.woff
--rw-r--r--   0 runner    (1001) docker     (123)    44728 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-semibold-italic-1935eb14.woff
--rw-r--r--   0 runner    (1001) docker     (123)    36904 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-semibold-italic-ae706d8c.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    40860 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-thin-6feca5dc.woff
--rw-r--r--   0 runner    (1001) docker     (123)    33696 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-thin-e85966f1.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    43504 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-thin-italic-2dffa092.woff
--rw-r--r--   0 runner    (1001) docker     (123)    35900 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/overpass-thin-italic-44db8e3d.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   276435 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/pfbg_2000-1f17de55.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    67491 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/pfbg_576-1d76d6cc.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   195594 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/pfbg_576@2x-4942ea78.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   116699 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/pfbg_768-8bc3cc8a.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   362032 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/pfbg_768@2x-037bce76.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   588571 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/pfbg_992@2x-9dfd9687.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/pficon-0a333dac.woff
--rw-r--r--   0 runner    (1001) docker     (123)    17700 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/pficon-86c74539.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/project-863f66b0.svg
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/right-aefe3c24.svg
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/right-shadow-58dd9abc.png
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/search-empty-13cbde15.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/setting-6d098443.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/status-icon-sprite-bc89cb14.svg
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/utils-de54785e.js
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/web-vitals-d4fac006.js
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/assets/wechat-cffee157.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-26 02:29:21.000000 starwhale-0.5.8/starwhale/web/ui/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-26 02:29:21.000000 starwhale-0.5.8/starwhale/web/ui/favicon_white.ico
--rw-r--r--   0 runner    (1001) docker     (123)    25155 2023-07-26 02:29:21.000000 starwhale-0.5.8/starwhale/web/ui/iconfont.js
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    45679 2023-07-26 02:29:32.000000 starwhale-0.5.8/starwhale/web/ui/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-26 02:29:21.000000 starwhale-0.5.8/starwhale/web/ui/robots.txt
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-26 02:18:02.000000 starwhale-0.5.8/starwhale/web/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20812 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13372 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 02:19:11.000000 starwhale-0.5.8/starwhale.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 02:29:34.000000 starwhale-0.5.8/starwhale.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    20812 2023-07-31 09:40:17.000000 starwhale-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-31 09:31:23.000000 starwhale-0.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-31 09:31:23.000000 starwhale-0.5.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5507 2023-07-31 09:31:23.000000 starwhale-0.5.9/scripts/sw-docker-entrypoint
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 09:40:17.000000 starwhale-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-31 09:31:23.000000 starwhale-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/api/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62504 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/_impl/data_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/api/_impl/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/_impl/dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/api/_impl/dataset/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/_impl/dataset/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/_impl/dataset/builder/mapping_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13378 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/_impl/dataset/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54921 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/_impl/dataset/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23368 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/_impl/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/_impl/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/_impl/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/_impl/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/_impl/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/_impl/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/api/_impl/track/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/_impl/track/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/_impl/track/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/_impl/track/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/_impl/track/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/_impl/track/hooker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/_impl/track/syncer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19566 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/_impl/track/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/_impl/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/api/track.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/base/blob/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/base/blob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/base/blob/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/base/blob/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9138 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/base/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/base/bundle_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/base/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/base/cloud_blob_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/base/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/base/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/base/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/base/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/base/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/base/scheduler/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/base/scheduler/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/base/scheduler/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/base/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/base/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/base/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/base/uri/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/base/uri/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/base/uri/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/base/uri/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/base/uri/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/base/uri/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/base/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/cli/assistance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/cli/assistance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/cli/assistance/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/cli/assistance/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/cli/assistance/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/cli/assistance/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/cli/assistance/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/cli/assistance/wait_console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/cli/board/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/cli/board/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/cli/board/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/cli/board/project_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/cli/board/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/cli/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/cli/mngt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/consts/
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/consts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/consts/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/core/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23117 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/dataset/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/dataset/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15479 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/dataset/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23851 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/dataset/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21237 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/dataset/tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31788 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/dataset/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/dataset/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/core/instance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/instance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/instance/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/instance/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/core/job/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/job/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/job/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/job/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/job/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/core/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24038 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/model/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/model/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33266 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/model/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16712 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/model/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/core/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/project/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/project/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/project/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/core/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25040 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/runtime/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78166 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/runtime/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/runtime/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/runtime/store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/core/runtime/template/
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/runtime/template/Dockerfile.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)    16244 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/runtime/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/core/track/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/core/track/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/integrations/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/integrations/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/integrations/huggingface/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/integrations/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/integrations/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/integrations/pytorch/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/integrations/pytorch/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/integrations/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/integrations/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/integrations/tensorflow/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/mngt/
+-rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/mngt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/proto_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/proto_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/proto_gen/model_package_storage_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/utils/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/utils/dict_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/utils/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/utils/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26882 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/utils/venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/utils/venv_pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/web/data_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/web/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/web/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/web/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/web/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/web/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/web/ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale/web/ui/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/BlockLabel-10abb1b4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/CarouselItem.svelte_svelte_type_style_lang-4dd9c624.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/Column-a843ed59.js
+-rw-r--r--   0 runner    (1001) docker     (123)    55885 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/DatasetForm-6dd7af50.js
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/File-220c5e21.js
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/Image-2df538c6.js
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/Image2-bbb64300.js
+-rw-r--r--   0 runner    (1001) docker     (123)   222410 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/LogViewer-b5684b3d.css
+-rw-r--r--   0 runner    (1001) docker     (123)   182906 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/LogViewer-e1f101c5.js
+-rw-r--r--   0 runner    (1001) docker     (123)   110084 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/Markdown-2b316973.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22837 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/Markdown-d8dda0b2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/Model3D-d49eae09.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/ModifyUpload-e3ca444a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36920 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/RedHatDisplay-Bold-44214a55.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    29045 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/RedHatDisplay-Bold-ca18645c.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    36532 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/RedHatDisplay-Medium-6ccf2158.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    28661 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/RedHatDisplay-Medium-6d3ccc0f.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    36432 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/RedHatDisplay-Regular-1b99a560.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    28745 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/RedHatDisplay-Regular-e6fb83d9.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    26372 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/RedHatDisplay-updated-Bold-66d1fc26.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    26532 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/RedHatDisplay-updated-Medium-da0621a9.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    25736 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/RedHatDisplay-updated-Regular-d0b90ff3.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    32012 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/RedHatDisplayVF-updated-ItalicModified-8483eece.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    30784 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/RedHatDisplayVFModified-updated-3a6592a3.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    20932 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/RedHatMono-updated-Regular-1686cd5c.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    29148 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/RedHatMonoVF-updated-4cca9c27.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    32496 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/RedHatMonoVF-updated-Italic-ca135ebd.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    37096 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/RedHatText-Medium-702e86ff.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    29049 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/RedHatText-Medium-eb14b046.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    28169 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/RedHatText-Regular-542423d0.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    35980 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/RedHatText-Regular-df36d7d0.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    26632 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/RedHatText-updated-Medium-721ddd64.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    25768 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/RedHatText-updated-Regular-2e08dbe8.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    31952 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/RedHatTextVF-updated-ItalicModified-9e1c1004.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    30092 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/RedHatTextVFModified-updated-942d38f7.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/RobotoMono-Regular-5c4ca672.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/Tabs-6664f57a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/Upload-6d14b4a6.js
+-rw-r--r--   0 runner    (1001) docker     (123)    52083 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/Webcam-d64f2534.js
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/_commonjsHelpers-23156833.js
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/account2-668f906e.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/bg-1920x1080-8b0d8feb.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/bg-2560x1440-c97cffa5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/bg-3840x2160-f974f4b1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/color-2fcdd2a9.js
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/csv-17a3ae92.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/dsv-62f8cd07.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/empty-chart-1e62901a.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/empty-f3091520.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/google-9d1a8b2b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/iconfont-0a880318.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/iconfont-10b60b11.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/iconfont-4c4e9d6d.woff
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index-4b525ef6.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index-87b297cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)    49490 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index-ddbcf299.css
+-rw-r--r--   0 runner    (1001) docker     (123)  3421639 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index-df1fb029.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3727911 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index-e17166cd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index10-7aed280d.js
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index11-df7b8b7d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21036 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index12-f581388d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18562 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index13-fd2d632d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index14-94c12d28.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index15-a31493a5.js
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index16-2b049823.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index17-d4811bf1.js
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index18-d4ad6d1d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index19-18249feb.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33614 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index2-667148f0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index20-0cc28676.js
+-rw-r--r--   0 runner    (1001) docker     (123)    40205 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index21-d3e36a16.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17932 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index22-34fa8df0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index23-b30a6092.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index24-11b8d91d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index25-4151ca38.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3544383 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index26-2968ddd0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index27-86c85604.js
+-rw-r--r--   0 runner    (1001) docker     (123)  4615279 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index28-fce682a3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index29-7f2f8cac.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index3-b632de7a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index30-449fed8c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index31-a39e3c8b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index32-5e251911.js
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index33-8befa193.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index34-d9e154ad.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index35-71968f90.js
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index36-6d6222b1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18675 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index37-03da10b3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index38-f8a193c1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17339 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index39-c97fb654.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index4-2684c49d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index5-264c6674.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index6-b60485d2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index7-ae38a6d6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index8-5ee4cbfe.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/index9-f552db0e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/invalid-file-82d62dec.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/left-8c88a49a.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/left-shadow-e0fdfe32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23111 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/linear-8d973619.js
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/logo_normal_en_blue-18b013e7.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/logo_normal_en_gray-163de1a0.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/logo_normal_en_white-ec11283c.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/logo_small_en_white-782559aa.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   117896 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/main-e0f2ffda.js
+-rw-r--r--   0 runner    (1001) docker     (123)    94147 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/module-ddaca3b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/module2-74df381a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/module3-49e9a615.js
+-rw-r--r--   0 runner    (1001) docker     (123)    42104 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-bold-452a631f.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    34752 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-bold-5c4ed5bb.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    37252 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-bold-italic-16cda7ef.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    45068 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-bold-italic-4926428e.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    41368 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-extrabold-613313c8.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    33808 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-extrabold-648ba0e7.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    44392 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-extrabold-italic-33533562.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    36660 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-extrabold-italic-a258578a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    42532 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-extralight-64fbbd3d.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    35056 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-extralight-f053be7c.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    44668 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-extralight-italic-6cbe5597.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    36800 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-extralight-italic-d23afde2.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    35640 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-heavy-5e0869ee.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    43316 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-heavy-c7e67c68.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    37972 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-heavy-italic-8f5fbf20.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    45720 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-heavy-italic-c702fef1.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    37368 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-italic-34df3d81.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    45240 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-italic-b81a6146.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    41936 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-light-3f8151f4.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    34472 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-light-9db6ab0a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    44372 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-light-italic-a1454ca5.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    36580 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-light-italic-ec333948.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    51572 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-mono-bold-2bf715ff.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    65060 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-mono-bold-9b29c79a.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    50112 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-mono-light-5bae063c.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    63324 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-mono-light-7fbe3706.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    65036 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-mono-regular-95881615.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    51524 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-mono-regular-a13dec50.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    64944 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-mono-semibold-085fb4a8.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    51308 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-mono-semibold-b39c5174.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    42584 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-regular-16b63547.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    35128 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-regular-8e2261df.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    33416 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-semibold-3d06895e.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    40620 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-semibold-ec5809e8.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    44728 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-semibold-italic-1935eb14.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    36904 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-semibold-italic-ae706d8c.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    40860 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-thin-6feca5dc.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    33696 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-thin-e85966f1.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    43504 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-thin-italic-2dffa092.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    35900 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/overpass-thin-italic-44db8e3d.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   276435 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/pfbg_2000-1f17de55.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    67491 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/pfbg_576-1d76d6cc.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   195594 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/pfbg_576@2x-4942ea78.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   116699 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/pfbg_768-8bc3cc8a.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   362032 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/pfbg_768@2x-037bce76.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   588571 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/pfbg_992@2x-9dfd9687.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/pficon-0a333dac.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17700 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/pficon-86c74539.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/project-863f66b0.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/right-aefe3c24.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/right-shadow-58dd9abc.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/search-empty-13cbde15.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/setting-6d098443.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/status-icon-sprite-bc89cb14.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/utils-de54785e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/web-vitals-d4fac006.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/assets/wechat-cffee157.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-31 09:40:07.000000 starwhale-0.5.9/starwhale/web/ui/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-31 09:40:07.000000 starwhale-0.5.9/starwhale/web/ui/favicon_white.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    25155 2023-07-31 09:40:07.000000 starwhale-0.5.9/starwhale/web/ui/iconfont.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    45679 2023-07-31 09:40:13.000000 starwhale-0.5.9/starwhale/web/ui/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-31 09:40:07.000000 starwhale-0.5.9/starwhale/web/ui/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-31 09:31:23.000000 starwhale-0.5.9/starwhale/web/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20812 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13372 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:32:01.000000 starwhale-0.5.9/starwhale.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-31 09:40:17.000000 starwhale-0.5.9/starwhale.egg-info/top_level.txt
```

### Comparing `starwhale-0.5.8/PKG-INFO` & `starwhale-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starwhale
-Version: 0.5.8
+Version: 0.5.9
 Summary: An MLOps Platform for Model Evaluation
 Home-page: https://github.com/star-whale/starwhale
 Author: Starwhale Team
 Author-email: developer@starwhale.ai
 License: Apache License 2.0
 Keywords: MLOps,AI,Starwhale,Model Evaluation
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: starwhale Version: 0.5.8 Summary: An MLOps Platform
+Metadata-Version: 2.1 Name: starwhale Version: 0.5.9 Summary: An MLOps Platform
 for Model Evaluation Home-page: https://github.com/star-whale/starwhale Author:
 Starwhale Team Author-email: developer@starwhale.ai License: Apache License 2.0
 Keywords: MLOps,AI,Starwhale,Model Evaluation Classifier: Development Status ::
 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
```

### Comparing `starwhale-0.5.8/pyproject.toml` & `starwhale-0.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/scripts/sw-docker-entrypoint` & `starwhale-0.5.9/scripts/sw-docker-entrypoint`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/setup.py` & `starwhale-0.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/__init__.py` & `starwhale-0.5.9/starwhale/__init__.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/api/_impl/data_store.py` & `starwhale-0.5.9/starwhale/api/_impl/data_store.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/api/_impl/dataset/__init__.py` & `starwhale-0.5.9/starwhale/api/_impl/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/api/_impl/dataset/builder/mapping_builder.py` & `starwhale-0.5.9/starwhale/api/_impl/dataset/builder/mapping_builder.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/api/_impl/dataset/loader.py` & `starwhale-0.5.9/starwhale/api/_impl/dataset/loader.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/api/_impl/dataset/model.py` & `starwhale-0.5.9/starwhale/api/_impl/dataset/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -344,15 +344,14 @@
         from starwhale import dataset, Binary
 
         ds = dataset("mnist").with_builder_blob_config(volume_size="32M", alignment_size=128)
         ds.append({"data": Binary(b"123")})
         ds.commit()
         ds.close()
         ```
-
         Returns:
             A Dataset Object
         """
         with self._builder_lock:
             if self._dataset_builder is not None:
                 raise RuntimeError(
                     "dataset has already accept some changed rows, forbid to config dataset blob attributes"
@@ -416,15 +415,33 @@
             manifest = DatasetStorage(uri).manifest
 
         return DatastoreRevision.from_manifest(manifest)
 
     def batch_iter(
         self, batch_size: int = 1, drop_not_full: bool = False
     ) -> t.Iterator[t.List[DataRow]]:
-        """Batch data into lists of length n. The last batch may be shorter."""
+        """Batch data into lists of length n. The last batch may be shorter.
+
+        Arguments:
+            batch_size: (int, optional) The size of each batch. Default is 1.
+            drop_not_full: (bool, optional) Whether to drop the last batch if it is not full.
+
+        Returns:
+            A generator of lists of length n.
+
+        Examples:
+        ```python
+        from starwhale import dataset
+
+        ds = dataset("mnist")
+        for batch_rows in ds.batch_iter(batch_size=2):
+            assert len(batch_rows) == 2
+            print(batch_rows[0].features)
+        ```
+        """
         it = self.__iter__()
         while True:
             batch_data = list(islice(it, batch_size))
             if not batch_data or (drop_not_full and len(batch_data) < batch_size):
                 return
             yield batch_data
 
@@ -620,27 +637,93 @@
 
     def to_pytorch(
         self,
         transform: t.Optional[t.Callable] = None,
         drop_index: bool = True,
         skip_default_transform: bool = False,
     ) -> TorchDataset:
+        """Convert Starwhale Dataset to PyTorch Dataset.
+
+        Arguments:
+            transform: (callable, optional) A transform function for input data.
+            drop_index: (bool, optional) Whether to drop the index column.
+            skip_default_transform: (bool, optional) If `transform` is not set,
+                by default the built-in Starwhale transform function will be used to transform the data.
+                This can be disabled with the `skip_default_transform` parameter.
+
+        Returns:
+            torch.utils.data.Dataset
+
+        Examples:
+        ```python
+        import torch.utils.data as tdata
+        from starwhale import dataset
+
+        ds = dataset("mnist")
+
+        torch_ds = ds.to_pytorch()
+        torch_loader = tdata.DataLoader(torch_ds, batch_size=2)
+        ```
+
+        ```python
+        import torch.utils.data as tdata
+        from starwhale import dataset
+
+        with dataset("mnist") as ds:
+            for i in range(0, 10):
+                ds.append({"txt": Text(f"data-{i}"), "label": i})
+
+            ds.commit()
+
+        def _custom_transform(data: t.Any) -> t.Any:
+            data = data.copy()
+            txt = data["txt"].to_str()
+            data["txt"] = f"custom-{txt}"
+            return data
+
+        torch_loader = tdata.DataLoader(
+            dataset(ds.uri).to_pytorch(transform=_custom_transform), batch_size=1
+        )
+        item = next(iter(torch_loader))
+        assert isinstance(item["label"], torch.Tensor)
+        assert item["txt"][0] in ("custom-data-0", "custom-data-1")
+        ```
+        """
         from starwhale.integrations.pytorch import TorchIterableDataset
 
         return TorchIterableDataset(
             dataset=self,
             transform=transform,
             drop_index=drop_index,
             skip_default_transform=skip_default_transform,
         )
 
     def to_tensorflow(
         self,
         drop_index: bool = True,
     ) -> tf.data.Dataset:
+        """Convert Starwhale Dataset to Tensorflow Dataset.
+
+        Arguments:
+            drop_index: (bool, optional) Whether to drop the index column.
+
+        Returns:
+            tensorflow.data.Dataset object
+
+        Examples:
+
+        ```python
+        from starwhale import dataset
+        import tensorflow as tf
+
+        ds = dataset("mnist")
+        tf_ds = ds.to_tensorflow(drop_index=True)
+        assert isinstance(tf_ds, tf.data.Dataset)
+        ```
+        """
         from starwhale.integrations.tensorflow import to_tf_dataset
 
         return to_tf_dataset(dataset=self, drop_index=drop_index)
 
     @_check_readonly
     def __setitem__(
         self, key: t.Union[str, int], value: t.Union[DataRow, t.Tuple, t.Dict]
@@ -741,15 +824,15 @@
         """
         return self._loading_version
 
     @property
     def pending_commit_version(self) -> str:
         """Next commit version.
         When you call the `commit` function, the pending_commit_version will be recorded in
-        the Standalone instance ,or Cloud instance.
+        the Standalone instance ,Server instance or Cloud instance.
 
         Returns:
             A str version
         """
         return self._pending_commit_version
 
     @property
@@ -949,23 +1032,32 @@
         dest_uri: str,
         dest_local_project_uri: str = "",
         force: bool = False,
         mode: str = DatasetChangeMode.PATCH.value,
     ) -> None:
         """Copy dataset to another instance.
 
-        Args:
+        Arguments:
             dest_uri: (str, required) destination dataset uri
             dest_local_project_uri: (str, optional) destination local project uri
             force: (bool, optional) force to copy
             mode: (str, optional) copy mode, default is 'patch'. Mode choices are: 'patch', 'overwrite'.
               `patch` mode: only update the changed rows and columns for the remote dataset;
               `overwrite` mode: update records and delete extraneous rows from the remote dataset
+
         Returns:
             None
+
+        Examples:
+
+        ```python
+        from starwhale import dataset
+        ds = dataset("mnist")
+        ds.copy("cloud://remote-instance/project/starwhale")
+        ```
         """
         CoreDataset.copy(
             self.uri,
             dest_uri,
             dest_local_project_uri=dest_local_project_uri,
             force=force,
             mode=DatasetChangeMode(mode),
@@ -995,15 +1087,15 @@
     ) -> Dataset:
         """Create or load a dataset from standalone instance or cloud instance.
 
         For a non-existed dataset, when you try to load it, you will get an Exception; when you try to append records and commit,
         the dataset will be created automatically.
 
         Arguments:
-            uri: (str, Resource, required) The dataset uri.
+            uri: (str, Resource, required) The dataset uri str or Resource object.
             create: (str, optional) The mode of dataset creating. The options are `auto`, `empty` and `forbid`.
                 `auto` mode: If the dataset already exists, creation is ignored. If it does not exist, the dataset is created automatically.
                 `empty` mode: If the dataset already exists, an Exception is raised; If it does not exist, an empty dataset is created. This mode ensures the creation of a new, empty dataset.
                 `forbid` mode: If the dataset already exists, nothing is done.If it does not exist, an Exception is raised. This mode ensures the existence of the dataset.
                 The default is `auto`.
             readonly: (bool, optional) For an existing dataset, you can specify the readonly=True argument to ensure
                 the dataset is in readonly mode. Default is False.
@@ -1075,17 +1167,18 @@
         """Create a new dataset from huggingface datasets.
 
         Arguments:
             name: (str, required) The dataset name you would like to use.
             repo: (str, required) The huggingface datasets repo name.
             subset: (str, optional) The subset name. If the huggingface dataset has multiple subsets, you must specify the subset name.
             split: (str, optional) The split name. If the split name is not specified, the all splits dataset will be built.
-            revision: (str, optional) The huggingface datasets revision. The default value is `main`. If the split name is not specified, the all splits dataset will be built.
+            revision: (str, optional) The huggingface datasets revision. The default value is `main`. The option value accepts tag name, or branch name, or commit hash.
             alignment_size: (int|str, optional) The blob alignment size. The default value is 128.
-            volume_size: (int|str, optional) The blob volume size. The default value is 64MB.
+            volume_size: (int|str, optional) The maximum size of a dataset blob file. A new blob file will be generated when the size exceeds this limit.
+              The default value is 64MB.
             mode: (str|DatasetChangeMode, optional) The dataset change mode. The default value is `patch`. Mode choices are `patch` and `overwrite`.
             cache: (bool, optional) Whether to use huggingface dataset cache(download + local hf dataset). The default value is True.
 
         Returns:
                 A Dataset Object
 
         Examples:
@@ -1145,38 +1238,38 @@
     ) -> Dataset:
         """Create a new dataset from a json text.
 
         Arguments:
             name: (str, required) The dataset name you would like to use.
             json_text: (str, required) The json text from which you would like to create this dataset.
             field_selector: (str, optional) The filed from which you would like to extract dataset array items.
-                The default value is "" which indicates that the dict is an array contains all the items.
+                The default value is "" which indicates that the json object is an array contains all the items.
             alignment_size: (int|str, optional) The blob alignment size. The default value is 128.
             volume_size: (int|str, optional) The blob volume size. The default value is 64MB.
             mode: (str|DatasetChangeMode, optional) The dataset change mode. The default value is `patch`. Mode choices are `patch` and `overwrite`.
 
         Returns:
                 A Dataset Object
 
         Examples:
         ```python
         from starwhale import Dataset
         myds = Dataset.from_json(
-            "translation",
-            '[{"en":"hello","zh-cn":"你好"},{"en":"how are you","zh-cn":"最近怎么样"}]'
+            name="translation",
+            json_text='[{"en":"hello","zh-cn":"你好"},{"en":"how are you","zh-cn":"最近怎么样"}]'
         )
         print(myds[0].features.en)
         ```
 
         ```python
         from starwhale import Dataset
         myds = Dataset.from_json(
-            "translation",
-            '{"content":{"child_content":[{"en":"hello","zh-cn":"你好"},{"en":"how are you","zh-cn":"最近怎么样"}]}}',
-            "content.child_content"
+            name="translation",
+            json_text='{"content":{"child_content":[{"en":"hello","zh-cn":"你好"},{"en":"how are you","zh-cn":"最近怎么样"}]}}',
+            field_selector="content.child_content"
         )
         print(myds[0].features["zh-cn"])
         ```
         """
         mode = DatasetChangeMode(mode)
         data_items = json.loads(json_text)
 
@@ -1223,26 +1316,26 @@
         kind: str | DatasetFolderSourceType,
         name: str | Resource = "",
         auto_label: bool = True,
         alignment_size: int | str = D_ALIGNMENT_SIZE,
         volume_size: int | str = D_FILE_VOLUME_SIZE,
         mode: DatasetChangeMode | str = DatasetChangeMode.PATCH,
     ) -> Dataset:
-        """Create a dataset from a folder of image files.
+        """Create a dataset from a folder of image/video/audio files.
 
-        The image folder building supports the following features:
+        The image/video/audio folder building supports the following features:
 
         - search the folder recursively.
         - support three kinds of folder type:
           - `image`: png/jpg/jpeg/webp/svg/apng types. The image file will be converted to Starwhale.Image type.
           - `video`: mp4/webm/avi types. The video file will be converted to Starwhale.Video type.
           - `audio`: mp3/wav types. The audio file will be converted to Starwhale.Audio type.
-        - auto labeling by the common prefix parent dir name.
+        - If `auto_label=True`, the name of the parent directory will be used as the label for that data item, corresponding to the `label` field. Files in the root directory will not be labeled.
         - auto fill caption with the txt file which is named the same as the image file, and located in the same folder.
-        - auto import metadata.csv or metadata.jsonl as the additional metadata information.
+        - auto import metadata.csv or metadata.jsonl (in the root dir) as the additional metadata information.
 
         When the auto_label is True, the function will try to ingest the label from the image folder(sub-folder) name.
         If the image file's folder is equal to the root folder, the label is empty.
         For example, the following structure will create a dataset with 2 labels: "cat" and "dog", 4 images in total.
 
         ```
         folder/dog/1.png
@@ -1277,28 +1370,34 @@
         folder/dog/1.png
         folder/dog/1.txt
         ```
 
         Arguments:
             folder: (str|Path, required) The folder path from which you would like to create this dataset.
             kind: (str|DatasetFolderSourceType, required) The dataset source type you would like to use, the choices are: image, video and audio.
+               Recursively searching for files of the specified `kind` in `folder`. Other file types will be ignored.
             name: (str|Resource, optional) The dataset name you would like to use. If not specified, the name is the folder name.
             auto_label: (bool, optional) Whether to auto label by the sub-folder name. The default value is True.
             alignment_size: (int|str, optional) The blob alignment size. The default value is 128.
             volume_size: (int|str, optional) The blob volume size. The default value is 64MB.
             mode: (str|DatasetChangeMode, optional) The dataset change mode. The default value is `patch`. Mode choices are `patch` and `overwrite`.
 
         Returns:
             A Dataset Object.
 
         Examples:
         ```python
         from starwhale import Dataset
 
-        ds = Dataset.from_folder("/path/to/image", "image", "my-image-dataset")  # create a my-image-dataset dataset from /path/to/image folder.
+        # create a my-image-dataset dataset from /path/to/image folder.
+        ds = Dataset.from_folder(
+            folder="/path/to/image",
+            kind="image",
+            name="my-image-dataset"
+        )
         ```
         """
         rootdir = Path(folder)
         if not rootdir.exists():
             raise RuntimeError(f"folder {rootdir} doesn't exist")
 
         name = name or rootdir.name
```

### Comparing `starwhale-0.5.8/starwhale/api/_impl/evaluation.py` & `starwhale-0.5.9/starwhale/api/_impl/evaluation.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,30 +34,28 @@
 class PipelineHandler(metaclass=ABCMeta):
     _INPUT_PREFIX = "input/"
 
     def __init__(
         self,
         predict_batch_size: int = 1,
         ignore_error: bool = False,
-        flush_result: bool = False,
         predict_auto_log: bool = True,
         predict_log_mode: str = PredictLogMode.PICKLE.value,
         predict_log_dataset_features: t.Optional[t.List[str]] = None,
         dataset_uris: t.Optional[t.List[str]] = None,
         **kwargs: t.Any,
     ) -> None:
         self.predict_batch_size = predict_batch_size
         self.svc = Service()
         self.context = Context.get_runtime_context()
 
         self.dataset_uris = self.context.dataset_uris or dataset_uris or []
 
         self.predict_log_dataset_features = predict_log_dataset_features
         self.ignore_error = ignore_error
-        self.flush_result = flush_result
         self.predict_auto_log = predict_auto_log
         self.predict_log_mode = PredictLogMode(predict_log_mode)
         self.kwargs = kwargs
 
         _logdir = JobStorage.local_run_dir(self.context.project, self.context.version)
         _run_dir = (
             _logdir / RunSubDirType.RUNLOG / self.context.step / str(self.context.index)
@@ -284,15 +282,15 @@
                         features=_features,
                         idx_with_ds=_idx_with_ds,
                         output=_result,
                         idx=_idx,
                         duration_seconds=_duration,
                     )
 
-        if self.flush_result and self.predict_auto_log:
+        if self.predict_auto_log:
             self.evaluation_store.flush_result()
 
         console.info(
             f"{self.context.step}-{self.context.index} handled {cnt} data items for dataset {self.dataset_uris}"
         )
 
     def _update_status(self, status: str) -> None:
@@ -511,43 +509,58 @@
 def predict(*args: t.Any, **kw: t.Any) -> t.Any:
     """Defines a predict function.
 
     This function can be used as a decorator to define an evaluation-predict function that maps the dataset data into
     the different predict workers.
 
     Arguments:
-        datasets: [Union[List[str], None], optional] Use the datasets rows as the input data for the predict function.
-        resources: [Dict, optional] Resources for the predict task, such as memory, gpu etc. Current only supports
-            the cloud instance.
-        concurrency: [int, optional] The concurrency of the predict tasks. Default is 1.
+        resources: [Dict, optional] Resources for the predict task, such as cpu, memory, nvidia.com/gpu etc. Current only supports
+            the Server instance.
         replicas: [int, optional] The number of the predict tasks. Default is 1.
         batch_size: [int, optional] Number of samples per batch. Default is 1.
         fail_on_error: [bool, optional] Fast fail on the exceptions in the predict function. Default is True.
         auto_log: [bool, optional] Auto log the return values of the predict function and the according dataset rows. Default is True.
         log_mode: [str, optional] When auto_log=True, the log_mode can be specified to control the log behavior. Options are `pickle` and `plain`. Default is `pickle`.
         log_dataset_features: [List[str], optional] When auto_log=True, the log_dataset_features can be specified to control the log dataset features behavior.
             Default is None, all dataset features will be logged. If the list is empty, no dataset features will be logged.
         needs: [List[Callable], optional] The list of the functions that need to be executed before the predict function.
 
     Examples:
     ```python
-
     from starwhale import evaluation
 
     @evaluation.predict
     def predict_image(data):
         ...
 
     @evaluation.predict(
         dataset="mnist/version/latest",
         batch_size=32,
         replicas=4,
+        needs=[predict_image],
     )
     def predict_batch_images(batch_data)
         ...
+
+    @evaluation.predict(
+        resources={"nvidia.com/gpu": 1,
+                "cpu": {"request": 1, "limit": 2},
+                "mem": 200 * 1024},  # 200MB
+        log_mode="plain",
+    )
+    def predict_with_resources(data):
+        ...
+
+    @evaluation.predict(
+        replicas=1,
+        log_mode="plain",
+        log_dataset_features=["txt", "img", "label"],
+    )
+    def predict_with_selected_features(data):
+        ...
     ```
 
     Returns:
         The decorated function.
     """
 
     # TODO: support runtime
@@ -603,16 +616,16 @@
     This function can be used as a decorator to define an evaluation-evaluate function that reduces the results of the
     predict function.
 
     Argument:
         needs: [List[Callable], required] The list of the functions that need to be executed before the evaluate function.
         use_predict_auto_log: [bool, optional] Passing the iterator of the predict auto-log results into the evaluate function.
             Default is True.
-        resources: [Dict, optional] Resources for the predict task, such as memory, gpu etc. Current only supports
-            the cloud instance.
+        resources: [Dict, optional] Resources for the predict task, such as memory, cpu, nvidia.com/gpu etc. Current only supports
+            the Server instance.
 
     Examples:
     ```python
     from starwhale import evaluation
 
     @evaluation.evaluate(needs=[predict_image])
     def evaluate_results(predict_result_iter):
```

### Comparing `starwhale-0.5.8/starwhale/api/_impl/experiment.py` & `starwhale-0.5.9/starwhale/api/_impl/experiment.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,35 +12,35 @@
     Argument:
         resources: [Dict, optional] Resources for the predict task, such as memory, gpu etc. Current only supports
             the cloud instance.
         needs: [List[Callable], optional] The list of functions that the fine-tune function depends on.
 
     Examples:
     ```python
-    from starwhale import experiment
+    from starwhale import fine_tune
 
-    @experiment.fine_tune
+    @fine_tune
     def ft():
         ...
 
-    @experiment.fine_tune(resources={"nvidia.com/gpu": 1}, needs=[prepare_handler])
+    @fine_tune(resources={"nvidia.com/gpu": 1}, needs=[prepare_handler])
     def ft():
         ...
     ```
 
     Returns:
         The decorated function
     """
 
     if len(args) == 1 and len(kw) == 0 and callable(args[0]):
         return fine_tune()(args[0])
     else:
 
         def _wrap(func: Callable) -> Any:
-            _register_ft(func, resources=kw.get("resources"))
+            _register_ft(func, resources=kw.get("resources"), needs=kw.get("needs"))
             setattr(func, DecoratorInjectAttr.FineTune, True)
             return func
 
     return _wrap
 
 
 def _register_ft(
```

### Comparing `starwhale-0.5.8/starwhale/api/_impl/job.py` & `starwhale-0.5.9/starwhale/api/_impl/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,44 +129,40 @@
         name: str = "",
         expose: int = 0,
         require_dataset: bool = False,
     ) -> t.Callable:
         """Register a function as a handler. Enable the function execute by needs handler, run with gpu/cpu/mem resources in server side,
         and control concurrency and replicas of handler run.
 
-        Args:
-            resources: [Dict, optional] Resources for the handler run, such as memory, gpu etc. Current only supports
-              the cloud instance.
-            concurrency: [int, optional] The concurrency of the handler run. Default is 1.
+        Arguments:
+            resources: [Dict, optional] Resources for the handler run, such as memory, cpu, nvidia.com/gpu etc. Current only supports
+              the server instance.
             replicas: [int, optional] The number of the handler run. Default is 1.
             needs: [List[Callable], optional] The list of the functions that need to be executed before the handler function.
               The depends callable objects must be decorated by `@handler`, `@evaluation.predict`, `@evaluation.evaluate` and `@experiment.fine_tune` .
             name: [str, optional] The user-friendly name of the handler. Default is the function name.
             expose: [int, optional] The expose port of the handler. Only used for the handler run as a service.
               Default is 0. If expose is 0, there is no expose port.
               Users must set the expose port when the handler run as a service on the server or cloud instance.
-            require_dataset: [bool] Whether you need datasets when execute the handler.
+            require_dataset: [bool, optional] Whether you need datasets when execute the handler.
               Default is False, It means that there is no need to select datasets when executing this handler on the server or cloud instance.
               If True, You must select datasets when executing on the server or cloud instance.
 
-
-
         Example:
         ```python
         from starwhale import handler
 
-        @handler(resources={"cpu": 1, "nvidia.com/gpu": 1}, concurrency=2, replicas=3)
+        @handler(resources={"cpu": 1, "nvidia.com/gpu": 1}, replicas=3)
         def my_handler():
             ...
 
         @handler(needs=[my_handler])
         def my_another_handler():
             ...
         ```
-
         Returns:
             [Callable] The decorator function.
         """
 
         def decorator(func: t.Callable) -> t.Callable:
             if not inspect.isfunction(func):
                 raise NoSupportError(
```

### Comparing `starwhale-0.5.8/starwhale/api/_impl/metric.py` & `starwhale-0.5.9/starwhale/api/_impl/metric.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/api/_impl/model.py` & `starwhale-0.5.9/starwhale/api/_impl/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 ) -> None:
     """Build Starwhale Model Package.
 
     In common case, you may call `build` function in your experiment scripts.`build` function is a shortcut for the `swcli model build` command.
     Build function will search all handlers from the `modules` argument or imported modules, and then build Starwhale Model Package.
 
     Arguments:
-        modules: (List[str|object] optional) The search modules supports object(function, class or module) or str(example: "to.path.module", "to.path.module:object").
+        modules: (List[str|object], optional) The search modules supports object(function, class or module) or str(example: "to.path.module", "to.path.module:object").
             If the argument is not specified, the search modules are the imported modules.
         name: (str, optional) The name of Starwhale Model Package, default is the current work dir.
         workdir: (str, Pathlib.Path, optional) The path of the rootdir. The default workdir is the current working dir.
             All files in the workdir will be packaged. If you want to ignore some files, you can add `.swignore` file in the workdir.
         desc: (str, optional) The description of the Starwhale Model Package.
         project_uri: (str, optional) The project uri of the Starwhale Model Package. If the argument is not specified,
             the project_uri is the config value of `swcli project select` command.
```

### Comparing `starwhale-0.5.8/starwhale/api/_impl/service.py` & `starwhale-0.5.9/starwhale/api/_impl/service.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/api/_impl/track/base.py` & `starwhale-0.5.9/starwhale/api/_impl/track/base.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/api/_impl/track/collector.py` & `starwhale-0.5.9/starwhale/api/_impl/track/collector.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/api/_impl/track/handler.py` & `starwhale-0.5.9/starwhale/api/_impl/track/handler.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/api/_impl/track/hooker.py` & `starwhale-0.5.9/starwhale/api/_impl/track/hooker.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/api/_impl/track/tracker.py` & `starwhale-0.5.9/starwhale/api/_impl/track/tracker.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/api/_impl/wrapper.py` & `starwhale-0.5.9/starwhale/api/_impl/wrapper.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/api/dataset.py` & `starwhale-0.5.9/starwhale/api/dataset.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/base/blob/file.py` & `starwhale-0.5.9/starwhale/base/blob/file.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/base/blob/store.py` & `starwhale-0.5.9/starwhale/base/blob/store.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/base/bundle.py` & `starwhale-0.5.9/starwhale/base/bundle.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/base/bundle_copy.py` & `starwhale-0.5.9/starwhale/base/bundle_copy.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/base/cloud.py` & `starwhale-0.5.9/starwhale/base/cloud.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/base/cloud_blob_cache.py` & `starwhale-0.5.9/starwhale/base/cloud_blob_cache.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/base/context.py` & `starwhale-0.5.9/starwhale/base/context.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/base/mixin.py` & `starwhale-0.5.9/starwhale/base/mixin.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/base/scheduler/__init__.py` & `starwhale-0.5.9/starwhale/base/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/base/scheduler/dag.py` & `starwhale-0.5.9/starwhale/base/scheduler/dag.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/base/scheduler/step.py` & `starwhale-0.5.9/starwhale/base/scheduler/step.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/base/scheduler/task.py` & `starwhale-0.5.9/starwhale/base/scheduler/task.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/base/store.py` & `starwhale-0.5.9/starwhale/base/store.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/base/tag.py` & `starwhale-0.5.9/starwhale/base/tag.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/base/type.py` & `starwhale-0.5.9/starwhale/base/type.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/base/uri/exceptions.py` & `starwhale-0.5.9/starwhale/base/uri/exceptions.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/base/uri/instance.py` & `starwhale-0.5.9/starwhale/base/uri/instance.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/base/uri/project.py` & `starwhale-0.5.9/starwhale/base/uri/project.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/base/uri/resource.py` & `starwhale-0.5.9/starwhale/base/uri/resource.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/base/view.py` & `starwhale-0.5.9/starwhale/base/view.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/cli/__init__.py` & `starwhale-0.5.9/starwhale/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/cli/assistance/broker.py` & `starwhale-0.5.9/starwhale/cli/assistance/broker.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/cli/assistance/cli.py` & `starwhale-0.5.9/starwhale/cli/assistance/cli.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/cli/assistance/common.py` & `starwhale-0.5.9/starwhale/cli/assistance/common.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/cli/assistance/host.py` & `starwhale-0.5.9/starwhale/cli/assistance/host.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/cli/assistance/remote.py` & `starwhale-0.5.9/starwhale/cli/assistance/remote.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/cli/assistance/wait_console.py` & `starwhale-0.5.9/starwhale/cli/assistance/wait_console.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/cli/board/board.py` & `starwhale-0.5.9/starwhale/cli/board/board.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/cli/board/project_tree.py` & `starwhale-0.5.9/starwhale/cli/board/project_tree.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/cli/board/widgets.py` & `starwhale-0.5.9/starwhale/cli/board/widgets.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/cli/completion.py` & `starwhale-0.5.9/starwhale/cli/completion.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/cli/mngt.py` & `starwhale-0.5.9/starwhale/cli/mngt.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/consts/__init__.py` & `starwhale-0.5.9/starwhale/consts/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -190,18 +190,22 @@
 DEFAULT_PYTHON_VERSION = "3.8"
 LATEST_TAG = "latest"
 
 YAML_TYPES = (".yaml", ".yml")
 
 DEFAULT_IMAGE_REPO = "docker-registry.starwhale.cn/star-whale"
 DEFAULT_IMAGE_NAME = "base"
-DEFAULT_IMAGE_TAG = LATEST_TAG  # "0.3.0"
+# When release a new base image version, remember to update the FIXED_RELEASE_BASE_IMAGE_VERSION.
+# refer to https://github.com/star-whale/starwhale/blob/main/docker/Makefile#L12
+FIXED_RELEASE_BASE_IMAGE_VERSION = "0.3.4"
 SW_IMAGE_FMT = "{repo}/{name}:{tag}"
 DEFAULT_SW_TASK_RUN_IMAGE = SW_IMAGE_FMT.format(
-    repo=DEFAULT_IMAGE_REPO, name=DEFAULT_IMAGE_NAME, tag=LATEST_TAG
+    repo=DEFAULT_IMAGE_REPO,
+    name=DEFAULT_IMAGE_NAME,
+    tag=FIXED_RELEASE_BASE_IMAGE_VERSION,
 )
 SW_IGNORE_FILE_NAME = ".swignore"
 
 CNTR_DEFAULT_PIP_CACHE_DIR = "/root/.cache/pip"
 
 SW_DEV_DUMMY_VERSION = "0.0.0.dev0"
 SW_PYPI_PKG_NAME = "starwhale"
```

### Comparing `starwhale-0.5.8/starwhale/core/dataset/cli.py` & `starwhale-0.5.9/starwhale/core/dataset/cli.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/core/dataset/copy.py` & `starwhale-0.5.9/starwhale/core/dataset/copy.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/core/dataset/model.py` & `starwhale-0.5.9/starwhale/core/dataset/model.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/core/dataset/store.py` & `starwhale-0.5.9/starwhale/core/dataset/store.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/core/dataset/tabular.py` & `starwhale-0.5.9/starwhale/core/dataset/tabular.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/core/dataset/type.py` & `starwhale-0.5.9/starwhale/core/dataset/type.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/core/dataset/view.py` & `starwhale-0.5.9/starwhale/core/dataset/view.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/core/instance/cli.py` & `starwhale-0.5.9/starwhale/core/instance/cli.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/core/instance/view.py` & `starwhale-0.5.9/starwhale/core/instance/view.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/core/job/cli.py` & `starwhale-0.5.9/starwhale/core/job/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -68,33 +68,42 @@
 @job_cmd.command("recover", help="Recover removed job")
 @click.argument("job")
 @click.option("-f", "--force", is_flag=True, help="Force to recover")
 def _recover(job: str, force: bool) -> None:
     JobTermView(job).recover(force)
 
 
-@job_cmd.command("pause", help="Pause job")
+@job_cmd.command("pause")
 @click.argument("job")
 @click.option("-f", "--force", is_flag=True, help="Force to pause")
 def _pause(job: str, force: bool) -> None:
+    """Pause job.
+    On Standalone instance, this command only takes effect for containerized jobs.
+    """
     click.confirm("continue to pause?", abort=True)
     JobTermView(job).pause(force)
 
 
-@job_cmd.command("resume", help="Resume job")
+@job_cmd.command("resume")
 @click.argument("job")
 @click.option("-f", "--force", is_flag=True, help="Force to resume")
 def _resume(job: str, force: bool) -> None:
+    """Resume job.
+    On Standalone instance, this command only takes effect for containerized jobs.
+    """
     JobTermView(job).resume(force)
 
 
-@job_cmd.command("cancel", help="Cancel job")
+@job_cmd.command("cancel")
 @click.argument("job")
 @click.option("-f", "--force", is_flag=True, help="Force to cancel")
 def _cancel(job: str, force: bool) -> None:
+    """Cancel job.
+    On Standalone instance, this command only takes effect for containerized jobs.
+    """
     click.confirm("continue to cancel?", abort=True)
     JobTermView(job).cancel(force)
 
 
 @job_cmd.command("info", help="Inspect job details")
 @click.argument("job")
 @click.option(
```

### Comparing `starwhale-0.5.8/starwhale/core/job/model.py` & `starwhale-0.5.9/starwhale/core/job/model.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/core/job/store.py` & `starwhale-0.5.9/starwhale/core/job/store.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/core/job/view.py` & `starwhale-0.5.9/starwhale/core/job/view.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/core/model/cli.py` & `starwhale-0.5.9/starwhale/core/model/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     default="",
     help="Project URI, default is the current selected project. The model package will store in the specified project.",
 )
 @click.option(
     "-f",
     "--model-yaml",
     default=None,
-    help="mode yaml path, default use ${workdir}/model.yaml file",
+    help="model yaml path, default use ${workdir}/model.yaml file",
 )
 @click.option(
     "-r",
     "--runtime",
     default="",
     help="runtime uri, build model in the runtime environment process",
 )
@@ -63,15 +63,16 @@
 @click.option("-n", "--name", default="", help="model name")
 @click.option("-d", "--desc", default="", help="Dataset description")
 @click.option(
     "--package-runtime/--no-package-runtime",
     is_flag=True,
     default=True,
     show_default=True,
-    help="Package Starwhale Runtime into the model.",
+    help="When using the `--runtime` parameter, by default, the corresponding Starwhale runtime will become the built-in runtime for the Starwhale model. "
+    "This feature can be disabled with the `--no-package-runtime` parameter.",
 )
 @click.option(
     "--add-all",
     is_flag=True,
     default=False,
     help="Add all files in the working directory to the model package"
     "(excludes python cache files and virtual environment files when disabled)."
@@ -142,15 +143,15 @@
     TARGET_DIR: target directory to extract model package.
 
     Example:
 
         \b
         - extract mnist model package to current directory
             swcli model extract mnist/version/xxxx .
-
+        \b
         - extract mnist model package to current directory and force to overwrite the files
             swcli model extract mnist/version/xxxx . -f
     """
     ModelTermView(model).extract(target=Path(target_dir), force=force)
 
 
 @model_cmd.command("tag", help="Model Tag Management, add or remove")
@@ -403,15 +404,17 @@
     is_flag=True,
     help="[ONLY Standalone]Use docker container to run model handler, the docker image or runtime uri must be set",
 )
 @optgroup.option(  # type: ignore[no-untyped-call]
     "-fs",
     "--forbid-snapshot",
     is_flag=True,
-    help="[ONLY STANDALONE]Forbid to use model run snapshot dir, use model src dir directly. When the `--workdir` option is set, this option will be ignored.",
+    help="In model URI mode, each model run uses a new snapshot directory."
+    "Setting this parameter will directly use the model's workdir as the run directory."
+    "In local dev mode, this parameter does not take effect, each run is in the `--workdir` specified directory.",
 )
 @optgroup.option(  # type: ignore[no-untyped-call]
     "--cleanup-snapshot/--no-cleanup-snapshot",
     is_flag=True,
     default=True,
     show_default=True,
     help="[ONLY STANDALONE]Cleanup snapshot dir after model run. When the `--workdir` option is set, this option will be ignored.",
@@ -433,15 +436,15 @@
     default="",
     help="runtime uri, model run in the runtime environment process",
 )
 @optgroup.option(  # type: ignore[no-untyped-call]
     "-i",
     "--image",
     default="",
-    help="[ONLY Standalone]docker image, works only when --use-docker is set",
+    help="[ONLY Standalone]docker image, works only when --in-container  is set",
 )
 @click.option(
     "--version",
     default=None,
     help="Run version",
     hidden=True,
 )
@@ -592,16 +595,18 @@
 @optgroup.option("-u", "--uri", help="Model URI")  # type: ignore[no-untyped-call]
 @click.option(  # type: ignore[no-untyped-call]
     "-f",
     "--model-yaml",
     help="Model yaml path, default use ${MODEL_DIR}/model.yaml file",
 )
 @click.option("-r", "--runtime", default="", help="runtime uri")
-@click.option("--host", default="", help="The host to listen on")
-@click.option("--port", default=8080, help="The port of the server")
+@click.option(
+    "--host", default="127.0.0.1", show_default=True, help="The host to listen on"
+)
+@click.option("--port", default=8080, show_default=True, help="The port of the server")
 @click.option(
     "-fpr",
     "--forbid-packaged-runtime",
     is_flag=True,
     help="[ONLY STANDALONE]Forbid to use packaged runtime in the model",
     hidden=True,
 )
```

### Comparing `starwhale-0.5.8/starwhale/core/model/copy.py` & `starwhale-0.5.9/starwhale/core/model/copy.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/core/model/model.py` & `starwhale-0.5.9/starwhale/core/model/model.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/core/model/store.py` & `starwhale-0.5.9/starwhale/core/model/store.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/core/model/view.py` & `starwhale-0.5.9/starwhale/core/model/view.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/core/project/cli.py` & `starwhale-0.5.9/starwhale/core/project/cli.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/core/project/model.py` & `starwhale-0.5.9/starwhale/core/project/model.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/core/project/view.py` & `starwhale-0.5.9/starwhale/core/project/view.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/core/runtime/cli.py` & `starwhale-0.5.9/starwhale/core/runtime/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
     "--include-local-wheel",
     is_flag=True,
     help="Include local wheel packages",
     hidden=True,
 )
 @optgroup.group(
     "\n  ** Conda/Venv/Shell Sources Configurations",
-    help="The configurations only work for `--from-conda-name`, `--from-conda-prefix-path`, `--from-venv-prefix-path` and `--from-shell` sources",
+    help="The configurations only work for `--conda`, `--conda-prefix`, `--venv` and `--shell` sources",
 )
 @optgroup.option(  # type: ignore[no-untyped-call]
     "--cuda",
     type=click.Choice(_SUPPORT_CUDA + [""], case_sensitive=False),
     default="",
     help="cuda version, works for shell, conda name, conda prefix path and venv prefix path sources",
 )
@@ -230,14 +230,22 @@
     type=click.Choice(
         [SupportArch.AMD64, SupportArch.ARM64, SupportArch.NOARCH],
         case_sensitive=False,
     ),
     default=SupportArch.NOARCH,
     help="system architecture, works for shell, conda name, conda prefix path and venv prefix path sources",
 )
+@optgroup.group("\n  ** Global Configurations")
+@optgroup.option("-n", "--name", default="", help="runtime name")  # type: ignore[no-untyped-call]
+@optgroup.option(  # type: ignore[no-untyped-call]
+    "-p",
+    "--project",
+    default="",
+    help="Project URI, default is the current selected project. The runtime package will store in the specified project.",
+)
 @optgroup.option(  # type: ignore[no-untyped-call]
     "-dad",
     "--download-all-deps",
     is_flag=True,
     help="Download all python dependencies into the runtime bundle file, the file size of swrt maybe very large.",
     hidden=True,
 )
@@ -263,22 +271,14 @@
 @optgroup.option(  # type: ignore[no-untyped-call]
     "-ilw",
     "--include-local-wheel",
     is_flag=True,
     help="Include local wheel packages",
     hidden=True,
 )
-@optgroup.group("\n  ** Global Configurations")
-@optgroup.option("-n", "--name", default="", help="runtime name")  # type: ignore[no-untyped-call]
-@optgroup.option(  # type: ignore[no-untyped-call]
-    "-p",
-    "--project",
-    default="",
-    help="Project URI, default is the current selected project. The runtime package will store in the specified project.",
-)
 def _build(
     name: str,
     project: str,
     cuda: str,
     cudnn: str,
     arch: str,
     download_all_deps: bool,
```

### Comparing `starwhale-0.5.8/starwhale/core/runtime/model.py` & `starwhale-0.5.9/starwhale/core/runtime/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,24 +36,24 @@
     SW_IMAGE_FMT,
     CREATED_AT_KEY,
     DEFAULT_PROJECT,
     DefaultYAMLName,
     SW_AUTO_DIRNAME,
     DEFAULT_PAGE_IDX,
     SW_PYPI_PKG_NAME,
-    DEFAULT_IMAGE_TAG,
     DEFAULT_PAGE_SIZE,
     ENV_SW_IMAGE_REPO,
     DEFAULT_IMAGE_NAME,
     DEFAULT_IMAGE_REPO,
     STANDALONE_INSTANCE,
     SW_DEV_DUMMY_VERSION,
     WHEEL_FILE_EXTENSION,
     DEFAULT_CONDA_CHANNEL,
     DEFAULT_MANIFEST_NAME,
+    FIXED_RELEASE_BASE_IMAGE_VERSION,
 )
 from starwhale.version import STARWHALE_VERSION
 from starwhale.base.tag import StandaloneTag
 from starwhale.utils.fs import (
     move_dir,
     empty_dir,
     ensure_dir,
@@ -1272,19 +1272,21 @@
                 _dest_name,
             )
 
     def _dump_docker_image(self, config: RuntimeConfig) -> None:
         custom_run_image = config.environment.docker.image
 
         image = DEFAULT_IMAGE_NAME
-        tag = DEFAULT_IMAGE_TAG
+        tag = os.environ.get(
+            "SW_CUSTOM_BASE_IMAGE_VERSION", FIXED_RELEASE_BASE_IMAGE_VERSION
+        )
         _cuda = config.environment.cuda
         _cudnn = config.environment.cudnn
         if _cuda:
-            # star-whale/cuda:11.5-cudnn8-base0.3.0
+            # star-whale/cuda:11.5-cudnn8-base0.3.4
             _tags = [_cuda]
 
             if _cudnn:
                 _tags.append(f"-cudnn{_cudnn}")
             _tags.append(f"-base{tag}")
 
             image = "cuda"
@@ -1303,21 +1305,21 @@
             )
 
         # Deprecated: base_image field works for controller server <=0.4.6. Prefer using image configured in runtime.yaml
         self._manifest["base_image"] = custom_run_image or builtin_run_image
         self._manifest["docker"] = {
             "custom_run_image": custom_run_image,
             # builtin run image example:
-            # - fullname = docker-registry.starwhale.cn/star-whale/starwhale:0.4.5-cuda11.7
+            # - fullname = docker-registry.starwhale.cn/star-whale/cuda:11.7-base0.3.4
             # - repo = docker-registry.starwhale.cn/star-whale
-            # - name = starwhale
-            # - tag = 0.4.5-cuda11.7
+            # - name = cuda
+            # - tag = 11.7-base0.3.4
             "builtin_run_image": {
                 "repo": repo,
-                "name": DEFAULT_IMAGE_NAME,
+                "name": image,
                 "tag": tag,
                 "fullname": builtin_run_image,
             },
         }
 
     def _lock_environment(
         self,
```

### Comparing `starwhale-0.5.8/starwhale/core/runtime/process.py` & `starwhale-0.5.9/starwhale/core/runtime/process.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/core/runtime/store.py` & `starwhale-0.5.9/starwhale/core/runtime/store.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/core/runtime/template/Dockerfile.tmpl` & `starwhale-0.5.9/starwhale/core/runtime/template/Dockerfile.tmpl`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/core/runtime/view.py` & `starwhale-0.5.9/starwhale/core/runtime/view.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/integrations/huggingface/dataset.py` & `starwhale-0.5.9/starwhale/integrations/huggingface/dataset.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/integrations/pytorch/dataset.py` & `starwhale-0.5.9/starwhale/integrations/pytorch/dataset.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/integrations/tensorflow/dataset.py` & `starwhale-0.5.9/starwhale/integrations/tensorflow/dataset.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/mngt/__init__.py` & `starwhale-0.5.9/starwhale/mngt/__init__.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/proto_gen/model_package_storage_pb2.py` & `starwhale-0.5.9/starwhale/proto_gen/model_package_storage_pb2.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/utils/__init__.py` & `starwhale-0.5.9/starwhale/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/utils/cli.py` & `starwhale-0.5.9/starwhale/utils/cli.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/utils/config.py` & `starwhale-0.5.9/starwhale/utils/config.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/utils/console.py` & `starwhale-0.5.9/starwhale/utils/console.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/utils/debug.py` & `starwhale-0.5.9/starwhale/utils/debug.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/utils/dict_util.py` & `starwhale-0.5.9/starwhale/utils/dict_util.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/utils/docker.py` & `starwhale-0.5.9/starwhale/utils/docker.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/utils/error.py` & `starwhale-0.5.9/starwhale/utils/error.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/utils/fs.py` & `starwhale-0.5.9/starwhale/utils/fs.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/utils/http.py` & `starwhale-0.5.9/starwhale/utils/http.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/utils/load.py` & `starwhale-0.5.9/starwhale/utils/load.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/utils/log.py` & `starwhale-0.5.9/starwhale/utils/log.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/utils/process.py` & `starwhale-0.5.9/starwhale/utils/process.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/utils/progress.py` & `starwhale-0.5.9/starwhale/utils/progress.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/utils/retry.py` & `starwhale-0.5.9/starwhale/utils/retry.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/utils/venv.py` & `starwhale-0.5.9/starwhale/utils/venv.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/utils/venv_pack.py` & `starwhale-0.5.9/starwhale/utils/venv_pack.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/data_store.py` & `starwhale-0.5.9/starwhale/web/data_store.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/panel.py` & `starwhale-0.5.9/starwhale/web/panel.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/project.py` & `starwhale-0.5.9/starwhale/web/project.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/server.py` & `starwhale-0.5.9/starwhale/web/server.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/BlockLabel-cddc2b81.js` & `starwhale-0.5.9/starwhale/web/ui/assets/BlockLabel-10abb1b4.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -13,15 +13,15 @@
     W as p,
     Y as I,
     Z as k,
     $ as v,
     a0 as z,
     a1 as B,
     ax as L
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function q(a) {
     let t, n, s, b, o, r, l;
     return s = new a[1]({}), {
         c() {
             t = u("div"), n = u("span"), h(s.$$.fragment), b = y(), o = w(a[0]), f(n, "class", "mr-2 h-[12px] w-[12px] opacity-80"), f(t, "class", r = "absolute left-0 top-0 py-1 px-2 rounded-br-lg shadow-sm text-xs text-gray-500 flex items-center pointer-events-none bg-white z-20 border-b border-r border-gray-100 dark:bg-gray-900 " + a[3]), c(t, "h-0", !a[2]), c(t, "sr-only", !a[2])
         },
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/CarouselItem.svelte_svelte_type_style_lang-08c76e7c.js` & `starwhale-0.5.9/starwhale/web/ui/assets/CarouselItem.svelte_svelte_type_style_lang-4dd9c624.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -20,15 +20,15 @@
     a0 as K,
     ap as N,
     a9 as Q,
     a7 as A,
     az as R,
     aA as U,
     aB as E
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function V(l) {
     let t, o, e, u, L, f, m = l[2] + 1 + "",
         v, p, _ = l[3].length + "",
         d, b, i, r, x, a;
     const w = l[9].default,
         n = q(w, l, l[8], null);
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/Column-07457f7d.js` & `starwhale-0.5.9/starwhale/web/ui/assets/Column-a843ed59.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
     Q as C,
     a3 as Z,
     a4 as q,
     a5 as F,
     Z as G,
     $ as H,
     a0 as J
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function N(a) {
     let e, t, m, f;
     const o = a[7].default,
         i = w(o, a, a[6], null);
     return {
         c() {
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/DatasetForm-aac5cbbf.js` & `starwhale-0.5.9/starwhale/web/ui/assets/DatasetForm-6dd7af50.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -26,15 +26,15 @@
     o as Lr,
     p as Br,
     U as zr,
     q as Mr,
     S as Nr,
     t as Ur,
     v as Vr
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 const Xt = e => e.type?.startsWith("image") ? "IMAGE" : e.type?.startsWith("video") ? "VIDEO" : e.type?.startsWith("audio") ? "AUDIO" : e.name?.includes(".csv") ? "CSV" : e.name?.includes(".json") ? "JSON" : e.name?.includes(".jsonL") ? "JSONL" : "",
     Te = e => e ? e.path ? e.path : e.originFileObj ? e.originFileObj?.webkitRelativePath ?? e.name : e.webkitRelativePath ?? e.name : "";
 
 function Ot(e) {
     const t = {};
     for (let o = 0; o < e.length; o++) {
         const i = Xt(e[o]);
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/File-15836fc4.js` & `starwhale-0.5.9/starwhale/web/ui/assets/File-220c5e21.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
     H as d,
     al as o,
     N as t,
     Q as f,
     V as l,
     am as r,
     a0 as u
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function m(i) {
     let e, a, s;
     return {
         c() {
             e = o("svg"), a = o("path"), s = o("polyline"), t(a, "d", "M13 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V9z"), t(s, "points", "13 2 13 9 20 9"), t(e, "xmlns", "http://www.w3.org/2000/svg"), t(e, "width", "100%"), t(e, "height", "100%"), t(e, "viewBox", "0 0 24 24"), t(e, "fill", "none"), t(e, "stroke", "currentColor"), t(e, "stroke-width", "1.5"), t(e, "stroke-linecap", "round"), t(e, "stroke-linejoin", "round"), t(e, "class", "feather feather-file")
         },
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/Image-aea3de20.js` & `starwhale-0.5.9/starwhale/web/ui/assets/Image-2df538c6.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
     H as o,
     J as _,
     N as n,
     an as l,
     Q as f,
     am as m,
     a0 as g
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function d(i) {
     let e, s;
     return {
         c() {
             e = _("img"), n(e, "class", "gr-sample-image object-contain h-20 w-20"), l(e.src, s = i[0]) || n(e, "src", s)
         },
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/Image2-1419ace7.js` & `starwhale-0.5.9/starwhale/web/ui/assets/Image2-bbb64300.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
     H as m,
     al as a,
     N as e,
     Q as d,
     V as i,
     am as l,
     a0 as u
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function f(c) {
     let t, r, s, n;
     return {
         c() {
             t = a("svg"), r = a("rect"), s = a("circle"), n = a("polyline"), e(r, "x", "3"), e(r, "y", "3"), e(r, "width", "18"), e(r, "height", "18"), e(r, "rx", "2"), e(r, "ry", "2"), e(s, "cx", "8.5"), e(s, "cy", "8.5"), e(s, "r", "1.5"), e(n, "points", "21 15 16 10 5 21"), e(t, "xmlns", "http://www.w3.org/2000/svg"), e(t, "width", "100%"), e(t, "height", "100%"), e(t, "viewBox", "0 0 24 24"), e(t, "fill", "none"), e(t, "stroke", "currentColor"), e(t, "stroke-width", "1.5"), e(t, "stroke-linecap", "round"), e(t, "stroke-linejoin", "round"), e(t, "class", "feather feather-image")
         },
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/LogViewer-b5684b3d.css` & `starwhale-0.5.9/starwhale/web/ui/assets/LogViewer-b5684b3d.css`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/LogViewer-f5bb7317.js` & `starwhale-0.5.9/starwhale/web/ui/assets/LogViewer-e1f101c5.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
     x as z,
     y as Zn,
     R as oe,
     z as Tr,
     k as pl,
     u as fl,
     A as dl
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 const Rr = x.createContext(null),
     To = x.createContext(null);
 
 function S(...e) {
     const t = [],
         n = {}.hasOwnProperty;
     return e.filter(Boolean).forEach(r => {
@@ -7979,15 +7979,15 @@
     onClose: n,
     onMessage: r
 }) {
     const s = x.useRef(void 0),
         o = x.useRef(void 0);
     x.useEffect(() => {
         const i = {
-            GIT_COMMIT_HASH: '"8d5dff52e757f1974b0ea9ea13a7efe032d7e50f"'
+            GIT_COMMIT_HASH: '"8b2b3adf40f05a1b24655cc34df5c624f68f09af"'
         }.DEBUG ? pl.bind(console.log, console, "[useWebSocket]") : (...p) => {};
         if (i("use effect", e), !e) return;
         o.current && (i("prev closed", o.current), o.current.close());
         const l = new WebSocket(e);
         o.current = l;
         const a = () => {
                 l?.readyState === l?.OPEN && l?.send("ping"), s.current = window.setTimeout(a, 2e3)
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/Markdown-d8dda0b2.css` & `starwhale-0.5.9/starwhale/web/ui/assets/Markdown-d8dda0b2.css`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/Markdown-fdfce605.js` & `starwhale-0.5.9/starwhale/web/ui/assets/Markdown-2b316973.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     C as me,
     R as Xn,
     D as ar,
     j as _n,
     P as T
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 const Te = ["http", "https", "mailto", "tel"];
 
 function jn(n) {
     const e = (n || "").trim(),
         t = e.charAt(0);
     if (t === "#" || t === "/") return e;
     const r = e.indexOf(":");
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/ModifyUpload-768fe082.js` & `starwhale-0.5.9/starwhale/web/ui/assets/ModifyUpload-e3ca444a.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -18,15 +18,15 @@
     a1 as $,
     a9 as B,
     am as f,
     X as E,
     al as g,
     aN as u,
     ah as N
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function q(o) {
     let e, a, t, l, n, r;
     return t = new o[0]({}), {
         c() {
             e = x("button"), a = x("div"), y(t.$$.fragment), s(a, "class", "m-t-1 w-[60%] h-[60%] opacity-80 dark:text-white"), s(e, "class", "text-gray-500 bg-white/90 h-5 w-5 flex items-center justify-center rounded shadow-sm hover:shadow-xl hover:ring-1 ring-inset ring-gray-200 z-10 dark:bg-gray-900 dark:ring-gray-600"), s(e, "aria-label", o[1])
         },
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/RedHatDisplay-Bold-44214a55.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/RedHatDisplay-Bold-44214a55.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/RedHatDisplay-Bold-ca18645c.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/RedHatDisplay-Bold-ca18645c.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/RedHatDisplay-Medium-6ccf2158.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/RedHatDisplay-Medium-6ccf2158.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/RedHatDisplay-Medium-6d3ccc0f.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/RedHatDisplay-Medium-6d3ccc0f.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/RedHatDisplay-Regular-1b99a560.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/RedHatDisplay-Regular-1b99a560.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/RedHatDisplay-Regular-e6fb83d9.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/RedHatDisplay-Regular-e6fb83d9.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/RedHatDisplay-updated-Bold-66d1fc26.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/RedHatDisplay-updated-Bold-66d1fc26.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/RedHatDisplay-updated-Medium-da0621a9.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/RedHatDisplay-updated-Medium-da0621a9.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/RedHatDisplay-updated-Regular-d0b90ff3.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/RedHatDisplay-updated-Regular-d0b90ff3.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/RedHatDisplayVF-updated-ItalicModified-8483eece.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/RedHatDisplayVF-updated-ItalicModified-8483eece.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/RedHatDisplayVFModified-updated-3a6592a3.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/RedHatDisplayVFModified-updated-3a6592a3.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/RedHatMono-updated-Regular-1686cd5c.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/RedHatMono-updated-Regular-1686cd5c.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/RedHatMonoVF-updated-4cca9c27.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/RedHatMonoVF-updated-4cca9c27.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/RedHatMonoVF-updated-Italic-ca135ebd.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/RedHatMonoVF-updated-Italic-ca135ebd.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/RedHatText-Medium-702e86ff.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/RedHatText-Medium-702e86ff.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/RedHatText-Medium-eb14b046.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/RedHatText-Medium-eb14b046.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/RedHatText-Regular-542423d0.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/RedHatText-Regular-542423d0.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/RedHatText-Regular-df36d7d0.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/RedHatText-Regular-df36d7d0.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/RedHatText-updated-Medium-721ddd64.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/RedHatText-updated-Medium-721ddd64.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/RedHatText-updated-Regular-2e08dbe8.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/RedHatText-updated-Regular-2e08dbe8.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/RedHatTextVF-updated-ItalicModified-9e1c1004.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/RedHatTextVF-updated-ItalicModified-9e1c1004.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/RedHatTextVFModified-updated-942d38f7.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/RedHatTextVFModified-updated-942d38f7.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/Tabs-fc1af0f2.js` & `starwhale-0.5.9/starwhale/web/ui/assets/Tabs-6664f57a.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
     ac as C,
     b0 as X,
     aB as Y,
     aA as Z,
     K as S,
     X as j,
     Y as q
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function K(n, e, s) {
     const t = n.slice();
     return t[11] = e[s], t
 }
 
 function P(n) {
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/Upload-0cd7f439.js` & `starwhale-0.5.9/starwhale/web/ui/assets/Upload-6d14b4a6.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -18,15 +18,15 @@
     Z as x,
     $,
     a0 as ee,
     ap as le,
     a9 as te,
     ah as y,
     ak as ae
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function ie(t) {
     let l, i, n, g, h, c, o, d, k, F;
     const _ = t[14].default,
         r = I(_, t, t[13], null);
     return {
         c() {
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/Webcam-37a04310.js` & `starwhale-0.5.9/starwhale/web/ui/assets/Webcam-d64f2534.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -20,15 +20,15 @@
     ak as Qe,
     al as W,
     am as I,
     M as Gt,
     W as qt,
     a1 as Ft,
     ac as Ze
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function Ke(a) {
     let t, e, i;
     return {
         c() {
             t = W("svg"), e = W("path"), i = W("circle"), p(e, "d", "M23 19a2 2 0 0 1-2 2H3a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h4l2-3h6l2 3h4a2 2 0 0 1 2 2z"), p(i, "cx", "12"), p(i, "cy", "13"), p(i, "r", "4"), p(t, "xmlns", "http://www.w3.org/2000/svg"), p(t, "width", "100%"), p(t, "height", "100%"), p(t, "viewBox", "0 0 24 24"), p(t, "fill", "none"), p(t, "stroke", "currentColor"), p(t, "stroke-width", "1.5"), p(t, "stroke-linecap", "round"), p(t, "stroke-linejoin", "round"), p(t, "class", "feather feather-camera")
         },
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/account2-668f906e.svg` & `starwhale-0.5.9/starwhale/web/ui/assets/account2-668f906e.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/dsv-62f8cd07.js` & `starwhale-0.5.9/starwhale/web/ui/assets/dsv-62f8cd07.js`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/empty-chart-1e62901a.svg` & `starwhale-0.5.9/starwhale/web/ui/assets/empty-chart-1e62901a.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/empty-f3091520.svg` & `starwhale-0.5.9/starwhale/web/ui/assets/empty-f3091520.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/google-9d1a8b2b.svg` & `starwhale-0.5.9/starwhale/web/ui/assets/google-9d1a8b2b.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index-3bbbd54b.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index-df1fb029.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -84935,15 +84935,15 @@
         }
     }, [r, n]);
     const x = S.useMemo(() => a.map((R, C) => d.jsx(wge, {
         id: R.id,
         type: R.type,
         path: [C],
         childWidgets: R.children
-    }, R.id)), [a]);
+    }, R.id ?? C)), [a]);
     return d.jsxs("div", {
         children: [x, d.jsx(SD0, {
             form: m.current,
             id: s?.payload?.id,
             isShow: c,
             setIsShow: u,
             store: r,
@@ -95391,15 +95391,15 @@
             options: xne,
             style: {
                 height: "100px"
             }
         })
     })
 }
-const S90 = j.lazy(() => T0(() => import("./main-99f2bbfd.js").then(e => e.m), []));
+const S90 = j.lazy(() => T0(() => import("./main-e0f2ffda.js").then(e => e.m), []));
 
 function cO({
     data: e,
     collapsed: t = 1,
     collapseStringsAfterLength: r = 10,
     style: n = {}
 }) {
@@ -98408,15 +98408,15 @@
             type: "heatmap"
         }],
         layout: {
             ...o
         }
     }
 }
-const pD0 = j.lazy(() => T0(() => import("./index-af425f4b.js"), ["assets/index-af425f4b.js", "assets/index-4b525ef6.css"])),
+const pD0 = j.lazy(() => T0(() => import("./index-e17166cd.js"), ["assets/index-e17166cd.js", "assets/index-4b525ef6.css"])),
     dD0 = {
         type: "ui:panel:rocauc",
         group: ab.PANEL,
         name: "Roc Auc",
         fieldConfig: {
             schema: {
                 tableName: {},
@@ -98462,15 +98462,15 @@
         children: d.jsx(pD0, {
             data: u
         })
     })
 }
 const bD0 = new q3(fD0, dD0),
     hD0 = bD0,
-    MD0 = j.lazy(() => T0(() => import("./index-af425f4b.js"), ["assets/index-af425f4b.js", "assets/index-4b525ef6.css"])),
+    MD0 = j.lazy(() => T0(() => import("./index-e17166cd.js"), ["assets/index-e17166cd.js", "assets/index-4b525ef6.css"])),
     mD0 = {
         type: "ui:panel:confusion_matrix",
         group: ab.PANEL,
         name: "Confusion Matrix"
     };
 
 function gD0(e) {
@@ -106206,15 +106206,15 @@
     return d.jsx(g1, {
         title: t("Run Model"),
         children: d.jsx(wX, {
             onSubmit: r
         })
     })
 }
-const LY0 = j.lazy(() => T0(() => import("./DatasetForm-aac5cbbf.js"), []));
+const LY0 = j.lazy(() => T0(() => import("./DatasetForm-6dd7af50.js"), []));
 
 function $Y0() {
     const {
         projectId: e,
         datasetId: t
     } = Tt(), {
         query: r
@@ -106455,15 +106455,15 @@
                     job: n,
                     task: c
                 })
             })]
         })]
     })
 }
-const IY0 = j.lazy(() => T0(() => import("./LogViewer-f5bb7317.js"), ["assets/LogViewer-f5bb7317.js", "assets/LogViewer-b5684b3d.css"]));
+const IY0 = j.lazy(() => T0(() => import("./LogViewer-e1f101c5.js"), ["assets/LogViewer-e1f101c5.js", "assets/LogViewer-b5684b3d.css"]));
 
 function woe() {
     const [e] = Ee(), [t, r] = S.useState(void 0), [, n] = S.useState(!1), [o, i] = S.useState({}), a = S.useCallback(async (c, u) => {
         r(u);
         const p = {};
         if ([nw.RUNNING].includes(u.taskStatus)) {
             const b = [u?.stepName, u?.id].join("@");
@@ -116520,53 +116520,53 @@
     ntt = (e, t = Qp()) => Hve(e, t),
     ont = TM([EM, j3], () => J0t);
 TM([EM], () => ett);
 TM([EM], () => ttt);
 TM([EM], () => rtt);
 TM([EM, j3], () => ntt);
 const ott = {
-    accordion: () => T0(() => import("./index-890d4a46.js"), ["assets/index-890d4a46.js", "assets/Column-07457f7d.js"]),
-    audio: () => T0(() => import("./index2-d042f67b.js"), ["assets/index2-d042f67b.js", "assets/Upload-0cd7f439.js", "assets/ModifyUpload-768fe082.js", "assets/BlockLabel-cddc2b81.js", "assets/utils-de54785e.js"]),
-    box: () => T0(() => import("./index3-b8136165.js"), []),
-    button: () => T0(() => import("./index4-d076a84c.js"), []),
-    carousel: () => T0(() => import("./index5-529df1c0.js"), ["assets/index5-529df1c0.js", "assets/CarouselItem.svelte_svelte_type_style_lang-08c76e7c.js"]),
-    carouselitem: () => T0(() => import("./index6-be007bee.js"), ["assets/index6-be007bee.js", "assets/CarouselItem.svelte_svelte_type_style_lang-08c76e7c.js"]),
-    chatbot: () => T0(() => import("./index7-c3badb00.js"), ["assets/index7-c3badb00.js", "assets/BlockLabel-cddc2b81.js"]),
-    checkbox: () => T0(() => import("./index8-2bbdfede.js"), []),
-    checkboxgroup: () => T0(() => import("./index9-0cbe1428.js"), []),
-    colorpicker: () => T0(() => import("./index10-4d13164f.js"), []),
-    column: () => T0(() => import("./index11-13eb176d.js"), ["assets/index11-13eb176d.js", "assets/Column-07457f7d.js"]),
-    dataframe: () => T0(() => import("./index12-de21ca8a.js"), ["assets/index12-de21ca8a.js", "assets/Upload-0cd7f439.js", "assets/dsv-62f8cd07.js"]),
-    dataset: () => T0(() => import("./index13-0661cc45.js"), ["assets/index13-0661cc45.js", "assets/Image-aea3de20.js", "assets/csv-17a3ae92.js", "assets/dsv-62f8cd07.js", "assets/Model3D-fba04936.js"]),
-    dropdown: () => T0(() => import("./index14-e2afac41.js"), []),
-    file: () => T0(() => import("./index15-9ee1eee9.js"), ["assets/index15-9ee1eee9.js", "assets/BlockLabel-cddc2b81.js", "assets/File-15836fc4.js", "assets/Upload-0cd7f439.js", "assets/ModifyUpload-768fe082.js", "assets/utils-de54785e.js"]),
-    form: () => T0(() => import("./index16-a0351c35.js"), []),
-    gallery: () => T0(() => import("./index17-a75792cc.js"), ["assets/index17-a75792cc.js", "assets/BlockLabel-cddc2b81.js", "assets/ModifyUpload-768fe082.js", "assets/utils-de54785e.js", "assets/Image2-1419ace7.js"]),
-    group: () => T0(() => import("./index18-0b10ab02.js"), []),
-    highlightedtext: () => T0(() => import("./index19-ceded876.js"), ["assets/index19-ceded876.js", "assets/color-07ebf074.js", "assets/BlockLabel-cddc2b81.js"]),
-    html: () => T0(() => import("./index20-d0bcc869.js"), []),
-    image: () => T0(() => import("./index21-d2f402e4.js"), ["assets/index21-d2f402e4.js", "assets/BlockLabel-cddc2b81.js", "assets/Image2-1419ace7.js", "assets/Webcam-37a04310.js", "assets/ModifyUpload-768fe082.js", "assets/Upload-0cd7f439.js", "assets/Image-aea3de20.js"]),
-    interpretation: () => T0(() => import("./index22-c5e0b0dd.js"), []),
-    json: () => T0(() => import("./index23-e492630c.js"), ["assets/index23-e492630c.js", "assets/BlockLabel-cddc2b81.js"]),
-    label: () => T0(() => import("./index24-1c64b765.js"), ["assets/index24-1c64b765.js", "assets/BlockLabel-cddc2b81.js"]),
-    markdown: () => T0(() => import("./index25-33571440.js"), []),
-    model3d: () => T0(() => import("./index26-d78d751e.js"), ["assets/index26-d78d751e.js", "assets/utils-de54785e.js", "assets/BlockLabel-cddc2b81.js", "assets/File-15836fc4.js", "assets/_commonjsHelpers-23156833.js", "assets/Upload-0cd7f439.js", "assets/ModifyUpload-768fe082.js", "assets/Model3D-fba04936.js"]),
-    number: () => T0(() => import("./index27-18127a28.js"), []),
-    plot: () => T0(() => import("./index28-34a5ed1a.js"), ["assets/index28-34a5ed1a.js", "assets/_commonjsHelpers-23156833.js", "assets/color-07ebf074.js", "assets/linear-8d973619.js", "assets/dsv-62f8cd07.js", "assets/BlockLabel-cddc2b81.js"]),
-    radio: () => T0(() => import("./index29-e4ca565e.js"), []),
-    row: () => T0(() => import("./index30-334d010c.js"), []),
-    slider: () => T0(() => import("./index31-1121988e.js"), []),
-    state: () => T0(() => import("./index32-80223294.js"), []),
-    statustracker: () => T0(() => import("./index33-a4713f90.js"), []),
-    tabs: () => T0(() => import("./index34-69d671c0.js"), ["assets/index34-69d671c0.js", "assets/Tabs-fc1af0f2.js"]),
-    tabitem: () => T0(() => import("./index35-91b6f450.js"), ["assets/index35-91b6f450.js", "assets/Tabs-fc1af0f2.js", "assets/Column-07457f7d.js"]),
-    textbox: () => T0(() => import("./index36-6ce81ba8.js"), []),
-    timeseries: () => T0(() => import("./index37-f530c08a.js"), ["assets/index37-f530c08a.js", "assets/Upload-0cd7f439.js", "assets/ModifyUpload-768fe082.js", "assets/BlockLabel-cddc2b81.js", "assets/color-07ebf074.js", "assets/linear-8d973619.js", "assets/csv-17a3ae92.js", "assets/dsv-62f8cd07.js"]),
-    uploadbutton: () => T0(() => import("./index38-fc6af5aa.js"), []),
-    video: () => T0(() => import("./index39-671ded20.js"), ["assets/index39-671ded20.js", "assets/utils-de54785e.js", "assets/Upload-0cd7f439.js", "assets/ModifyUpload-768fe082.js", "assets/BlockLabel-cddc2b81.js", "assets/Webcam-37a04310.js"])
+    accordion: () => T0(() => import("./index-87b297cf.js"), ["assets/index-87b297cf.js", "assets/Column-a843ed59.js"]),
+    audio: () => T0(() => import("./index2-667148f0.js"), ["assets/index2-667148f0.js", "assets/Upload-6d14b4a6.js", "assets/ModifyUpload-e3ca444a.js", "assets/BlockLabel-10abb1b4.js", "assets/utils-de54785e.js"]),
+    box: () => T0(() => import("./index3-b632de7a.js"), []),
+    button: () => T0(() => import("./index4-2684c49d.js"), []),
+    carousel: () => T0(() => import("./index5-264c6674.js"), ["assets/index5-264c6674.js", "assets/CarouselItem.svelte_svelte_type_style_lang-4dd9c624.js"]),
+    carouselitem: () => T0(() => import("./index6-b60485d2.js"), ["assets/index6-b60485d2.js", "assets/CarouselItem.svelte_svelte_type_style_lang-4dd9c624.js"]),
+    chatbot: () => T0(() => import("./index7-ae38a6d6.js"), ["assets/index7-ae38a6d6.js", "assets/BlockLabel-10abb1b4.js"]),
+    checkbox: () => T0(() => import("./index8-5ee4cbfe.js"), []),
+    checkboxgroup: () => T0(() => import("./index9-f552db0e.js"), []),
+    colorpicker: () => T0(() => import("./index10-7aed280d.js"), []),
+    column: () => T0(() => import("./index11-df7b8b7d.js"), ["assets/index11-df7b8b7d.js", "assets/Column-a843ed59.js"]),
+    dataframe: () => T0(() => import("./index12-f581388d.js"), ["assets/index12-f581388d.js", "assets/Upload-6d14b4a6.js", "assets/dsv-62f8cd07.js"]),
+    dataset: () => T0(() => import("./index13-fd2d632d.js"), ["assets/index13-fd2d632d.js", "assets/Image-2df538c6.js", "assets/csv-17a3ae92.js", "assets/dsv-62f8cd07.js", "assets/Model3D-d49eae09.js"]),
+    dropdown: () => T0(() => import("./index14-94c12d28.js"), []),
+    file: () => T0(() => import("./index15-a31493a5.js"), ["assets/index15-a31493a5.js", "assets/BlockLabel-10abb1b4.js", "assets/File-220c5e21.js", "assets/Upload-6d14b4a6.js", "assets/ModifyUpload-e3ca444a.js", "assets/utils-de54785e.js"]),
+    form: () => T0(() => import("./index16-2b049823.js"), []),
+    gallery: () => T0(() => import("./index17-d4811bf1.js"), ["assets/index17-d4811bf1.js", "assets/BlockLabel-10abb1b4.js", "assets/ModifyUpload-e3ca444a.js", "assets/utils-de54785e.js", "assets/Image2-bbb64300.js"]),
+    group: () => T0(() => import("./index18-d4ad6d1d.js"), []),
+    highlightedtext: () => T0(() => import("./index19-18249feb.js"), ["assets/index19-18249feb.js", "assets/color-2fcdd2a9.js", "assets/BlockLabel-10abb1b4.js"]),
+    html: () => T0(() => import("./index20-0cc28676.js"), []),
+    image: () => T0(() => import("./index21-d3e36a16.js"), ["assets/index21-d3e36a16.js", "assets/BlockLabel-10abb1b4.js", "assets/Image2-bbb64300.js", "assets/Webcam-d64f2534.js", "assets/ModifyUpload-e3ca444a.js", "assets/Upload-6d14b4a6.js", "assets/Image-2df538c6.js"]),
+    interpretation: () => T0(() => import("./index22-34fa8df0.js"), []),
+    json: () => T0(() => import("./index23-b30a6092.js"), ["assets/index23-b30a6092.js", "assets/BlockLabel-10abb1b4.js"]),
+    label: () => T0(() => import("./index24-11b8d91d.js"), ["assets/index24-11b8d91d.js", "assets/BlockLabel-10abb1b4.js"]),
+    markdown: () => T0(() => import("./index25-4151ca38.js"), []),
+    model3d: () => T0(() => import("./index26-2968ddd0.js"), ["assets/index26-2968ddd0.js", "assets/utils-de54785e.js", "assets/BlockLabel-10abb1b4.js", "assets/File-220c5e21.js", "assets/_commonjsHelpers-23156833.js", "assets/Upload-6d14b4a6.js", "assets/ModifyUpload-e3ca444a.js", "assets/Model3D-d49eae09.js"]),
+    number: () => T0(() => import("./index27-86c85604.js"), []),
+    plot: () => T0(() => import("./index28-fce682a3.js"), ["assets/index28-fce682a3.js", "assets/_commonjsHelpers-23156833.js", "assets/color-2fcdd2a9.js", "assets/linear-8d973619.js", "assets/dsv-62f8cd07.js", "assets/BlockLabel-10abb1b4.js"]),
+    radio: () => T0(() => import("./index29-7f2f8cac.js"), []),
+    row: () => T0(() => import("./index30-449fed8c.js"), []),
+    slider: () => T0(() => import("./index31-a39e3c8b.js"), []),
+    state: () => T0(() => import("./index32-5e251911.js"), []),
+    statustracker: () => T0(() => import("./index33-8befa193.js"), []),
+    tabs: () => T0(() => import("./index34-d9e154ad.js"), ["assets/index34-d9e154ad.js", "assets/Tabs-6664f57a.js"]),
+    tabitem: () => T0(() => import("./index35-71968f90.js"), ["assets/index35-71968f90.js", "assets/Tabs-6664f57a.js", "assets/Column-a843ed59.js"]),
+    textbox: () => T0(() => import("./index36-6d6222b1.js"), []),
+    timeseries: () => T0(() => import("./index37-03da10b3.js"), ["assets/index37-03da10b3.js", "assets/Upload-6d14b4a6.js", "assets/ModifyUpload-e3ca444a.js", "assets/BlockLabel-10abb1b4.js", "assets/color-2fcdd2a9.js", "assets/linear-8d973619.js", "assets/csv-17a3ae92.js", "assets/dsv-62f8cd07.js"]),
+    uploadbutton: () => T0(() => import("./index38-f8a193c1.js"), []),
+    video: () => T0(() => import("./index39-c97fb654.js"), ["assets/index39-c97fb654.js", "assets/utils-de54785e.js", "assets/Upload-6d14b4a6.js", "assets/ModifyUpload-e3ca444a.js", "assets/BlockLabel-10abb1b4.js", "assets/Webcam-d64f2534.js"])
 };
 
 function itt() {
     const e = bb({}),
         t = [],
         r = [],
         n = new Map,
@@ -121307,15 +121307,15 @@
                     task: u
                 })
             })]
         })]
     })
 }
 var T4e = (e => (e.CREATED = "CREATED", e.UPLOADING = "UPLOADING", e.BUILDING = "BUILDING", e.SUCCESS = "SUCCESS", e.FAILED = "FAILED", e))(T4e || {});
-const yrt = j.lazy(() => T0(() => import("./LogViewer-f5bb7317.js"), ["assets/LogViewer-f5bb7317.js", "assets/LogViewer-b5684b3d.css"]));
+const yrt = j.lazy(() => T0(() => import("./LogViewer-e1f101c5.js"), ["assets/LogViewer-e1f101c5.js", "assets/LogViewer-b5684b3d.css"]));
 
 function Art() {
     const [e] = Ee(), [t, r] = S.useState(void 0), [, n] = S.useState(!1), [o, i] = S.useState({}), a = S.useCallback(async (c, u) => {
         r(u);
         const p = {},
             f = [u?.datasetName, u?.id].join("@");
         if ([T4e.BUILDING].includes(u.status)) p[f] = "ws";
@@ -121374,15 +121374,15 @@
     } = Mve(), n = t?.name, o = r?.name, {
         modelVersionId: i
     } = Tt();
     return {
         content: _0(`fetchModelVersionFile:${n}:${o}:${i}:${e}`, () => xX(n, o, i, To(), e)).data
     }
 }
-const wrt = j.lazy(() => T0(() => import("./Markdown-fdfce605.js"), ["assets/Markdown-fdfce605.js", "assets/Markdown-d8dda0b2.css"]));
+const wrt = j.lazy(() => T0(() => import("./Markdown-2b316973.js"), ["assets/Markdown-2b316973.js", "assets/Markdown-d8dda0b2.css"]));
 
 function xrt() {
     const {
         content: e
     } = qrt("src/README.md");
     return d.jsxs("div", {
         className: "markdown-body flex-column",
@@ -121836,15 +121836,15 @@
                 })
             })
         })
     })
 }
 window.g = null;
 window.i = null;
-console.log('"8d5dff52e757f1974b0ea9ea13a7efe032d7e50f"');
+console.log('"8b2b3adf40f05a1b24655cc34df5c624f68f09af"');
 async function krt() {
     return {}
 }
 async function jrt() {
     const {
         authed: e,
         unauthed: t,
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index-890d4a46.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index-87b297cf.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -17,18 +17,18 @@
     $ as k,
     a0 as J,
     a1 as K,
     a2 as L,
     a3 as M,
     a4 as N,
     a5 as O
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 import {
     C as Q
-} from "./Column-07457f7d.js";
+} from "./Column-a843ed59.js";
 
 function S(a) {
     let e;
     const s = a[6].default,
         t = L(s, a, a[7], null);
     return {
         c() {
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index-af425f4b.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index-e17166cd.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -3,15 +3,15 @@
     r as Ch,
     j as xl,
     b4 as zp,
     b5 as Op,
     b6 as Bp,
     C as Np,
     k as Up
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function Hp({
     style: Go = {},
     isLoading: js = !1,
     className: Gl = "",
     children: wi,
     loaderType: co = "spinner",
@@ -149346,15 +149346,15 @@
 
             function d() {
                 var t;
                 try {
                     t = Z.storage.debug
                 } catch {}
                 return !t && typeof M < "u" && "env" in M && (t = {
-                    GIT_COMMIT_HASH: '"8d5dff52e757f1974b0ea9ea13a7efe032d7e50f"'
+                    GIT_COMMIT_HASH: '"8b2b3adf40f05a1b24655cc34df5c624f68f09af"'
                 }.DEBUG), t
             }
             Z.enable(d());
 
             function g() {
                 try {
                     return window.localStorage
@@ -151439,18 +151439,18 @@
                     return K.apply(this, arguments)
                 }
                 return fe
             };
             var L = {},
                 S = /^$/;
             if ({
-                    GIT_COMMIT_HASH: '"8d5dff52e757f1974b0ea9ea13a7efe032d7e50f"'
+                    GIT_COMMIT_HASH: '"8b2b3adf40f05a1b24655cc34df5c624f68f09af"'
                 }.NODE_DEBUG) {
                 var d = {
-                    GIT_COMMIT_HASH: '"8d5dff52e757f1974b0ea9ea13a7efe032d7e50f"'
+                    GIT_COMMIT_HASH: '"8b2b3adf40f05a1b24655cc34df5c624f68f09af"'
                 }.NODE_DEBUG;
                 d = d.replace(/[|\\{}()[\]^$+?.]/g, "\\$&").replace(/\*/g, ".*").replace(/,/g, "$|^").toUpperCase(), S = new RegExp("^" + d + "$", "i")
             }
             Z.debuglog = function(K) {
                 if (K = K.toUpperCase(), !L[K])
                     if (S.test(K)) {
                         var q = M.pid;
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index-ddbcf299.css` & `starwhale-0.5.9/starwhale/web/ui/assets/index-ddbcf299.css`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index10-4d13164f.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index10-7aed280d.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
     N as y,
     V as G,
     aI as H,
     X as V,
     a9 as W,
     K as X,
     Y
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function Z(a) {
     let e;
     return {
         c() {
             e = X(a[1])
         },
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index12-de21ca8a.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index12-f581388d.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -33,18 +33,18 @@
     aL as oe,
     ag as fe,
     al as ve,
     aI as Ae,
     ah as De,
     ac as ol,
     aE as fl
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 import {
     U as dl
-} from "./Upload-0cd7f439.js";
+} from "./Upload-6d14b4a6.js";
 import {
     d as cl
 } from "./dsv-62f8cd07.js";
 var Le = Object.prototype.hasOwnProperty;
 
 function te(r, e) {
     var l, t;
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index13-0661cc45.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index13-fd2d632d.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -26,27 +26,27 @@
     M as Y,
     W as Z,
     a1 as J,
     ak as He,
     ap as ge,
     an as X,
     aw as U
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 import {
     E as je
-} from "./Image-aea3de20.js";
+} from "./Image-2df538c6.js";
 import {
     c as Ce
 } from "./csv-17a3ae92.js";
 import {
     d as Ae
 } from "./dsv-62f8cd07.js";
 import {
     E as Ee
-} from "./Model3D-fba04936.js";
+} from "./Model3D-d49eae09.js";
 var Le = Ae("	"),
     Ne = Le.parseRows;
 
 function Te(r) {
     let e, t;
     return {
         c() {
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index14-e2afac41.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index14-94c12d28.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -27,15 +27,15 @@
     aP as C,
     X as z,
     at as A,
     a9 as I,
     K as F,
     Y as H,
     aQ as R
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function G(t, l, a) {
     const n = t.slice();
     return n[7] = l[a], n
 }
 
 function U(t) {
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index15-9ee1eee9.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index15-a31493a5.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -29,27 +29,27 @@
     am as K,
     ak as Z,
     aq as O,
     ar as R,
     K as y,
     Y as U,
     at as x
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 import {
     B as $
-} from "./BlockLabel-cddc2b81.js";
+} from "./BlockLabel-10abb1b4.js";
 import {
     F as Q
-} from "./File-15836fc4.js";
+} from "./File-220c5e21.js";
 import {
     U as ee
-} from "./Upload-0cd7f439.js";
+} from "./Upload-6d14b4a6.js";
 import {
     M as de
-} from "./ModifyUpload-768fe082.js";
+} from "./ModifyUpload-e3ca444a.js";
 import {
     n as be
 } from "./utils-de54785e.js";
 const me = a => {
         let e = ["B", "KB", "MB", "GB", "PB"],
             i = 0;
         for (; a > 1024;) a /= 1024, i++;
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index17-a75792cc.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index17-d4811bf1.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -31,27 +31,27 @@
     am as F,
     an as M,
     aN as X,
     at as ae,
     ap as Le,
     K as oe,
     Y as se
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 import {
     B as De
-} from "./BlockLabel-cddc2b81.js";
+} from "./BlockLabel-10abb1b4.js";
 import {
     M as He
-} from "./ModifyUpload-768fe082.js";
+} from "./ModifyUpload-e3ca444a.js";
 import {
     n as Y
 } from "./utils-de54785e.js";
 import {
     I as Q
-} from "./Image2-1419ace7.js";
+} from "./Image2-bbb64300.js";
 
 function Z(t, e, l) {
     const i = t.slice();
     return i[30] = e[l][0], i[31] = e[l][1], i[33] = l, i
 }
 
 function P(t, e, l) {
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index18-0b10ab02.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index18-d4ad6d1d.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -9,15 +9,15 @@
     Q as v,
     a3 as g,
     a4 as b,
     a5 as h,
     Z as G,
     $ as C,
     a0 as p
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function q(a) {
     let s, i;
     const o = a[3].default,
         t = m(o, a, a[2], null);
     return {
         c() {
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index19-ceded876.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index19-18249feb.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -28,21 +28,21 @@
     at as q,
     aN as C,
     K as V,
     Y as S,
     X as L,
     ap as de,
     O as R
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 import {
     g as me
-} from "./color-07ebf074.js";
+} from "./color-2fcdd2a9.js";
 import {
     B as ge
-} from "./BlockLabel-cddc2b81.js";
+} from "./BlockLabel-10abb1b4.js";
 
 function he(r) {
     let e, n, l;
     return {
         c() {
             e = E("svg"), n = E("path"), l = E("path"), c(n, "fill", "currentColor"), c(n, "d", "M12 15H5a3 3 0 0 1-3-3v-2a3 3 0 0 1 3-3h5V5a1 1 0 0 0-1-1H3V2h6a3 3 0 0 1 3 3zM5 9a1 1 0 0 0-1 1v2a1 1 0 0 0 1 1h5V9zm15 14v2a1 1 0 0 0 1 1h5v-4h-5a1 1 0 0 0-1 1z"), c(l, "fill", "currentColor"), c(l, "d", "M2 30h28V2Zm26-2h-7a3 3 0 0 1-3-3v-2a3 3 0 0 1 3-3h5v-2a1 1 0 0 0-1-1h-6v-2h6a3 3 0 0 1 3 3Z"), c(e, "xmlns", "http://www.w3.org/2000/svg"), c(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), c(e, "aria-hidden", "true"), c(e, "role", "img"), c(e, "class", "iconify iconify--carbon"), c(e, "width", "100%"), c(e, "height", "100%"), c(e, "preserveAspectRatio", "xMidYMid meet"), c(e, "viewBox", "0 0 32 32")
         },
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index2-d042f67b.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index2-667148f0.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -40,24 +40,24 @@
     as as Se,
     at as _l,
     au as Cl,
     K as U,
     Y as C,
     av as Ol,
     aw as de
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 import {
     U as Kl
-} from "./Upload-0cd7f439.js";
+} from "./Upload-6d14b4a6.js";
 import {
     M as Yl
-} from "./ModifyUpload-768fe082.js";
+} from "./ModifyUpload-e3ca444a.js";
 import {
     B as dl
-} from "./BlockLabel-cddc2b81.js";
+} from "./BlockLabel-10abb1b4.js";
 import {
     n as jl
 } from "./utils-de54785e.js";
 
 function Ql(l) {
     let e, i, a, n;
     return {
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index20-d0bcc869.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index20-0cc28676.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -17,15 +17,15 @@
     O as f,
     Q as k,
     ad as J,
     ae as N,
     a0 as H,
     ah as O,
     am as T
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function Q(n) {
     let e;
     return {
         c() {
             e = q("div"), c(e, "class", "output-html"), c(e, "id", n[0]), f(e, "min-h-[6rem]", n[3]), f(e, "!hidden", !n[2])
         },
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index21-d2f402e4.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index21-d3e36a16.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -44,38 +44,38 @@
     aT as Ke,
     aN as Xe,
     aU as St,
     ap as pt,
     aI as Re,
     aV as Rt,
     aW as $e
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 import {
     B as wt
-} from "./BlockLabel-cddc2b81.js";
+} from "./BlockLabel-10abb1b4.js";
 import {
     I as De
-} from "./Image2-1419ace7.js";
+} from "./Image2-bbb64300.js";
 import {
     W as Dt,
     C as Et,
     i as Lt,
     U as Ut
-} from "./Webcam-37a04310.js";
+} from "./Webcam-d64f2534.js";
 import {
     M as Le,
     I as Ee,
     C as Nt
-} from "./ModifyUpload-768fe082.js";
+} from "./ModifyUpload-e3ca444a.js";
 import {
     U as Ft
-} from "./Upload-0cd7f439.js";
+} from "./Upload-6d14b4a6.js";
 import {
     E as On
-} from "./Image-aea3de20.js";
+} from "./Image-2df538c6.js";
 
 function qt(t) {
     let e, n, i;
     return {
         c() {
             e = X("svg"), n = X("path"), i = X("path"), d(n, "d", "M28.828 3.172a4.094 4.094 0 0 0-5.656 0L4.05 22.292A6.954 6.954 0 0 0 2 27.242V30h2.756a6.952 6.952 0 0 0 4.95-2.05L28.828 8.829a3.999 3.999 0 0 0 0-5.657zM10.91 18.26l2.829 2.829l-2.122 2.121l-2.828-2.828zm-2.619 8.276A4.966 4.966 0 0 1 4.756 28H4v-.759a4.967 4.967 0 0 1 1.464-3.535l1.91-1.91l2.829 2.828zM27.415 7.414l-12.261 12.26l-2.829-2.828l12.262-12.26a2.047 2.047 0 0 1 2.828 0a2 2 0 0 1 0 2.828z"), d(n, "fill", "currentColor"), d(i, "d", "M6.5 15a3.5 3.5 0 0 1-2.475-5.974l3.5-3.5a1.502 1.502 0 0 0 0-2.121a1.537 1.537 0 0 0-2.121 0L3.415 5.394L2 3.98l1.99-1.988a3.585 3.585 0 0 1 4.95 0a3.504 3.504 0 0 1 0 4.949L5.439 10.44a1.502 1.502 0 0 0 0 2.121a1.537 1.537 0 0 0 2.122 0l4.024-4.024L13 9.95l-4.025 4.024A3.475 3.475 0 0 1 6.5 15z"), d(i, "fill", "currentColor"), d(e, "width", "100%"), d(e, "height", "100%"), d(e, "viewBox", "0 0 32 32")
         },
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index22-c5e0b0dd.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index22-34fa8df0.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -24,15 +24,15 @@
     al as z,
     O as D,
     K as j,
     Y as S,
     an as H,
     aD as ge,
     ak as J
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 const w = i => {
         var e = null;
         return i < 0 ? e = [52, 152, 219] : e = [231, 76, 60], _e(de(Math.abs(i), [255, 255, 255], e))
     },
     de = (i, e, t) => {
         i > 1 && (i = 1), i = Math.sqrt(i);
         var n = [0, 0, 0],
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index23-e492630c.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index23-b30a6092.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -32,18 +32,18 @@
     ai as ae,
     aO as se,
     aX as ce,
     aW as I,
     aY as fe,
     O as W,
     at as R
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 import {
     B as ue
-} from "./BlockLabel-cddc2b81.js";
+} from "./BlockLabel-10abb1b4.js";
 
 function _e(c) {
     let e, t;
     return {
         c() {
             e = E("svg"), t = E("path"), d(t, "fill", "currentColor"), d(t, "d", "M5 3h2v2H5v5a2 2 0 0 1-2 2a2 2 0 0 1 2 2v5h2v2H5c-1.07-.27-2-.9-2-2v-4a2 2 0 0 0-2-2H0v-2h1a2 2 0 0 0 2-2V5a2 2 0 0 1 2-2m14 0a2 2 0 0 1 2 2v4a2 2 0 0 0 2 2h1v2h-1a2 2 0 0 0-2 2v4a2 2 0 0 1-2 2h-2v-2h2v-5a2 2 0 0 1 2-2a2 2 0 0 1-2-2V5h-2V3h2m-7 12a1 1 0 0 1 1 1a1 1 0 0 1-1 1a1 1 0 0 1-1-1a1 1 0 0 1 1-1m-4 0a1 1 0 0 1 1 1a1 1 0 0 1-1 1a1 1 0 0 1-1-1a1 1 0 0 1 1-1m8 0a1 1 0 0 1 1 1a1 1 0 0 1-1 1a1 1 0 0 1-1-1a1 1 0 0 1 1-1Z"), d(e, "xmlns", "http://www.w3.org/2000/svg"), d(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), d(e, "aria-hidden", "true"), d(e, "role", "img"), d(e, "class", "iconify iconify--mdi"), d(e, "width", "100%"), d(e, "height", "100%"), d(e, "preserveAspectRatio", "xMidYMid meet"), d(e, "viewBox", "0 0 24 24")
         },
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index24-1c64b765.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index24-11b8d91d.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -25,18 +25,18 @@
     am as H,
     al as F,
     K as C,
     O as B,
     aN as Z,
     Y as q,
     at as $
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 import {
     B as ee
-} from "./BlockLabel-cddc2b81.js";
+} from "./BlockLabel-10abb1b4.js";
 
 function le(i) {
     let e, n;
     return {
         c() {
             e = F("svg"), n = F("path"), d(n, "fill", "currentColor"), d(n, "d", "M4 2H2v26a2 2 0 0 0 2 2h26v-2H4v-3h22v-8H4v-4h14V5H4Zm20 17v4H4v-4ZM16 7v4H4V7Z"), d(e, "xmlns", "http://www.w3.org/2000/svg"), d(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), d(e, "aria-hidden", "true"), d(e, "role", "img"), d(e, "class", "iconify iconify--carbon"), d(e, "width", "100%"), d(e, "height", "100%"), d(e, "preserveAspectRatio", "xMidYMid meet"), d(e, "viewBox", "0 0 32 32")
         },
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index25-33571440.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index25-4151ca38.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -19,15 +19,15 @@
     ad as E,
     ae as F,
     a0 as w,
     ah as G,
     aN as J,
     am as M,
     ak as O
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function Q(a) {
     let e;
     return {
         c() {
             e = N("div"), d(e, "id", a[0]), d(e, "class", "output-markdown gr-prose"), J(e, "max-width", "100%"), f(e, "min-h-[6rem]", a[3]), f(e, "hidden", !a[1])
         },
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index26-d78d751e.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index26-2968ddd0.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -30,36 +30,36 @@
     N as Lo,
     V as ou,
     am as Do,
     aq as wv,
     ar as Fv,
     K as Io,
     Y as iu
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 import {
     n as Bv
 } from "./utils-de54785e.js";
 import {
     B as Od
-} from "./BlockLabel-cddc2b81.js";
+} from "./BlockLabel-10abb1b4.js";
 import {
     F as du
-} from "./File-15836fc4.js";
+} from "./File-220c5e21.js";
 import {
     c as Qi
 } from "./_commonjsHelpers-23156833.js";
 import {
     U as Uv
-} from "./Upload-0cd7f439.js";
+} from "./Upload-6d14b4a6.js";
 import {
     M as Vv
-} from "./ModifyUpload-768fe082.js";
+} from "./ModifyUpload-e3ca444a.js";
 import {
     E as _b
-} from "./Model3D-fba04936.js";
+} from "./Model3D-d49eae09.js";
 var Gr = {
     exports: {}
 };
 (function(dt, Ze) {
     (function(Ie, y) {
         dt.exports = y()
     })(typeof self < "u" ? self : typeof Qi < "u" ? Qi : Qi, function() {
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index27-18127a28.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index27-86c85604.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -27,15 +27,15 @@
     X as y,
     aV as V,
     ap as Y,
     a9 as Z,
     K as z,
     Y as A,
     aJ as O
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function P(l) {
     let e;
     return {
         c() {
             e = z(l[2])
         },
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index28-34a5ed1a.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index28-fce682a3.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -31,23 +31,23 @@
     J as Gh,
     an as wD,
     K as FZ,
     Y as NZ,
     aq as BZ,
     ar as jZ,
     a9 as UZ
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 import {
     c as Ro,
     a as Qx,
     g as VZ
 } from "./_commonjsHelpers-23156833.js";
 import {
     g as qZ
-} from "./color-07ebf074.js";
+} from "./color-2fcdd2a9.js";
 import {
     d as yC,
     e as xC,
     _ as VN,
     b as Hw,
     f as eS,
     p as HZ,
@@ -104,15 +104,15 @@
     a2 as dJ
 } from "./linear-8d973619.js";
 import {
     d as pJ
 } from "./dsv-62f8cd07.js";
 import {
     B as gJ
-} from "./BlockLabel-cddc2b81.js";
+} from "./BlockLabel-10abb1b4.js";
 var mJ = Object.defineProperty,
     vJ = Object.defineProperties,
     yJ = Object.getOwnPropertyDescriptors,
     SD = Object.getOwnPropertySymbols,
     xJ = Object.prototype.hasOwnProperty,
     bJ = Object.prototype.propertyIsEnumerable,
     ED = (t, n, e) => n in t ? mJ(t, n, {
@@ -188970,15 +188970,15 @@
     YL = {
         SEMVER_SPEC_VERSION: rTe,
         MAX_LENGTH: iTe,
         MAX_SAFE_INTEGER: aTe,
         MAX_SAFE_COMPONENT_LENGTH: oTe
     },
     sTe = typeof process == "object" && {
-        GIT_COMMIT_HASH: '"8d5dff52e757f1974b0ea9ea13a7efe032d7e50f"'
+        GIT_COMMIT_HASH: '"8b2b3adf40f05a1b24655cc34df5c624f68f09af"'
     } && {}.NODE_DEBUG && /\bsemver\b/i.test({}.NODE_DEBUG) ? function() {
         for (var t = arguments.length, n = new Array(t), e = 0; e < t; e++) n[e] = arguments[e];
         return console.error("SEMVER", ...n)
     } : () => {},
     qT = sTe;
 (function(t, n) {
     var e = YL.MAX_SAFE_COMPONENT_LENGTH,
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index29-e4ca565e.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index29-7f2f8cac.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -27,15 +27,15 @@
     a9 as z,
     ax as A,
     K as j,
     Y as D,
     O as G,
     V as k,
     X as I
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function K(n, e, t) {
     const l = n.slice();
     return l[11] = e[t], l[13] = t, l
 }
 
 function P(n) {
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index3-b8136165.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index3-b632de7a.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -8,15 +8,15 @@
     Z as f,
     $ as r,
     a1 as g,
     a2 as p,
     a3 as $,
     a4 as v,
     a5 as h
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function k(a) {
     let s;
     const l = a[2].default,
         e = p(l, a, a[3], null);
     return {
         c() {
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index30-334d010c.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index30-449fed8c.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -9,15 +9,15 @@
     Q as v,
     a3 as q,
     a4 as b,
     a5 as w,
     Z as C,
     $ as R,
     a0 as F
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function G(s) {
     let e, t;
     const u = s[5].default,
         l = c(u, s, s[4], null);
     return {
         c() {
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index31-1121988e.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index31-a39e3c8b.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -26,15 +26,15 @@
     aI as S,
     X as M,
     aV as D,
     ap as Z,
     a9 as z,
     K as A,
     Y as O
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function P(l) {
     let e;
     return {
         c() {
             e = A(l[5])
         },
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index34-69d671c0.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index34-d9e154ad.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -12,18 +12,18 @@
     a1 as q,
     a9 as C,
     a2 as w,
     a3 as D,
     a4 as E,
     a5 as F,
     ah as G
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 import {
     T as H
-} from "./Tabs-fc1af0f2.js";
+} from "./Tabs-6664f57a.js";
 
 function M(s) {
     let e;
     const l = s[3].default,
         t = w(l, s, s[6], null);
     return {
         c() {
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index35-91b6f450.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index35-71968f90.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -18,21 +18,21 @@
     Q as D,
     a0 as E,
     a9 as F,
     ay as G,
     a7 as H,
     aM as I,
     aJ as Q
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 import {
     a as W
-} from "./Tabs-fc1af0f2.js";
+} from "./Tabs-6664f57a.js";
 import {
     C as Z
-} from "./Column-07457f7d.js";
+} from "./Column-a843ed59.js";
 
 function j(s) {
     let n;
     const a = s[5].default,
         t = p(a, s, s[6], null);
     return {
         c() {
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index37-f530c08a.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index37-03da10b3.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -32,27 +32,27 @@
     aM as Ce,
     aN as F,
     aF as Q,
     ao as Be,
     aw as Ne,
     aO as Te,
     aS as Fe
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 import {
     U as Ue
-} from "./Upload-0cd7f439.js";
+} from "./Upload-6d14b4a6.js";
 import {
     M as De
-} from "./ModifyUpload-768fe082.js";
+} from "./ModifyUpload-e3ca444a.js";
 import {
     B as He
-} from "./BlockLabel-cddc2b81.js";
+} from "./BlockLabel-10abb1b4.js";
 import {
     g as Ie
-} from "./color-07ebf074.js";
+} from "./color-2fcdd2a9.js";
 import {
     l as R,
     _ as Z,
     o as x
 } from "./linear-8d973619.js";
 import {
     a as Ve
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index38-fc6af5aa.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index38-f8a193c1.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -24,15 +24,15 @@
     X as R,
     a3 as V,
     a4 as p,
     a5 as x,
     ap as $,
     ax as ee,
     ak as te
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function le(l) {
     let e, i, n, u, c, o, r, f, b, m;
     const y = l[13].default,
         _ = Z(y, l, l[12], null);
     return {
         c() {
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index39-671ded20.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index39-c97fb654.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -39,31 +39,31 @@
     X as j,
     as as fe,
     aU as Te,
     ap as je,
     b2 as Ce,
     b3 as Ue,
     aJ as Xe
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 import {
     n as Fe
 } from "./utils-de54785e.js";
 import {
     U as qe
-} from "./Upload-0cd7f439.js";
+} from "./Upload-6d14b4a6.js";
 import {
     M as ze
-} from "./ModifyUpload-768fe082.js";
+} from "./ModifyUpload-e3ca444a.js";
 import {
     B as be
-} from "./BlockLabel-cddc2b81.js";
+} from "./BlockLabel-10abb1b4.js";
 import {
     W as Pe,
     U as Se
-} from "./Webcam-37a04310.js";
+} from "./Webcam-d64f2534.js";
 
 function We(n) {
     let e, l;
     return {
         c() {
             e = I("svg"), l = I("path"), c(l, "d", "M8 3H5a2 2 0 0 0-2 2v3m18 0V5a2 2 0 0 0-2-2h-3m0 18h3a2 2 0 0 0 2-2v-3M3 16v3a2 2 0 0 0 2 2h3"), c(e, "xmlns", "http://www.w3.org/2000/svg"), c(e, "width", "100%"), c(e, "height", "100%"), c(e, "viewBox", "0 0 24 24"), c(e, "fill", "none"), c(e, "stroke", "currentColor"), c(e, "stroke-width", "1.5"), c(e, "stroke-linecap", "round"), c(e, "stroke-linejoin", "round")
         },
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index4-d076a84c.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index4-2684c49d.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -19,15 +19,15 @@
     N as c,
     O as m,
     X as M,
     a3 as N,
     a4 as O,
     a5 as Q,
     ax as R
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function S(n) {
     let e, l, t, s, f;
     const r = n[7].default,
         a = J(r, n, n[6], null);
     return {
         c() {
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index5-529df1c0.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index5-264c6674.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -15,18 +15,18 @@
     ad as S,
     ae as j,
     a3 as q,
     a4 as F,
     a5 as G,
     a0 as H,
     ah as L
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 import {
     C as M
-} from "./CarouselItem.svelte_svelte_type_style_lang-08c76e7c.js";
+} from "./CarouselItem.svelte_svelte_type_style_lang-4dd9c624.js";
 
 function Q(l) {
     let t, o, s;
     const i = [l[2]];
     let r = {};
     for (let e = 0; e < i.length; e += 1) r = v(r, i[e]);
     t = new C({
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index6-be007bee.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index6-b60485d2.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -19,18 +19,18 @@
     V as L,
     a0 as O,
     ay as D,
     a7 as E,
     ai as F,
     K as G,
     Y as H
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 import {
     a as J
-} from "./CarouselItem.svelte_svelte_type_style_lang-08c76e7c.js";
+} from "./CarouselItem.svelte_svelte_type_style_lang-4dd9c624.js";
 
 function p(n) {
     let t, a;
     return {
         c() {
             t = w("div"), a = G(n[0]), I(t, "class", "absolute left-0 top-0 py-1 px-2 rounded-br-lg shadow-sm text-xs text-gray-500 flex items-center pointer-events-none bg-white z-20 dark:bg-gray-800")
         },
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index7-c3badb00.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index7-ae38a6d6.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -26,18 +26,18 @@
     a9 as G,
     aC as I,
     aD as J,
     al as M,
     ak as O,
     aE as Q,
     aF as V
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 import {
     B as W
-} from "./BlockLabel-cddc2b81.js";
+} from "./BlockLabel-10abb1b4.js";
 
 function Y(n) {
     let e, s, t;
     return {
         c() {
             e = M("svg"), s = M("path"), t = M("path"), _(s, "fill", "currentColor"), _(s, "d", "M17.74 30L16 29l4-7h6a2 2 0 0 0 2-2V8a2 2 0 0 0-2-2H6a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h9v2H6a4 4 0 0 1-4-4V8a4 4 0 0 1 4-4h20a4 4 0 0 1 4 4v12a4 4 0 0 1-4 4h-4.84Z"), _(t, "fill", "currentColor"), _(t, "d", "M8 10h16v2H8zm0 6h10v2H8z"), _(e, "xmlns", "http://www.w3.org/2000/svg"), _(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), _(e, "aria-hidden", "true"), _(e, "role", "img"), _(e, "class", "iconify iconify--carbon"), _(e, "width", "100%"), _(e, "height", "100%"), _(e, "preserveAspectRatio", "xMidYMid meet"), _(e, "viewBox", "0 0 32 32")
         },
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index8-2bbdfede.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index8-5ee4cbfe.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -24,15 +24,15 @@
     N as d,
     O as q,
     V as m,
     X as V,
     Y as W,
     am as S,
     a9 as X
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function Y(n) {
     let e, t, a, i, c, r, f;
     return {
         c() {
             e = g("label"), t = g("input"), a = B(), i = g("span"), c = Q(n[2]), t.disabled = n[1], t.checked = n[0], d(t, "type", "checkbox"), d(t, "name", "test"), d(t, "class", "gr-check-radio gr-checkbox"), d(i, "class", "ml-2"), d(e, "class", "flex items-center text-gray-700 text-sm space-x-2 rounded-lg cursor-pointer dark:bg-transparent "), q(e, "!cursor-not-allowed", n[1])
         },
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/index9-0cbe1428.js` & `starwhale-0.5.9/starwhale/web/ui/assets/index9-f552db0e.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -26,15 +26,15 @@
     a9 as Z,
     ax as z,
     K as E,
     Y as F,
     O,
     V as k,
     X as I
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function S(l, e, t) {
     const a = l.slice();
     return a[10] = e[t], a
 }
 
 function P(l) {
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/invalid-file-82d62dec.svg` & `starwhale-0.5.9/starwhale/web/ui/assets/invalid-file-82d62dec.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/left-8c88a49a.svg` & `starwhale-0.5.9/starwhale/web/ui/assets/left-8c88a49a.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/linear-8d973619.js` & `starwhale-0.5.9/starwhale/web/ui/assets/linear-8d973619.js`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/logo_normal_en_gray-163de1a0.svg` & `starwhale-0.5.9/starwhale/web/ui/assets/logo_normal_en_gray-163de1a0.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/logo_normal_en_white-ec11283c.svg` & `starwhale-0.5.9/starwhale/web/ui/assets/logo_normal_en_white-ec11283c.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/logo_small_en_white-782559aa.svg` & `starwhale-0.5.9/starwhale/web/ui/assets/logo_small_en_white-782559aa.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/main-99f2bbfd.js` & `starwhale-0.5.9/starwhale/web/ui/assets/main-e0f2ffda.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 import {
     C as Ct,
     r as St,
     E as wt
-} from "./index-3bbbd54b.js";
+} from "./index-df1fb029.js";
 
 function At(rt, pt) {
     for (var Ye = 0; Ye < pt.length; Ye++) {
         const o = pt[Ye];
         if (typeof o != "string" && !Array.isArray(o)) {
             for (const n in o)
                 if (n !== "default" && !(n in rt)) {
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/module-ddaca3b9.js` & `starwhale-0.5.9/starwhale/web/ui/assets/module-ddaca3b9.js`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/module2-74df381a.js` & `starwhale-0.5.9/starwhale/web/ui/assets/module2-74df381a.js`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/module3-49e9a615.js` & `starwhale-0.5.9/starwhale/web/ui/assets/module3-49e9a615.js`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-bold-452a631f.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-bold-452a631f.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-bold-5c4ed5bb.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-bold-5c4ed5bb.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-bold-italic-16cda7ef.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-bold-italic-16cda7ef.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-bold-italic-4926428e.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-bold-italic-4926428e.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-extrabold-613313c8.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-extrabold-613313c8.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-extrabold-648ba0e7.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-extrabold-648ba0e7.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-extrabold-italic-33533562.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-extrabold-italic-33533562.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-extrabold-italic-a258578a.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-extrabold-italic-a258578a.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-extralight-64fbbd3d.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-extralight-64fbbd3d.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-extralight-f053be7c.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-extralight-f053be7c.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-extralight-italic-6cbe5597.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-extralight-italic-6cbe5597.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-extralight-italic-d23afde2.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-extralight-italic-d23afde2.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-heavy-5e0869ee.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-heavy-5e0869ee.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-heavy-c7e67c68.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-heavy-c7e67c68.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-heavy-italic-8f5fbf20.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-heavy-italic-8f5fbf20.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-heavy-italic-c702fef1.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-heavy-italic-c702fef1.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-italic-34df3d81.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-italic-34df3d81.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-italic-b81a6146.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-italic-b81a6146.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-light-3f8151f4.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-light-3f8151f4.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-light-9db6ab0a.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-light-9db6ab0a.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-light-italic-a1454ca5.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-light-italic-a1454ca5.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-light-italic-ec333948.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-light-italic-ec333948.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-mono-bold-2bf715ff.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-mono-bold-2bf715ff.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-mono-bold-9b29c79a.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-mono-bold-9b29c79a.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-mono-light-5bae063c.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-mono-light-5bae063c.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-mono-light-7fbe3706.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-mono-light-7fbe3706.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-mono-regular-95881615.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-mono-regular-95881615.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-mono-regular-a13dec50.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-mono-regular-a13dec50.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-mono-semibold-085fb4a8.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-mono-semibold-085fb4a8.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-mono-semibold-b39c5174.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-mono-semibold-b39c5174.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-regular-16b63547.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-regular-16b63547.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-regular-8e2261df.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-regular-8e2261df.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-semibold-3d06895e.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-semibold-3d06895e.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-semibold-ec5809e8.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-semibold-ec5809e8.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-semibold-italic-1935eb14.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-semibold-italic-1935eb14.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-semibold-italic-ae706d8c.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-semibold-italic-ae706d8c.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-thin-6feca5dc.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-thin-6feca5dc.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-thin-e85966f1.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-thin-e85966f1.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-thin-italic-2dffa092.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-thin-italic-2dffa092.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/overpass-thin-italic-44db8e3d.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/overpass-thin-italic-44db8e3d.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/pfbg_2000-1f17de55.jpg` & `starwhale-0.5.9/starwhale/web/ui/assets/pfbg_2000-1f17de55.jpg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/pfbg_576-1d76d6cc.jpg` & `starwhale-0.5.9/starwhale/web/ui/assets/pfbg_576-1d76d6cc.jpg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/pfbg_576@2x-4942ea78.jpg` & `starwhale-0.5.9/starwhale/web/ui/assets/pfbg_576@2x-4942ea78.jpg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/pfbg_768-8bc3cc8a.jpg` & `starwhale-0.5.9/starwhale/web/ui/assets/pfbg_768-8bc3cc8a.jpg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/pfbg_768@2x-037bce76.jpg` & `starwhale-0.5.9/starwhale/web/ui/assets/pfbg_768@2x-037bce76.jpg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/pfbg_992@2x-9dfd9687.jpg` & `starwhale-0.5.9/starwhale/web/ui/assets/pfbg_992@2x-9dfd9687.jpg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/pficon-0a333dac.woff` & `starwhale-0.5.9/starwhale/web/ui/assets/pficon-0a333dac.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/pficon-86c74539.woff2` & `starwhale-0.5.9/starwhale/web/ui/assets/pficon-86c74539.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/project-863f66b0.svg` & `starwhale-0.5.9/starwhale/web/ui/assets/project-863f66b0.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/right-aefe3c24.svg` & `starwhale-0.5.9/starwhale/web/ui/assets/right-aefe3c24.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/search-empty-13cbde15.svg` & `starwhale-0.5.9/starwhale/web/ui/assets/search-empty-13cbde15.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/setting-6d098443.svg` & `starwhale-0.5.9/starwhale/web/ui/assets/setting-6d098443.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/status-icon-sprite-bc89cb14.svg` & `starwhale-0.5.9/starwhale/web/ui/assets/status-icon-sprite-bc89cb14.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/web-vitals-d4fac006.js` & `starwhale-0.5.9/starwhale/web/ui/assets/web-vitals-d4fac006.js`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/assets/wechat-cffee157.svg` & `starwhale-0.5.9/starwhale/web/ui/assets/wechat-cffee157.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/favicon.ico` & `starwhale-0.5.9/starwhale/web/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/favicon_white.ico` & `starwhale-0.5.9/starwhale/web/ui/favicon_white.ico`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/iconfont.js` & `starwhale-0.5.9/starwhale/web/ui/iconfont.js`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.8/starwhale/web/ui/index.html` & `starwhale-0.5.9/starwhale/web/ui/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     <head>
         <meta charset="utf-8" />
         <!-- <link rel="icon" href="%PUBLIC_URL%/favicon.ico" /> -->
         <meta name="viewport" content="width=device-width, initial-scale=1" />
         <meta http-equiv="Cache-Control" content="public" />
         <meta name="theme-color" content="#000000" />
         <meta name="description" content="Homepage | Starwhale MLOps service" />
+        
         <!--
       manifest.json provides metadata used when your web app is installed on a
       user's mobile device or desktop. See https://developers.google.com/web/fundamentals/web-app-manifest/
     -->
         <!-- <link rel="manifest" href="%PUBLIC_URL%/manifest.json" /> -->
         <!--
       Notice the use of %PUBLIC_URL% in the tags above.
@@ -18,15 +19,15 @@
       Only files inside the `public` folder can be referenced from the HTML.
 
       Unlike "/favicon.ico" or "favicon.ico", "%PUBLIC_URL%/favicon.ico" will
       work correctly both with client-side routing and a non-root public URL.
       Learn how to configure a non-root public URL by running `npm run build`.
     -->
         <title>Starwhale Console</title>
-      <script type="module" crossorigin src="/assets/index-3bbbd54b.js"></script>
+      <script type="module" crossorigin src="/assets/index-df1fb029.js"></script>
       <link rel="stylesheet" href="/assets/index-ddbcf299.css">
     </head>
     <body>
         <noscript>You need to enable JavaScript to run this app.</noscript>
         <div id="root"></div>
         <!--
       This HTML file is a template.
```

### Comparing `starwhale-0.5.8/starwhale/web/ui/manifest.json` & `starwhale-0.5.9/starwhale/web/ui/manifest.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.834067820444225%*

 * *Differences: {"'_BlockLabel-10abb1b4.js'": "OrderedDict([('file', 'assets/BlockLabel-10abb1b4.js'), ('imports', "*

 * *                              "['index.html'])])",*

 * * "'_CarouselItem.svelte_svelte_type_style_lang-4dd9c624.js'": "OrderedDict([('file', "*

 * *                                                              "'assets/CarouselItem.svelte_svelte_type_style_lang-4dd9c624.js'), "*

 * *                                                              "('imports', ['index.html'])])",*

 * * "'_Column-a843ed59.js'": "OrderedDict([('file' […]*

```diff
@@ -1,79 +1,79 @@
 {
-    "_BlockLabel-cddc2b81.js": {
-        "file": "assets/BlockLabel-cddc2b81.js",
+    "_BlockLabel-10abb1b4.js": {
+        "file": "assets/BlockLabel-10abb1b4.js",
         "imports": [
             "index.html"
         ]
     },
-    "_CarouselItem.svelte_svelte_type_style_lang-08c76e7c.js": {
-        "file": "assets/CarouselItem.svelte_svelte_type_style_lang-08c76e7c.js",
+    "_CarouselItem.svelte_svelte_type_style_lang-4dd9c624.js": {
+        "file": "assets/CarouselItem.svelte_svelte_type_style_lang-4dd9c624.js",
         "imports": [
             "index.html"
         ]
     },
-    "_Column-07457f7d.js": {
-        "file": "assets/Column-07457f7d.js",
+    "_Column-a843ed59.js": {
+        "file": "assets/Column-a843ed59.js",
         "imports": [
             "index.html"
         ]
     },
-    "_File-15836fc4.js": {
-        "file": "assets/File-15836fc4.js",
+    "_File-220c5e21.js": {
+        "file": "assets/File-220c5e21.js",
         "imports": [
             "index.html"
         ]
     },
-    "_Image-aea3de20.js": {
-        "file": "assets/Image-aea3de20.js",
+    "_Image-2df538c6.js": {
+        "file": "assets/Image-2df538c6.js",
         "imports": [
             "index.html"
         ]
     },
-    "_Image2-1419ace7.js": {
-        "file": "assets/Image2-1419ace7.js",
+    "_Image2-bbb64300.js": {
+        "file": "assets/Image2-bbb64300.js",
         "imports": [
             "index.html"
         ]
     },
-    "_Model3D-fba04936.js": {
-        "file": "assets/Model3D-fba04936.js",
+    "_Model3D-d49eae09.js": {
+        "file": "assets/Model3D-d49eae09.js",
         "imports": [
             "index.html"
         ]
     },
-    "_ModifyUpload-768fe082.js": {
-        "file": "assets/ModifyUpload-768fe082.js",
+    "_ModifyUpload-e3ca444a.js": {
+        "file": "assets/ModifyUpload-e3ca444a.js",
         "imports": [
             "index.html"
         ]
     },
-    "_Tabs-fc1af0f2.js": {
-        "file": "assets/Tabs-fc1af0f2.js",
+    "_Tabs-6664f57a.js": {
+        "file": "assets/Tabs-6664f57a.js",
         "imports": [
             "index.html"
         ]
     },
-    "_Upload-0cd7f439.js": {
-        "file": "assets/Upload-0cd7f439.js",
+    "_Upload-6d14b4a6.js": {
+        "file": "assets/Upload-6d14b4a6.js",
         "imports": [
             "index.html"
         ]
     },
-    "_Webcam-37a04310.js": {
-        "file": "assets/Webcam-37a04310.js",
+    "_Webcam-d64f2534.js": {
+        "file": "assets/Webcam-d64f2534.js",
         "imports": [
             "index.html"
         ]
     },
     "__commonjsHelpers-23156833.js": {
         "file": "assets/_commonjsHelpers-23156833.js"
     },
-    "_color-07ebf074.js": {
-        "file": "assets/color-07ebf074.js",
+    "_color-2fcdd2a9.js": {
+        "file": "assets/color-2fcdd2a9.js",
         "imports": [
             "index.html"
         ]
     },
     "_csv-17a3ae92.js": {
         "file": "assets/csv-17a3ae92.js",
         "imports": [
@@ -82,16 +82,16 @@
     },
     "_dsv-62f8cd07.js": {
         "file": "assets/dsv-62f8cd07.js"
     },
     "_linear-8d973619.js": {
         "file": "assets/linear-8d973619.js"
     },
-    "_main-99f2bbfd.js": {
-        "file": "assets/main-99f2bbfd.js",
+    "_main-e0f2ffda.js": {
+        "file": "assets/main-e0f2ffda.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true
     },
     "_module2-74df381a.js": {
         "file": "assets/module2-74df381a.js"
@@ -131,15 +131,15 @@
             "assets/iconfont-10b60b11.ttf"
         ],
         "css": [
             "assets/index-ddbcf299.css"
         ],
         "dynamicImports": [
             "node_modules/web-vitals/dist/web-vitals.js",
-            "_main-99f2bbfd.js",
+            "_main-e0f2ffda.js",
             "packages/starwhale-ui/src/Plotly/index.ts",
             "packages/starwhale-ui/src/Plotly/index.ts",
             "src/domain/dataset/components/DatasetForm.tsx",
             "src/components/LogViewer/LogViewer.tsx",
             "src/assets/GradioWidget/es/index.js",
             "src/assets/GradioWidget/es/index2.js",
             "src/assets/GradioWidget/es/index3.js",
@@ -178,15 +178,15 @@
             "src/assets/GradioWidget/es/index36.js",
             "src/assets/GradioWidget/es/index37.js",
             "src/assets/GradioWidget/es/index38.js",
             "src/assets/GradioWidget/es/index39.js",
             "src/components/LogViewer/LogViewer.tsx",
             "packages/starwhale-ui/src/Markdown/Markdown.tsx"
         ],
-        "file": "assets/index-3bbbd54b.js",
+        "file": "assets/index-df1fb029.js",
         "isEntry": true,
         "src": "index.html"
     },
     "node_modules/@patternfly/react-core/dist/styles/assets/fonts/RedHatDisplay/RedHatDisplay-Bold.woff": {
         "file": "assets/RedHatDisplay-Bold-44214a55.woff",
         "src": "node_modules/@patternfly/react-core/dist/styles/assets/fonts/RedHatDisplay/RedHatDisplay-Bold.woff"
     },
@@ -527,407 +527,407 @@
         "file": "assets/Markdown-d8dda0b2.css",
         "src": "packages/starwhale-ui/src/Markdown/Markdown.css"
     },
     "packages/starwhale-ui/src/Markdown/Markdown.tsx": {
         "css": [
             "assets/Markdown-d8dda0b2.css"
         ],
-        "file": "assets/Markdown-fdfce605.js",
+        "file": "assets/Markdown-2b316973.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "packages/starwhale-ui/src/Markdown/Markdown.tsx"
     },
     "packages/starwhale-ui/src/Plotly/index.css": {
         "file": "assets/index-4b525ef6.css",
         "src": "packages/starwhale-ui/src/Plotly/index.css"
     },
     "packages/starwhale-ui/src/Plotly/index.ts": {
         "css": [
             "assets/index-4b525ef6.css"
         ],
-        "file": "assets/index-af425f4b.js",
+        "file": "assets/index-e17166cd.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "packages/starwhale-ui/src/Plotly/index.ts"
     },
     "src/assets/GradioWidget/es/index.js": {
-        "file": "assets/index-890d4a46.js",
+        "file": "assets/index-87b297cf.js",
         "imports": [
             "index.html",
-            "_Column-07457f7d.js"
+            "_Column-a843ed59.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index.js"
     },
     "src/assets/GradioWidget/es/index10.js": {
-        "file": "assets/index10-4d13164f.js",
+        "file": "assets/index10-7aed280d.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index10.js"
     },
     "src/assets/GradioWidget/es/index11.js": {
-        "file": "assets/index11-13eb176d.js",
+        "file": "assets/index11-df7b8b7d.js",
         "imports": [
-            "_Column-07457f7d.js",
+            "_Column-a843ed59.js",
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index11.js"
     },
     "src/assets/GradioWidget/es/index12.js": {
-        "file": "assets/index12-de21ca8a.js",
+        "file": "assets/index12-f581388d.js",
         "imports": [
             "index.html",
-            "_Upload-0cd7f439.js",
+            "_Upload-6d14b4a6.js",
             "_dsv-62f8cd07.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index12.js"
     },
     "src/assets/GradioWidget/es/index13.js": {
-        "file": "assets/index13-0661cc45.js",
+        "file": "assets/index13-fd2d632d.js",
         "imports": [
             "index.html",
-            "_Image-aea3de20.js",
+            "_Image-2df538c6.js",
             "_csv-17a3ae92.js",
             "_dsv-62f8cd07.js",
-            "_Model3D-fba04936.js"
+            "_Model3D-d49eae09.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index13.js"
     },
     "src/assets/GradioWidget/es/index14.js": {
-        "file": "assets/index14-e2afac41.js",
+        "file": "assets/index14-94c12d28.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index14.js"
     },
     "src/assets/GradioWidget/es/index15.js": {
-        "file": "assets/index15-9ee1eee9.js",
+        "file": "assets/index15-a31493a5.js",
         "imports": [
             "index.html",
-            "_BlockLabel-cddc2b81.js",
-            "_File-15836fc4.js",
-            "_Upload-0cd7f439.js",
-            "_ModifyUpload-768fe082.js",
+            "_BlockLabel-10abb1b4.js",
+            "_File-220c5e21.js",
+            "_Upload-6d14b4a6.js",
+            "_ModifyUpload-e3ca444a.js",
             "_utils-de54785e.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index15.js"
     },
     "src/assets/GradioWidget/es/index16.js": {
-        "file": "assets/index16-a0351c35.js",
+        "file": "assets/index16-2b049823.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index16.js"
     },
     "src/assets/GradioWidget/es/index17.js": {
-        "file": "assets/index17-a75792cc.js",
+        "file": "assets/index17-d4811bf1.js",
         "imports": [
             "index.html",
-            "_BlockLabel-cddc2b81.js",
-            "_ModifyUpload-768fe082.js",
+            "_BlockLabel-10abb1b4.js",
+            "_ModifyUpload-e3ca444a.js",
             "_utils-de54785e.js",
-            "_Image2-1419ace7.js"
+            "_Image2-bbb64300.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index17.js"
     },
     "src/assets/GradioWidget/es/index18.js": {
-        "file": "assets/index18-0b10ab02.js",
+        "file": "assets/index18-d4ad6d1d.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index18.js"
     },
     "src/assets/GradioWidget/es/index19.js": {
-        "file": "assets/index19-ceded876.js",
+        "file": "assets/index19-18249feb.js",
         "imports": [
             "index.html",
-            "_color-07ebf074.js",
-            "_BlockLabel-cddc2b81.js"
+            "_color-2fcdd2a9.js",
+            "_BlockLabel-10abb1b4.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index19.js"
     },
     "src/assets/GradioWidget/es/index2.js": {
         "dynamicImports": [
             "src/assets/GradioWidget/es/module.js",
             "src/assets/GradioWidget/es/module3.js"
         ],
-        "file": "assets/index2-d042f67b.js",
+        "file": "assets/index2-667148f0.js",
         "imports": [
             "index.html",
-            "_Upload-0cd7f439.js",
-            "_ModifyUpload-768fe082.js",
-            "_BlockLabel-cddc2b81.js",
+            "_Upload-6d14b4a6.js",
+            "_ModifyUpload-e3ca444a.js",
+            "_BlockLabel-10abb1b4.js",
             "_utils-de54785e.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index2.js"
     },
     "src/assets/GradioWidget/es/index20.js": {
-        "file": "assets/index20-d0bcc869.js",
+        "file": "assets/index20-0cc28676.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index20.js"
     },
     "src/assets/GradioWidget/es/index21.js": {
-        "file": "assets/index21-d2f402e4.js",
+        "file": "assets/index21-d3e36a16.js",
         "imports": [
             "index.html",
-            "_BlockLabel-cddc2b81.js",
-            "_Image2-1419ace7.js",
-            "_Webcam-37a04310.js",
-            "_ModifyUpload-768fe082.js",
-            "_Upload-0cd7f439.js",
-            "_Image-aea3de20.js"
+            "_BlockLabel-10abb1b4.js",
+            "_Image2-bbb64300.js",
+            "_Webcam-d64f2534.js",
+            "_ModifyUpload-e3ca444a.js",
+            "_Upload-6d14b4a6.js",
+            "_Image-2df538c6.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index21.js"
     },
     "src/assets/GradioWidget/es/index22.js": {
-        "file": "assets/index22-c5e0b0dd.js",
+        "file": "assets/index22-34fa8df0.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index22.js"
     },
     "src/assets/GradioWidget/es/index23.js": {
-        "file": "assets/index23-e492630c.js",
+        "file": "assets/index23-b30a6092.js",
         "imports": [
             "index.html",
-            "_BlockLabel-cddc2b81.js"
+            "_BlockLabel-10abb1b4.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index23.js"
     },
     "src/assets/GradioWidget/es/index24.js": {
-        "file": "assets/index24-1c64b765.js",
+        "file": "assets/index24-11b8d91d.js",
         "imports": [
             "index.html",
-            "_BlockLabel-cddc2b81.js"
+            "_BlockLabel-10abb1b4.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index24.js"
     },
     "src/assets/GradioWidget/es/index25.js": {
-        "file": "assets/index25-33571440.js",
+        "file": "assets/index25-4151ca38.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index25.js"
     },
     "src/assets/GradioWidget/es/index26.js": {
-        "file": "assets/index26-d78d751e.js",
+        "file": "assets/index26-2968ddd0.js",
         "imports": [
             "index.html",
             "_utils-de54785e.js",
-            "_BlockLabel-cddc2b81.js",
-            "_File-15836fc4.js",
+            "_BlockLabel-10abb1b4.js",
+            "_File-220c5e21.js",
             "__commonjsHelpers-23156833.js",
-            "_Upload-0cd7f439.js",
-            "_ModifyUpload-768fe082.js",
-            "_Model3D-fba04936.js"
+            "_Upload-6d14b4a6.js",
+            "_ModifyUpload-e3ca444a.js",
+            "_Model3D-d49eae09.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index26.js"
     },
     "src/assets/GradioWidget/es/index27.js": {
-        "file": "assets/index27-18127a28.js",
+        "file": "assets/index27-86c85604.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index27.js"
     },
     "src/assets/GradioWidget/es/index28.js": {
-        "file": "assets/index28-34a5ed1a.js",
+        "file": "assets/index28-fce682a3.js",
         "imports": [
             "index.html",
             "__commonjsHelpers-23156833.js",
-            "_color-07ebf074.js",
+            "_color-2fcdd2a9.js",
             "_linear-8d973619.js",
             "_dsv-62f8cd07.js",
-            "_BlockLabel-cddc2b81.js"
+            "_BlockLabel-10abb1b4.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index28.js"
     },
     "src/assets/GradioWidget/es/index29.js": {
-        "file": "assets/index29-e4ca565e.js",
+        "file": "assets/index29-7f2f8cac.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index29.js"
     },
     "src/assets/GradioWidget/es/index3.js": {
-        "file": "assets/index3-b8136165.js",
+        "file": "assets/index3-b632de7a.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index3.js"
     },
     "src/assets/GradioWidget/es/index30.js": {
-        "file": "assets/index30-334d010c.js",
+        "file": "assets/index30-449fed8c.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index30.js"
     },
     "src/assets/GradioWidget/es/index31.js": {
-        "file": "assets/index31-1121988e.js",
+        "file": "assets/index31-a39e3c8b.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index31.js"
     },
     "src/assets/GradioWidget/es/index32.js": {
-        "file": "assets/index32-80223294.js",
+        "file": "assets/index32-5e251911.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index32.js"
     },
     "src/assets/GradioWidget/es/index33.js": {
-        "file": "assets/index33-a4713f90.js",
+        "file": "assets/index33-8befa193.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index33.js"
     },
     "src/assets/GradioWidget/es/index34.js": {
-        "file": "assets/index34-69d671c0.js",
+        "file": "assets/index34-d9e154ad.js",
         "imports": [
             "index.html",
-            "_Tabs-fc1af0f2.js"
+            "_Tabs-6664f57a.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index34.js"
     },
     "src/assets/GradioWidget/es/index35.js": {
-        "file": "assets/index35-91b6f450.js",
+        "file": "assets/index35-71968f90.js",
         "imports": [
             "index.html",
-            "_Tabs-fc1af0f2.js",
-            "_Column-07457f7d.js"
+            "_Tabs-6664f57a.js",
+            "_Column-a843ed59.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index35.js"
     },
     "src/assets/GradioWidget/es/index36.js": {
-        "file": "assets/index36-6ce81ba8.js",
+        "file": "assets/index36-6d6222b1.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index36.js"
     },
     "src/assets/GradioWidget/es/index37.js": {
-        "file": "assets/index37-f530c08a.js",
+        "file": "assets/index37-03da10b3.js",
         "imports": [
             "index.html",
-            "_Upload-0cd7f439.js",
-            "_ModifyUpload-768fe082.js",
-            "_BlockLabel-cddc2b81.js",
-            "_color-07ebf074.js",
+            "_Upload-6d14b4a6.js",
+            "_ModifyUpload-e3ca444a.js",
+            "_BlockLabel-10abb1b4.js",
+            "_color-2fcdd2a9.js",
             "_linear-8d973619.js",
             "_csv-17a3ae92.js",
             "_dsv-62f8cd07.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index37.js"
     },
     "src/assets/GradioWidget/es/index38.js": {
-        "file": "assets/index38-fc6af5aa.js",
+        "file": "assets/index38-f8a193c1.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index38.js"
     },
     "src/assets/GradioWidget/es/index39.js": {
-        "file": "assets/index39-671ded20.js",
+        "file": "assets/index39-c97fb654.js",
         "imports": [
             "index.html",
             "_utils-de54785e.js",
-            "_Upload-0cd7f439.js",
-            "_ModifyUpload-768fe082.js",
-            "_BlockLabel-cddc2b81.js",
-            "_Webcam-37a04310.js"
+            "_Upload-6d14b4a6.js",
+            "_ModifyUpload-e3ca444a.js",
+            "_BlockLabel-10abb1b4.js",
+            "_Webcam-d64f2534.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index39.js"
     },
     "src/assets/GradioWidget/es/index4.js": {
-        "file": "assets/index4-d076a84c.js",
+        "file": "assets/index4-2684c49d.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index4.js"
     },
     "src/assets/GradioWidget/es/index5.js": {
-        "file": "assets/index5-529df1c0.js",
+        "file": "assets/index5-264c6674.js",
         "imports": [
             "index.html",
-            "_CarouselItem.svelte_svelte_type_style_lang-08c76e7c.js"
+            "_CarouselItem.svelte_svelte_type_style_lang-4dd9c624.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index5.js"
     },
     "src/assets/GradioWidget/es/index6.js": {
-        "file": "assets/index6-be007bee.js",
+        "file": "assets/index6-b60485d2.js",
         "imports": [
             "index.html",
-            "_CarouselItem.svelte_svelte_type_style_lang-08c76e7c.js"
+            "_CarouselItem.svelte_svelte_type_style_lang-4dd9c624.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index6.js"
     },
     "src/assets/GradioWidget/es/index7.js": {
-        "file": "assets/index7-c3badb00.js",
+        "file": "assets/index7-ae38a6d6.js",
         "imports": [
             "index.html",
-            "_BlockLabel-cddc2b81.js"
+            "_BlockLabel-10abb1b4.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index7.js"
     },
     "src/assets/GradioWidget/es/index8.js": {
-        "file": "assets/index8-2bbdfede.js",
+        "file": "assets/index8-5ee4cbfe.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index8.js"
     },
     "src/assets/GradioWidget/es/index9.js": {
-        "file": "assets/index9-0cbe1428.js",
+        "file": "assets/index9-f552db0e.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index9.js"
     },
     "src/assets/GradioWidget/es/module.js": {
@@ -1065,23 +1065,23 @@
             "assets/pficon-86c74539.woff2",
             "assets/pficon-0a333dac.woff",
             "assets/status-icon-sprite-bc89cb14.svg"
         ],
         "css": [
             "assets/LogViewer-b5684b3d.css"
         ],
-        "file": "assets/LogViewer-f5bb7317.js",
+        "file": "assets/LogViewer-e1f101c5.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/components/LogViewer/LogViewer.tsx"
     },
     "src/domain/dataset/components/DatasetForm.tsx": {
-        "file": "assets/DatasetForm-aac5cbbf.js",
+        "file": "assets/DatasetForm-6dd7af50.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/domain/dataset/components/DatasetForm.tsx"
     }
 }
```

### Comparing `starwhale-0.5.8/starwhale.egg-info/PKG-INFO` & `starwhale-0.5.9/starwhale.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starwhale
-Version: 0.5.8
+Version: 0.5.9
 Summary: An MLOps Platform for Model Evaluation
 Home-page: https://github.com/star-whale/starwhale
 Author: Starwhale Team
 Author-email: developer@starwhale.ai
 License: Apache License 2.0
 Keywords: MLOps,AI,Starwhale,Model Evaluation
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: starwhale Version: 0.5.8 Summary: An MLOps Platform
+Metadata-Version: 2.1 Name: starwhale Version: 0.5.9 Summary: An MLOps Platform
 for Model Evaluation Home-page: https://github.com/star-whale/starwhale Author:
 Starwhale Team Author-email: developer@starwhale.ai License: Apache License 2.0
 Keywords: MLOps,AI,Starwhale,Model Evaluation Classifier: Development Status ::
 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
```

### Comparing `starwhale-0.5.8/starwhale.egg-info/SOURCES.txt` & `starwhale-0.5.9/starwhale.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -156,27 +156,27 @@
 starwhale/web/user.py
 starwhale/web/ui/favicon.ico
 starwhale/web/ui/favicon_white.ico
 starwhale/web/ui/iconfont.js
 starwhale/web/ui/index.html
 starwhale/web/ui/manifest.json
 starwhale/web/ui/robots.txt
-starwhale/web/ui/assets/BlockLabel-cddc2b81.js
-starwhale/web/ui/assets/CarouselItem.svelte_svelte_type_style_lang-08c76e7c.js
-starwhale/web/ui/assets/Column-07457f7d.js
-starwhale/web/ui/assets/DatasetForm-aac5cbbf.js
-starwhale/web/ui/assets/File-15836fc4.js
-starwhale/web/ui/assets/Image-aea3de20.js
-starwhale/web/ui/assets/Image2-1419ace7.js
+starwhale/web/ui/assets/BlockLabel-10abb1b4.js
+starwhale/web/ui/assets/CarouselItem.svelte_svelte_type_style_lang-4dd9c624.js
+starwhale/web/ui/assets/Column-a843ed59.js
+starwhale/web/ui/assets/DatasetForm-6dd7af50.js
+starwhale/web/ui/assets/File-220c5e21.js
+starwhale/web/ui/assets/Image-2df538c6.js
+starwhale/web/ui/assets/Image2-bbb64300.js
 starwhale/web/ui/assets/LogViewer-b5684b3d.css
-starwhale/web/ui/assets/LogViewer-f5bb7317.js
+starwhale/web/ui/assets/LogViewer-e1f101c5.js
+starwhale/web/ui/assets/Markdown-2b316973.js
 starwhale/web/ui/assets/Markdown-d8dda0b2.css
-starwhale/web/ui/assets/Markdown-fdfce605.js
-starwhale/web/ui/assets/Model3D-fba04936.js
-starwhale/web/ui/assets/ModifyUpload-768fe082.js
+starwhale/web/ui/assets/Model3D-d49eae09.js
+starwhale/web/ui/assets/ModifyUpload-e3ca444a.js
 starwhale/web/ui/assets/RedHatDisplay-Bold-44214a55.woff
 starwhale/web/ui/assets/RedHatDisplay-Bold-ca18645c.woff2
 starwhale/web/ui/assets/RedHatDisplay-Medium-6ccf2158.woff
 starwhale/web/ui/assets/RedHatDisplay-Medium-6d3ccc0f.woff2
 starwhale/web/ui/assets/RedHatDisplay-Regular-1b99a560.woff
 starwhale/web/ui/assets/RedHatDisplay-Regular-e6fb83d9.woff2
 starwhale/web/ui/assets/RedHatDisplay-updated-Bold-66d1fc26.woff2
@@ -192,83 +192,83 @@
 starwhale/web/ui/assets/RedHatText-Regular-542423d0.woff2
 starwhale/web/ui/assets/RedHatText-Regular-df36d7d0.woff
 starwhale/web/ui/assets/RedHatText-updated-Medium-721ddd64.woff2
 starwhale/web/ui/assets/RedHatText-updated-Regular-2e08dbe8.woff2
 starwhale/web/ui/assets/RedHatTextVF-updated-ItalicModified-9e1c1004.woff2
 starwhale/web/ui/assets/RedHatTextVFModified-updated-942d38f7.woff2
 starwhale/web/ui/assets/RobotoMono-Regular-5c4ca672.ttf
-starwhale/web/ui/assets/Tabs-fc1af0f2.js
-starwhale/web/ui/assets/Upload-0cd7f439.js
-starwhale/web/ui/assets/Webcam-37a04310.js
+starwhale/web/ui/assets/Tabs-6664f57a.js
+starwhale/web/ui/assets/Upload-6d14b4a6.js
+starwhale/web/ui/assets/Webcam-d64f2534.js
 starwhale/web/ui/assets/_commonjsHelpers-23156833.js
 starwhale/web/ui/assets/account2-668f906e.svg
 starwhale/web/ui/assets/bg-1920x1080-8b0d8feb.jpg
 starwhale/web/ui/assets/bg-2560x1440-c97cffa5.jpg
 starwhale/web/ui/assets/bg-3840x2160-f974f4b1.jpg
-starwhale/web/ui/assets/color-07ebf074.js
+starwhale/web/ui/assets/color-2fcdd2a9.js
 starwhale/web/ui/assets/csv-17a3ae92.js
 starwhale/web/ui/assets/dsv-62f8cd07.js
 starwhale/web/ui/assets/empty-chart-1e62901a.svg
 starwhale/web/ui/assets/empty-f3091520.svg
 starwhale/web/ui/assets/google-9d1a8b2b.svg
 starwhale/web/ui/assets/iconfont-0a880318.woff2
 starwhale/web/ui/assets/iconfont-10b60b11.ttf
 starwhale/web/ui/assets/iconfont-4c4e9d6d.woff
-starwhale/web/ui/assets/index-3bbbd54b.js
 starwhale/web/ui/assets/index-4b525ef6.css
-starwhale/web/ui/assets/index-890d4a46.js
-starwhale/web/ui/assets/index-af425f4b.js
+starwhale/web/ui/assets/index-87b297cf.js
 starwhale/web/ui/assets/index-ddbcf299.css
-starwhale/web/ui/assets/index10-4d13164f.js
-starwhale/web/ui/assets/index11-13eb176d.js
-starwhale/web/ui/assets/index12-de21ca8a.js
-starwhale/web/ui/assets/index13-0661cc45.js
-starwhale/web/ui/assets/index14-e2afac41.js
-starwhale/web/ui/assets/index15-9ee1eee9.js
-starwhale/web/ui/assets/index16-a0351c35.js
-starwhale/web/ui/assets/index17-a75792cc.js
-starwhale/web/ui/assets/index18-0b10ab02.js
-starwhale/web/ui/assets/index19-ceded876.js
-starwhale/web/ui/assets/index2-d042f67b.js
-starwhale/web/ui/assets/index20-d0bcc869.js
-starwhale/web/ui/assets/index21-d2f402e4.js
-starwhale/web/ui/assets/index22-c5e0b0dd.js
-starwhale/web/ui/assets/index23-e492630c.js
-starwhale/web/ui/assets/index24-1c64b765.js
-starwhale/web/ui/assets/index25-33571440.js
-starwhale/web/ui/assets/index26-d78d751e.js
-starwhale/web/ui/assets/index27-18127a28.js
-starwhale/web/ui/assets/index28-34a5ed1a.js
-starwhale/web/ui/assets/index29-e4ca565e.js
-starwhale/web/ui/assets/index3-b8136165.js
-starwhale/web/ui/assets/index30-334d010c.js
-starwhale/web/ui/assets/index31-1121988e.js
-starwhale/web/ui/assets/index32-80223294.js
-starwhale/web/ui/assets/index33-a4713f90.js
-starwhale/web/ui/assets/index34-69d671c0.js
-starwhale/web/ui/assets/index35-91b6f450.js
-starwhale/web/ui/assets/index36-6ce81ba8.js
-starwhale/web/ui/assets/index37-f530c08a.js
-starwhale/web/ui/assets/index38-fc6af5aa.js
-starwhale/web/ui/assets/index39-671ded20.js
-starwhale/web/ui/assets/index4-d076a84c.js
-starwhale/web/ui/assets/index5-529df1c0.js
-starwhale/web/ui/assets/index6-be007bee.js
-starwhale/web/ui/assets/index7-c3badb00.js
-starwhale/web/ui/assets/index8-2bbdfede.js
-starwhale/web/ui/assets/index9-0cbe1428.js
+starwhale/web/ui/assets/index-df1fb029.js
+starwhale/web/ui/assets/index-e17166cd.js
+starwhale/web/ui/assets/index10-7aed280d.js
+starwhale/web/ui/assets/index11-df7b8b7d.js
+starwhale/web/ui/assets/index12-f581388d.js
+starwhale/web/ui/assets/index13-fd2d632d.js
+starwhale/web/ui/assets/index14-94c12d28.js
+starwhale/web/ui/assets/index15-a31493a5.js
+starwhale/web/ui/assets/index16-2b049823.js
+starwhale/web/ui/assets/index17-d4811bf1.js
+starwhale/web/ui/assets/index18-d4ad6d1d.js
+starwhale/web/ui/assets/index19-18249feb.js
+starwhale/web/ui/assets/index2-667148f0.js
+starwhale/web/ui/assets/index20-0cc28676.js
+starwhale/web/ui/assets/index21-d3e36a16.js
+starwhale/web/ui/assets/index22-34fa8df0.js
+starwhale/web/ui/assets/index23-b30a6092.js
+starwhale/web/ui/assets/index24-11b8d91d.js
+starwhale/web/ui/assets/index25-4151ca38.js
+starwhale/web/ui/assets/index26-2968ddd0.js
+starwhale/web/ui/assets/index27-86c85604.js
+starwhale/web/ui/assets/index28-fce682a3.js
+starwhale/web/ui/assets/index29-7f2f8cac.js
+starwhale/web/ui/assets/index3-b632de7a.js
+starwhale/web/ui/assets/index30-449fed8c.js
+starwhale/web/ui/assets/index31-a39e3c8b.js
+starwhale/web/ui/assets/index32-5e251911.js
+starwhale/web/ui/assets/index33-8befa193.js
+starwhale/web/ui/assets/index34-d9e154ad.js
+starwhale/web/ui/assets/index35-71968f90.js
+starwhale/web/ui/assets/index36-6d6222b1.js
+starwhale/web/ui/assets/index37-03da10b3.js
+starwhale/web/ui/assets/index38-f8a193c1.js
+starwhale/web/ui/assets/index39-c97fb654.js
+starwhale/web/ui/assets/index4-2684c49d.js
+starwhale/web/ui/assets/index5-264c6674.js
+starwhale/web/ui/assets/index6-b60485d2.js
+starwhale/web/ui/assets/index7-ae38a6d6.js
+starwhale/web/ui/assets/index8-5ee4cbfe.js
+starwhale/web/ui/assets/index9-f552db0e.js
 starwhale/web/ui/assets/invalid-file-82d62dec.svg
 starwhale/web/ui/assets/left-8c88a49a.svg
 starwhale/web/ui/assets/left-shadow-e0fdfe32.png
 starwhale/web/ui/assets/linear-8d973619.js
 starwhale/web/ui/assets/logo_normal_en_blue-18b013e7.png
 starwhale/web/ui/assets/logo_normal_en_gray-163de1a0.svg
 starwhale/web/ui/assets/logo_normal_en_white-ec11283c.svg
 starwhale/web/ui/assets/logo_small_en_white-782559aa.svg
-starwhale/web/ui/assets/main-99f2bbfd.js
+starwhale/web/ui/assets/main-e0f2ffda.js
 starwhale/web/ui/assets/module-ddaca3b9.js
 starwhale/web/ui/assets/module2-74df381a.js
 starwhale/web/ui/assets/module3-49e9a615.js
 starwhale/web/ui/assets/overpass-bold-452a631f.woff
 starwhale/web/ui/assets/overpass-bold-5c4ed5bb.woff2
 starwhale/web/ui/assets/overpass-bold-italic-16cda7ef.woff2
 starwhale/web/ui/assets/overpass-bold-italic-4926428e.woff
```

### Comparing `starwhale-0.5.8/starwhale.egg-info/requires.txt` & `starwhale-0.5.9/starwhale.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -33,53 +33,53 @@
 urllib3<1.27
 pydantic<2.0.0
 
 [:python_version < "3.8"]
 importlib-metadata<=4.2.0,>=4.0.0
 
 [all]
-boto3>=1.26.14
-pyyaml==6.0
 requests>=2.1.0
-uvicorn
 typing-extensions>=4.0.0
-commonmark>=0.9.1
-GitPython>=3.1.24
+lz4>=3.1.10
 attrs>=21.4.0
-protobuf>=3.19.0
-dill>=0.3.6
-httpx>=0.22.0
-pillow
-fs>=2.4.0
-urllib3<1.27
-click>=8.0.4
-shellingham>=1.4.0
 textual==0.1.18
-psutil>=5.5.0
-scikit-learn>=0.20.0
-packaging>=21.3
-tenacity>=8.0.1
-lz4>=3.1.10
-click-option-group==0.5.5
-virtualenv>=13.0.0
-types-protobuf>=3.19.0
 soundfile
-gradio
+cattrs>=1.7.1
+pyarrow>=8.0.0
+conda-pack==0.6.0
+GitPython>=3.1.24
+trio>=0.22.0
+click-option-group==0.5.5
+fs>=2.4.0
+Jinja2>=3.1.2
 gradio~=3.15.0
+gradio
 jsonlines==3.0.0
-cattrs>=1.7.1
+types-protobuf>=3.19.0
+commonmark>=0.9.1
+scikit-learn>=0.20.0
+tenacity>=8.0.1
+shellingham>=1.4.0
+virtualenv>=13.0.0
+boto3>=1.26.14
+packaging>=21.3
+click>=8.0.4
 filelock
-loguru==0.6.0
-conda-pack==0.6.0
-pyarrow>=8.0.0
+uvicorn
 fastapi
-trio>=0.22.0
-pydantic<2.0.0
+loguru==0.6.0
+urllib3<1.27
+protobuf>=3.19.0
+httpx>=0.22.0
+psutil>=5.5.0
+dill>=0.3.6
+pyyaml==6.0
+pillow
 requests-toolbelt>=0.9.0
-Jinja2>=3.1.2
+pydantic<2.0.0
 
 [all:python_version < "3.8"]
 importlib-metadata<=4.2.0,>=4.0.0
 
 [audio]
 soundfile
```

