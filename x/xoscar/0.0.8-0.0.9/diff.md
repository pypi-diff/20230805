# Comparing `tmp/xoscar-0.0.8.tar.gz` & `tmp/xoscar-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xoscar-0.0.8.tar", last modified: Fri Jul  7 08:47:40 2023, max compression
+gzip compressed data, was "xoscar-0.0.9.tar", last modified: Sat Aug  5 11:01:58 2023, max compression
```

## Comparing `xoscar-0.0.8.tar` & `xoscar-0.0.9.tar`

### file list

```diff
@@ -1,98 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.385716 xoscar-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-07 08:47:06.000000 xoscar-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-07-07 08:47:40.385716 xoscar-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-07 08:47:06.000000 xoscar-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-07 08:47:40.389716 xoscar-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-07-07 08:47:06.000000 xoscar-0.0.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-07-07 08:47:06.000000 xoscar-0.0.8/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.373715 xoscar-0.0.8/xoscar/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/_utils.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    23719 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.377715 xoscar-0.0.8/xoscar/aio/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/aio/_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/aio/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/aio/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/aio/lru.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/aio/parallelism.py
--rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.377715 xoscar-0.0.8/xoscar/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/allocate_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.381716 xoscar-0.0.8/xoscar/backends/communication/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/communication/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/communication/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/communication/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/communication/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/communication/socket.py
--rw-r--r--   0 runner    (1001) docker     (123)    19359 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/communication/ucx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/communication/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15285 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.381716 xoscar-0.0.8/xoscar/backends/indigen/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/indigen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/indigen/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/indigen/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/indigen/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/message.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    57991 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.381716 xoscar-0.0.8/xoscar/backends/test/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/test/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/test/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.381716 xoscar-0.0.8/xoscar/collective/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/collective/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.381716 xoscar-0.0.8/xoscar/collective/rendezvous/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/collective/rendezvous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.381716 xoscar-0.0.8/xoscar/collective/rendezvous/test/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/collective/rendezvous/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/collective/rendezvous/test/test_tcp_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/context.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/context.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/core.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/core.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/libcpp.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.381716 xoscar-0.0.8/xoscar/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/metrics/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.381716 xoscar-0.0.8/xoscar/metrics/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/metrics/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.385716 xoscar-0.0.8/xoscar/metrics/backends/console/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/metrics/backends/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/metrics/backends/console/console_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/metrics/backends/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.385716 xoscar-0.0.8/xoscar/metrics/backends/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/metrics/backends/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/metrics/backends/prometheus/prometheus_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    20412 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/nvutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.385716 xoscar-0.0.8/xoscar/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/serialization/aio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/serialization/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/serialization/core.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    29468 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/serialization/core.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/serialization/cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/serialization/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/serialization/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/serialization/scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14610 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.373715 xoscar-0.0.8/xoscar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-07-07 08:47:40.000000 xoscar-0.0.8/xoscar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-07 08:47:40.000000 xoscar-0.0.8/xoscar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:47:40.000000 xoscar-0.0.8/xoscar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:47:39.000000 xoscar-0.0.8/xoscar.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-07 08:47:40.000000 xoscar-0.0.8/xoscar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-07 08:47:40.000000 xoscar-0.0.8/xoscar.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:01:57.998177 xoscar-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-05 11:01:27.000000 xoscar-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-08-05 11:01:57.998177 xoscar-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-08-05 11:01:27.000000 xoscar-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-08-05 11:01:57.998177 xoscar-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    13149 2023-08-05 11:01:27.000000 xoscar-0.0.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-08-05 11:01:27.000000 xoscar-0.0.9/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:01:57.994177 xoscar-0.0.9/xoscar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/_utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    23719 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:01:57.994177 xoscar-0.0.9/xoscar/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/aio/_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/aio/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/aio/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/aio/lru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/aio/parallelism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:01:57.994177 xoscar-0.0.9/xoscar/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/backends/allocate_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:01:57.994177 xoscar-0.0.9/xoscar/backends/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/backends/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/backends/communication/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/backends/communication/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/backends/communication/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/backends/communication/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/backends/communication/socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/backends/communication/ucx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/backends/communication/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/backends/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15285 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/backends/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/backends/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:01:57.994177 xoscar-0.0.9/xoscar/backends/indigen/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/backends/indigen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/backends/indigen/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/backends/indigen/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/backends/indigen/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/backends/message.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    57991 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/backends/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/backends/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:01:57.994177 xoscar-0.0.9/xoscar/backends/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/backends/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/backends/test/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/backends/test/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:01:57.994177 xoscar-0.0.9/xoscar/collective/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/collective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/collective/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10227 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/collective/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/collective/process_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/collective/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/context.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/context.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/core.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    20965 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/core.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/libcpp.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:01:57.994177 xoscar-0.0.9/xoscar/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/metrics/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:01:57.998177 xoscar-0.0.9/xoscar/metrics/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/metrics/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:01:57.998177 xoscar-0.0.9/xoscar/metrics/backends/console/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/metrics/backends/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/metrics/backends/console/console_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/metrics/backends/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:01:57.998177 xoscar-0.0.9/xoscar/metrics/backends/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/metrics/backends/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/metrics/backends/prometheus/prometheus_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20412 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/nvutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:01:57.998177 xoscar-0.0.9/xoscar/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/serialization/aio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/serialization/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/serialization/core.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    29468 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/serialization/core.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/serialization/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/serialization/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/serialization/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/serialization/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14672 2023-08-05 11:01:27.000000 xoscar-0.0.9/xoscar/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:01:57.994177 xoscar-0.0.9/xoscar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-08-05 11:01:57.000000 xoscar-0.0.9/xoscar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-08-05 11:01:57.000000 xoscar-0.0.9/xoscar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 11:01:57.000000 xoscar-0.0.9/xoscar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 11:01:57.000000 xoscar-0.0.9/xoscar.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-05 11:01:57.000000 xoscar-0.0.9/xoscar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-05 11:01:57.000000 xoscar-0.0.9/xoscar.egg-info/top_level.txt
```

### Comparing `xoscar-0.0.8/PKG-INFO` & `xoscar-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xoscar
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python actor framework for heterogeneous computing.
 Home-page: http://github.com/xorbitsai/xoscar
 Author: Qin Xuye
 Author-email: qinxuye@xprobe.io
 Maintainer: Qin Xuye
 Maintainer-email: qinxuye@xprobe.io
 License: Apache License 2.0
