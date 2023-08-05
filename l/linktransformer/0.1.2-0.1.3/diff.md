# Comparing `tmp/linktransformer-0.1.2.tar.gz` & `tmp/linktransformer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktransformer-0.1.2.tar", last modified: Fri Aug  4 23:57:46 2023, max compression
+gzip compressed data, was "linktransformer-0.1.3.tar", last modified: Sat Aug  5 10:39:29 2023, max compression
```

## Comparing `linktransformer-0.1.2.tar` & `linktransformer-0.1.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 23:57:46.566081 linktransformer-0.1.2/
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1078 2023-07-31 06:29:08.000000 linktransformer-0.1.2/LICENSE.txt
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      122 2023-08-01 02:28:30.000000 linktransformer-0.1.2/MANIFEST.in
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     8297 2023-08-04 23:57:46.566081 linktransformer-0.1.2/PKG-INFO
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     6506 2023-08-04 09:13:15.000000 linktransformer-0.1.2/README.md
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1159 2023-08-04 23:57:44.000000 linktransformer-0.1.2/pyproject.toml
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)       38 2023-08-04 23:57:46.566081 linktransformer-0.1.2/setup.cfg
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 23:57:46.562081 linktransformer-0.1.2/src/
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 23:57:46.566081 linktransformer-0.1.2/src/linktransformer/
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      228 2023-08-04 23:54:50.000000 linktransformer-0.1.2/src/linktransformer/__init__.py
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 23:57:46.566081 linktransformer-0.1.2/src/linktransformer/configs/
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      155 2023-07-30 23:26:02.000000 linktransformer-0.1.2/src/linktransformer/configs/__init__.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      527 2023-08-04 23:10:37.000000 linktransformer-0.1.2/src/linktransformer/configs/linkage.json
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 23:57:46.566081 linktransformer-0.1.2/src/linktransformer/data/
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      100 2023-07-30 23:26:04.000000 linktransformer-0.1.2/src/linktransformer/data/__init__.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      124 2023-07-29 23:45:13.000000 linktransformer-0.1.2/src/linktransformer/data/coarse.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)   436216 2023-07-29 23:45:13.000000 linktransformer-0.1.2/src/linktransformer/data/es_mexican_products.xlsx
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      355 2023-07-29 23:45:13.000000 linktransformer-0.1.2/src/linktransformer/data/fine.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      300 2023-07-29 23:45:13.000000 linktransformer-0.1.2/src/linktransformer/data/toy_comp_1.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      310 2023-07-29 23:45:13.000000 linktransformer-0.1.2/src/linktransformer/data/toy_comp_2.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      415 2023-07-30 17:00:18.000000 linktransformer-0.1.2/src/linktransformer/data/toy_multi_1.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1064 2023-07-30 17:05:16.000000 linktransformer-0.1.2/src/linktransformer/data/toy_multi_2.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      388 2023-08-04 05:38:49.000000 linktransformer-0.1.2/src/linktransformer/data/toy_pairs.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      631 2023-07-30 17:19:37.000000 linktransformer-0.1.2/src/linktransformer/data/translation_1.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      529 2023-07-30 17:20:21.000000 linktransformer-0.1.2/src/linktransformer/data/translation_2.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    19683 2023-08-04 22:38:51.000000 linktransformer-0.1.2/src/linktransformer/infer.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     5743 2023-08-04 23:42:29.000000 linktransformer-0.1.2/src/linktransformer/model_card_templates.py
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 23:57:46.566081 linktransformer-0.1.2/src/linktransformer/modified_sbert/
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    13152 2023-08-04 23:44:13.000000 linktransformer-0.1.2/src/linktransformer/modified_sbert/LinkTransformer.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-07-31 04:10:46.000000 linktransformer-0.1.2/src/linktransformer/modified_sbert/__init__.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     3380 2023-08-04 23:50:58.000000 linktransformer-0.1.2/src/linktransformer/modified_sbert/cluster_fns.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      735 2023-07-30 00:14:40.000000 linktransformer-0.1.2/src/linktransformer/modified_sbert/data_loaders.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    21144 2023-08-02 20:50:51.000000 linktransformer-0.1.2/src/linktransformer/modified_sbert/evaluation.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     4668 2023-07-30 18:14:18.000000 linktransformer-0.1.2/src/linktransformer/modified_sbert/losses.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     6510 2023-08-04 23:41:01.000000 linktransformer-0.1.2/src/linktransformer/modified_sbert/train.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    25645 2023-08-03 02:50:02.000000 linktransformer-0.1.2/src/linktransformer/preprocess.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     9029 2023-08-04 23:23:11.000000 linktransformer-0.1.2/src/linktransformer/train_model.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     4218 2023-08-04 21:56:40.000000 linktransformer-0.1.2/src/linktransformer/utils.py
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 23:57:46.566081 linktransformer-0.1.2/src/linktransformer.egg-info/
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     8297 2023-08-04 23:57:46.000000 linktransformer-0.1.2/src/linktransformer.egg-info/PKG-INFO
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1330 2023-08-04 23:57:46.000000 linktransformer-0.1.2/src/linktransformer.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)        1 2023-08-04 23:57:46.000000 linktransformer-0.1.2/src/linktransformer.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      116 2023-08-04 23:57:46.000000 linktransformer-0.1.2/src/linktransformer.egg-info/requires.txt
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)       16 2023-08-04 23:57:46.000000 linktransformer-0.1.2/src/linktransformer.egg-info/top_level.txt
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-05 10:39:29.781688 linktransformer-0.1.3/
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1078 2023-07-31 06:29:08.000000 linktransformer-0.1.3/LICENSE.txt
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      122 2023-08-01 02:28:30.000000 linktransformer-0.1.3/MANIFEST.in
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     8297 2023-08-05 10:39:29.781688 linktransformer-0.1.3/PKG-INFO
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     6506 2023-08-04 09:13:15.000000 linktransformer-0.1.3/README.md
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1159 2023-08-05 10:39:08.000000 linktransformer-0.1.3/pyproject.toml
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)       38 2023-08-05 10:39:29.781688 linktransformer-0.1.3/setup.cfg
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-05 10:39:29.777688 linktransformer-0.1.3/src/
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-05 10:39:29.777688 linktransformer-0.1.3/src/linktransformer/
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      228 2023-08-05 10:39:03.000000 linktransformer-0.1.3/src/linktransformer/__init__.py
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-05 10:39:29.777688 linktransformer-0.1.3/src/linktransformer/configs/
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      155 2023-07-30 23:26:02.000000 linktransformer-0.1.3/src/linktransformer/configs/__init__.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      527 2023-08-04 23:10:37.000000 linktransformer-0.1.3/src/linktransformer/configs/linkage.json
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-05 10:39:29.777688 linktransformer-0.1.3/src/linktransformer/data/
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      100 2023-07-30 23:26:04.000000 linktransformer-0.1.3/src/linktransformer/data/__init__.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      124 2023-07-29 23:45:13.000000 linktransformer-0.1.3/src/linktransformer/data/coarse.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)   436216 2023-07-29 23:45:13.000000 linktransformer-0.1.3/src/linktransformer/data/es_mexican_products.xlsx
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      355 2023-07-29 23:45:13.000000 linktransformer-0.1.3/src/linktransformer/data/fine.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      300 2023-07-29 23:45:13.000000 linktransformer-0.1.3/src/linktransformer/data/toy_comp_1.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      310 2023-07-29 23:45:13.000000 linktransformer-0.1.3/src/linktransformer/data/toy_comp_2.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      415 2023-07-30 17:00:18.000000 linktransformer-0.1.3/src/linktransformer/data/toy_multi_1.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1064 2023-07-30 17:05:16.000000 linktransformer-0.1.3/src/linktransformer/data/toy_multi_2.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      388 2023-08-04 05:38:49.000000 linktransformer-0.1.3/src/linktransformer/data/toy_pairs.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      631 2023-07-30 17:19:37.000000 linktransformer-0.1.3/src/linktransformer/data/translation_1.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      529 2023-07-30 17:20:21.000000 linktransformer-0.1.3/src/linktransformer/data/translation_2.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    19683 2023-08-05 10:39:24.000000 linktransformer-0.1.3/src/linktransformer/infer.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     5743 2023-08-04 23:42:29.000000 linktransformer-0.1.3/src/linktransformer/model_card_templates.py
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-05 10:39:29.781688 linktransformer-0.1.3/src/linktransformer/modified_sbert/
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    13223 2023-08-05 10:30:03.000000 linktransformer-0.1.3/src/linktransformer/modified_sbert/LinkTransformer.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-07-31 04:10:46.000000 linktransformer-0.1.3/src/linktransformer/modified_sbert/__init__.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     3380 2023-08-04 23:50:58.000000 linktransformer-0.1.3/src/linktransformer/modified_sbert/cluster_fns.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      735 2023-07-30 00:14:40.000000 linktransformer-0.1.3/src/linktransformer/modified_sbert/data_loaders.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    21144 2023-08-02 20:50:51.000000 linktransformer-0.1.3/src/linktransformer/modified_sbert/evaluation.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     4668 2023-07-30 18:14:18.000000 linktransformer-0.1.3/src/linktransformer/modified_sbert/losses.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     6838 2023-08-05 10:39:17.000000 linktransformer-0.1.3/src/linktransformer/modified_sbert/train.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    25645 2023-08-03 02:50:02.000000 linktransformer-0.1.3/src/linktransformer/preprocess.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     9281 2023-08-05 10:29:44.000000 linktransformer-0.1.3/src/linktransformer/train_model.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     4218 2023-08-04 21:56:40.000000 linktransformer-0.1.3/src/linktransformer/utils.py
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-05 10:39:29.777688 linktransformer-0.1.3/src/linktransformer.egg-info/
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     8297 2023-08-05 10:39:29.000000 linktransformer-0.1.3/src/linktransformer.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1330 2023-08-05 10:39:29.000000 linktransformer-0.1.3/src/linktransformer.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)        1 2023-08-05 10:39:29.000000 linktransformer-0.1.3/src/linktransformer.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      116 2023-08-05 10:39:29.000000 linktransformer-0.1.3/src/linktransformer.egg-info/requires.txt
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)       16 2023-08-05 10:39:29.000000 linktransformer-0.1.3/src/linktransformer.egg-info/top_level.txt
```

### Comparing `linktransformer-0.1.2/LICENSE.txt` & `linktransformer-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.2/PKG-INFO` & `linktransformer-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktransformer
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple way to do link dataframes using large language models.
 Author-email: "Abhishek Arora, Sam Jones and Melissa Dell" <llmklinkpython@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 dell-research-harvard
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `linktransformer-0.1.2/README.md` & `linktransformer-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.2/pyproject.toml` & `linktransformer-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "linktransformer"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
        "scikit-learn",
         "faiss-cpu",
         "hdbscan",
         "networkx",
         "torch",
         "sentence_transformers",
```

