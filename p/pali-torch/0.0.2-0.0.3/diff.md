# Comparing `tmp/pali-torch-0.0.2.tar.gz` & `tmp/pali-torch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pali-torch-0.0.2.tar", last modified: Thu Aug  3 12:26:40 2023, max compression
+gzip compressed data, was "pali-torch-0.0.3.tar", last modified: Sat Aug  5 16:31:38 2023, max compression
```

## Comparing `pali-torch-0.0.2.tar` & `pali-torch-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:26:40.558350 pali-torch-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-03 12:26:27.000000 pali-torch-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-03 12:26:40.554350 pali-torch-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-08-03 12:26:27.000000 pali-torch-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:26:40.554350 pali-torch-0.0.2/pali/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-03 12:26:27.000000 pali-torch-0.0.2/pali/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-03 12:26:27.000000 pali-torch-0.0.2/pali/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:26:40.554350 pali-torch-0.0.2/pali_torch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-03 12:26:40.000000 pali-torch-0.0.2/pali_torch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-03 12:26:40.000000 pali-torch-0.0.2/pali_torch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:26:40.000000 pali-torch-0.0.2/pali_torch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-03 12:26:40.000000 pali-torch-0.0.2/pali_torch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 12:26:40.000000 pali-torch-0.0.2/pali_torch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 12:26:40.558350 pali-torch-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-03 12:26:27.000000 pali-torch-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:31:38.819581 pali-torch-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-05 16:31:26.000000 pali-torch-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-05 16:31:38.819581 pali-torch-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-08-05 16:31:26.000000 pali-torch-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:31:38.815581 pali-torch-0.0.3/pali/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-05 16:31:26.000000 pali-torch-0.0.3/pali/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-08-05 16:31:26.000000 pali-torch-0.0.3/pali/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-08-05 16:31:26.000000 pali-torch-0.0.3/pali/autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-08-05 16:31:26.000000 pali-torch-0.0.3/pali/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55564 2023-08-05 16:31:26.000000 pali-torch-0.0.3/pali/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:31:38.819581 pali-torch-0.0.3/pali_torch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-05 16:31:38.000000 pali-torch-0.0.3/pali_torch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-08-05 16:31:38.000000 pali-torch-0.0.3/pali_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 16:31:38.000000 pali-torch-0.0.3/pali_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-05 16:31:38.000000 pali-torch-0.0.3/pali_torch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-05 16:31:38.000000 pali-torch-0.0.3/pali_torch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 16:31:38.819581 pali-torch-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-05 16:31:26.000000 pali-torch-0.0.3/setup.py
```

### Comparing `pali-torch-0.0.2/LICENSE` & `pali-torch-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pali-torch-0.0.2/PKG-INFO` & `pali-torch-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pali-torch
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pali - PyTorch
 Home-page: https://github.com/kyegomez/Pali
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pali-torch-0.0.2/README.md` & `pali-torch-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pali-torch-0.0.2/pali_torch.egg-info/PKG-INFO` & `pali-torch-0.0.3/pali_torch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pali-torch
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pali - PyTorch
 Home-page: https://github.com/kyegomez/Pali
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pali-torch-0.0.2/setup.py` & `pali-torch-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pali-torch',
     packages=find_packages(exclude=[]),
-    version='0.0.2',
+    version='0.0.3',
     license='MIT',
     description='Pali - PyTorch',
     author='Kye Gomez',
     author_email='kye@apac.ai',
     long_description_content_type='text/markdown',
     url='https://github.com/kyegomez/Pali',
     keywords=[
```

