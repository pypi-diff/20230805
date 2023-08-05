# Comparing `tmp/litellm-0.1.232.tar.gz` & `tmp/litellm-0.1.233.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.232.tar", last modified: Fri Aug  4 21:56:14 2023, max compression
+gzip compressed data, was "litellm-0.1.233.tar", last modified: Sat Aug  5 16:13:28 2023, max compression
```

## Comparing `litellm-0.1.232.tar` & `litellm-0.1.233.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-08-04 21:56:14.761462 litellm-0.1.232/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-07-27 00:10:35.000000 litellm-0.1.232/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      215 2023-08-04 21:56:14.761350 litellm-0.1.232/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     2285 2023-08-03 17:46:06.000000 litellm-0.1.232/README.md
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-08-04 21:56:14.759959 litellm-0.1.232/litellm/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1872 2023-08-04 21:54:38.000000 litellm-0.1.232/litellm/__init__.py
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-08-04 21:56:14.761144 litellm-0.1.232/litellm/integrations/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       15 2023-08-03 17:46:06.000000 litellm-0.1.232/litellm/integrations/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3548 2023-08-03 17:46:06.000000 litellm-0.1.232/litellm/integrations/helicone.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)    12673 2023-08-04 21:54:38.000000 litellm-0.1.232/litellm/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     2893 2023-08-03 17:46:06.000000 litellm-0.1.232/litellm/timeout.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)    15221 2023-08-03 17:46:06.000000 litellm-0.1.232/litellm/utils.py
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-08-04 21:56:14.760813 litellm-0.1.232/litellm.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      215 2023-08-04 21:56:14.000000 litellm-0.1.232/litellm.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      333 2023-08-04 21:56:14.000000 litellm-0.1.232/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-08-04 21:56:14.000000 litellm-0.1.232/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       80 2023-08-04 21:56:14.000000 litellm-0.1.232/litellm.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        8 2023-08-04 21:56:14.000000 litellm-0.1.232/litellm.egg-info/top_level.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      473 2023-08-03 04:02:44.000000 litellm-0.1.232/pyproject.toml
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-08-04 21:56:14.761501 litellm-0.1.232/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      546 2023-08-04 21:54:59.000000 litellm-0.1.232/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:13:28.366069 litellm-0.1.233/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1065 2023-08-05 16:13:16.000000 litellm-0.1.233/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-05 16:13:28.366069 litellm-0.1.233/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2285 2023-08-05 16:13:16.000000 litellm-0.1.233/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:13:28.362069 litellm-0.1.233/litellm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1964 2023-08-05 16:13:16.000000 litellm-0.1.233/litellm/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:13:28.366069 litellm-0.1.233/litellm/integrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2023-08-05 16:13:16.000000 litellm-0.1.233/litellm/integrations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3548 2023-08-05 16:13:16.000000 litellm-0.1.233/litellm/integrations/helicone.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12673 2023-08-05 16:13:16.000000 litellm-0.1.233/litellm/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2893 2023-08-05 16:13:16.000000 litellm-0.1.233/litellm/timeout.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15221 2023-08-05 16:13:16.000000 litellm-0.1.233/litellm/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:13:28.366069 litellm-0.1.233/litellm.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-05 16:13:28.000000 litellm-0.1.233/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      333 2023-08-05 16:13:28.000000 litellm-0.1.233/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-05 16:13:28.000000 litellm-0.1.233/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-08-05 16:13:28.000000 litellm-0.1.233/litellm.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-08-05 16:13:28.000000 litellm-0.1.233/litellm.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2023-08-05 16:13:16.000000 litellm-0.1.233/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-05 16:13:28.366069 litellm-0.1.233/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      546 2023-08-05 16:13:16.000000 litellm-0.1.233/setup.py
```

### Comparing `litellm-0.1.232/LICENSE` & `litellm-0.1.233/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.232/README.md` & `litellm-0.1.233/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.232/litellm/__init__.py` & `litellm-0.1.233/litellm/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -43,14 +43,18 @@
 ]
 open_ai_text_completion_models = [
     'text-davinci-003'
 ]
 
 cohere_models = [
     'command-nightly',
+    "command", 
+    "command-light", 
+    "command-medium-beta", 
+    "command-xlarge-beta"
 ]
 
 anthropic_models = [
   "claude-2", 
   "claude-instant-1"
 ]
```

### Comparing `litellm-0.1.232/litellm/integrations/helicone.py` & `litellm-0.1.233/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.232/litellm/main.py` & `litellm-0.1.233/litellm/main.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.232/litellm/timeout.py` & `litellm-0.1.233/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.232/litellm/utils.py` & `litellm-0.1.233/litellm/utils.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.232/setup.py` & `litellm-0.1.233/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='litellm',
-    version='0.1.232',
+    version='0.1.233',
     description='Library to easily interface with LLM API providers',
     author='BerriAI',
     packages=[
         'litellm'
     ],
     package_data={
         "litellm": ["integrations/*"],  # Specify the directory path relative to your package
```