### Comparing `linktransformer-0.1.2/src/linktransformer/configs/linkage.json` & `linktransformer-0.1.3/src/linktransformer/configs/linkage.json`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.2/src/linktransformer/data/es_mexican_products.xlsx` & `linktransformer-0.1.3/src/linktransformer/data/es_mexican_products.xlsx`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.2/src/linktransformer/data/toy_multi_2.csv` & `linktransformer-0.1.3/src/linktransformer/data/toy_multi_2.csv`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.2/src/linktransformer/data/translation_1.csv` & `linktransformer-0.1.3/src/linktransformer/data/translation_1.csv`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.2/src/linktransformer/data/translation_2.csv` & `linktransformer-0.1.3/src/linktransformer/data/translation_2.csv`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.2/src/linktransformer/infer.py` & `linktransformer-0.1.3/src/linktransformer/infer.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.2/src/linktransformer/model_card_templates.py` & `linktransformer-0.1.3/src/linktransformer/model_card_templates.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.2/src/linktransformer/modified_sbert/LinkTransformer.py` & `linktransformer-0.1.3/src/linktransformer/modified_sbert/LinkTransformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,17 +227,18 @@
             # If user provides local files, copy them.
             if local_model_path:
                 copy_tree(local_model_path, tmp_dir)
             else:  # Else, save model directly into local repo.
                 create_model_card = replace_model_card or not os.path.exists(os.path.join(tmp_dir, 'README.md'))
                 self.save(tmp_dir, model_name=full_model_name, create_model_card=create_model_card, train_datasets=train_datasets)
 
