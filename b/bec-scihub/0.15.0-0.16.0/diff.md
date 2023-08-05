# Comparing `tmp/bec_scihub-0.15.0.tar.gz` & `tmp/bec_scihub-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_scihub-0.15.0.tar", last modified: Thu Aug  3 19:22:59 2023, max compression
+gzip compressed data, was "bec_scihub-0.16.0.tar", last modified: Fri Aug  4 18:28:16 2023, max compression
```

## Comparing `bec_scihub-0.15.0.tar` & `bec_scihub-0.16.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 19:22:59.139918 bec_scihub-0.15.0/
--rw-r--r--   0 root         (0) root         (0)      478 2023-08-03 19:22:59.139918 bec_scihub-0.15.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 19:22:59.139918 bec_scihub-0.15.0/bec_scihub.egg-info/
--rw-r--r--   0 root         (0) root         (0)      478 2023-08-03 19:22:59.000000 bec_scihub-0.15.0/bec_scihub.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      569 2023-08-03 19:22:59.000000 bec_scihub-0.15.0/bec_scihub.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 19:22:59.000000 bec_scihub-0.15.0/bec_scihub.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-08-03 19:22:59.000000 bec_scihub-0.15.0/bec_scihub.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-08-03 19:22:59.000000 bec_scihub-0.15.0/bec_scihub.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-08-03 19:22:59.000000 bec_scihub-0.15.0/bec_scihub.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 19:22:59.136918 bec_scihub-0.15.0/scihub/
--rw-r--r--   0 root         (0) root         (0)       56 2023-07-08 15:33:35.000000 bec_scihub-0.15.0/scihub/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 19:22:59.137918 bec_scihub-0.15.0/scihub/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 15:01:50.000000 bec_scihub-0.15.0/scihub/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      782 2023-07-08 15:33:35.000000 bec_scihub-0.15.0/scihub/cli/launch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 19:22:59.138918 bec_scihub-0.15.0/scihub/scibec/
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-06-19 08:14:59.000000 bec_scihub-0.15.0/scihub/scibec/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7654 2023-06-28 10:41:58.000000 bec_scihub-0.15.0/scihub/scibec/config_handler.py
--rw-r--r--   0 root         (0) root         (0)    15033 2023-06-28 10:41:58.000000 bec_scihub-0.15.0/scihub/scibec/scibec.py
--rw-r--r--   0 root         (0) root         (0)     4428 2023-06-28 10:41:58.000000 bec_scihub-0.15.0/scihub/scibec/scibec_connector.py
--rw-r--r--   0 root         (0) root         (0)     4126 2023-06-28 10:41:58.000000 bec_scihub-0.15.0/scihub/scibec/scibec_metadata_handler.py
--rw-rw-rw-   0 root         (0) root         (0)      880 2023-06-19 08:14:59.000000 bec_scihub-0.15.0/scihub/scibec/scibec_validator.py
--rw-r--r--   0 root         (0) root         (0)      902 2023-06-28 10:41:58.000000 bec_scihub-0.15.0/scihub/scihub.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 19:22:59.138918 bec_scihub-0.15.0/scihub/scilog/
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-19 08:14:59.000000 bec_scihub-0.15.0/scihub/scilog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3330 2023-06-28 10:41:58.000000 bec_scihub-0.15.0/scihub/scilog/scilog.py
--rw-r--r--   0 root         (0) root         (0)      538 2023-08-03 19:22:59.140918 bec_scihub-0.15.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1758 2023-08-03 19:22:53.000000 bec_scihub-0.15.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 18:28:16.464328 bec_scihub-0.16.0/
+-rw-r--r--   0 root         (0) root         (0)      478 2023-08-04 18:28:16.465328 bec_scihub-0.16.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 18:28:16.464328 bec_scihub-0.16.0/bec_scihub.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      478 2023-08-04 18:28:16.000000 bec_scihub-0.16.0/bec_scihub.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      569 2023-08-04 18:28:16.000000 bec_scihub-0.16.0/bec_scihub.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 18:28:16.000000 bec_scihub-0.16.0/bec_scihub.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-08-04 18:28:16.000000 bec_scihub-0.16.0/bec_scihub.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-08-04 18:28:16.000000 bec_scihub-0.16.0/bec_scihub.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-08-04 18:28:16.000000 bec_scihub-0.16.0/bec_scihub.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 18:28:16.462328 bec_scihub-0.16.0/scihub/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-08 15:33:35.000000 bec_scihub-0.16.0/scihub/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 18:28:16.462328 bec_scihub-0.16.0/scihub/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 15:01:50.000000 bec_scihub-0.16.0/scihub/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      782 2023-07-08 15:33:35.000000 bec_scihub-0.16.0/scihub/cli/launch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 18:28:16.463328 bec_scihub-0.16.0/scihub/scibec/
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-06-19 08:14:59.000000 bec_scihub-0.16.0/scihub/scibec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7654 2023-06-28 10:41:58.000000 bec_scihub-0.16.0/scihub/scibec/config_handler.py
+-rw-r--r--   0 root         (0) root         (0)    15033 2023-06-28 10:41:58.000000 bec_scihub-0.16.0/scihub/scibec/scibec.py
+-rw-r--r--   0 root         (0) root         (0)     4428 2023-06-28 10:41:58.000000 bec_scihub-0.16.0/scihub/scibec/scibec_connector.py
+-rw-r--r--   0 root         (0) root         (0)     4126 2023-06-28 10:41:58.000000 bec_scihub-0.16.0/scihub/scibec/scibec_metadata_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)      880 2023-06-19 08:14:59.000000 bec_scihub-0.16.0/scihub/scibec/scibec_validator.py
+-rw-r--r--   0 root         (0) root         (0)      902 2023-06-28 10:41:58.000000 bec_scihub-0.16.0/scihub/scihub.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 18:28:16.463328 bec_scihub-0.16.0/scihub/scilog/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-19 08:14:59.000000 bec_scihub-0.16.0/scihub/scilog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3330 2023-06-28 10:41:58.000000 bec_scihub-0.16.0/scihub/scilog/scilog.py
+-rw-r--r--   0 root         (0) root         (0)      538 2023-08-04 18:28:16.465328 bec_scihub-0.16.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1758 2023-08-04 18:28:09.000000 bec_scihub-0.16.0/setup.py
```

### Comparing `bec_scihub-0.15.0/bec_scihub.egg-info/SOURCES.txt` & `bec_scihub-0.16.0/bec_scihub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.15.0/scihub/cli/launch.py` & `bec_scihub-0.16.0/scihub/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.15.0/scihub/scibec/config_handler.py` & `bec_scihub-0.16.0/scihub/scibec/config_handler.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.15.0/scihub/scibec/scibec.py` & `bec_scihub-0.16.0/scihub/scibec/scibec.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.15.0/scihub/scibec/scibec_connector.py` & `bec_scihub-0.16.0/scihub/scibec/scibec_connector.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.15.0/scihub/scibec/scibec_metadata_handler.py` & `bec_scihub-0.16.0/scihub/scibec/scibec_metadata_handler.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.15.0/scihub/scibec/scibec_validator.py` & `bec_scihub-0.16.0/scihub/scibec/scibec_validator.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.15.0/scihub/scihub.py` & `bec_scihub-0.16.0/scihub/scihub.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.15.0/scihub/scilog/scilog.py` & `bec_scihub-0.16.0/scihub/scilog/scilog.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.15.0/setup.cfg` & `bec_scihub-0.16.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.15.0/setup.py` & `bec_scihub-0.16.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 current_path = pathlib.Path(__file__).parent.resolve()
 
 bec_lib = f"{current_path}/../bec_lib/"
 
 
-__version__ = "0.15.0"
+__version__ = "0.16.0"
 
 
 def run_install(setup_args: dict, bec_deps: list, editable=False):
     """
     Run the setup function with the given arguments.
 
     Args:
```

