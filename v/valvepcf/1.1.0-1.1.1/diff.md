# Comparing `tmp/valvepcf-1.1.0.tar.gz` & `tmp/valvepcf-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valvepcf-1.1.0.tar", last modified: Fri Aug 27 21:03:05 2021, max compression
+gzip compressed data, was "valvepcf-1.1.1.tar", last modified: Sat Aug  5 03:26:59 2023, max compression
```

## Comparing `valvepcf-1.1.0.tar` & `valvepcf-1.1.1.tar`

### file list

```diff
@@ -1,12 +1,20 @@
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2021-08-27 21:03:05.234702 valvepcf-1.1.0/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1051 2021-08-27 21:03:05.234702 valvepcf-1.1.0/PKG-INFO
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       40 2021-08-23 06:54:27.813855 valvepcf-1.1.0/setup.cfg
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1183 2021-08-27 20:59:45.704485 valvepcf-1.1.0/setup.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2021-08-27 21:03:05.234702 valvepcf-1.1.0/valvepcf/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      261 2021-08-23 06:54:27.813855 valvepcf-1.1.0/valvepcf/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     5040 2021-08-27 20:40:34.554297 valvepcf-1.1.0/valvepcf/classes.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      524 2021-08-23 06:54:27.813855 valvepcf-1.1.0/valvepcf/constants.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     5936 2021-08-27 20:28:12.036934 valvepcf-1.1.0/valvepcf/loader.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1448 2021-08-25 08:00:20.308399 valvepcf-1.1.0/valvepcf/pcf.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     2814 2021-08-23 06:54:27.813855 valvepcf-1.1.0/valvepcf/structs.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     7012 2021-08-27 20:30:13.904462 valvepcf-1.1.0/valvepcf/unloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:26:59.637333 valvepcf-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-05 03:26:48.000000 valvepcf-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-08-05 03:26:59.637333 valvepcf-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-08-05 03:26:48.000000 valvepcf-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 03:26:59.637333 valvepcf-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-08-05 03:26:57.000000 valvepcf-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:26:59.637333 valvepcf-1.1.1/valvepcf/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-05 03:26:48.000000 valvepcf-1.1.1/valvepcf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-08-05 03:26:48.000000 valvepcf-1.1.1/valvepcf/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-05 03:26:48.000000 valvepcf-1.1.1/valvepcf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-08-05 03:26:48.000000 valvepcf-1.1.1/valvepcf/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-08-05 03:26:48.000000 valvepcf-1.1.1/valvepcf/pcf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-08-05 03:26:48.000000 valvepcf-1.1.1/valvepcf/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-08-05 03:26:48.000000 valvepcf-1.1.1/valvepcf/unloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:26:59.637333 valvepcf-1.1.1/valvepcf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-08-05 03:26:59.000000 valvepcf-1.1.1/valvepcf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-05 03:26:59.000000 valvepcf-1.1.1/valvepcf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 03:26:59.000000 valvepcf-1.1.1/valvepcf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-05 03:26:59.000000 valvepcf-1.1.1/valvepcf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 03:26:59.000000 valvepcf-1.1.1/valvepcf.egg-info/top_level.txt
```

### Comparing `valvepcf-1.1.0/valvepcf/classes.py` & `valvepcf-1.1.1/valvepcf/classes.py`

 * *Files identical despite different names*

### Comparing `valvepcf-1.1.0/valvepcf/constants.py` & `valvepcf-1.1.1/valvepcf/constants.py`

 * *Files identical despite different names*

### Comparing `valvepcf-1.1.0/valvepcf/loader.py` & `valvepcf-1.1.1/valvepcf/loader.py`

 * *Files identical despite different names*

### Comparing `valvepcf-1.1.0/valvepcf/pcf.py` & `valvepcf-1.1.1/valvepcf/pcf.py`

 * *Files identical despite different names*

### Comparing `valvepcf-1.1.0/valvepcf/structs.py` & `valvepcf-1.1.1/valvepcf/structs.py`

 * *Files identical despite different names*

### Comparing `valvepcf-1.1.0/valvepcf/unloader.py` & `valvepcf-1.1.1/valvepcf/unloader.py`

 * *Files identical despite different names*

