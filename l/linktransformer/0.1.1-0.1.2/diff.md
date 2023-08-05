# Comparing `tmp/linktransformer-0.1.1.tar.gz` & `tmp/linktransformer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktransformer-0.1.1.tar", last modified: Fri Aug  4 09:12:20 2023, max compression
+gzip compressed data, was "linktransformer-0.1.2.tar", last modified: Fri Aug  4 23:57:46 2023, max compression
```

## Comparing `linktransformer-0.1.1.tar` & `linktransformer-0.1.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 09:12:20.778906 linktransformer-0.1.1/
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1078 2023-07-31 06:29:08.000000 linktransformer-0.1.1/LICENSE.txt
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      122 2023-08-01 02:28:30.000000 linktransformer-0.1.1/MANIFEST.in
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     8297 2023-08-04 09:12:20.778906 linktransformer-0.1.1/PKG-INFO
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     6506 2023-08-04 08:35:37.000000 linktransformer-0.1.1/README.md
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1159 2023-08-01 15:57:37.000000 linktransformer-0.1.1/pyproject.toml
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)       38 2023-08-04 09:12:20.778906 linktransformer-0.1.1/setup.cfg
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 09:12:20.770906 linktransformer-0.1.1/src/
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 09:12:20.774906 linktransformer-0.1.1/src/linktransformer/
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      228 2023-08-04 07:11:40.000000 linktransformer-0.1.1/src/linktransformer/__init__.py
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 09:12:20.774906 linktransformer-0.1.1/src/linktransformer/configs/
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      155 2023-07-30 23:26:02.000000 linktransformer-0.1.1/src/linktransformer/configs/__init__.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      489 2023-08-03 18:53:19.000000 linktransformer-0.1.1/src/linktransformer/configs/linkage.json
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 09:12:20.774906 linktransformer-0.1.1/src/linktransformer/data/
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      100 2023-07-30 23:26:04.000000 linktransformer-0.1.1/src/linktransformer/data/__init__.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      124 2023-07-29 23:45:13.000000 linktransformer-0.1.1/src/linktransformer/data/coarse.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)   436216 2023-07-29 23:45:13.000000 linktransformer-0.1.1/src/linktransformer/data/es_mexican_products.xlsx
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      355 2023-07-29 23:45:13.000000 linktransformer-0.1.1/src/linktransformer/data/fine.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      300 2023-07-29 23:45:13.000000 linktransformer-0.1.1/src/linktransformer/data/toy_comp_1.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      310 2023-07-29 23:45:13.000000 linktransformer-0.1.1/src/linktransformer/data/toy_comp_2.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      415 2023-07-30 17:00:18.000000 linktransformer-0.1.1/src/linktransformer/data/toy_multi_1.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1064 2023-07-30 17:05:16.000000 linktransformer-0.1.1/src/linktransformer/data/toy_multi_2.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      388 2023-08-04 05:38:49.000000 linktransformer-0.1.1/src/linktransformer/data/toy_pairs.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      631 2023-07-30 17:19:37.000000 linktransformer-0.1.1/src/linktransformer/data/translation_1.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      529 2023-07-30 17:20:21.000000 linktransformer-0.1.1/src/linktransformer/data/translation_2.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    17215 2023-08-04 06:03:40.000000 linktransformer-0.1.1/src/linktransformer/infer.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     5675 2023-08-04 08:58:00.000000 linktransformer-0.1.1/src/linktransformer/model_card_templates.py
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 09:12:20.778906 linktransformer-0.1.1/src/linktransformer/modified_sbert/
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    12778 2023-08-04 08:39:49.000000 linktransformer-0.1.1/src/linktransformer/modified_sbert/LinkTransformer.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-07-31 04:10:46.000000 linktransformer-0.1.1/src/linktransformer/modified_sbert/__init__.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     3382 2023-08-01 01:32:03.000000 linktransformer-0.1.1/src/linktransformer/modified_sbert/cluster_fns.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      735 2023-07-30 00:14:40.000000 linktransformer-0.1.1/src/linktransformer/modified_sbert/data_loaders.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    21144 2023-08-02 20:50:51.000000 linktransformer-0.1.1/src/linktransformer/modified_sbert/evaluation.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     4668 2023-07-30 18:14:18.000000 linktransformer-0.1.1/src/linktransformer/modified_sbert/losses.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     6296 2023-08-04 06:19:29.000000 linktransformer-0.1.1/src/linktransformer/modified_sbert/train.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    25645 2023-08-03 02:50:02.000000 linktransformer-0.1.1/src/linktransformer/preprocess.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     8408 2023-08-04 08:53:23.000000 linktransformer-0.1.1/src/linktransformer/train_model.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     4148 2023-08-04 06:26:48.000000 linktransformer-0.1.1/src/linktransformer/utils.py
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 09:12:20.774906 linktransformer-0.1.1/src/linktransformer.egg-info/
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     8297 2023-08-04 09:12:20.000000 linktransformer-0.1.1/src/linktransformer.egg-info/PKG-INFO
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1330 2023-08-04 09:12:20.000000 linktransformer-0.1.1/src/linktransformer.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)        1 2023-08-04 09:12:20.000000 linktransformer-0.1.1/src/linktransformer.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      116 2023-08-04 09:12:20.000000 linktransformer-0.1.1/src/linktransformer.egg-info/requires.txt
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)       16 2023-08-04 09:12:20.000000 linktransformer-0.1.1/src/linktransformer.egg-info/top_level.txt
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 23:57:46.566081 linktransformer-0.1.2/
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1078 2023-07-31 06:29:08.000000 linktransformer-0.1.2/LICENSE.txt
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      122 2023-08-01 02:28:30.000000 linktransformer-0.1.2/MANIFEST.in
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     8297 2023-08-04 23:57:46.566081 linktransformer-0.1.2/PKG-INFO
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     6506 2023-08-04 09:13:15.000000 linktransformer-0.1.2/README.md
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1159 2023-08-04 23:57:44.000000 linktransformer-0.1.2/pyproject.toml
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)       38 2023-08-04 23:57:46.566081 linktransformer-0.1.2/setup.cfg
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 23:57:46.562081 linktransformer-0.1.2/src/
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 23:57:46.566081 linktransformer-0.1.2/src/linktransformer/
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      228 2023-08-04 23:54:50.000000 linktransformer-0.1.2/src/linktransformer/__init__.py
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 23:57:46.566081 linktransformer-0.1.2/src/linktransformer/configs/
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      155 2023-07-30 23:26:02.000000 linktransformer-0.1.2/src/linktransformer/configs/__init__.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      527 2023-08-04 23:10:37.000000 linktransformer-0.1.2/src/linktransformer/configs/linkage.json
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 23:57:46.566081 linktransformer-0.1.2/src/linktransformer/data/
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      100 2023-07-30 23:26:04.000000 linktransformer-0.1.2/src/linktransformer/data/__init__.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      124 2023-07-29 23:45:13.000000 linktransformer-0.1.2/src/linktransformer/data/coarse.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)   436216 2023-07-29 23:45:13.000000 linktransformer-0.1.2/src/linktransformer/data/es_mexican_products.xlsx
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      355 2023-07-29 23:45:13.000000 linktransformer-0.1.2/src/linktransformer/data/fine.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      300 2023-07-29 23:45:13.000000 linktransformer-0.1.2/src/linktransformer/data/toy_comp_1.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      310 2023-07-29 23:45:13.000000 linktransformer-0.1.2/src/linktransformer/data/toy_comp_2.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      415 2023-07-30 17:00:18.000000 linktransformer-0.1.2/src/linktransformer/data/toy_multi_1.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1064 2023-07-30 17:05:16.000000 linktransformer-0.1.2/src/linktransformer/data/toy_multi_2.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      388 2023-08-04 05:38:49.000000 linktransformer-0.1.2/src/linktransformer/data/toy_pairs.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      631 2023-07-30 17:19:37.000000 linktransformer-0.1.2/src/linktransformer/data/translation_1.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      529 2023-07-30 17:20:21.000000 linktransformer-0.1.2/src/linktransformer/data/translation_2.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    19683 2023-08-04 22:38:51.000000 linktransformer-0.1.2/src/linktransformer/infer.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     5743 2023-08-04 23:42:29.000000 linktransformer-0.1.2/src/linktransformer/model_card_templates.py
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 23:57:46.566081 linktransformer-0.1.2/src/linktransformer/modified_sbert/
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    13152 2023-08-04 23:44:13.000000 linktransformer-0.1.2/src/linktransformer/modified_sbert/LinkTransformer.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-07-31 04:10:46.000000 linktransformer-0.1.2/src/linktransformer/modified_sbert/__init__.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     3380 2023-08-04 23:50:58.000000 linktransformer-0.1.2/src/linktransformer/modified_sbert/cluster_fns.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      735 2023-07-30 00:14:40.000000 linktransformer-0.1.2/src/linktransformer/modified_sbert/data_loaders.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    21144 2023-08-02 20:50:51.000000 linktransformer-0.1.2/src/linktransformer/modified_sbert/evaluation.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     4668 2023-07-30 18:14:18.000000 linktransformer-0.1.2/src/linktransformer/modified_sbert/losses.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     6510 2023-08-04 23:41:01.000000 linktransformer-0.1.2/src/linktransformer/modified_sbert/train.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    25645 2023-08-03 02:50:02.000000 linktransformer-0.1.2/src/linktransformer/preprocess.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     9029 2023-08-04 23:23:11.000000 linktransformer-0.1.2/src/linktransformer/train_model.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     4218 2023-08-04 21:56:40.000000 linktransformer-0.1.2/src/linktransformer/utils.py
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 23:57:46.566081 linktransformer-0.1.2/src/linktransformer.egg-info/
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     8297 2023-08-04 23:57:46.000000 linktransformer-0.1.2/src/linktransformer.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1330 2023-08-04 23:57:46.000000 linktransformer-0.1.2/src/linktransformer.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)        1 2023-08-04 23:57:46.000000 linktransformer-0.1.2/src/linktransformer.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      116 2023-08-04 23:57:46.000000 linktransformer-0.1.2/src/linktransformer.egg-info/requires.txt
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)       16 2023-08-04 23:57:46.000000 linktransformer-0.1.2/src/linktransformer.egg-info/top_level.txt
```

### Comparing `linktransformer-0.1.1/LICENSE.txt` & `linktransformer-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.1/PKG-INFO` & `linktransformer-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktransformer
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple way to do link dataframes using large language models.
 Author-email: "Abhishek Arora, Sam Jones and Melissa Dell" <llmklinkpython@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 dell-research-harvard
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `linktransformer-0.1.1/README.md` & `linktransformer-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.1/pyproject.toml` & `linktransformer-0.1.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "linktransformer"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
        "scikit-learn",
         "faiss-cpu",
         "hdbscan",
         "networkx",
         "torch",
         "sentence_transformers",
```

