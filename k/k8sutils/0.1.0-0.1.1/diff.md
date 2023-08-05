# Comparing `tmp/k8sutils-0.1.0.tar.gz` & `tmp/k8sutils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k8sutils-0.1.0.tar", last modified: Sat Aug  5 15:50:32 2023, max compression
+gzip compressed data, was "k8sutils-0.1.1.tar", last modified: Sat Aug  5 17:12:05 2023, max compression
```

## Comparing `k8sutils-0.1.0.tar` & `k8sutils-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:50:32.910396 k8sutils-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-05 15:50:23.000000 k8sutils-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-05 15:50:32.910396 k8sutils-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-05 15:50:23.000000 k8sutils-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:50:32.906396 k8sutils-0.1.0/k8sutils/
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-08-05 15:50:23.000000 k8sutils-0.1.0/k8sutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:50:32.906396 k8sutils-0.1.0/k8sutils/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 15:50:23.000000 k8sutils-0.1.0/k8sutils/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-05 15:50:23.000000 k8sutils-0.1.0/k8sutils/local/minikube.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-05 15:50:23.000000 k8sutils-0.1.0/k8sutils/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:50:32.906396 k8sutils-0.1.0/k8sutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-05 15:50:32.000000 k8sutils-0.1.0/k8sutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-08-05 15:50:32.000000 k8sutils-0.1.0/k8sutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 15:50:32.000000 k8sutils-0.1.0/k8sutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-05 15:50:32.000000 k8sutils-0.1.0/k8sutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 15:50:32.000000 k8sutils-0.1.0/k8sutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-05 15:50:23.000000 k8sutils-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 15:50:32.910396 k8sutils-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:12:05.203942 k8sutils-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-05 17:11:55.000000 k8sutils-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-05 17:12:05.203942 k8sutils-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-05 17:11:55.000000 k8sutils-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:12:05.199941 k8sutils-0.1.1/k8sutils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-08-05 17:11:55.000000 k8sutils-0.1.1/k8sutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:12:05.203942 k8sutils-0.1.1/k8sutils/crds/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-05 17:11:55.000000 k8sutils-0.1.1/k8sutils/crds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-05 17:11:55.000000 k8sutils-0.1.1/k8sutils/crds/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:12:05.203942 k8sutils-0.1.1/k8sutils/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 17:11:55.000000 k8sutils-0.1.1/k8sutils/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-05 17:11:55.000000 k8sutils-0.1.1/k8sutils/local/minikube.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-05 17:11:55.000000 k8sutils-0.1.1/k8sutils/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:12:05.199941 k8sutils-0.1.1/k8sutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-05 17:12:05.000000 k8sutils-0.1.1/k8sutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-05 17:12:05.000000 k8sutils-0.1.1/k8sutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 17:12:05.000000 k8sutils-0.1.1/k8sutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-05 17:12:05.000000 k8sutils-0.1.1/k8sutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 17:12:05.000000 k8sutils-0.1.1/k8sutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-05 17:11:55.000000 k8sutils-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 17:12:05.203942 k8sutils-0.1.1/setup.cfg
```

### Comparing `k8sutils-0.1.0/LICENSE` & `k8sutils-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `k8sutils-0.1.0/k8sutils/__init__.py` & `k8sutils-0.1.1/k8sutils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-import json
 import logging
 import os
 import requests
 import subprocess
 import tempfile
 from urllib.parse import urlparse
-from termcolor import colored
-from prettytable import PrettyTable
 
 
 # Configure the logger
 logging.basicConfig(level=logging.DEBUG,
                     format="%(asctime)s %(filename)s %(lineno)d> %(message)s",
                     datefmt="%Y-%m-%d %H:%M:%S")
 
@@ -38,34 +35,14 @@
 
     subprocess.run(f"bash {filename}", shell=True, check=True, capture_output=False)
 
 
     os.remove(filename)
 
 
-def list_crds():
-    json_text = subprocess.run("kubectl get crds -o json", shell=True, check=True, capture_output=True, text=True)
-    crds = json.loads(json_text.stdout)
-    return crds
-
-
-def print_crds(highlight=None):
-    crds = list_crds()
-    table = PrettyTable(["Name", "Creation Date"])
-
-    for crd in crds['items']:
-        table.add_row([crd['metadata']['name'], crd['metadata']['creationTimestamp']])
-
-    for line in str(table).split("\n"):
-        if highlight and highlight in line:
-            print(colored(line, 'green'))
-        else:
-            print(line)
-
-
 class Kind:
     def __init__(self):
         pass
 
     @staticmethod
     def create(version='1.26.3', config=None):
         cmd = f"kind create cluster --image=kindest/node:v{version}"
```

### Comparing `k8sutils-0.1.0/pyproject.toml` & `k8sutils-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "k8sutils"
-version = "0.1.0"
+version = "0.1.1"
 description = "Kubernetes helper module for Python"
 authors = [{ name = "Rui Vieira", email = "ruidevieira@googlemail.com" }]
 license = { text = "Apache License Version 2.0" }
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

