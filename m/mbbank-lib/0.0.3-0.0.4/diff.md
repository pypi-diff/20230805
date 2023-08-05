# Comparing `tmp/mbbank-lib-0.0.3.tar.gz` & `tmp/mbbank-lib-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbbank-lib-0.0.3.tar", last modified: Sat Aug  5 07:30:37 2023, max compression
+gzip compressed data, was "mbbank-lib-0.0.4.tar", last modified: Sat Aug  5 08:07:22 2023, max compression
```

## Comparing `mbbank-lib-0.0.3.tar` & `mbbank-lib-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:30:37.747768 mbbank-lib-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-05 07:30:31.000000 mbbank-lib-0.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-08-05 07:30:37.747768 mbbank-lib-0.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:30:37.747768 mbbank-lib-0.0.3/mbbank/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-05 07:30:31.000000 mbbank-lib-0.0.3/mbbank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-08-05 07:30:31.000000 mbbank-lib-0.0.3/mbbank/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:30:37.747768 mbbank-lib-0.0.3/mbbank_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-08-05 07:30:37.000000 mbbank-lib-0.0.3/mbbank_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-05 07:30:37.000000 mbbank-lib-0.0.3/mbbank_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 07:30:37.000000 mbbank-lib-0.0.3/mbbank_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-05 07:30:37.000000 mbbank-lib-0.0.3/mbbank_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-05 07:30:37.000000 mbbank-lib-0.0.3/mbbank_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 07:30:37.747768 mbbank-lib-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-05 07:30:31.000000 mbbank-lib-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 08:07:22.276631 mbbank-lib-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-05 08:07:09.000000 mbbank-lib-0.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-08-05 08:07:22.276631 mbbank-lib-0.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 08:07:22.276631 mbbank-lib-0.0.4/mbbank/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-05 08:07:09.000000 mbbank-lib-0.0.4/mbbank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-08-05 08:07:09.000000 mbbank-lib-0.0.4/mbbank/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 08:07:22.276631 mbbank-lib-0.0.4/mbbank_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-08-05 08:07:22.000000 mbbank-lib-0.0.4/mbbank_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-05 08:07:22.000000 mbbank-lib-0.0.4/mbbank_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 08:07:22.000000 mbbank-lib-0.0.4/mbbank_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-05 08:07:22.000000 mbbank-lib-0.0.4/mbbank_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-05 08:07:22.000000 mbbank-lib-0.0.4/mbbank_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 08:07:22.276631 mbbank-lib-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-05 08:07:09.000000 mbbank-lib-0.0.4/setup.py
```

### Comparing `mbbank-lib-0.0.3/LICENSE.txt` & `mbbank-lib-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mbbank-lib-0.0.3/PKG-INFO` & `mbbank-lib-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbbank-lib
-Version: 0.0.3
+Version: 0.0.4
 Summary: A unofficially light weight Python Api for the "Military Commercial Joint Stock Bank" accounts
 Home-page: https://github.com/thedtvn/MBBank
 Author: The DT
 License: Apache License, Version 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `mbbank-lib-0.0.3/mbbank/main.py` & `mbbank-lib-0.0.4/mbbank/main.py`

 * *Files identical despite different names*

### Comparing `mbbank-lib-0.0.3/mbbank_lib.egg-info/PKG-INFO` & `mbbank-lib-0.0.4/mbbank_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbbank-lib
-Version: 0.0.3
+Version: 0.0.4
 Summary: A unofficially light weight Python Api for the "Military Commercial Joint Stock Bank" accounts
 Home-page: https://github.com/thedtvn/MBBank
 Author: The DT
 License: Apache License, Version 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `mbbank-lib-0.0.3/setup.py` & `mbbank-lib-0.0.4/setup.py`

 * *Files identical despite different names*

