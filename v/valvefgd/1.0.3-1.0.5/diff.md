# Comparing `tmp/valvefgd-1.0.3.tar.gz` & `tmp/valvefgd-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valvefgd-1.0.3.tar", last modified: Tue Nov  8 16:58:12 2022, max compression
+gzip compressed data, was "valvefgd-1.0.5.tar", last modified: Sat Aug  5 04:31:44 2023, max compression
```

## Comparing `valvefgd-1.0.3.tar` & `valvefgd-1.0.5.tar`

### file list

```diff
@@ -1,9 +1,17 @@
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2022-11-08 16:58:12.746605 valvefgd-1.0.3/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1032 2022-11-08 16:58:12.746605 valvefgd-1.0.3/PKG-INFO
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       39 2021-07-09 17:34:26.237039 valvefgd-1.0.3/setup.cfg
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1165 2022-11-08 16:55:07.782614 valvefgd-1.0.3/setup.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2022-11-08 16:58:12.746605 valvefgd-1.0.3/valvefgd/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      321 2021-07-09 17:34:26.269039 valvefgd-1.0.3/valvefgd/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    32741 2022-11-08 16:49:54.178964 valvefgd-1.0.3/valvefgd/fgd.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     7997 2022-11-08 16:40:00.567350 valvefgd-1.0.3/valvefgd/parser.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      405 2021-07-09 17:34:26.269039 valvefgd-1.0.3/valvefgd/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:31:44.548215 valvefgd-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-05 04:31:37.000000 valvefgd-1.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-08-05 04:31:44.548215 valvefgd-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-08-05 04:31:37.000000 valvefgd-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 04:31:44.548215 valvefgd-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-05 04:31:43.000000 valvefgd-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:31:44.548215 valvefgd-1.0.5/valvefgd/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-08-05 04:31:37.000000 valvefgd-1.0.5/valvefgd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32741 2023-08-05 04:31:37.000000 valvefgd-1.0.5/valvefgd/fgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-08-05 04:31:37.000000 valvefgd-1.0.5/valvefgd/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-05 04:31:37.000000 valvefgd-1.0.5/valvefgd/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:31:44.548215 valvefgd-1.0.5/valvefgd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-08-05 04:31:44.000000 valvefgd-1.0.5/valvefgd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-05 04:31:44.000000 valvefgd-1.0.5/valvefgd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 04:31:44.000000 valvefgd-1.0.5/valvefgd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-05 04:31:44.000000 valvefgd-1.0.5/valvefgd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 04:31:44.000000 valvefgd-1.0.5/valvefgd.egg-info/top_level.txt
```

### Comparing `valvefgd-1.0.3/valvefgd/fgd.py` & `valvefgd-1.0.5/valvefgd/fgd.py`

 * *Files identical despite different names*

### Comparing `valvefgd-1.0.3/valvefgd/parser.py` & `valvefgd-1.0.5/valvefgd/parser.py`

 * *Files identical despite different names*

