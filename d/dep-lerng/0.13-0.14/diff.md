# Comparing `tmp/dep_lerng-0.13.tar.gz` & `tmp/dep_lerng-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dep_lerng-0.13.tar", last modified: Fri Aug  4 23:57:46 2023, max compression
+gzip compressed data, was "dep_lerng-0.14.tar", last modified: Sat Aug  5 00:01:51 2023, max compression
```

## Comparing `dep_lerng-0.13.tar` & `dep_lerng-0.14.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 23:57:46.797351 dep_lerng-0.13/
--rw-rw-rw-   0        0        0      211 2023-08-04 23:57:46.797351 dep_lerng-0.13/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-04 23:57:46.792351 dep_lerng-0.13/dep_lerng/
--rw-rw-rw-   0        0        0     3666 2023-08-04 23:22:08.000000 dep_lerng-0.13/dep_lerng/ClassifierNet.py
--rw-rw-rw-   0        0        0     3101 2023-08-04 23:22:09.000000 dep_lerng-0.13/dep_lerng/ConvBlock.py
--rw-rw-rw-   0        0        0     1268 2023-08-04 23:22:10.000000 dep_lerng-0.13/dep_lerng/Dataset.py
--rw-rw-rw-   0        0        0     7116 2023-08-04 23:22:09.000000 dep_lerng-0.13/dep_lerng/ResBlock.py
--rw-rw-rw-   0        0        0     7818 2023-08-04 23:56:29.000000 dep_lerng-0.13/dep_lerng/ResNet.py
--rw-rw-rw-   0        0        0       75 2023-08-04 23:22:07.000000 dep_lerng-0.13/dep_lerng/__init__.py
--rw-rw-rw-   0        0        0    10166 2023-08-04 23:22:08.000000 dep_lerng-0.13/dep_lerng/custom_blocks.py
--rw-rw-rw-   0        0        0     9601 2023-08-04 23:52:33.000000 dep_lerng-0.13/dep_lerng/model_init.py
-drwxrwxrwx   0        0        0        0 2023-08-04 23:57:46.796351 dep_lerng-0.13/dep_lerng.egg-info/
--rw-rw-rw-   0        0        0      211 2023-08-04 23:57:46.000000 dep_lerng-0.13/dep_lerng.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2023-08-04 23:57:46.000000 dep_lerng-0.13/dep_lerng.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 23:57:46.000000 dep_lerng-0.13/dep_lerng.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-04 23:57:46.000000 dep_lerng-0.13/dep_lerng.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-08-04 23:57:46.000000 dep_lerng-0.13/dep_lerng.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 23:57:46.797351 dep_lerng-0.13/setup.cfg
--rw-rw-rw-   0        0        0      276 2023-08-04 23:56:43.000000 dep_lerng-0.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 00:01:51.588224 dep_lerng-0.14/
+-rw-rw-rw-   0        0        0      211 2023-08-05 00:01:51.588224 dep_lerng-0.14/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-05 00:01:51.583548 dep_lerng-0.14/dep_lerng/
+-rw-rw-rw-   0        0        0     3666 2023-08-04 23:22:08.000000 dep_lerng-0.14/dep_lerng/ClassifierNet.py
+-rw-rw-rw-   0        0        0     3101 2023-08-04 23:22:09.000000 dep_lerng-0.14/dep_lerng/ConvBlock.py
+-rw-rw-rw-   0        0        0     1268 2023-08-04 23:22:10.000000 dep_lerng-0.14/dep_lerng/Dataset.py
+-rw-rw-rw-   0        0        0     7116 2023-08-04 23:22:09.000000 dep_lerng-0.14/dep_lerng/ResBlock.py
+-rw-rw-rw-   0        0        0     7818 2023-08-04 23:56:29.000000 dep_lerng-0.14/dep_lerng/ResNet.py
+-rw-rw-rw-   0        0        0       75 2023-08-04 23:22:07.000000 dep_lerng-0.14/dep_lerng/__init__.py
+-rw-rw-rw-   0        0        0    10166 2023-08-04 23:22:08.000000 dep_lerng-0.14/dep_lerng/custom_blocks.py
+-rw-rw-rw-   0        0        0     9602 2023-08-05 00:00:37.000000 dep_lerng-0.14/dep_lerng/model_init.py
+drwxrwxrwx   0        0        0        0 2023-08-05 00:01:51.586810 dep_lerng-0.14/dep_lerng.egg-info/
+-rw-rw-rw-   0        0        0      211 2023-08-05 00:01:51.000000 dep_lerng-0.14/dep_lerng.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-08-05 00:01:51.000000 dep_lerng-0.14/dep_lerng.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 00:01:51.000000 dep_lerng-0.14/dep_lerng.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-05 00:00:57.000000 dep_lerng-0.14/dep_lerng.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-08-05 00:01:51.000000 dep_lerng-0.14/dep_lerng.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 00:01:51.588224 dep_lerng-0.14/setup.cfg
+-rw-rw-rw-   0        0        0      276 2023-08-05 00:01:42.000000 dep_lerng-0.14/setup.py
```

### Comparing `dep_lerng-0.13/dep_lerng/ClassifierNet.py` & `dep_lerng-0.14/dep_lerng/ClassifierNet.py`

 * *Files identical despite different names*

### Comparing `dep_lerng-0.13/dep_lerng/ConvBlock.py` & `dep_lerng-0.14/dep_lerng/ConvBlock.py`

 * *Files identical despite different names*

### Comparing `dep_lerng-0.13/dep_lerng/Dataset.py` & `dep_lerng-0.14/dep_lerng/Dataset.py`

 * *Files identical despite different names*

### Comparing `dep_lerng-0.13/dep_lerng/ResBlock.py` & `dep_lerng-0.14/dep_lerng/ResBlock.py`

 * *Files identical despite different names*

### Comparing `dep_lerng-0.13/dep_lerng/ResNet.py` & `dep_lerng-0.14/dep_lerng/ResNet.py`

 * *Files identical despite different names*

### Comparing `dep_lerng-0.13/dep_lerng/custom_blocks.py` & `dep_lerng-0.14/dep_lerng/custom_blocks.py`

 * *Files identical despite different names*

### Comparing `dep_lerng-0.13/dep_lerng/model_init.py` & `dep_lerng-0.14/dep_lerng/model_init.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from ResNet import Resnet
+from .ResNet import Resnet
 from pytorch_lightning import LightningModule
 
 import torch
 from torch.optim import Adam
 from torch.optim.lr_scheduler import ReduceLROnPlateau
 from torch.nn import functional as F
```