```

### Comparing `xoscar-0.0.8/pyproject.toml` & `xoscar-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/setup.cfg` & `xoscar-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/setup.py` & `xoscar-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import platform
 import re
 import subprocess
 import sys
 from distutils.command.build_ext import build_ext as _du_build_ext
 from distutils.file_util import copy_file
 from pathlib import Path
+
 from sysconfig import get_config_vars
 
 import numpy as np
 from Cython.Build import cythonize
 from pkg_resources import parse_version
 from setuptools import Extension, setup
 from setuptools.command.build_ext import build_ext
@@ -142,25 +143,25 @@
     "win-arm64": "ARM64",
 }
 
 
 # A CMakeExtension needs a sourcedir instead of a file list.
 # The name must be the _single_ output extension from the CMake build.
 # If you need multiple extensions, see scikit-build.
-class XoscarStoreExtension(Extension):
+class XoscarCmakeExtension(Extension):
     def __init__(self, name: str, sourcedir: str = "") -> None:
         super().__init__(name, sources=[])
         self.sourcedir = os.fspath(Path(sourcedir).resolve())
 
 
 class CMakeBuild(build_ext):
     def copy_extensions_to_source(self):
         build_py = self.get_finalized_command('build_py')
         for ext in self.extensions:
-            if not isinstance(ext, XoscarStoreExtension):
+            if not isinstance(ext, XoscarCmakeExtension):
                 fullname = self.get_ext_fullname(ext.name)
                 filename = self.get_ext_filename(fullname)
                 modpath = fullname.split('.')
                 package = '.'.join(modpath[:-1])
                 package_dir = build_py.get_package_dir(package)
                 dest_filename = os.path.join(package_dir,
                                              os.path.basename(filename))
