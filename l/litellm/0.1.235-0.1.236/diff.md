# Comparing `tmp/litellm-0.1.235.tar.gz` & `tmp/litellm-0.1.236.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.235.tar", last modified: Sat Aug  5 16:26:41 2023, max compression
+gzip compressed data, was "litellm-0.1.236.tar", last modified: Sat Aug  5 16:32:06 2023, max compression
```

## Comparing `litellm-0.1.235.tar` & `litellm-0.1.236.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:26:41.237317 litellm-0.1.235/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1065 2023-08-05 16:26:31.000000 litellm-0.1.235/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-05 16:26:41.237317 litellm-0.1.235/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2285 2023-08-05 16:26:31.000000 litellm-0.1.235/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:26:41.237317 litellm-0.1.235/litellm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1964 2023-08-05 16:26:31.000000 litellm-0.1.235/litellm/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:26:41.237317 litellm-0.1.235/litellm/integrations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2023-08-05 16:26:31.000000 litellm-0.1.235/litellm/integrations/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3548 2023-08-05 16:26:31.000000 litellm-0.1.235/litellm/integrations/helicone.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12702 2023-08-05 16:26:31.000000 litellm-0.1.235/litellm/main.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2893 2023-08-05 16:26:31.000000 litellm-0.1.235/litellm/timeout.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15221 2023-08-05 16:26:31.000000 litellm-0.1.235/litellm/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:26:41.237317 litellm-0.1.235/litellm.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-05 16:26:41.000000 litellm-0.1.235/litellm.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      333 2023-08-05 16:26:41.000000 litellm-0.1.235/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-05 16:26:41.000000 litellm-0.1.235/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-08-05 16:26:41.000000 litellm-0.1.235/litellm.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-08-05 16:26:41.000000 litellm-0.1.235/litellm.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2023-08-05 16:26:31.000000 litellm-0.1.235/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-05 16:26:41.237317 litellm-0.1.235/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      546 2023-08-05 16:26:31.000000 litellm-0.1.235/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:32:06.285492 litellm-0.1.236/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1065 2023-08-05 16:31:56.000000 litellm-0.1.236/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-05 16:32:06.285492 litellm-0.1.236/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2285 2023-08-05 16:31:56.000000 litellm-0.1.236/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:32:06.285492 litellm-0.1.236/litellm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1964 2023-08-05 16:31:56.000000 litellm-0.1.236/litellm/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:32:06.285492 litellm-0.1.236/litellm/integrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2023-08-05 16:31:56.000000 litellm-0.1.236/litellm/integrations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3548 2023-08-05 16:31:56.000000 litellm-0.1.236/litellm/integrations/helicone.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12702 2023-08-05 16:31:56.000000 litellm-0.1.236/litellm/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2893 2023-08-05 16:31:56.000000 litellm-0.1.236/litellm/timeout.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15221 2023-08-05 16:31:56.000000 litellm-0.1.236/litellm/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:32:06.285492 litellm-0.1.236/litellm.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-05 16:32:06.000000 litellm-0.1.236/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      333 2023-08-05 16:32:06.000000 litellm-0.1.236/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-05 16:32:06.000000 litellm-0.1.236/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-08-05 16:32:06.000000 litellm-0.1.236/litellm.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-08-05 16:32:06.000000 litellm-0.1.236/litellm.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2023-08-05 16:31:56.000000 litellm-0.1.236/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-05 16:32:06.285492 litellm-0.1.236/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      546 2023-08-05 16:31:56.000000 litellm-0.1.236/setup.py
```

### Comparing `litellm-0.1.235/LICENSE` & `litellm-0.1.236/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.235/README.md` & `litellm-0.1.236/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.235/litellm/__init__.py` & `litellm-0.1.236/litellm/__init__.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.235/litellm/integrations/helicone.py` & `litellm-0.1.236/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.235/litellm/main.py` & `litellm-0.1.236/litellm/main.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.235/litellm/timeout.py` & `litellm-0.1.236/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.235/litellm/utils.py` & `litellm-0.1.236/litellm/utils.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.235/setup.py` & `litellm-0.1.236/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='litellm',
-    version='0.1.235',
+    version='0.1.236',
     description='Library to easily interface with LLM API providers',
     author='BerriAI',
     packages=[
         'litellm'
     ],
     package_data={
         "litellm": ["integrations/*"],  # Specify the directory path relative to your package
```

