# Comparing `tmp/py-msgraph-0.0.1.tar.gz` & `tmp/py-msgraph-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\SUPERANT\Projects\django\pipy\py-msgraph\dist\.tmp-pi1_txxz\py-msgraph-0.0.1.tar", last modified: Sat Aug  5 00:35:31 2023, max compression
+gzip compressed data, was "C:\Users\SUPERANT\Projects\django\pipy\py-msgraph\dist\.tmp-n_or0ln1\py-msgraph-0.0.2.tar", last modified: Sat Aug  5 04:00:57 2023, max compression
```

## Comparing `py-msgraph-0.0.1.tar` & `py-msgraph-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 00:35:31.962839 py-msgraph-0.0.1/
--rw-rw-rw-   0        0        0     1096 2023-08-04 23:42:13.000000 py-msgraph-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     4177 2023-08-05 00:35:31.962839 py-msgraph-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2441 2023-08-05 00:23:51.000000 py-msgraph-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-05 00:35:31.949836 py-msgraph-0.0.1/py_msgraph/
--rw-rw-rw-   0        0        0        0 2023-08-05 00:29:00.000000 py-msgraph-0.0.1/py_msgraph/__init__.py
--rw-rw-rw-   0        0        0     3312 2023-08-04 23:41:33.000000 py-msgraph-0.0.1/py_msgraph/msgraph.py
-drwxrwxrwx   0        0        0        0 2023-08-05 00:35:31.960839 py-msgraph-0.0.1/py_msgraph.egg-info/
--rw-rw-rw-   0        0        0     4177 2023-08-05 00:35:31.000000 py-msgraph-0.0.1/py_msgraph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-08-05 00:35:31.000000 py-msgraph-0.0.1/py_msgraph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 00:35:31.000000 py-msgraph-0.0.1/py_msgraph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-08-05 00:35:31.000000 py-msgraph-0.0.1/py_msgraph.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      627 2023-08-04 23:46:04.000000 py-msgraph-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-05 00:35:31.962839 py-msgraph-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-08-04 23:43:08.000000 py-msgraph-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 04:00:57.120831 py-msgraph-0.0.2/
+-rw-rw-rw-   0        0        0     1096 2023-08-04 23:42:13.000000 py-msgraph-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4224 2023-08-05 04:00:57.120831 py-msgraph-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2488 2023-08-05 03:45:56.000000 py-msgraph-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 04:00:57.120831 py-msgraph-0.0.2/py_msgraph/
+-rw-rw-rw-   0        0        0       82 2023-08-05 03:45:22.000000 py-msgraph-0.0.2/py_msgraph/__init__.py
+-rw-rw-rw-   0        0        0     3312 2023-08-04 23:41:33.000000 py-msgraph-0.0.2/py_msgraph/msgraph.py
+drwxrwxrwx   0        0        0        0 2023-08-05 04:00:57.120831 py-msgraph-0.0.2/py_msgraph.egg-info/
+-rw-rw-rw-   0        0        0     4224 2023-08-05 04:00:57.000000 py-msgraph-0.0.2/py_msgraph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-08-05 04:00:57.000000 py-msgraph-0.0.2/py_msgraph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 04:00:57.000000 py-msgraph-0.0.2/py_msgraph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-05 04:00:57.000000 py-msgraph-0.0.2/py_msgraph.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      627 2023-08-05 03:27:28.000000 py-msgraph-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-05 04:00:57.136478 py-msgraph-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-08-04 23:43:08.000000 py-msgraph-0.0.2/setup.py
```

### Comparing `py-msgraph-0.0.1/LICENSE` & `py-msgraph-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py-msgraph-0.0.1/PKG-INFO` & `py-msgraph-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-msgraph
-Version: 0.0.1
+Version: 0.0.2
 Summary: library to use MS graph API
 Author-email: Sungwon Um <shineum@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Sungwon Um
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,15 +34,15 @@
 License-File: LICENSE
 
 # Installation
 
 Use pip:
 
 ```
-pip install py_msgraph
+pip install py-msgraph
 ```
 or
 
 ```
 pip install git+https://github.com/shineum/py_msgraph.git
 ```
 
@@ -64,14 +64,16 @@
 ```
 
 
 # Getting Started
 Initialize MSGraphServiceClient instance.
 
 ```
+from py_msgraph import MSGraphServiceClient
+
 config = {
     'tenant_id':      '<tentant_id>',
     'client_id':      '<client_id>',
     'client_secret':  '<client_secret>'
 }
 
 client: MSGraphServiceClient = MSGraphServiceClient(config)
```

### Comparing `py-msgraph-0.0.1/README.md` & `py-msgraph-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Installation
 
 Use pip:
 
 ```
-pip install py_msgraph
+pip install py-msgraph
 ```
 or
 
 ```
 pip install git+https://github.com/shineum/py_msgraph.git
 ```
 
@@ -29,14 +29,16 @@
 ```
 
 
 # Getting Started
 Initialize MSGraphServiceClient instance.
 
 ```
+from py_msgraph import MSGraphServiceClient
+
 config = {
     'tenant_id':      '<tentant_id>',
     'client_id':      '<client_id>',
     'client_secret':  '<client_secret>'
 }
 
 client: MSGraphServiceClient = MSGraphServiceClient(config)
```

### Comparing `py-msgraph-0.0.1/py_msgraph/msgraph.py` & `py-msgraph-0.0.2/py_msgraph/msgraph.py`

 * *Files identical despite different names*

### Comparing `py-msgraph-0.0.1/py_msgraph.egg-info/PKG-INFO` & `py-msgraph-0.0.2/py_msgraph.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-msgraph
-Version: 0.0.1
+Version: 0.0.2
 Summary: library to use MS graph API
 Author-email: Sungwon Um <shineum@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Sungwon Um
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,15 +34,15 @@
 License-File: LICENSE
 
 # Installation
 
 Use pip:
 
 ```
-pip install py_msgraph
+pip install py-msgraph
 ```
 or
 
 ```
 pip install git+https://github.com/shineum/py_msgraph.git
 ```
 
@@ -64,14 +64,16 @@
 ```
 
 
 # Getting Started
 Initialize MSGraphServiceClient instance.
 
 ```
+from py_msgraph import MSGraphServiceClient
+
 config = {
     'tenant_id':      '<tentant_id>',
     'client_id':      '<client_id>',
     'client_secret':  '<client_secret>'
 }
 
 client: MSGraphServiceClient = MSGraphServiceClient(config)
```

### Comparing `py-msgraph-0.0.1/pyproject.toml` & `py-msgraph-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py-msgraph"
-version = "0.0.1"
+version = "0.0.2"
 description = "library to use MS graph API"
 readme = "README.md"
 authors = [{ name = "Sungwon Um", email = "shineum@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