@@ -171,41 +172,66 @@
                 # used.
                 copy_file(
                     src_filename, dest_filename, verbose=self.verbose,
                     dry_run=self.dry_run
                 )
                 if ext._needs_stub:
                     self.write_stub(package_dir or os.curdir, ext, True)
+            elif sys.platform.startswith('win'):
+                fullname = self.get_ext_fullname(ext.name)
+                filename = self.get_ext_filename(fullname)
+                modpath = fullname.split('.')
+                package = '.'.join(modpath[:-1])
+                package_dir = build_py.get_package_dir(package)
+                if package_dir=="" and ext.name=="xoscar_pygloo":
+                    package_dir="xoscar/collective"
+                dest_filename = os.path.join(package_dir,
+                                                os.path.basename(filename))
+                src_filename = os.path.join(self.build_lib, filename)
+
+                # Always copy, even if source is older than destination, to ensure
+                # that the right extensions for the current Python/platform are
+                # used.
+                copy_file(
+                    src_filename, dest_filename, verbose=self.verbose,
+                    dry_run=self.dry_run
+                )
+                if ext._needs_stub:
+                    self.write_stub(package_dir or os.curdir, ext, True)
 
     def build_extension(self, ext):
         # TODO: support windows compilation
         is_windows = sys.platform.startswith('win')
-        if isinstance(ext, XoscarStoreExtension) and not is_windows:
-            self.build_store(ext)
-        elif isinstance(ext, XoscarStoreExtension) and is_windows:
+        bit_number = platform.architecture()[0]
+        if isinstance(ext, XoscarCmakeExtension) and not (is_windows and bit_number=="32bit"):
+            self.build_Cmake(ext)
+        elif isinstance(ext, XoscarCmakeExtension) and (is_windows and bit_number=="32bit"):
             pass
         else:
             ext._convert_pyx_sources_to_lang()
             _compiler = self.compiler
             try:
                 if isinstance(ext, Library):
                     self.compiler = self.shlib_compiler
                 _build_ext.build_extension(self, ext)
                 if ext._needs_stub:
                     build_lib = self.get_finalized_command('build_py').build_lib
                     self.write_stub(build_lib, ext)
             finally:
                 self.compiler = _compiler
 
-    def build_store(self, ext: XoscarStoreExtension) -> None:
+    def build_Cmake(self, ext: XoscarCmakeExtension) -> None:
         # Must be in this form due to bug in .resolve() only fixed in Python 3.10+
         ext_fullpath = Path.cwd() / self.get_ext_fullpath(ext.name)
         extdir = ext_fullpath.parent.resolve()
         source_dir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-        output_directory = Path(source_dir) / "python" / "xoscar" / "collective" / "rendezvous"
+        output_directory_collective = Path(source_dir) / "python" / "xoscar" / "collective"
+        build_temp = Path(self.build_temp) / ext.name
+        if not build_temp.exists():
+            build_temp.mkdir(parents=True)
 
         # Using this requires trailing slash for auto-detection & inclusion of
         # auxiliary "native" libs
 
         debug = int(os.environ.get("DEBUG", 0)) if self.debug is None else self.debug
         cfg = "Debug" if debug else "Release"
 