-            ##Save the model config (_lt_model_config) to the repo
-            with open(os.path.join(tmp_dir, 'LT_training_config.json'), 'w') as fOut:
-                json.dump(self._lt_model_config, fOut, indent=2)
+            ##Save the model config (_lt_model_config) to the repo if it exists
+            if hasattr(self, '_lt_model_config'):
+                with open(os.path.join(tmp_dir, 'LT_training_config.json'), 'w') as fOut:
+                    json.dump(self._lt_model_config, fOut, indent=2)
 
             #Find files larger 5M and track with git-lfs
             large_files = []
             for root, dirs, files in os.walk(tmp_dir):
                 for filename in files:
                     file_path = os.path.join(root, filename)
                     rel_path = os.path.relpath(file_path, tmp_dir)
```

### Comparing `linktransformer-0.1.2/src/linktransformer/modified_sbert/cluster_fns.py` & `linktransformer-0.1.3/src/linktransformer/modified_sbert/cluster_fns.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.2/src/linktransformer/modified_sbert/data_loaders.py` & `linktransformer-0.1.3/src/linktransformer/modified_sbert/data_loaders.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.2/src/linktransformer/modified_sbert/evaluation.py` & `linktransformer-0.1.3/src/linktransformer/modified_sbert/evaluation.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.2/src/linktransformer/modified_sbert/losses.py` & `linktransformer-0.1.3/src/linktransformer/modified_sbert/losses.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.2/src/linktransformer/modified_sbert/train.py` & `linktransformer-0.1.3/src/linktransformer/modified_sbert/train.py`

 * *Files 11% similar despite different names*

```diff
@@ -139,17 +139,21 @@
         checkpoint_save_steps=math.ceil(len(train_dataloader)/eval_steps_perc),
         checkpoint_path=model_save_path,
         save_best_model=True,
         checkpoint_save_total_limit=2,
         optimizer_params = optimizer_params,
     )
 