### Comparing `linktransformer-0.1.1/src/linktransformer/data/es_mexican_products.xlsx` & `linktransformer-0.1.2/src/linktransformer/data/es_mexican_products.xlsx`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.1/src/linktransformer/data/toy_multi_2.csv` & `linktransformer-0.1.2/src/linktransformer/data/toy_multi_2.csv`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.1/src/linktransformer/data/translation_1.csv` & `linktransformer-0.1.2/src/linktransformer/data/translation_1.csv`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.1/src/linktransformer/data/translation_2.csv` & `linktransformer-0.1.2/src/linktransformer/data/translation_2.csv`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.1/src/linktransformer/infer.py` & `linktransformer-0.1.2/src/linktransformer/infer.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import numpy as np
 import pandas as pd
 import faiss
 from typing import Union, List, Optional, Tuple,Dict, Any
 from pandas import DataFrame
 
 from linktransformer.modified_sbert.cluster_fns import cluster
-from linktransformer.utils import serialize_columns, infer_embeddings, load_model, cosine_similarity
-
+from linktransformer.utils import serialize_columns, infer_embeddings, load_model, cosine_similarity_corresponding_pairs
+from sklearn.metrics.pairwise import cosine_similarity
+from itertools import combinations
 
 
 
 
 
 
 def merge(
@@ -321,16 +322,15 @@
         embeddings2 = np.expand_dims(embeddings2, axis=0)
     ## Normalize embedding tensors using numpy
 
     embeddings1 = embeddings1 / np.linalg.norm(embeddings1, axis=1, keepdims=True)
     embeddings2 = embeddings2 / np.linalg.norm(embeddings2, axis=1, keepdims=True)
 
     ## Compute cosine similarity between CORRESPONDING pair of embeddings
-    cosine_similarity_12 = cosine_similarity(embeddings1,embeddings2)
-    print(cosine_similarity_12.shape)
+    cosine_similarity_12 = cosine_similarity_corresponding_pairs(embeddings1,embeddings2)
 
     ## Add cosine similarity to df
     df["score"] = cosine_similarity_12.flatten()
 
     return df
 
 def cluster_rows(
@@ -362,24 +362,18 @@
     :param model (str): Language model to use.
     :param on (Union[str, List[str]]): Column(s) to deduplicate on.
     :param cluster_type (str): Clustering method to use. Defaults to "SLINK".
     :param cluster_params (Dict[str, Any]): Parameters for clustering method. Defaults to {'threshold': 0.5, "min cluster size": 2, "metric": "cosine"}.
     :param openai_key (str): OpenAI API key
     :return: DataFrame: The deduplicated dataframe.
     """
-    print(f"Deduplicating dataframe with originally {len(df)} rows")
 
     df = df.copy()
 
-    ### First, deduplicate based on exact matches
-    df = df.drop_duplicates(subset=on, keep="first")
-    print(f"Exact matches found: dropping them")
-    print(f"Number of rows after exact match deduplication: {len(df)}")
 
-    ### Now, deduplicate based on similarity threshold
     ## First, get the embeddings
     ### If len(on)>1, then we need to serialize the columns
     if isinstance(on, list):
         strings = serialize_columns(df, on, model=model)
     else:
         strings = df[on].tolist()
     
@@ -414,21 +408,85 @@
     :param on (Union[str, List[str]]): Column(s) to deduplicate on.
     :param cluster_type (str): Clustering method to use. Defaults to "SLINK".
     :param cluster_params (Dict[str, Any]): Parameters for clustering method. Defaults to {'threshold': 0.5, "min cluster size": 2, "metric": "cosine"}.
     :param openai_key (str): OpenAI API key
     :return: DataFrame: The deduplicated dataframe.
     """
 
+    df = df.copy()
+
+    
+
     print(f"Deduplicating dataframe with originally {len(df)} rows")
+    ##Drop exact duplicates
+    print("Checking for and dropping exact duplicates")
+    df = df.drop_duplicates(subset=on, keep="first")
+    print(f"Number of rows after dropping exact duplicates: {len(df)}")
+
     df = cluster_rows(df, model, on, cluster_type, cluster_params, openai_key)
     df = df.drop_duplicates(subset="cluster", keep="first")
     df = df.drop(columns=["cluster"])
     print(f"Number of rows after deduplication: {len(df)}")
 
     return df
 
 
     
 
+def all_pair_combos_evaluate(df,model,left_on,right_on,openai_key=None):
+    """
+    Get similarity scores for every pair of rows in a dataframe. 
+    We make this efficient by only embedding each string once and get all possible pairwise distances
+    and add the expanded rows and their scores to the dataframe
+    :param df (DataFrame): Dataframe to evaluate.
+    :param model (str): Language model to use.
+    :param left_on (Union[str, List[str]]): Column(s) to evaluate on in df.
+    :param right_on (Union[str, List[str]]): Reference column(s) to evaluate on in df.
+    :param openai_key (str): OpenAI API key
+    :return: DataFrame: The evaluated dataframe.
+    """
+
+    ###Get the embeddings for the left_on column
+    if isinstance(left_on, list):
+        strings_left = serialize_columns(df, left_on, model=model)
+    else:
+        strings_left = df[left_on].tolist()
+    
+    ## Infer embeddings for df1
+    embeddings1 = infer_embeddings(strings_left, model, batch_size=128, openai_key=openai_key)
+    embeddings1 = embeddings1 / np.linalg.norm(embeddings1, axis=1, keepdims=True)
+
+    ###Get the embeddings for the right_on column
+    if isinstance(right_on, list):
+        strings_right = serialize_columns(df, right_on, model=model)
+    else:
+        strings_right = df[right_on].tolist()
     
+    ## Infer embeddings for df1
+    embeddings2 = infer_embeddings(strings_right, model, batch_size=128, openai_key=openai_key)
+    embeddings2 = embeddings2 / np.linalg.norm(embeddings2, axis=1, keepdims=True)
+
+    ###calculate the cosine similarity between all pairs of rows
+    cosine_similarity_12_all_pairs = cosine_similarity(embeddings1,embeddings2)
+    ##Flatten the matrix
+    cosine_similarity_12_all_pairs = cosine_similarity_12_all_pairs.flatten()
+
+    ###This gives an n*n matrix of cosine similarities. 
+
+    ###Similarly, make an n*n matrix of the left_on column and right_on column
+    left_on_all_pairs = np.repeat(df[left_on].values, len(df[right_on]), axis=0)
+
+
+    ###Left part of the df was repeating n times. We also want the right one to repeat, but 
+
+
+    right_on_all_pairs = np.tile(df[right_on].values, (len(df[left_on]),1))
+
+    ###Now, flattenn the right on pairs
+    right_on_all_pairs = right_on_all_pairs.flatten()
+
+    ###Now, we can make a dataframe with the left_on, right_on and cosine similarity
+    df_concat = pd.DataFrame({"left_on":left_on_all_pairs,"right_on":right_on_all_pairs,"score":cosine_similarity_12_all_pairs})
+
+    return df_concat
```

### Comparing `linktransformer-0.1.1/src/linktransformer/model_card_templates.py` & `linktransformer-0.1.2/src/linktransformer/model_card_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 import logging
 
 from sentence_transformers.util import fullname
 
 class ModelCardTemplate:
-    __TAGS__ = ["link-transformers","sentence-transformers", "sentence-similarity","tabular-classification"]
+    __TAGS__ = ["linktransformer","sentence-transformers", "sentence-similarity","tabular-classification"]
     __DEFAULT_VARS__ = {
         "{PIPELINE_TAG}": "sentence-similarity",
         "{MODEL_DESCRIPTION}": "<!--- Describe your model here -->",
         "{TRAINING_SECTION}": "",
         "{USAGE_TRANSFORMERS_SECTION}": "",
         "{EVALUATION}": "<!--- Describe how your model was evaluated -->",
         "{CITING}": "<!--- Describe where people can find more information -->"
     }
 
     __MODEL_CARD__ = """
 ---
 pipeline_tag: {PIPELINE_TAG}
+language: 
+{LANGUAGE}
 tags:
 {TAGS}
 {DATASETS}
 ---
 
 # {MODEL_NAME}
 
 This is a [LinkTransformer](https://github.com/dell-research-harvard/linktransformer) model. At its core this model this is a sentence transformer model [sentence-transformers](https://www.SBERT.net) model- it just wraps around the class. 
 It is designed for quick and easy record linkage (entity-matching) through the LinkTransformer package. The tasks include clustering, deduplication, linking, aggregation and more.
 Notwithstanding that, it can be used for any sentence similarity task within the sentence-transformers framework as well. 
 It maps sentences & paragraphs to a {NUM_DIMENSIONS} dimensional dense vector space and can be used for tasks like clustering or semantic search.
 Take a look at the documentation of [sentence-transformers](https://www.sbert.net/index.html) if you want to use this model for more than what we support in our applications. 
 
 
-This model has been fine-tuned on the model : {BASE_MODEL}. 
+This model has been fine-tuned on the model : {BASE_MODEL}. It is pretrained for the language : {LANGUAGE}.
+
 
 {MODEL_DESCRIPTION}
 
 ## Usage (LinkTransformer)
 
 Using this model becomes easy when you have [LinkTransformer](https://github.com/dell-research-harvard/linktransformer) installed:
```

### Comparing `linktransformer-0.1.1/src/linktransformer/modified_sbert/LinkTransformer.py` & `linktransformer-0.1.2/src/linktransformer/modified_sbert/LinkTransformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,33 +39,40 @@
     :param cache_folder: Path to store models. Can be also set by SENTENCE_TRANSFORMERS_HOME enviroment variable.
     :param use_auth_token: HuggingFace authentication token to download private models.
     """
     def __init__(self, model_name_or_path: Optional[str] = None,
                  modules: Optional[Iterable[nn.Module]] = None,
                  device: Optional[str] = None,
                  cache_folder: Optional[str] = None,
-                 use_auth_token: Union[bool, str, None] = None
+                 use_auth_token: Union[bool, str, None] = None,
+                 opt_model_description: Optional[str] = None,
+                 opt_model_lang: Optional[str] = None,
                  ):
 
-        print("LinkTransformer's custom LinkTransformer class")
 
         super().__init__(model_name_or_path=model_name_or_path, modules=modules, device=device, cache_folder=cache_folder, use_auth_token=use_auth_token)
 
         ##If it is a local path, we need to load the config (LT) from the file FLAG - CLEAN THIS UP
         if os.path.isdir(model_name_or_path):
             ###If config file exists, load it. It will be in the parent folder of the model
             if os.path.isfile(os.path.join(os.path.dirname(model_name_or_path), 'LT_training_config.json')):
                 with open(os.path.join(os.path.dirname(model_name_or_path), 'LT_training_config.json'), 'r') as fIn:
                     self._lt_model_config = json.load(fIn)
                     print("Loaded LinkTransformer model config from {}".format(os.path.join(model_name_or_path, 'LT_training_config.json')))
                 self.base_model_name_or_path = self._lt_model_config['base_model_path']
+                self.opt_model_description = self._lt_model_config['opt_model_description']
+                self.opt_model_lang = self._lt_model_config['opt_model_lang']
         else:
             ###If huggningface model, then assign ##Implement later
             self.base_model_name_or_path = model_name_or_path
 
+            self.opt_model_description = opt_model_description
+            self.opt_model_lang = opt_model_lang
+            
+
 
 
     def save(self, path: str, model_name: Optional[str] = None, create_model_card: bool = True, train_datasets: Optional[List[str]] = None):
         """
         Saves all elements for this seq. sentence embedder into different sub-folders
         :param path: Path on disc
         :param model_name: Optional model name
@@ -116,33 +123,42 @@
         """
         if self._model_card_text is not None and len(self._model_card_text) > 0:
             model_card = self._model_card_text
         else:
             tags = ModelCardTemplate.__TAGS__.copy()
             model_card = ModelCardTemplate.__MODEL_CARD__
 
-            # if len(self._modules) == 2 and isinstance(self._first_module(), Transformer) and isinstance(self._last_module(), Pooling) and self._last_module().get_pooling_mode_str() in ['cls', 'max', 'mean']:
-            #     # pooling_fct_name, pooling_fct = ModelCardTemplate.model_card_get_pooling_function(pooling_mode)
-            #     # model_card = model_card.replace("{POOLING_FUNCTION}", pooling_fct).replace("{POOLING_FUNCTION_NAME}", pooling_fct_name).replace("{POOLING_MODE}", pooling_mode)
-            #     tags.append('transformers')
-
             # Print full model
             model_card = model_card.replace("{FULL_MODEL_STR}", str(self))
 
             # Add tags
             model_card = model_card.replace("{TAGS}", "\n".join(["- "+t for t in tags]))
 
             datasets_str = ""
             if train_datasets is not None:
                 datasets_str = "datasets:\n"+"\n".join(["- " + d for d in train_datasets])
             model_card = model_card.replace("{DATASETS}", datasets_str)
 
             ###Add base model name
             model_card=model_card.replace("{BASE_MODEL}",self.base_model_name_or_path)
 
+            ##ADd optional model description
+            if self.opt_model_description is not None:
+                model_card=model_card.replace("{MODEL_DESCRIPTION}",self.opt_model_description)
+            else:
+                pass
+                
+            ##ADd optional model language
+            if self.opt_model_lang is not None:
+                model_card = model_card.replace("{LANGUAGE}", "\n".join(["- "+t for t in [self.opt_model_lang]]))
+
+                model_card=model_card.replace("{LANGUAGE}",self.opt_model_lang)
+            else:
+                pass
+
             # Add dim info
             self._model_card_vars["{NUM_DIMENSIONS}"] = self.get_sentence_embedding_dimension()
 
             # Replace vars we created while using the model
             for name, value in self._model_card_vars.items():
                 model_card = model_card.replace(name, str(value))
```

### Comparing `linktransformer-0.1.1/src/linktransformer/modified_sbert/cluster_fns.py` & `linktransformer-0.1.2/src/linktransformer/modified_sbert/cluster_fns.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             raise ValueError(f'cluster_params must contain "{param}"')
 
     if cluster_type == "agglomerative":
         clustering_model = AgglomerativeClustering(
             n_clusters=None,
             distance_threshold=cluster_params["threshold"],
             linkage=cluster_params["clustering linkage"],
-            affinity=cluster_params["metric"]
+            metric=cluster_params["metric"]
         )
 
     if cluster_type == "SLINK":
         clustering_model = DBSCAN(
             eps=cluster_params["threshold"],
             min_samples=cluster_params["min cluster size"],
             metric=cluster_params["metric"]
```

### Comparing `linktransformer-0.1.1/src/linktransformer/modified_sbert/data_loaders.py` & `linktransformer-0.1.2/src/linktransformer/modified_sbert/data_loaders.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.1/src/linktransformer/modified_sbert/evaluation.py` & `linktransformer-0.1.2/src/linktransformer/modified_sbert/evaluation.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.1/src/linktransformer/modified_sbert/losses.py` & `linktransformer-0.1.2/src/linktransformer/modified_sbert/losses.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.1/src/linktransformer/modified_sbert/train.py` & `linktransformer-0.1.2/src/linktransformer/modified_sbert/train.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,15 +41,18 @@
         warm_up_perc=0.1,
         optimizer_params: Dict[str, object] = {'lr': 2e-7},
         loss_params=None,
         model_save_path="output",
         wandb_names=None,
         already_clustered_train=False,
         eval_steps_perc=0.1,
-        eval_type="retrieval"
+        eval_type="retrieval",
+        opt_model_description=None,
+        opt_model_lang=None
+
 ):
 
     # Logging
     if wandb_names: 
         if 'run' in wandb_names:
             wandb.init(project=wandb_names['project'], entity=wandb_names['id'], reinit=True, name=wandb_names['run'])
         else:
@@ -64,19 +67,19 @@
 
     os.makedirs(model_save_path, exist_ok=True)
 
     # Base language model
     if add_pooling_layer:
         word_embedding_model = models.Transformer(base_model, max_seq_length=512)
         pooling_model = models.Pooling(word_embedding_model.get_word_embedding_dimension(), pooling_mode='mean')
-        model = LinkTransformer(modules=[word_embedding_model, pooling_model])
+        model = LinkTransformer(modules=[word_embedding_model, pooling_model],opt_model_description=opt_model_description,opt_model_lang=opt_model_lang)
     elif type(base_model) == LinkTransformer:
         model = base_model
     else:
-        model = LinkTransformer(base_model)
+        model = LinkTransformer(base_model,opt_model_description=opt_model_description,opt_model_lang=opt_model_lang)
 
     if wandb_names is not None:
         wandb.watch(model)
 
 
     train_loss = losses.SupConLoss_wandb(model=model,**loss_params if loss_params is not None else {},wandb_names=wandb_names)
```

### Comparing `linktransformer-0.1.1/src/linktransformer/preprocess.py` & `linktransformer-0.1.2/src/linktransformer/preprocess.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.1/src/linktransformer/train_model.py` & `linktransformer-0.1.2/src/linktransformer/train_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,19 @@
                             train_batch_size:int=None,
                             num_epochs:int=None,
                             warm_up_perc:float=None,
                             learning_rate:float=None,
                             val_perc:float=None,
                             wandb_names:dict=None,
                             add_pooling_layer:bool=None,
-                            language:str=None):
+                            opt_model_description:str=None,
+                            opt_model_lang:str=None,
+                            test_at_end:bool=None,
+                            save_val_test_pickles:bool=None
+                            ):
     """
     Function to create a training config
     :param config_save_path (str): Path to save the config
     :param base_config_path (str): Path to the base config
     :param model_save_dir (str): Path to save the model
     :param model_save_name (str): Name of the model
     :param train_batch_size (int): Batch size for training
@@ -59,16 +63,23 @@
         config["learning_rate"]=learning_rate
     if val_perc is not None:
         config["val_perc"]=val_perc
     if wandb_names is not None:
         config["wandb_names"]=wandb_names
     if add_pooling_layer is not None:
         config["add_pooling_layer"]=add_pooling_layer
-    if language is not None:
-        config["language"]=language
+    if opt_model_description is not None:
+        config["opt_model_description"]=opt_model_description
+    if opt_model_lang is not None:
+        config["opt_model_lang"]=opt_model_lang
+    if test_at_end is not None:
+        config["test_at_end"]=test_at_end
+    if save_val_test_pickles is not None:
+        config["save_val_test_pickles"]=save_val_test_pickles
+
     
 
     with open(config_save_path, "w") as config_file:
         json.dump(config, config_file)
 
     print("Config saved at: ", config_save_path)
     print("Keep it handy for future use")
@@ -90,14 +101,15 @@
     right_col_names: List[str] = ['description48'],
     left_id_name: List[str] = ['tariffcode47'],
     right_id_name: List[str] = ['tariffcode48'],
     label_col_name: str = None,
     config_path: str = LINKAGE_CONFIG_PATH,
     training_args: dict = {"num_epochs":10},
     log_wandb: bool = False,
+
 ) -> str:
     """
     Train the LinkTransformer model.
 
     :param: model_path (str): The name of the model to use.
     :param: data (str): Path to the dataset in Excel or CSV format or a dataframe object.
     :param: left_col_names (List[str]): List of column names to use as left side data.