@@ -213,15 +239,16 @@
         # Can be set with Conda-Build, for example.
         cmake_generator = os.environ.get("CMAKE_GENERATOR", "")
 
         # Set Python_EXECUTABLE instead if you use PYBIND11_FINDPYTHON
         # EXAMPLE_VERSION_INFO shows you how to pass a value into the C++ code
         # from Python.
         cmake_args = [
-            f"-DLIBRARY_OUTPUT_DIRECTORY={output_directory}",
+            f"-DBUILD_TMP_DIR={build_temp}",
+            f"-DLIBRARY_OUTPUT_DIRECTORY={output_directory_collective}",
             f"-DPYTHON_PATH={sys.executable}",
             f"-DCMAKE_BUILD_TYPE={cfg}",  # not used on MSVC, but no harm
         ]
         build_args = []
         # Adding CMake arguments set as environment variable
         # (needed e.g. to build for ARM OSx on conda-forge)
         if "CMAKE_ARGS" in os.environ:
@@ -276,27 +303,25 @@
         if "CMAKE_BUILD_PARALLEL_LEVEL" not in os.environ:
             # self.parallel is a Python 3 only way to set parallel jobs by hand
             # using -j in the build_ext call, not supported by pip or PyPA-build.
             if hasattr(self, "parallel") and self.parallel:
                 # CMake 3.12+ only.
                 build_args += [f"-j{self.parallel}"]
 
-        build_temp = Path(self.build_temp) / ext.name
-        if not build_temp.exists():
-            build_temp.mkdir(parents=True)
+
 
         subprocess.run(
             ["cmake", source_dir, *cmake_args], cwd=build_temp, check=True
         )
         subprocess.run(
             ["cmake", "--build", ".", *build_args], cwd=build_temp, check=True
         )
 
 
 setup_options = dict(
     version=versioneer.get_version(),
-    ext_modules=extensions + [XoscarStoreExtension("xoscar_store")],
+    ext_modules=extensions + [XoscarCmakeExtension("xoscar_pygloo")],
     cmdclass={"build_ext": CMakeBuild},
     long_description=build_long_description(),
     long_description_content_type="text/markdown",
 )
 setup(**setup_options)
```

### Comparing `xoscar-0.0.8/versioneer.py` & `xoscar-0.0.9/versioneer.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/__init__.py` & `xoscar-0.0.9/xoscar/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     setup_cluster,
     wait_actor_pool_recovered,
     get_pool_config,
 )
 from .backends import allocate_strategy
 from .backends.pool import MainActorPoolType
 from .batch import extensible