+    ###Get the best model path among the saved checkpoints
+    ##take the last saved checkpoints = best
+    ###look in the dir and get the last checkpoint (subdirs are named as numbers, take the max one)
+    best_model_path = os.path.join(model_save_path, str(max([int(x) for x in os.listdir(model_save_path) if x.isdigit()])))
     ###Evaluate on the test set using the best model
     if test_data is not None:
         logger.info("Evaluating on the test set (0.5 of val data)")
         ##Load the best model
-        print("Loading best model from:", model_save_path)
-        best_model=LinkTransformer(model_save_path)
+        print("Loading best model from:", best_model_path)
+        best_model=LinkTransformer(best_model_path)
         test_evaluator(best_model, epoch=0, steps=0, output_path=model_save_path)
 
-    return model_save_path
+    return best_model_path
```

### Comparing `linktransformer-0.1.2/src/linktransformer/preprocess.py` & `linktransformer-0.1.3/src/linktransformer/preprocess.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.2/src/linktransformer/train_model.py` & `linktransformer-0.1.3/src/linktransformer/train_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,23 @@
     else:
         config["eval_type"]="retrieval"
 
     ##Prep model directories if they don't exist
     if not os.path.exists(config["model_save_dir"]):
         os.makedirs(config["model_save_dir"])
 
+
+    ##Add the dataset used in the config 
+    config["training_dataset"]=data if isinstance(data,str) else "dataframe"
+    config["base_model_path"]=model_path
+
+    ##Save the config before training begins
+    with open(os.path.join(config["model_save_dir"], config["model_save_name"], "LT_training_config.json"), "w") as config_file:
+        json.dump(config, config_file)
+
     print("Training")
     best_model_path = train_biencoder(
         train_data=train_data,
         dev_data=val_data,
         test_data=test_data,
         base_model=model_path,
         add_pooling_layer=config["add_pooling_layer"],
@@ -200,23 +209,21 @@
         optimizer_params={'lr': config["learning_rate"]},
         eval_type=config["eval_type"],
         opt_model_description=config["opt_model_description"],
         opt_model_lang=config["opt_model_lang"]
     )
     print(f"Best model saved on the path: {best_model_path} ")
 
-    ##Add the dataset used in the config 
-    config["training_dataset"]=data if isinstance(data,str) else "dataframe"
+
+        
     ##Add the best model path in the config
     config["best_model_path"]=best_model_path
-    config["base_model_path"]=model_path
+    
 
-    ##Save the config
+    ##Save the config after training with the best model
     with open(os.path.join(config["model_save_dir"], config["model_save_name"], "LT_training_config.json"), "w") as config_file:
         json.dump(config, config_file)
-        
-    
 
     return best_model_path
```

### Comparing `linktransformer-0.1.2/src/linktransformer/utils.py` & `linktransformer-0.1.3/src/linktransformer/utils.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.2/src/linktransformer.egg-info/PKG-INFO` & `linktransformer-0.1.3/src/linktransformer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktransformer
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple way to do link dataframes using large language models.
 Author-email: "Abhishek Arora, Sam Jones and Melissa Dell" <llmklinkpython@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 dell-research-harvard
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `linktransformer-0.1.2/src/linktransformer.egg-info/SOURCES.txt` & `linktransformer-0.1.3/src/linktransformer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