@@ -182,15 +194,17 @@
         add_pooling_layer=config["add_pooling_layer"],
         train_batch_size=config["train_batch_size"],
         num_epochs=config["num_epochs"],
         warm_up_perc=config["warm_up_perc"],
         model_save_path=os.path.join(config["model_save_dir"], config["model_save_name"]),
         wandb_names=config["wandb_names"] if log_wandb else None,
         optimizer_params={'lr': config["learning_rate"]},
-        eval_type=config["eval_type"]
+        eval_type=config["eval_type"],
+        opt_model_description=config["opt_model_description"],
+        opt_model_lang=config["opt_model_lang"]
     )
     print(f"Best model saved on the path: {best_model_path} ")
 
     ##Add the dataset used in the config 
     config["training_dataset"]=data if isinstance(data,str) else "dataframe"
     ##Add the best model path in the config
     config["best_model_path"]=best_model_path
```

### Comparing `linktransformer-0.1.1/src/linktransformer/utils.py` & `linktransformer-0.1.2/src/linktransformer/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from linktransformer.modified_sbert.LinkTransformer import LinkTransformer
 import numpy as np
 import pandas as pd
 import transformers
 import openai
+from itertools import combinations
 
 
 def load_model(model_path: str) -> LinkTransformer:
     """
     Load a saved LinkTransformer model.
 
     :param model_path: Path to the saved model.
@@ -19,21 +20,26 @@
         print("Can't load the model, please check your path. All transformer based models from [HuggingFace](https://huggingface.co/) are supported. \
                We recommend [sentence-transformers](https://www.sbert.net/docs/pretrained_models.html) for these tasks as they are trained for \
                semantic similarity tasks. ")
 
     return model
 
 
-def cosine_similarity(vector1, vector2):
+def cosine_similarity_corresponding_pairs(vector1, vector2):
     dot_product = np.sum(vector1 * vector2, axis=1)
     norm_vector1 = np.linalg.norm(vector1, axis=1)
     norm_vector2 = np.linalg.norm(vector2, axis=1)
     cosine_sim = dot_product / (norm_vector1 * norm_vector2)
     return cosine_sim
 
+
+    
+
+
+
 def serialize_columns(df: pd.DataFrame, columns: list, sep_token: str=None, model: str = None) -> list:
     """
     Serialize columns of a DataFrame into a single string.
 
     :param df: The DataFrame.
     :param columns: The columns to serialize.
     :param sep_token: The token to use to separate columns.
@@ -96,7 +102,13 @@
         response = openai.Embedding.create(input=strings, model=model)["data"]
         f = lambda x: x["embedding"]
         embeddings = list(map(f, response))
         embeddings = np.array(list(map(f, response)), dtype=np.float32)
 
     return embeddings
 
+
+
+
+
+
+
```

### Comparing `linktransformer-0.1.1/src/linktransformer.egg-info/PKG-INFO` & `linktransformer-0.1.2/src/linktransformer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktransformer
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple way to do link dataframes using large language models.
 Author-email: "Abhishek Arora, Sam Jones and Melissa Dell" <llmklinkpython@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 dell-research-harvard
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `linktransformer-0.1.1/src/linktransformer.egg-info/SOURCES.txt` & `linktransformer-0.1.2/src/linktransformer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