-from .core import ActorRef
+from .core import ActorRef, no_lock
 from .debug import set_debug_options, get_debug_options, DebugOptions
 from .errors import (
     ActorNotExist,
     ActorAlreadyExist,
     ServerClosed,
     SendMessageFailed,
     Return,
```

### Comparing `xoscar-0.0.8/xoscar/_utils.pxd` & `xoscar-0.0.9/xoscar/_utils.pxd`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/_utils.pyx` & `xoscar-0.0.9/xoscar/_utils.pyx`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/_version.py` & `xoscar-0.0.9/xoscar/_version.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/aio/__init__.py` & `xoscar-0.0.9/xoscar/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/aio/_threads.py` & `xoscar-0.0.9/xoscar/aio/_threads.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/aio/base.py` & `xoscar-0.0.9/xoscar/aio/base.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/aio/file.py` & `xoscar-0.0.9/xoscar/aio/file.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/aio/lru.py` & `xoscar-0.0.9/xoscar/aio/lru.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/aio/parallelism.py` & `xoscar-0.0.9/xoscar/aio/parallelism.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/api.py` & `xoscar-0.0.9/xoscar/api.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/backend.py` & `xoscar-0.0.9/xoscar/backend.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/backends/__init__.py` & `xoscar-0.0.9/xoscar/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/backends/allocate_strategy.py` & `xoscar-0.0.9/xoscar/backends/allocate_strategy.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/backends/communication/__init__.py` & `xoscar-0.0.9/xoscar/backends/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/backends/communication/base.py` & `xoscar-0.0.9/xoscar/backends/communication/base.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/backends/communication/core.py` & `xoscar-0.0.9/xoscar/backends/communication/core.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/backends/communication/dummy.py` & `xoscar-0.0.9/xoscar/backends/communication/dummy.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/backends/communication/errors.py` & `xoscar-0.0.9/xoscar/backends/communication/errors.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/backends/communication/socket.py` & `xoscar-0.0.9/xoscar/backends/communication/socket.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/backends/communication/ucx.py` & `xoscar-0.0.9/xoscar/backends/communication/ucx.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,16 +308,15 @@
                 meta_buffers = await self._serialize(meta)
 
             async with self._send_lock:
                 if meta_buffers:
                     for buf in meta_buffers:
                         await self.ucp_endpoint.send(buf)
                 for buffer in buffers:
-                    if buffer.nbytes if hasattr(buffer, "nbytes") else len(buffer) > 0:
-                        await self.ucp_endpoint.send(buffer)
+                    await self.ucp_endpoint.send(buffer)
         except ucp.exceptions.UCXBaseException:  # pragma: no cover
             self.abort()
             raise ChannelClosed("While writing, the connection was closed")
 
     async def recv_buffers(self, buffers: list):
         async with self._recv_lock:
             try:
```

### Comparing `xoscar-0.0.8/xoscar/backends/communication/utils.py` & `xoscar-0.0.9/xoscar/backends/communication/utils.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/backends/config.py` & `xoscar-0.0.9/xoscar/backends/config.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/backends/context.py` & `xoscar-0.0.9/xoscar/backends/context.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/backends/core.py` & `xoscar-0.0.9/xoscar/backends/core.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/backends/indigen/__init__.py` & `xoscar-0.0.9/xoscar/backends/indigen/__init__.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/backends/indigen/backend.py` & `xoscar-0.0.9/xoscar/backends/indigen/backend.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/backends/indigen/driver.py` & `xoscar-0.0.9/xoscar/backends/indigen/driver.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/backends/indigen/pool.py` & `xoscar-0.0.9/xoscar/backends/indigen/pool.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/backends/message.pyx` & `xoscar-0.0.9/xoscar/backends/message.pyx`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/backends/pool.py` & `xoscar-0.0.9/xoscar/backends/pool.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/backends/router.py` & `xoscar-0.0.9/xoscar/backends/router.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/backends/test/__init__.py` & `xoscar-0.0.9/xoscar/backends/test/__init__.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/backends/test/backend.py` & `xoscar-0.0.9/xoscar/backends/test/backend.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/backends/test/pool.py` & `xoscar-0.0.9/xoscar/backends/test/pool.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/batch.py` & `xoscar-0.0.9/xoscar/batch.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 import asyncio
 import inspect
 import textwrap
 from collections import namedtuple
 from dataclasses import dataclass
 from typing import Any, Callable
 
+from .core import NO_LOCK_ATTRIBUTE_HINT
+
 
 def build_args_binder(func, remove_self: bool = True) -> Callable | None:
     try:
         spec = inspect.getfullargspec(func)
     except TypeError:  # pragma: no cover
         return None
 
@@ -217,18 +219,25 @@
         )
         bind_func = (
             self.bind_func.__get__(instance, owner)
             if self.bind_func is not None
             else None
         )
 
-        return _ExtensibleWrapper(
+        wrapper = _ExtensibleWrapper(
             func, batch_func=batch_func, bind_func=bind_func, is_async=self.is_async
         )
 
+        if (
+            getattr(self.func, NO_LOCK_ATTRIBUTE_HINT, None) is True
+            or getattr(self.batch_func, NO_LOCK_ATTRIBUTE_HINT, None) is True
+        ):
+            setattr(wrapper, NO_LOCK_ATTRIBUTE_HINT, True)
+        return wrapper
+
 
 def extensible(func: Callable):
     """
     `extensible` means this func could be functionality extended,
     especially for batch operations.
 
     Consider remote function calls, each function may have operations
```

### Comparing `xoscar-0.0.8/xoscar/collective/__init__.py` & `xoscar-0.0.9/xoscar/metrics/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/collective/rendezvous/__init__.py` & `xoscar-0.0.9/xoscar/metrics/backends/console/__init__.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/collective/rendezvous/test/__init__.py` & `xoscar-0.0.9/xoscar/metrics/backends/prometheus/__init__.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/constants.py` & `xoscar-0.0.9/xoscar/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 from pathlib import Path
 
-XOSCAR_TEMP_DIR = Path.home() / ".xoscar"
+XOSCAR_TEMP_DIR = Path(os.getenv("XOSCAR_DIR", Path.home())) / ".xoscar"
 
 # unix socket.
-XOSCAR_UNIX_SOCKET_DIR = os.path.join(XOSCAR_TEMP_DIR, "socket")
+XOSCAR_UNIX_SOCKET_DIR = XOSCAR_TEMP_DIR / "socket"
```

### Comparing `xoscar-0.0.8/xoscar/context.pxd` & `xoscar-0.0.9/xoscar/context.pxd`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/context.pyx` & `xoscar-0.0.9/xoscar/context.pyx`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/core.pxd` & `xoscar-0.0.9/xoscar/core.pxd`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/core.pyx` & `xoscar-0.0.9/xoscar/core.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -14,36 +14,41 @@
 # limitations under the License.
 
 import asyncio
 import inspect
 import logging
 import sys
 import weakref
-from typing import Any, AsyncGenerator
+from typing import Any, AsyncGenerator, Callable
 
 cimport cython
 
 from .aio import AioFileObject
 from .context cimport get_context
 
 from .errors import ActorNotExist, Return
 
 from ._utils cimport is_async_generator
 
 CALL_METHOD_DEFAULT = 0
 CALL_METHOD_BATCH = 1
+NO_LOCK_ATTRIBUTE_HINT = "__XOSCAR_ACTOR_METHOD_NO_LOCK__"
 
 logger = logging.getLogger(__name__)
 
 cdef:
     bint _log_unhandled_errors = False
     bint _log_cycle_send = False
     dict _local_pool_map = dict()
     object _actor_method_wrapper
 
+def no_lock(func: Callable):
+    setattr(func, NO_LOCK_ATTRIBUTE_HINT, True)
+    return func
+
 
 def set_debug_options(options):
     global _log_unhandled_errors, _log_cycle_send
     if options is None:
         _log_unhandled_errors = _log_cycle_send = False
     else:
         _log_unhandled_errors = options.log_unhandled_errors
@@ -258,19 +263,32 @@
             return method
 
     def __repr__(self):
         return 'LocalActorRef(uid={!r}, address={!r}), actor_weakref={!r}'.format(
             self.uid, self.address, self._actor_weakref)
 
 
+def _has_no_lock_hint_for_method(method) -> bool:
+    if getattr(method, NO_LOCK_ATTRIBUTE_HINT, False) is True:
+        return True
+    if hasattr(method, "__self__"):
+        return getattr(method.__self__, NO_LOCK_ATTRIBUTE_HINT, False) is True
+    return False
+
+
 async def __pyx_actor_method_wrapper(method, result_handler, lock, args, kwargs):
-    async with lock:
+    if _has_no_lock_hint_for_method(method):
         result = method(*args, **kwargs)
         if asyncio.iscoroutine(result):
             result = await result
+    else:
+        async with lock:
+            result = method(*args, **kwargs)
+            if asyncio.iscoroutine(result):
+                result = await result
     return await result_handler(result)
 
 # Avoid global lookup.
 _actor_method_wrapper = __pyx_actor_method_wrapper
 
 
 cdef class LocalActorRefMethod:
```

### Comparing `xoscar-0.0.8/xoscar/debug.py` & `xoscar-0.0.9/xoscar/debug.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/driver.py` & `xoscar-0.0.9/xoscar/driver.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/entrypoints.py` & `xoscar-0.0.9/xoscar/entrypoints.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/errors.py` & `xoscar-0.0.9/xoscar/errors.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/libcpp.pxd` & `xoscar-0.0.9/xoscar/libcpp.pxd`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/metrics/__init__.py` & `xoscar-0.0.9/xoscar/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/metrics/api.py` & `xoscar-0.0.9/xoscar/metrics/api.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/metrics/backends/console/console_metric.py` & `xoscar-0.0.9/xoscar/metrics/backends/console/console_metric.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/metrics/backends/metric.py` & `xoscar-0.0.9/xoscar/metrics/backends/metric.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/metrics/backends/prometheus/prometheus_metric.py` & `xoscar-0.0.9/xoscar/metrics/backends/prometheus/prometheus_metric.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/nvutils.py` & `xoscar-0.0.9/xoscar/nvutils.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/profiling.py` & `xoscar-0.0.9/xoscar/profiling.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/serialization/__init__.py` & `xoscar-0.0.9/xoscar/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/serialization/aio.py` & `xoscar-0.0.9/xoscar/serialization/aio.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/serialization/arrow.py` & `xoscar-0.0.9/xoscar/serialization/arrow.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/serialization/core.pxd` & `xoscar-0.0.9/xoscar/serialization/core.pxd`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/serialization/core.pyx` & `xoscar-0.0.9/xoscar/serialization/core.pyx`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/serialization/cuda.py` & `xoscar-0.0.9/xoscar/serialization/cuda.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/serialization/exception.py` & `xoscar-0.0.9/xoscar/serialization/exception.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/serialization/numpy.py` & `xoscar-0.0.9/xoscar/serialization/numpy.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/serialization/scipy.py` & `xoscar-0.0.9/xoscar/serialization/scipy.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.8/xoscar/utils.py` & `xoscar-0.0.9/xoscar/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -454,7 +454,11 @@
 
 def is_cuda_buffer(cuda_buffer: Union["_cupy.ndarray", "_rmm.DeviceBuffer"]) -> bool:  # type: ignore
     return hasattr(cuda_buffer, "__cuda_array_interface__")
 
 
 def is_windows():
     return sys.platform.startswith("win")
+
+
+def is_linux():
+    return sys.platform.startswith("linux")
```

### Comparing `xoscar-0.0.8/xoscar.egg-info/PKG-INFO` & `xoscar-0.0.9/xoscar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xoscar
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python actor framework for heterogeneous computing.
 Home-page: http://github.com/xorbitsai/xoscar
 Author: Qin Xuye
 Author-email: qinxuye@xprobe.io
 Maintainer: Qin Xuye
 Maintainer-email: qinxuye@xprobe.io
 License: Apache License 2.0
```

### Comparing `xoscar-0.0.8/xoscar.egg-info/SOURCES.txt` & `xoscar-0.0.9/xoscar.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -55,17 +55,18 @@
 xoscar/backends/indigen/backend.py
 xoscar/backends/indigen/driver.py
 xoscar/backends/indigen/pool.py
 xoscar/backends/test/__init__.py
 xoscar/backends/test/backend.py
 xoscar/backends/test/pool.py
 xoscar/collective/__init__.py
-xoscar/collective/rendezvous/__init__.py
-xoscar/collective/rendezvous/test/__init__.py
-xoscar/collective/rendezvous/test/test_tcp_store.py
+xoscar/collective/common.py
+xoscar/collective/core.py
+xoscar/collective/process_group.py
+xoscar/collective/utils.py
 xoscar/metrics/__init__.py
 xoscar/metrics/api.py
 xoscar/metrics/backends/__init__.py
 xoscar/metrics/backends/metric.py
 xoscar/metrics/backends/console/__init__.py
 xoscar/metrics/backends/console/console_metric.py
 xoscar/metrics/backends/prometheus/__init__.py
```

### Comparing `xoscar-0.0.8/xoscar.egg-info/requires.txt` & `xoscar-0.0.9/xoscar.egg-info/requires.txt`

 * *Files identical despite different names*

