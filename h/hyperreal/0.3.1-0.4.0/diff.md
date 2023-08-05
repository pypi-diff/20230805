# Comparing `tmp/hyperreal-0.3.1.tar.gz` & `tmp/hyperreal-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperreal-0.3.1.tar", last modified: Tue May 30 06:25:56 2023, max compression
+gzip compressed data, was "hyperreal-0.4.0.tar", last modified: Sat Aug  5 13:07:43 2023, max compression
```

## Comparing `hyperreal-0.3.1.tar` & `hyperreal-0.4.0.tar`

### file list

```diff
@@ -1,43 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:25:56.370131 hyperreal-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-30 06:25:08.000000 hyperreal-0.3.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:25:56.362131 hyperreal-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:25:56.366131 hyperreal-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-30 06:25:08.000000 hyperreal-0.3.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-30 06:25:08.000000 hyperreal-0.3.1/.github/workflows/test_python.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-30 06:25:08.000000 hyperreal-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-30 06:25:08.000000 hyperreal-0.3.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-30 06:25:08.000000 hyperreal-0.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 06:25:08.000000 hyperreal-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-30 06:25:56.370131 hyperreal-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-30 06:25:08.000000 hyperreal-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:25:56.370131 hyperreal-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-30 06:25:08.000000 hyperreal-0.3.1/docs/definitions.md
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-30 06:25:08.000000 hyperreal-0.3.1/docs/design.md
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-30 06:25:08.000000 hyperreal-0.3.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:25:56.370131 hyperreal-0.3.1/hyperreal/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/_index_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    32888 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/db_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    72458 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:25:56.370131 hyperreal-0.3.1/hyperreal/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/templates/cluster.html
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/templates/details.html
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/templates/index_listing.html
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/templates/macros.html
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:25:56.370131 hyperreal-0.3.1/hyperreal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-30 06:25:56.000000 hyperreal-0.3.1/hyperreal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-30 06:25:56.000000 hyperreal-0.3.1/hyperreal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 06:25:56.000000 hyperreal-0.3.1/hyperreal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-30 06:25:56.000000 hyperreal-0.3.1/hyperreal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-30 06:25:56.000000 hyperreal-0.3.1/hyperreal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 06:25:56.000000 hyperreal-0.3.1/hyperreal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 06:25:56.370131 hyperreal-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-30 06:25:08.000000 hyperreal-0.3.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-30 06:25:08.000000 hyperreal-0.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:07:43.475441 hyperreal-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-05 13:06:58.000000 hyperreal-0.4.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:07:43.459442 hyperreal-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:07:43.467441 hyperreal-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-08-05 13:06:58.000000 hyperreal-0.4.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-05 13:06:58.000000 hyperreal-0.4.0/.github/workflows/test_python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-05 13:06:58.000000 hyperreal-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-05 13:06:58.000000 hyperreal-0.4.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-05 13:06:58.000000 hyperreal-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-05 13:06:58.000000 hyperreal-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-08-05 13:07:43.475441 hyperreal-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-08-05 13:06:58.000000 hyperreal-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:07:43.467441 hyperreal-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-05 13:06:58.000000 hyperreal-0.4.0/docs/definitions.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-05 13:06:58.000000 hyperreal-0.4.0/docs/design.md
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-05 13:06:58.000000 hyperreal-0.4.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:07:43.459442 hyperreal-0.4.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:07:43.467441 hyperreal-0.4.0/examples/australian_federal_hansard/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-08-05 13:06:58.000000 hyperreal-0.4.0/examples/australian_federal_hansard/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-08-05 13:06:58.000000 hyperreal-0.4.0/examples/australian_federal_hansard/download_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20827 2023-08-05 13:06:58.000000 hyperreal-0.4.0/examples/australian_federal_hansard/hansard_corpus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:07:43.467441 hyperreal-0.4.0/examples/stackoverflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-08-05 13:06:58.000000 hyperreal-0.4.0/examples/stackoverflow/prepare_data.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:07:43.471441 hyperreal-0.4.0/hyperreal/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-05 13:06:58.000000 hyperreal-0.4.0/hyperreal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-08-05 13:06:58.000000 hyperreal-0.4.0/hyperreal/_index_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15353 2023-08-05 13:06:58.000000 hyperreal-0.4.0/hyperreal/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35798 2023-08-05 13:06:58.000000 hyperreal-0.4.0/hyperreal/corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-05 13:06:58.000000 hyperreal-0.4.0/hyperreal/db_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82167 2023-08-05 13:06:58.000000 hyperreal-0.4.0/hyperreal/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17147 2023-08-05 13:06:58.000000 hyperreal-0.4.0/hyperreal/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:07:43.475441 hyperreal-0.4.0/hyperreal/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 13:06:58.000000 hyperreal-0.4.0/hyperreal/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-08-05 13:06:58.000000 hyperreal-0.4.0/hyperreal/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-08-05 13:06:58.000000 hyperreal-0.4.0/hyperreal/templates/cluster.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-08-05 13:06:58.000000 hyperreal-0.4.0/hyperreal/templates/details.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-08-05 13:06:58.000000 hyperreal-0.4.0/hyperreal/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-05 13:06:58.000000 hyperreal-0.4.0/hyperreal/templates/index_listing.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-08-05 13:06:58.000000 hyperreal-0.4.0/hyperreal/templates/macros.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-08-05 13:06:58.000000 hyperreal-0.4.0/hyperreal/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:07:43.471441 hyperreal-0.4.0/hyperreal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-08-05 13:07:43.000000 hyperreal-0.4.0/hyperreal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-05 13:07:43.000000 hyperreal-0.4.0/hyperreal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 13:07:43.000000 hyperreal-0.4.0/hyperreal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-05 13:07:43.000000 hyperreal-0.4.0/hyperreal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-05 13:07:43.000000 hyperreal-0.4.0/hyperreal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-05 13:07:43.000000 hyperreal-0.4.0/hyperreal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-05 13:06:58.000000 hyperreal-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 13:07:43.475441 hyperreal-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-08-05 13:06:58.000000 hyperreal-0.4.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-05 13:06:58.000000 hyperreal-0.4.0/tox.ini
```

### Comparing `hyperreal-0.3.1/.coveragerc` & `hyperreal-0.4.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.1/.github/workflows/publish.yml` & `hyperreal-0.4.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.1/.github/workflows/test_python.yml` & `hyperreal-0.4.0/.github/workflows/test_python.yml`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.1/CITATION.cff` & `hyperreal-0.4.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.1/LICENSE.txt` & `hyperreal-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.1/PKG-INFO` & `hyperreal-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: hyperreal
-Version: 0.3.1
+Version: 0.4.0
 Summary: Hyperreal is a library and tool for intepretive topic modelling.
 Home-page: https://github.com/SamHames/hyperreal/
 Author: Sam Hames
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: stackexchange
 License-File: LICENSE.txt
 
 # Hyperreal
 
 Hyperreal is a Python tool for interactive qualitative analysis of large
 collections of documents.
 
@@ -38,15 +39,15 @@
 ## Usage
 
 Hyperreal can be used in three different ways to flexibly support different
 use cases:
 
 - as a command line application
 - as a Python library
-- via the built in web application
+- as a local web application
 
 All of hyperreal's functionality is available from the Python library, but you
 will need to write Python code to use it directly. The command line interface
 allows for quick and repeatable experimentation and automation for standard
 data types - for example if you often work with Twitter data the command line
 will allow you to rapidly work with many different Twitter data collections.
 The web application is currently focused solely on creating and interactive
@@ -63,15 +64,15 @@
 If you haven't worked with the command line before, you might find the
 following resources useful:
 
 - [Software Carpentry resources for Mac](https://swcarpentry.github.io/shell-novice/)
 - [Open Water Foundation resources for Windows](https://learn.openwaterfoundation.org/owf-learn-windows-shell/)
 
 ```
-# Create a corpus database from the plaintext file
+# Create a corpus database from a plaintext file
 hyperreal plaintext-corpus create corpus.txt corpus.db
 
 # Create an index from the corpus
 hyperreal plaintext-corpus index corpus.db corpus_index.db
 
 # Create a model from that index, in this case with 128 clusters and
 # only include features present in 10 or more documents.
@@ -99,46 +100,48 @@
   # This will drop any line that has no text (such as a paragraph break)
   docs = (line for line in f if line.strip())
   c.replace_docs(docs)
 
 
 # Index that corpus - note that we need to pass the corpus object for
 # initialisation.
-i = index.Index('corpus_index.db', corpus=c)
+idx = index.Index('corpus_index.db', corpus=c)
 # This only needs to be done once, unless the corpus changes.
-i.index()
+idx.index()
 
 # Create a model on this index, with 128 clusters and only including features
 # that match at least 10 documents.
-i.initialise_clusters(n_clusters=128, min_docs=10)
+idx.initialise_clusters(n_clusters=128, min_docs=10)
 # Refine the model for 10 iterations. Note that you can continue to refine
 # the model without initialising the clusters.
-i.refine_clusters(iterations=10)
+idx.refine_clusters(iterations=10)
 
 # Inspect the output of the model using the index instance (currently quite
 # limited). This will print the top 10 most frequent features in each
 # cluster.
-for cluster_id in i.cluster_ids:
-    cluster_features = i.cluster_features(cluster_id)
+for cluster_id in idx.cluster_ids:
+    cluster_features = idx.cluster_features(cluster_id)
     for feature in cluster_features[:10]:
         print(feature)
 
 # Perform a boolean query on the corpus, looking for documents that contain
 # both apples AND oranges in the text field.
 q = i[('text', 'apples')] & i[('text', 'oranges')]
 # Lookup all of the documents in the corpus that match this query.
-docs = i.get_docs(q)
+docs = idx.get_docs(q)
 
 # 'Pivot' the features in the index with respect to all cluster in the model.
 #  This will show the top 10 features in each cluster that are similar to the
 #  query.
-i.pivot_clusters_by_query(query, top_k=10)
+for cluster_detail in idx.pivot_clusters_by_query(query, top_k=10):
+    print(cluster_detail)
 
 # This will show the top 10 features for a selected set of cluster_ids.
-i.pivot_clusters_by_query(query, cluster_ids=[3,5,7], top_k=10)
+for cluster_detail in idx.pivot_clusters_by_query(query, cluster_ids=[3,5,7], top_k=10):
+    print(cluster_detail)
 
 ```
 
 
 ## Development
 
 ### Installation
```

### Comparing `hyperreal-0.3.1/README.md` & `hyperreal-0.4.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ## Usage
 
 Hyperreal can be used in three different ways to flexibly support different
 use cases:
 
 - as a command line application
 - as a Python library
-- via the built in web application
+- as a local web application
 
 All of hyperreal's functionality is available from the Python library, but you
 will need to write Python code to use it directly. The command line interface
 allows for quick and repeatable experimentation and automation for standard
 data types - for example if you often work with Twitter data the command line
 will allow you to rapidly work with many different Twitter data collections.
 The web application is currently focused solely on creating and interactive
@@ -48,15 +48,15 @@
 If you haven't worked with the command line before, you might find the
 following resources useful:
 
 - [Software Carpentry resources for Mac](https://swcarpentry.github.io/shell-novice/)
 - [Open Water Foundation resources for Windows](https://learn.openwaterfoundation.org/owf-learn-windows-shell/)
 
 ```
-# Create a corpus database from the plaintext file
+# Create a corpus database from a plaintext file
 hyperreal plaintext-corpus create corpus.txt corpus.db
 
 # Create an index from the corpus
 hyperreal plaintext-corpus index corpus.db corpus_index.db
 
 # Create a model from that index, in this case with 128 clusters and
 # only include features present in 10 or more documents.
@@ -84,46 +84,48 @@
   # This will drop any line that has no text (such as a paragraph break)
   docs = (line for line in f if line.strip())
   c.replace_docs(docs)
 
 
 # Index that corpus - note that we need to pass the corpus object for
 # initialisation.
-i = index.Index('corpus_index.db', corpus=c)
+idx = index.Index('corpus_index.db', corpus=c)
 # This only needs to be done once, unless the corpus changes.
-i.index()
+idx.index()
 
 # Create a model on this index, with 128 clusters and only including features
 # that match at least 10 documents.
-i.initialise_clusters(n_clusters=128, min_docs=10)
+idx.initialise_clusters(n_clusters=128, min_docs=10)
 # Refine the model for 10 iterations. Note that you can continue to refine
 # the model without initialising the clusters.
-i.refine_clusters(iterations=10)
+idx.refine_clusters(iterations=10)
 
 # Inspect the output of the model using the index instance (currently quite
 # limited). This will print the top 10 most frequent features in each
 # cluster.
-for cluster_id in i.cluster_ids:
-    cluster_features = i.cluster_features(cluster_id)
+for cluster_id in idx.cluster_ids:
+    cluster_features = idx.cluster_features(cluster_id)
     for feature in cluster_features[:10]:
         print(feature)
 
 # Perform a boolean query on the corpus, looking for documents that contain
 # both apples AND oranges in the text field.
 q = i[('text', 'apples')] & i[('text', 'oranges')]
 # Lookup all of the documents in the corpus that match this query.
-docs = i.get_docs(q)
+docs = idx.get_docs(q)
 
 # 'Pivot' the features in the index with respect to all cluster in the model.
 #  This will show the top 10 features in each cluster that are similar to the
 #  query.
-i.pivot_clusters_by_query(query, top_k=10)
+for cluster_detail in idx.pivot_clusters_by_query(query, top_k=10):
+    print(cluster_detail)
 
 # This will show the top 10 features for a selected set of cluster_ids.
-i.pivot_clusters_by_query(query, cluster_ids=[3,5,7], top_k=10)
+for cluster_detail in idx.pivot_clusters_by_query(query, cluster_ids=[3,5,7], top_k=10):
+    print(cluster_detail)
 
 ```
 
 
 ## Development
 
 ### Installation
```

### Comparing `hyperreal-0.3.1/docs/design.md` & `hyperreal-0.4.0/docs/design.md`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.1/hyperreal/_index_schema.py` & `hyperreal-0.4.0/hyperreal/_index_schema.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,17 +10,27 @@
     - a sequence of statements to be run after applying CURRENT_SCHEMA
 
 """
 
 # The application ID uses SQLite's pragma application_id to quickly identify index
 # databases from everything else.
 MAGIC_APPLICATION_ID = 715973853
-CURRENT_SCHEMA_VERSION = 8
+CURRENT_SCHEMA_VERSION = 9
 
 CURRENT_SCHEMA = f"""
+    create table if not exists settings (
+        key primary key,
+        value
+    );
+
+    --------
+    -- Migrated indexes will have no position information.
+    replace into settings values('position_window_size', 0);
+
+    --------
     create table if not exists doc_key (
         doc_id integer primary key,
         doc_key unique
     );
 
     --------
     create table if not exists inverted_index (
@@ -29,29 +39,43 @@
         value not null,
         docs_count integer not null,
         doc_ids roaring_bitmap not null,
         unique (field, value)
     );
 
     --------
+    create table if not exists position_doc_map (
+        field text not null,
+        first_doc_id integer not null,
+        last_doc_id integer not null,
+        docs_count integer not null,
+        doc_ids roaring_bitmap not null,
+        doc_boundaries roaring_bitmap not null,
+        primary key (field, first_doc_id)
+    );
+
+    --------
+    create table if not exists position_index (
+        feature_id references inverted_index on delete cascade,
+        first_doc_id integer,
+        position_count integer,
+        positions roaring_bitmap,
+        primary key (feature_id, first_doc_id)
+    );
+
+    --------
     create table if not exists field_summary (
         field text primary key,
         distinct_values integer,
         min_value,
         max_value
     );
 
     --------
-    create table if not exists skipgram_count (
-        feature_id_a integer references inverted_index(feature_id) on delete cascade,
-        feature_id_b integer references inverted_index(feature_id) on delete cascade,
-        distance integer,
-        docs_count integer,
-        primary key (feature_id_a, feature_id_b, distance)
-    ) without rowid;
+    drop table if exists skipgram_count;
 
     --------
     create index if not exists docs_counts on inverted_index(docs_count);
     --------
     create index if not exists field_docs_counts on inverted_index(field, docs_count);
 
     --------
@@ -160,14 +184,15 @@
     7: (
         [
             "alter table cluster add column pinned bool default 0",
             "alter table feature_cluster add column pinned bool default 0",
         ],
         [],
     ),
+    8: ([], []),
 }
 
 
 class MigrationError(ValueError):
     pass
```

### Comparing `hyperreal-0.3.1/hyperreal/cli.py` & `hyperreal-0.4.0/hyperreal/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,23 +7,103 @@
 import concurrent.futures as cf
 import json
 import logging
 import multiprocessing as mp
 import os
 
 import click
+import networkx as nx
 
 import hyperreal.corpus
 import hyperreal.index
 import hyperreal.server
 
 
 logging.basicConfig(level=logging.INFO)
 
 
+# Utility for making exporters that take three arguments, just with a
+# different corpus type.
+def make_csv_exporter(CorpusType):
+    @click.argument("corpus_db", type=click.Path(exists=True, dir_okay=False))
+    @click.argument("index_db", type=click.Path(exists=True, dir_okay=False))
+    @click.argument("output_file", type=click.Path(dir_okay=False))
+    @click.option(
+        "--docs-per-cluster",
+        type=click.INT,
+        default=50,
+        help="The maximum number of documents to sample from each cluster. "
+        "If set to 0, all documents in clusters will be returned.",
+    )
+    def export_graph(corpus_db, index_db, output_file, docs_per_cluster):
+        """
+        Export a sample of documents from each cluster in the model.
+
+        """
+        if not hyperreal.index.Index.is_index_db(index_db):
+            raise ValueError(f"{index_db} is not a valid index file.")
+
+        corpus = CorpusType(corpus_db)
+        idx = hyperreal.index.Index(index_db, corpus=corpus)
+
+        cluster_samples, sample_clusters = idx.structured_doc_sample(
+            docs_per_cluster=docs_per_cluster
+        )
+        idx.export_document_sample(cluster_samples, sample_clusters, output_file)
+
+    return export_graph
+
+
+def make_two_file_indexer(CorpusType):
+    @click.argument("corpus_db", type=click.Path(exists=True, dir_okay=False))
+    @click.argument("index_db", type=click.Path(dir_okay=False))
+    @click.option(
+        "--doc-batch-size",
+        type=int,
+        default=DEFAULT_DOC_BATCH_SIZE,
+        help="The size of individual batches of documents sent for indexing. "
+        "Larger sizes will require more ram, but might be more efficient for "
+        "large collections.",
+    )
+    @click.option(
+        "--position-window-size",
+        default=0,
+        type=int,
+        help="""
+        The window size to record approximate positional information. The
+        default value of 0 disables recording this information. When > 0,
+        approximate positions of values are recorded up to the given
+        granularity. Smaller values require more space, but enable precise
+        querying. Setting position size to 1 enables recording of exact term
+        positions and precise querying for phrases, but currently only 2**32
+        positions can be recorded in a single field.
+        """,
+    )
+    def corpus_indexer(corpus_db, index_db, doc_batch_size, position_window_size):
+        """
+        Creates the index database representing the given corpus.
+
+        If the index already exists it will be reindexed.
+
+        """
+        click.echo(f"Indexing {corpus_db} into {index_db}.")
+
+        doc_corpus = CorpusType(corpus_db)
+
+        mp_context = mp.get_context("spawn")
+        with cf.ProcessPoolExecutor(mp_context=mp_context) as pool:
+            doc_index = hyperreal.index.Index(index_db, corpus=doc_corpus, pool=pool)
+
+            doc_index.index(
+                doc_batch_size=doc_batch_size, position_window_size=position_window_size
+            )
+
+    return corpus_indexer
+
+
 # The main entry command is always hyperreal
 @click.group(name="hyperreal")
 def cli():
     pass
 
 
 @cli.group()
@@ -56,59 +136,14 @@
     with open(text_file, "r", encoding="utf-8") as infile:
         f = csv.reader(infile)
         # The only documents we drop are lines that are only whitespace.
         docs = (line[0] for line in f if line and line[0].strip())
         doc_corpus.replace_docs(docs)
 
 
-@plaintext_corpus.command(name="index")
-@click.argument("corpus_db", type=click.Path(exists=True, dir_okay=False))
-@click.argument("index_db", type=click.Path(dir_okay=False))
-@click.option(
-    "--doc_batch_size",
-    type=int,
-    default=DEFAULT_DOC_BATCH_SIZE,
-    help="The size of individual batches of documents sent for indexing. "
-    "Larger sizes will require more ram, but might be more efficient for "
-    "large collections.",
-)
-@click.option(
-    "--skipgram-window-size",
-    default=0,
-    help="Size of window to extract skipgrams from. "
-    "Default is 0, which disables this functionality",
-)
-@click.option(
-    "--skipgram-min-docs",
-    default=3,
-    help="Minimum number of docs containing a skipgram for the count to be retained. "
-    "This threshold limits the size of the table used to store skipgrams - set to 1 "
-    "to keep all counts (not recommended).",
-)
-def plaintext_corpus_index(
-    corpus_db, index_db, doc_batch_size, skipgram_window_size, skipgram_min_docs
-):
-    """
-    Creates the index database representing the given plaintext corpus.
-
-    If the index already exists it will be reindexed.
-
-    """
-    click.echo(f"Indexing {corpus_db} into {index_db}.")
-
-    doc_corpus = hyperreal.corpus.PlainTextSqliteCorpus(corpus_db)
-    doc_index = hyperreal.index.Index(index_db, corpus=doc_corpus)
-
-    doc_index.index(
-        doc_batch_size=doc_batch_size,
-        skipgram_window_size=skipgram_window_size,
-        skipgram_min_docs=skipgram_min_docs,
-    )
-
-
 @plaintext_corpus.command(name="serve")
 @click.argument("corpus_db", type=click.Path(exists=True, dir_okay=False))
 @click.argument("index_db", type=click.Path(exists=True, dir_okay=False))
 def plaintext_corpus_serve(corpus_db, index_db):
     """
     Serve the given plaintext corpus and index via the webserver.
 
@@ -126,14 +161,23 @@
             corpus_class=hyperreal.corpus.PlainTextSqliteCorpus,
             corpus_args=[corpus_db],
             pool=pool,
         )
         hyperreal.server.launch_web_server(index_server)
 
 
+plaintext_corpus.command(name="index")(
+    make_two_file_indexer(hyperreal.corpus.PlainTextSqliteCorpus)
+)
+
+plaintext_corpus.command(name="sample")(
+    make_csv_exporter(hyperreal.corpus.PlainTextSqliteCorpus)
+)
+
+
 @cli.group()
 def stackexchange_corpus():
     pass
 
 
 @stackexchange_corpus.command(name="add-site")
 @click.argument("posts_file", type=click.Path(exists=True, dir_okay=False))
@@ -160,59 +204,14 @@
     click.echo(f"Adding {site_url} data into {corpus_db}.")
 
     doc_corpus = hyperreal.corpus.StackExchangeCorpus(corpus_db)
 
     doc_corpus.add_site_data(posts_file, comments_file, users_file, site_url)
 
 
-@stackexchange_corpus.command(name="index")
-@click.argument("corpus_db", type=click.Path(exists=True, dir_okay=False))
-@click.argument("index_db", type=click.Path(dir_okay=False))
-@click.option(
-    "--doc_batch_size",
-    type=int,
-    default=DEFAULT_DOC_BATCH_SIZE,
-    help="The size of individual batches of documents sent for indexing. "
-    "Larger sizes will require more ram, but might be more efficient for "
-    "large collections.",
-)
-@click.option(
-    "--skipgram-window-size",
-    default=0,
-    help="Size of window to extract skipgrams from. "
-    "Default is 0, which disables this functionality",
-)
-@click.option(
-    "--skipgram-min-docs",
-    default=3,
-    help="Minimum number of docs containing a skipgram for the count to be retained. "
-    "This threshold limits the size of the table used to store skipgrams - set to 1 "
-    "to keep all counts (not recommended).",
-)
-def stackexchange_corpus_index(
-    corpus_db, index_db, doc_batch_size, skipgram_window_size, skipgram_min_docs
-):
-    """
-    Creates the index database representing the given Stack Exchange corpus.
-
-    If the index already exists it will be reindexed.
-
-    """
-    click.echo(f"Indexing {corpus_db} into {index_db}.")
-
-    doc_corpus = hyperreal.corpus.StackExchangeCorpus(corpus_db)
-    doc_index = hyperreal.index.Index(index_db, corpus=doc_corpus)
-
-    doc_index.index(
-        doc_batch_size=doc_batch_size,
-        skipgram_window_size=skipgram_window_size,
-        skipgram_min_docs=skipgram_min_docs,
-    )
-
-
 @stackexchange_corpus.command(name="serve")
 @click.argument("corpus_db", type=click.Path(exists=True, dir_okay=False))
 @click.argument("index_db", type=click.Path(exists=True, dir_okay=False))
 def stackexchange_corpus_serve(corpus_db, index_db):
     """
     Serve the given StackExchange corpus and index via the webserver.
 
@@ -230,62 +229,31 @@
             corpus_class=hyperreal.corpus.StackExchangeCorpus,
             corpus_args=[corpus_db],
             pool=pool,
         )
         hyperreal.server.launch_web_server(index_server)
 
 
-@cli.group()
-def twittersphere_corpus():
-    pass
-
-
-@twittersphere_corpus.command(name="index")
-@click.argument("corpus_db", type=click.Path(exists=True, dir_okay=False))
-@click.argument("index_db", type=click.Path(dir_okay=False))
-@click.option(
-    "--doc_batch_size",
-    type=int,
-    default=100000,
-    help="The size of individual batches of documents sent for indexing. "
-    "Larger sizes will require more ram, but might be more efficient for "
-    "large collections.",
-)
-@click.option(
-    "--skipgram-window-size",
-    default=0,
-    help="Size of window to extract skipgrams from. "
-    "Default is 0, which disables this functionality",
+stackexchange_corpus.command(name="sample")(
+    make_csv_exporter(hyperreal.corpus.StackExchangeCorpus)
 )
-@click.option(
-    "--skipgram-min-docs",
-    default=3,
-    help="Minimum number of docs containing a skipgram for the count to be retained. "
-    "This threshold limits the size of the table used to store skipgrams - set to 1 "
-    "to keep all counts (not recommended).",
+
+stackexchange_corpus.command(name="index")(
+    make_two_file_indexer(hyperreal.corpus.StackExchangeCorpus)
 )
-def twittersphere_corpus_index(
-    corpus_db, index_db, doc_batch_size, skipgram_window_size, skipgram_min_docs
-):
-    """
-    Creates the index database representing the given Stack Exchange corpus.
 
-    If the index already exists it will be reindexed.
 
-    """
-    click.echo(f"Indexing {corpus_db} into {index_db}.")
+@cli.group()
+def twittersphere_corpus():
+    pass
 
-    doc_corpus = hyperreal.corpus.TwittersphereCorpus(corpus_db)
-    doc_index = hyperreal.index.Index(index_db, corpus=doc_corpus)
 
-    doc_index.index(
-        doc_batch_size=doc_batch_size,
-        skipgram_window_size=skipgram_window_size,
-        skipgram_min_docs=skipgram_min_docs,
-    )
+twittersphere_corpus.command(name="index")(
+    make_two_file_indexer(hyperreal.corpus.TwittersphereCorpus)
+)
 
 
 @twittersphere_corpus.command(name="serve")
 @click.argument("corpus_db", type=click.Path(exists=True, dir_okay=False))
 @click.argument("index_db", type=click.Path(exists=True, dir_okay=False))
 def twittersphere_corpus_serve(corpus_db, index_db):
     """
@@ -399,14 +367,80 @@
 
     click.echo(f"Refining for {iterations} iterations on {index_db}.")
     doc_index.refine_clusters(
         iterations=iterations, target_clusters=clusters, tolerance=tolerance
     )
 
 
+@cli.group()
+def export():
+    pass
+
+
+@export.command(name="graph")
+@click.argument("index_db", type=click.Path(exists=True, dir_okay=False))
+@click.argument("graph_file", type=click.Path(dir_okay=False))
+@click.option(
+    "--top-k-features",
+    type=click.INT,
+    default=5,
+    help="The number of top features to include in the node labels.",
+)
+@click.option(
+    "--include-field-in-label/--exclude-field-in-label",
+    default=True,
+    help="Include or exclude the field in node labels. This can be used "
+    "to exclude showing fields when you only have a single field in the model.",
+)
+def export_graph(index_db, graph_file, top_k_features, include_field_in_label):
+    """
+    Export the clustering in the given index into the given file as graphml.
+    """
+    if not hyperreal.index.Index.is_index_db(index_db):
+        raise ValueError(f"{index_db} is not a valid index file.")
+
+    mp_context = mp.get_context("spawn")
+    with cf.ProcessPoolExecutor(mp_context=mp_context) as pool:
+        idx = hyperreal.index.Index(index_db, pool=pool)
+        graph = idx.create_cluster_cooccurrence_graph(
+            top_k=top_k_features, include_field_in_label=include_field_in_label
+        )
+        nx.write_graphml(graph, graph_file)
+
+
+@export.command(name="clusters")
+@click.argument("index_db", type=click.Path(exists=True, dir_okay=False))
+@click.argument("cluster_file", type=click.Path(dir_okay=False))
+@click.option(
+    "--top-k-features",
+    type=click.INT,
+    default=10,
+    help="The number of top features to include from each cluster."
+    "Setting this to 0 will export all features in each cluster.",
+)
+def export_clusters(index_db, cluster_file, top_k_features):
+    """
+    Export all cluster features in the model to the given csv file.
+    """
+    if not hyperreal.index.Index.is_index_db(index_db):
+        raise ValueError(f"{index_db} is not a valid index file.")
+
+    idx = hyperreal.index.Index(index_db)
+
+    with open(cluster_file, "w", encoding="utf-8") as output:
+        writer = csv.writer(output, dialect="excel", quoting=csv.QUOTE_ALL)
+        writer.writerow(("cluster_id", "feature_id", "field", "value", "docs_count"))
+
+        top_k = top_k_features or 2**62
+        features = idx.top_cluster_features(top_k=top_k)
+        for cluster_id, _, cluster_features in features:
+            for row in cluster_features:
+                writer.writerow([cluster_id, *row])
+
+
 @cli.command()
 @click.argument("index_db", type=click.Path(exists=True, dir_okay=False))
 def serve(index_db):
     """
     Serve the given index file.
 
     Note that this method of serving will not provide access to the underlying
```

### Comparing `hyperreal-0.3.1/hyperreal/corpus.py` & `hyperreal-0.4.0/hyperreal/corpus.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,20 +10,22 @@
 """
 
 import abc
 from collections import defaultdict
 import datetime as dt
 import gzip
 import html
+from html.parser import HTMLParser
 import json
 import re
-from typing import Protocol, runtime_checkable
+from typing import Protocol, Sequence, runtime_checkable, Any
 from urllib.parse import urlparse
 from xml.etree import ElementTree
 
+from lxml.html import fragment_fromstring
 from dateutil.parser import isoparse
 from jinja2 import Template
 from markupsafe import Markup
 
 from hyperreal import utilities
 from hyperreal.db_utilities import connect_sqlite, dict_factory
 
@@ -32,14 +34,15 @@
 class BaseCorpus(Protocol):
     """
     - provides access to documents, and describes how to index them.
     - needs to be picklable and safely enable concurrent read access
     - Designed to enable small batches of work, and avoid representing entire
       collections in memory/work on collections much larger than memory.
     - Designed to enable downstream concurrent computing on those small batches.
+
     """
 
     CORPUS_TYPE: str
 
     @abc.abstractmethod
     def docs(self, doc_keys=None):
         """
@@ -54,47 +57,64 @@
     def keys(self):
         """An iterator of all document keys present."""
         pass
 
     @abc.abstractmethod
     def index(self, doc):
         """
-        Returns a mapping of:
+        Returns a mapping of the indexable fields in the document:
 
             {
                 "field1": [value1, value2],
-                "field2": [value]
+                "field2": [value],
+                "field3": {value_a, value_b}
             }
 
         Values need not be deduplicated: the indexer will take care of that
         for the boolean query construction, and leaving duplicates allows for
         things like Bag of Feature counts.
 
         """
         pass
 
-    @abc.abstractmethod
-    def serialize(self):
-        pass
-
-    @classmethod
-    @abc.abstractmethod
-    def deserialize(cls, state):
-        pass
-
     def close(self):
         pass
 
     def __getitem__(self, doc_key):
         return self.docs([doc_key])
 
     def __iter__(self):
         return self.docs(doc_keys=None)
 
 
+@runtime_checkable
+class WebRenderableCorpus(BaseCorpus, Protocol):
+    @abc.abstractmethod
+    def render_docs_html(self, doc_keys):
+        """Render documents into a list of HTML strings."""
+        pass
+
+
+@runtime_checkable
+class TableRenderableCorpus(BaseCorpus, Protocol):
+    @property
+    def table_fields(self) -> Sequence[str]:
+        pass
+
+    @abc.abstractmethod
+    def render_docs_table(self, doc_keys) -> Sequence[tuple[Any, dict[str, Any]]]:
+        """
+        Render a series of documents into a form suitable for a spreadsheet.
+
+        This enables spreadsheet export and sampling of documents.
+
+        """
+        pass
+
+
 class SqliteBackedCorpus(BaseCorpus):
     def __init__(self, db_path):
         """
         A helper class for creating corpuses backed by SQLite databases.
 
         This handles some basic things like saving the database path and ensuring
         that the corpus object is picklable for multiprocessing.
@@ -118,28 +138,22 @@
 
     def __getstate__(self):
         return self.db_path
 
     def __setstate__(self, db_path):
         self.__init__(db_path)
 
-    def serialize(self):
-        return self.db_path
-
-    @classmethod
-    def deserialize(cls, data):
-        return cls(data)
-
     def close(self):
         if self._db is not None:
             self._db.close()
 
 
 class PlainTextSqliteCorpus(SqliteBackedCorpus):
     CORPUS_TYPE = "PlainTextSqliteCorpus"
+    table_fields = ["text"]
 
     def __init__(self, db_path, tokeniser=utilities.tokens):
         super().__init__(db_path)
 
         self.tokeniser = tokeniser
 
     def __getstate__(self):
@@ -202,17 +216,42 @@
             "text": self.tokeniser(doc["text"]),
         }
 
     def render_docs_html(self, doc_keys):
         """Return the given documents as HTML."""
         return [(key, doc["text"]) for key, doc in self.docs(doc_keys=doc_keys)]
 
+    def render_docs_table(self, doc_keys):
+        """
+        Return the documents for rendering in a spreadsheet or table.
+
+        The only field is "text" in this case.
+
+        """
+        return [
+            (key, {"text": doc["text"]}) for key, doc in self.docs(doc_keys=doc_keys)
+        ]
+
 
 class StackExchangeCorpus(SqliteBackedCorpus):
     CORPUS_TYPE = "StackExchangeCorpus"
+    table_fields = [
+        "site_url",
+        "Id",
+        "OwnerUserId",
+        "DisplayName",
+        "ContentLicense",
+        "PostType",
+        "Body",
+        "ParentId",
+        "QuestionTitle",
+        "LiveLink",
+        "tags",
+        "comments",
+    ]
 
     def add_site_data(self, posts_file, comments_file, users_file, site_url):
         """
         Add the data for a specific stackexchange site to the model.
 
         The site_url is used for differentiating sites, and constructing links
         to relevant pages on the correct site.
@@ -454,15 +493,16 @@
                                     from User
                                     where
                                         (User.site_id, User.Id) =
                                         (Post.site_id, Post.OwnerUserId)
                                 ),
                                 '<Deleted User>'
                             ) as DisplayName,
-                            CreationDate
+                            CreationDate,
+                            PostType
                         from Post
                         inner join Site using(site_id)
                         where Post.doc_id = ?
                         """,
                         [key],
                     )
                 )[0]
@@ -504,45 +544,46 @@
 
         finally:
             self.db.execute("release docs")
 
     TEMPLATE = Template(
         """
         <details>
-            <summary>{{ base_fields["PostType"] }} from {{ base_fields["site_url"] }}: "{{ base_fields["QuestionTitle"] }}"</summary>
-
-            <a href="{{ '{}/questions/{}'.format(base_fields["site_url"], base_fields["Id"])  }}">Live Link</a>
-
-            {{ base_fields["Body"] }}
-
+            <summary><em>{{ base_fields["QuestionTitle"] }}</em> - {{ base_fields["PostType"] }} from {{ base_fields["site_url"] }}</summary>
+            
             <p>
                 <small>
+                    <a href="{{ base_fields["LiveLink"] }}">Live Link</a>
                     Copyright {{ base_fields["ContentLicense"]}} by
                     {% if base_fields["OwnerUserId"] %}
                     <a href="{{ '{}/users/{}'.format(base_fields["site_url"], base_fields["OwnerUserId"]) }}">
                         {{ base_fields["DisplayName"] }}
                     </a>
                     {% else %}
                     <Deleted User>
                     {% endif %}
                 </small>
             </p>
 
+            {{ base_fields["Body"] }}
+
             <details>
                 <summary>Tags:</summary>
                 <ul>
-                    {{ tags }}
+                    {% for tag in tags %}
+                    <li>{{ tag }}
+                    {% endfor %}
                 </ul>
             </details>
 
             <details>
                 <summary>Comments:</summary>
                 <ul>
                     {% for comment in user_comments %}
-                        <li>{{ comment["Text"] }}
+                        <li>{{ comment["Text"] | e}}
                             <small>
                                 Copyright {{ comment["ContentLicense"]}} by
                                 {% if comment["UserId"] %}
                                 <a href="{{ '{}/users/{}'.format(comment["site_url"], comment["UserId"]) }}">
                                     {{ comment["DisplayName"] }}
                                 </a>
                                 {% else %}
@@ -553,15 +594,15 @@
                     {% endfor %}
                 </ul>
             </details>
         </details>
         """
     )
 
-    def _render_doc_key(self, key):
+    def _get_rendered_doc_fields(self, key):
         base_fields = list(
             self.db.execute(
                 """
                 select
                     Post.site_id,
                     site_url,
                     Post.Id,
@@ -575,34 +616,35 @@
                         where
                             (User.site_id, User.Id) =
                             (Post.site_id, Post.OwnerUserId)
                     ) as DisplayName,
                     post.ContentLicense,
                     post.PostType,
                     post.Body,
+                    Post.ParentId,
                     coalesce(Post.Title, parent.Title) as QuestionTitle,
-                    coalesce(Post.ParentId, Post.Id) as TagPostId
+                    site_url || '/questions/' || Post.Id as LiveLink
                 from Post
                 inner join site using(site_id)
                 left outer join Post parent
                     on (parent.site_id, parent.Id) =
                         (Post.site_id, Post.ParentId)
                 where Post.doc_id = ?
                 """,
                 [key],
             )
         )[0]
 
-        tags = "\n".join(
-            f"<li>  { r['Tag'] }"
+        tags = {
+            r["Tag"]
             for r in self.db.execute(
                 "select Tag from PostTag where (site_id, PostId) = (:site_id, :TagPostId)",
                 base_fields,
             )
-        )
+        }
 
         user_comments = list(
             self.db.execute(
                 """
                 select
                     site_url,
                     UserId,
@@ -619,61 +661,111 @@
                 inner join site using(site_id)
                 where (site_id, PostId) = (:site_id, :Id)
                 """,
                 base_fields,
             )
         )
 
-        return Markup(
-            self.TEMPLATE.render(
-                base_fields=base_fields, tags=tags, user_comments=user_comments
-            )
-        )
+        return base_fields, tags, user_comments
 
     def render_docs_html(self, doc_keys):
+        """Render a HTML version of the stackexchange posts, including metadata."""
         self.db.execute("savepoint render_docs_html")
 
-        docs = [(key, self._render_doc_key(key)) for key in doc_keys]
+        docs = []
+
+        for key in doc_keys:
+            base_fields, tags, user_comments = self._get_rendered_doc_fields(key)
+            docs.append(
+                (
+                    key,
+                    Markup(
+                        self.TEMPLATE.render(
+                            base_fields=base_fields,
+                            tags=tags,
+                            user_comments=user_comments,
+                        )
+                    ),
+                )
+            )
 
         self.db.execute("release render_docs_html")
 
         return docs
 
+    def render_docs_table(self, doc_keys):
+        """Render a simplified tabular version of the stackexchange posts, including metadata."""
+        self.db.execute("savepoint render_docs_spreadsheet")
+
+        docs = []
+
+        for key in doc_keys:
+            base_fields, tags, user_comments = self._get_rendered_doc_fields(key)
+            base_fields["tags"] = ", ".join(tags)
+            base_fields["comments"] = json.dumps(
+                [
+                    {
+                        key: comment[key]
+                        for key in ["DisplayName", "Text", "ContentLicense"]
+                    }
+                    for comment in user_comments
+                ]
+            )
+            docs.append((key, base_fields))
+
+        self.db.execute("release render_docs_spreadsheet")
+
+        return docs
+
     def keys(self):
         return (r["doc_id"] for r in self.db.execute("select doc_id from Post"))
 
     def index(self, doc):
+        code_blocks = []
+
+        if doc["Body"]:
+            body_html = fragment_fromstring(doc["Body"], create_parent="div")
+
+            for node in body_html.xpath("pre/code"):
+                # Extract text of code blocks
+                code_blocks.append(" ".join(node.itertext()))
+                # Then remove them, treat everything else as post text
+                node.getparent().remove(node)
+
+            # This is a little wrong, ideally we'd handle the cases where
+            # the code blocks are removed with a sentinel...
+            post_text = " ".join(body_html.itertext())
+
+        else:
+            post_text = ""
+
         indexed = {
             "UserPosting": set([doc["DisplayName"]]),
-            # Note tokenise different components separately, so there are
-            # sentinels included for long distance bigrams.
-            "Post": utilities.tokens((doc["Title"] or "")) +
-            # Todo: this is pretty basic, in the future may want to pull out
-            # some markup into a separate field, like for code.
-            [
-                t
-                for l in utilities.text_from_html(doc["Body"] or "")
-                for t in utilities.tokens(l)
+            "Post": utilities.tokens((doc["Title"] or ""))
+            + utilities.tokens(post_text),
+            "CodeBlock": [
+                t for line in code_blocks for t in utilities.tokens(line) if line
             ],
             "Tag": doc["Tags"],
             # Comments from deleted users remain, but have no UserId associated.
             "UserCommenting": {u["DisplayName"] for u in doc["UserComments"]},
             "Comment": [
                 t for c in doc["UserComments"] for t in utilities.tokens(c["Text"])
             ],
             "Site": set([doc["site_url"]]),
+            "PostType": set([doc["PostType"]]),
         }
 
         created_at = isoparse(doc["CreationDate"])
         rounded_times = utilities.round_datetime(created_at)
         for granularity, dt in rounded_times.items():
             # Don't bother indexing at minute/hour granularity - just day/month/year
             if granularity in ("minute", "hour"):
                 continue
-            indexed[f"created_{granularity}"] = [dt.isoformat()]
+            indexed[f"created_{granularity}"] = set([dt.isoformat()])
 
         return indexed
 
 
 class TwittersphereCorpus(SqliteBackedCorpus):
 
     """
```

### Comparing `hyperreal-0.3.1/hyperreal/db_utilities.py` & `hyperreal-0.4.0/hyperreal/db_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,16 @@
     if row_factory:
         conn.row_factory = row_factory
 
     return conn
 
 
 def save_bitmap(bm):
+    bm.shrink_to_fit()
+    bm.run_optimize()
     return bm.serialize()
 
 
 def load_bitmap(bm_bytes):
     return pyroaring.BitMap.deserialize(bm_bytes)
 
 
@@ -52,8 +54,8 @@
     def __init__(self):
         self.bitmap = pyroaring.BitMap()
 
     def step(self, bitmap):
         self.bitmap |= pyroaring.BitMap.deserialize(bitmap)
 
     def finalize(self):
-        return self.bitmap.serialize()
+        return save_bitmap(self.bitmap)
```

### Comparing `hyperreal-0.3.1/hyperreal/index.py` & `hyperreal-0.4.0/hyperreal/index.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,65 +5,79 @@
 """
 
 import array
 import atexit
 import collections
 from collections.abc import Sequence, Iterable
 import concurrent.futures as cf
+import csv
 from functools import wraps
 import heapq
 import logging
 import math
 import multiprocessing as mp
 import os
 import random
 import sqlite3
 import tempfile
 from typing import Any, Union, Hashable, Optional
 
+import networkx as nx
 from pyroaring import BitMap, FrozenBitMap, AbstractBitMap
 
 from hyperreal import db_utilities, corpus, _index_schema, utilities
 
 
 logger = logging.getLogger(__name__)
 
 
 class CorpusMissingError(AttributeError):
     pass
 
 
+class UnsupportedCorpusOperation(AttributeError):
+    pass
+
+
 class IndexingError(AttributeError):
     pass
 
 
 FeatureKey = tuple[str, Any]
 FeatureKeyOrId = Union[FeatureKey, int]
 FeatureIdAndKey = tuple[int, str, Any]
 BitSlice = list[BitMap]
 
 
-def requires_corpus(func):
+def requires_corpus(RequiredCorpus):
     """
-    Mark method as requiring a corpus object.
+    Mark method as requiring specific corpus functionality.
 
     Raises an AttributeError if no corpus object is present on this index.
 
     """
 
-    @wraps(func)
-    def wrapper_func(self, *args, **kwargs):
-        if self.corpus is None:
-            raise CorpusMissingError(
-                "A Corpus must be provided to the index for this functionality."
-            )
+    def corpus_wrapper(func):
+        @wraps(func)
+        def wrapper_func(self, *args, **kwargs):
+            if self.corpus is None:
+                raise CorpusMissingError(
+                    "A Corpus must be provided to the index for this functionality."
+                )
 
-        return func(self, *args, **kwargs)
+            if not isinstance(self.corpus, RequiredCorpus):
+                raise UnsupportedCorpusOperation(
+                    "The required functionality is not available on this corpus."
+                )
 
-    return wrapper_func
+            return func(self, *args, **kwargs)
+
+        return wrapper_func
+
+    return corpus_wrapper
 
 
 def atomic(writes=False):
     """
     Wrap the decorated interaction with SQLite in a transaction or savepoint.
 
     Uses savepoints - if no enclosing transaction is present, this will create
@@ -157,14 +171,20 @@
         if migrated:
             self.db.execute("begin")
             self._update_changed_clusters()
             self.db.execute("commit")
 
         self.corpus = corpus
 
+        self.position_window_size = list(
+            self.db.execute(
+                "select value from settings where key = 'position_window_size'"
+            )
+        )[0][0]
+
         # For tracking the state of nested transactions. This is incremented
         # everytime a savepoint is entered with the @atomic() decorator, and
         # decremented on leaving. Housekeeping functions will run when leaving
         # the last savepoint by committing a transaction.
         self._transaction_level = 0
         self._changed = False
 
@@ -303,22 +323,21 @@
         )
 
         if results:
             return results[0][0]
         else:
             raise KeyError(f"Feature with key '{key}' not found.")
 
-    @requires_corpus
+    @requires_corpus(corpus.BaseCorpus)
     def index(
         self,
         doc_batch_size=1000,
-        merge_batches=10,
         working_dir=None,
-        skipgram_window_size=0,
-        skipgram_min_docs=3,
+        workers=None,
+        position_window_size=0,
     ):
         """
         Indexes the corpus, using the provided function or the corpus default.
 
         This method will index the entire corpus from scratch. If the corpus has
         already been indexed, it will be atomically replaced.
 
@@ -336,37 +355,32 @@
         - limits the number of batches in flight at the same time
         - incrementally merges background batches to a single file
         - new index content is created in the background, and indexed content is
           written to the index in the background.
 
         """
 
-        workers = self.pool._max_workers
+        workers = workers or self.pool._max_workers
 
         try:
+            self.db.execute("pragma foreign_keys=0")
             self.db.execute("begin")
         except sqlite3.OperationalError:
             raise IndexingError(
                 "The `index` method can't be called in a nested transaction."
             )
 
-        if merge_batches > 10:
-            raise ValueError(f"merge_batches must be <= 10.")
-
         try:
-            tempdir = working_dir or tempfile.TemporaryDirectory()
-            current_temp_file_counter = 0
+            manager = mp.Manager()
+            write_lock = manager.Lock()
 
-            def get_next_temp_file():
-                nonlocal current_temp_file_counter
-                temp_file_path = os.path.join(
-                    tempdir.name, str(current_temp_file_counter)
-                )
-                current_temp_file_counter += 1
-                return temp_file_path
+            detach = False
+
+            tempdir = working_dir or tempfile.TemporaryDirectory()
+            temp_index = os.path.join(tempdir.name, "temp_index.db")
 
             # We're still inside a transaction here, so processes reading from
             # the index won't see any of these changes until the release at
             # the end.
             self.db.execute("delete from doc_key")
 
             # we will associate document keys to internal document ids
@@ -374,15 +388,14 @@
             doc_keys = enumerate(self.corpus.keys())
 
             batch_doc_ids = []
             batch_doc_keys = []
             batch_size = 0
 
             futures = set()
-            to_merge = collections.defaultdict(list)
 
             self.logger.info("Beginning indexing.")
 
             for doc_key in doc_keys:
                 self.db.execute("insert into doc_key values(?, ?)", doc_key)
                 batch_doc_ids.append(doc_key[0])
                 batch_doc_keys.append(doc_key[1])
@@ -394,156 +407,127 @@
                     # Dispatch the batch
                     futures.add(
                         self.pool.submit(
                             _index_docs,
                             self.corpus,
                             batch_doc_ids,
                             batch_doc_keys,
-                            get_next_temp_file(),
-                            skipgram_window_size,
+                            temp_index,
+                            position_window_size,
+                            write_lock,
                         )
                     )
                     batch_doc_ids = []
                     batch_doc_keys = []
                     batch_size = 0
 
-                    if len(futures) >= workers:
+                    # Be polite and avoid filling up the queue.
+                    if len(futures) >= workers + 1:
                         done, futures = cf.wait(futures, return_when="FIRST_COMPLETED")
 
                         for f in done:
-                            try:
-                                segment_path, level = f.result()
-                                to_merge[level].append(segment_path)
-                            except Exception:
-                                self.logger.exception(
-                                    "Caught indexing exception from background."
-                                )
-                                raise
-
-                        # Note that there's an SQLite limit to how many db's
-                        # we can attach at once, so we can't dispatch more than
-                        # to_merge at any time, even if there's more available.
-                        for level, paths in list(to_merge.items()):
-                            if len(paths) >= merge_batches:
-                                futures.add(
-                                    self.pool.submit(
-                                        _merge_indices,
-                                        get_next_temp_file(),
-                                        level + 1,
-                                        *paths[:merge_batches],
-                                    )
-                                )
-                                self.logger.debug(
-                                    f"Dispatching batches {paths[:merge_batches]}for merging."
-                                )
-                                to_merge[level] = paths[merge_batches:]
+                            f.result()
 
             # Dispatch the final batch.
             if batch_doc_keys:
                 self.logger.debug("Dispatching final batch for indexing.")
                 futures.add(
                     self.pool.submit(
                         _index_docs,
                         self.corpus,
                         batch_doc_ids,
                         batch_doc_keys,
-                        get_next_temp_file(),
-                        skipgram_window_size,
+                        temp_index,
+                        position_window_size,
+                        write_lock,
                     )
                 )
 
             self.logger.info("Waiting for batches to complete.")
 
-            # Finalise all segment indexing
-            while futures:
-                done, futures = cf.wait(futures, return_when="FIRST_COMPLETED")
-
-                for future in done:
-                    segment_path, level = future.result()
-                    to_merge[level].append(segment_path)
-
-                for level, paths in list(to_merge.items()):
-                    if len(paths) >= merge_batches:
-                        futures.add(
-                            self.pool.submit(
-                                _merge_indices,
-                                get_next_temp_file(),
-                                level + 1,
-                                *paths[:merge_batches],
-                            )
-                        )
-                        to_merge[level] = paths[merge_batches:]
-
-            self.logger.info("Merging batches.")
-            # The merge strategy is different now: if we are below merge_batches left, just go
-            # straight to that, otherwise dispatch as many chunks as possible
-            to_merge = [p for paths in to_merge.values() for p in paths]
-
-            while len(to_merge) > 1:
-                futures = set()
-                merge_blocks = math.ceil(len(to_merge) / merge_batches)
-                # Now to try to dispatch more similar chunks of work, regardless of level.
+            # Zero out existing features, but don't reassign them
+            self.db.execute(
+                """
+                update inverted_index set
+                    docs_count = 0,
+                    doc_ids = ?1
+                """,
+                [BitMap()],
+            )
 
-                for i in range(merge_blocks):
-                    futures.add(
-                        self.pool.submit(
-                            _merge_indices,
-                            get_next_temp_file(),
-                            level + 1,
-                            *to_merge[i::merge_blocks],
-                        )
-                    )
+            # Zero out positional information
+            self.db.execute("delete from position_doc_map")
+            self.db.execute("delete from position_index")
 
-                to_merge = []
-                for f in cf.as_completed(futures):
-                    to_merge.append(f.result()[0])
+            self.db.execute(
+                "replace into settings values('position_window_size', ?)",
+                [position_window_size],
+            )
 
-            merge_file = to_merge[0]
+            # Make sure all of the batches have completed.
+            for f in cf.as_completed(futures):
+                f.result()
 
-            self.logger.info("Finalising indexing.")
+            self.logger.info("Batches complete - merging into main index.")
 
             # Now merge back to the original index, preserving feature_ids
             # if this is a reindex operation.
-            # Deleted features will be removed
-            self.db.execute("attach ? as merged", [merge_file])
-            to_detach = True
+            self.db.execute("attach ? as tempindex", [temp_index])
+            detach = True
 
-            # Zero out existing features, but don't reassign them
             self.db.execute(
-                "update inverted_index set docs_count = 0, doc_ids = ?",
-                [BitMap()],
+                """
+                create index tempindex.field_value on inverted_index_segment(
+                    field, value, first_doc_id
+                )
+                """
             )
 
-            # Ensure there's a feature_id for every field, value
+            # Actually populate the new values - inverted index
             self.db.execute(
                 """
-                insert or ignore into inverted_index
-                    select null, field, value, 0, ?
-                    from merged.inverted_index_segment
-                    -- Assign smaller feature_ids to more
-                    -- frequent features.
-                    order by docs_count desc
-                """,
-                [BitMap()],
+                replace into inverted_index(feature_id, field, value, docs_count, doc_ids)
+                    select
+                        (
+                            select feature_id
+                            from inverted_index ii
+                            where (ii.field, ii.value) = (iis.field, iis.value)
+                        ),
+                        field,
+                        value,
+                        sum(docs_count) as docs_count,
+                        roaring_union(doc_ids) as doc_ids
+                    from inverted_index_segment iis
+                    group by field, value
+                """
             )
-            # Update all features that are present in the new indexing.
+
+            # Position index
             self.db.execute(
                 """
-                update inverted_index set
-                    (docs_count, doc_ids) = (
-                        select
-                            docs_count,
-                            doc_ids
-                        from merged.inverted_index_segment
-                        where (field, value) = (inverted_index.field, inverted_index.value)
-                    )
-                where (field, value) in (
-                    select field, value
-                    from merged.inverted_index_segment
-                )
+                insert into position_index(feature_id, first_doc_id, position_count, positions)
+                    select
+                        (
+                            select feature_id
+                            from inverted_index ii
+                            where (ii.field, ii.value) = (iis.field, iis.value)
+                        ),
+                        first_doc_id,
+                        position_count,
+                        positions
+                    from inverted_index_segment iis
+                    where position_count > 0
+                """
+            )
+
+            self.db.execute(
+                """
+                insert into position_doc_map
+                    select *
+                    from batch_position
                 """
             )
 
             # Update docs_counts in the clusters
             self.db.execute(
                 """
                 update feature_cluster set
@@ -551,37 +535,14 @@
                         select docs_count
                         from inverted_index ii
                         where ii.feature_id = feature_cluster.feature_id
                     )
                 """
             )
 
-            self.db.execute("DELETE from skipgram_count")
-            self.db.execute(
-                """
-                INSERT into main.skipgram_count
-                select
-                    (
-                        select feature_id
-                        from inverted_index ii
-                        where (msc.field, msc.value_a) = (ii.field, ii.value)
-                    ),
-                    (
-                        select feature_id
-                        from inverted_index ii2
-                        where (msc.field, msc.value_b) = (ii2.field, ii2.value)
-                    ),
-                    distance,
-                    docs_count
-                from merged.skipgram_count msc
-                where docs_count >= ?
-                """,
-                [skipgram_min_docs],
-            )
-
             # Write the field summary
             self.db.execute("delete from field_summary")
             self.db.execute(
                 """
                 insert into field_summary
                 select
                     field,
@@ -595,66 +556,317 @@
 
             # Update all cluster stats based on new index stats
             self.db.execute(
                 "insert into changed_cluster select cluster_id from cluster"
             )
 
             self.db.execute("commit")
-            self.db.execute("detach merged")
 
             self.db.execute("begin")
             self._update_changed_clusters()
             self.db.execute("commit")
 
         except Exception:
             self.logger.exception("Indexing failure.")
             self.db.execute("rollback")
             raise
 
         finally:
+            self.db.execute("pragma foreign_keys=1")
+            manager.shutdown()
+
+            if detach:
+                self.db.execute("detach tempindex")
+
             tempdir.cleanup()
 
+        self.position_window_size = position_window_size
         self.logger.info("Indexing completed.")
 
     @atomic()
     def convert_query_to_keys(self, query):
         """Generate the doc_keys one by one for the given query."""
 
         for doc_id in query:
             doc_key = list(
                 self.db.execute(
                     "select doc_key from doc_key where doc_id = ?", [doc_id]
                 )
             )[0][0]
             yield doc_key
 
-    @requires_corpus
+    @atomic()
+    def iter_field_docs(self, field, min_docs=1):
+        """
+        Iterate through all values and corresponding doc_ids for the given field.
+
+        Iteration is by lexicographical order of the values.
+
+        """
+
+        value_docs = self.db.execute(
+            """
+            select value, docs_count, doc_ids
+            from inverted_index
+            where field = ?1
+                and docs_count >= ?2
+            order by value
+            """,
+            [field, min_docs],
+        )
+
+        for item in value_docs:
+            yield item
+
+    def intersect_queries_with_field(
+        self, queries: dict[Hashable, AbstractBitMap], field: str
+    ) -> tuple[list[Any], list[int], dict[Hashable, list[int]]]:
+        """
+        Intersect all the given queries with all values in the chosen field.
+
+        Note that this can take a long time with fields with many values, such
+        as tokenised text. This is best used with single value fields of low
+        cardinality (<1000 distinct values). Examples of this might be
+        datetimes truncated to a month, or ordinal ranges such as a likert
+        scale.
+
+        """
+
+        intersections = collections.defaultdict(list)
+        values = []
+        totals = []
+
+        for value, docs_count, doc_ids in self.iter_field_docs(field):
+            values.append(value)
+            totals.append(docs_count)
+
+            for name, query in queries.items():
+                inter = query.intersection_cardinality(doc_ids)
+                intersections[name].append(inter)
+
+        return values, totals, intersections
+
+    @requires_corpus(corpus.BaseCorpus)
     def docs(self, query):
         """Retrieve the documents matching the given query set."""
         keys = self.convert_query_to_keys(query)
         return self.corpus.docs(doc_keys=keys)
 
-    @requires_corpus
-    def render_docs(self, query, random_sample_size=None):
+    @requires_corpus(corpus.BaseCorpus)
+    @atomic()
+    def extract_matching_windows(
+        self, query, features, window_size, random_sample_size=None
+    ):
+        """
+        Retrieve cooccurrence windows around each matching feature in each of
+        the given documents.
+
+        window_size is the number of features to extract either size of a match.
+
+        See also the concordance function which turns features back into
+        strings.
+
+        """
+        if random_sample_size is not None:
+            query = self.sample_bitmap(query, random_sample_size)
+
+        field_features = collections.defaultdict(set)
+
+        for feature in features:
+            if isinstance(feature, int):
+                field, value = self.lookup_feature(feature)
+            elif isinstance(feature, tuple):
+                field, value = feature
+            else:
+                raise TypeError(
+                    f"Unknown feature type {feature} "
+                    "- try an integer feature ID or a ('field', value) tuple"
+                )
+
+            field_features[field].add(value)
+
+        for doc_id, (doc_key, doc) in zip(query, self.docs(query)):
+            indexed = self.corpus.index(doc)
+
+            doc_cooccurrence = dict()
+
+            for field, to_match in field_features.items():
+                cooccurrence = []
+                values = indexed.get(field, [])
+
+                for i, value in enumerate(values):
+                    if value in to_match:
+                        start_window = max(0, i - window_size)
+                        cooccurrence.append(
+                            (value, values[start_window : i + window_size + 1])
+                        )
+
+                doc_cooccurrence[field] = cooccurrence
+
+            yield (doc_key, doc_id, doc_cooccurrence)
+
+    def concordances(self, query, features, window_size, random_sample_size=None):
+        """
+        A utility function that wraps the cooccurrence function to produce
+        text strings instead.
+
+        """
+        for doc_key, doc_id, cooccurrence_windows in self.extract_matching_windows(
+            query, features, window_size, random_sample_size=random_sample_size
+        ):
+            yield doc_key, doc_id, {
+                field: [
+                    " ".join(w for w in window if w is not None)
+                    for _, window in windows
+                ]
+                for field, windows in cooccurrence_windows.items()
+            }
+
+    def sample_bitmap(self, bitmap, random_sample_size):
+        """
+        Sample up to random_sample_size members from bitmap.
+
+        If there are fewer than the sample size members in the bitmap, return
+        a copy of the bitmap.
+
+        Uses the current state of the indexes random number generator to
+        enable repeatable runs.
+
+        """
+
+        b = len(bitmap)
+        if b > random_sample_size:
+            sampled = BitMap(
+                bitmap[i] for i in self.random.sample(range(b), random_sample_size)
+            )
+            return sampled
+
+        else:
+            return bitmap.copy()
+
+    @requires_corpus(corpus.WebRenderableCorpus)
+    def render_docs_html(self, query, random_sample_size=None):
         """
         Return the rendered representation of the docs matching this query.
 
         Optionally take a random sample of documents before rendering.
         """
 
         if random_sample_size is not None:
-            q = len(query)
-            if q > random_sample_size:
-                query = BitMap(
-                    query[i] for i in self.random.sample(range(q), random_sample_size)
-                )
+            query = self.sample_bitmap(query, random_sample_size)
 
         doc_keys = self.convert_query_to_keys(query)
         return self.corpus.render_docs_html(doc_keys)
 
+    @requires_corpus(corpus.TableRenderableCorpus)
+    def render_docs_table(self, query, random_sample_size=None):
+        """
+        Return the rendered representation of the docs matching this query.
+
+        Optionally take a random sample of documents before rendering.
+        """
+
+        if random_sample_size is not None:
+            query = self.sample_bitmap(query, random_sample_size)
+
+        doc_keys = self.convert_query_to_keys(query)
+        return self.corpus.render_docs_table(doc_keys)
+
+    @atomic()
+    def structured_doc_sample(self, docs_per_cluster=100, cluster_ids=None):
+        """
+        Create a sample of documents, using the current clustering as a sampling
+        structure.
+
+        By default 100 documents will be sampled from each cluster - sampling can be
+        disabled by setting docs_per_cluster to 0.
+
+        Optionally specify specific clusters to sample from using `cluster_ids`,
+        otherwise all clusters will be sampled.
+
+        Documents will be sampled from clusters in order of increasing frequency, and
+        will be sampled without replacement.
+
+        Will return a mapping of cluster_ids to sampled documents, and also a map of all
+        clusters for each of those documents.
+
+        """
+        all_clusters = self.top_cluster_features(top_k=0)
+        cluster_order = reversed(all_clusters)
+
+        cluster_ids = set(cluster_ids or self.cluster_ids)
+
+        already_sampled = BitMap()
+        cluster_samples = dict()
+
+        # Per cluster samples
+        for cluster_id, _, _ in cluster_order:
+            if cluster_id in cluster_ids:
+                cluster_docs = self.cluster_docs(cluster_id) - already_sampled
+                if docs_per_cluster > 0:
+                    sample = self.sample_bitmap(cluster_docs, docs_per_cluster)
+                else:
+                    sample = cluster_docs
+                cluster_samples[cluster_id] = sample
+                already_sampled |= sample
+
+        # Clusters for all of the sampled documents.
+        sample_clusters = {
+            cluster_id: c
+            for cluster_id, _, _ in all_clusters
+            if (c := already_sampled & self.cluster_docs(cluster_id))
+        }
+
+        return cluster_samples, sample_clusters
+
+    @atomic()
+    @requires_corpus(corpus.TableRenderableCorpus)
+    def export_document_sample(self, sample_docs, sample_clusters, output_path):
+        """
+        Export the given sample of documents to CSV.
+
+        It is currently assumed that all documents have the same fields.
+
+        This method uses the fields exposed in the table_fields property of
+        the corpus to determine what to export - if a document has additional
+        fields these are silently dropped.
+
+        """
+
+        with open(output_path, "w", encoding="utf-8") as out:
+            table_fields = (
+                ["doc_key", "sampled_cluster"]
+                + self.corpus.table_fields
+                + [f"cluster_{cluster_id}" for cluster_id in sorted(sample_clusters)]
+            )
+
+            writer = csv.DictWriter(
+                out,
+                table_fields,
+                extrasaction="ignore",
+                dialect="excel",
+                quoting=csv.QUOTE_ALL,
+            )
+
+            writer.writeheader()
+
+            for cluster_id, sample_docs in sample_docs.items():
+                write_docs = self.corpus.render_docs_table(
+                    self.convert_query_to_keys(sample_docs)
+                )
+
+                for doc_id, (key, doc) in zip(sample_docs, write_docs):
+                    doc["doc_key"] = key
+                    doc["sampled_cluster"] = cluster_id
+                    for other_cluster_id, cluster_docs in sample_clusters.items():
+                        if doc_id in cluster_docs:
+                            doc[f"cluster_{other_cluster_id}"] = 1
+
+                    writer.writerow(doc)
+
     def indexed_field_summary(self):
         """
         Return a summary tables of the indexed fields.
 
         """
         return list(self.db.execute("select * from field_summary"))
 
@@ -878,60 +1090,77 @@
     @atomic()
     def pivot_clusters_by_query(
         self, query, cluster_ids=None, top_k=20, scoring="jaccard"
     ):
         """
         Sort all clusters and features within clusters by similarity with the probe query.
 
+        This function is optimised to yield top ranking results as early as possible,
+        to enable streaming outputs as soon as they're ready, such as in the web interface.
+
+        Returns:
+
+            Generator of clusters and features sorted by similarity with the
+            associated query.
+
         Args:
             query: the query object as a bitmap of document IDs
             cluster_ids: an optional sequence
             top_k: the number of top features to return in each cluster
-            scoring: The similarity scoring function, currently "jaccard"
-                and "chi_squared" are supported.
+            scoring: The similarity scoring function, currently only "jaccard"
+                is supported.
 
         """
 
         cluster_ids = cluster_ids or [
             r[0]
             for r in self.db.execute(
                 "select cluster_id from cluster order by feature_count desc"
             )
         ]
 
-        if scoring == "jaccard":
-            work = [
-                (self.db_path, query, cluster_id, top_k) for cluster_id in cluster_ids
-            ]
-            pivoted = (
-                r for r in self.pool.map(_pivot_cluster_by_query_jaccard, work) if r[1]
+        jobs = self.pool._max_workers * 2
+        futures = [
+            self.pool.submit(
+                _calculate_query_cluster_cooccurrence,
+                self.db_path,
+                0,
+                query,
+                cluster_ids[i::jobs],
             )
+            for i in range(jobs)
+        ]
+
+        weights = []
+
+        for f in cf.as_completed(futures):
+            weights.extend(f.result()[1])
 
-        elif scoring == "chi_squared":
-            N = list(self.db.execute("select count(*) from doc_key"))[0][0]
-            work = [
-                (self.db_path, query, cluster_id, top_k, N)
-                for cluster_id in cluster_ids
+        process_order = sorted(weights, key=lambda x: x[1], reverse=True)
+
+        if scoring == "jaccard":
+            futures = [
+                self.pool.submit(
+                    _pivot_cluster_features_by_query_jaccard,
+                    self.db_path,
+                    query,
+                    cluster_id,
+                    top_k,
+                    inter,
+                )
+                for cluster_id, _, inter in process_order
             ]
-            pivoted = (
-                r
-                for r in self.pool.map(_pivot_cluster_by_query_chi_squared, work)
-                if r[1]
-            )
 
-        clusters = [
-            (r[0][1], r[0][0], r[1])
-            for r in sorted(
-                pivoted,
-                reverse=True,
-                key=lambda r: r[0],
+        else:
+            raise ValueError(
+                f"{scoring} method is not supported. "
+                "Only jaccard is currently supported."
             )
-        ]
 
-        return clusters
+        return (future.result() for future in futures)
 
     def cluster_features(self, cluster_id, top_k=2**62):
         """
         Returns an impact ordered list of features for the given cluster.
 
         If top_k is specified, only the top_k most frequent features by
         document count are returned in descending order.
@@ -1047,17 +1276,14 @@
 
         cluster_feature - the current cluster: features mapping
         cluster_check_features - mapping of cluster: features to check
             against moving into this cluster. Note that features will
             be removed from this set if they are already in this cluster
             in cluster_feature.
 
-        acceptance_probability is a softening factor, used to prevent
-        cycling between the same states on repeated iteration.
-
         top_k: the number of best scores to keep - the default is to only
             the single best scoring feature.
 
         """
 
         # preflight check:
         missing_clusters = {
@@ -1098,25 +1324,144 @@
                     heapq.heappushpop(best_clusters[feature], (delta, test_cluster))
 
         return {
             key: sorted(feature_scores, reverse=True)
             for key, feature_scores in best_clusters.items()
         }
 
+    def _next_nearest_clusters(
+        self,
+        cluster_feature: dict[int, set[int]],
+        movable_features=None,
+        top_k=1,
+        group_test=True,
+        probe_query=None,
+    ):
+        """
+        Find the approximate next nearest cluster for each feature in this clustering.
+        """
+        cluster_ids = list(cluster_feature.keys())
+        self.random.shuffle(cluster_ids)
+
+        movable_features = movable_features or set.union(*cluster_feature.values())
+
+        # If we're looking for more neighbours, test more batches so that we
+        # spend roughly the same amount of time looking at group tests vs
+        # feature tests.
+        n_batches = math.ceil((len(cluster_ids) * top_k) ** 0.5)
+
+        # Group testing if there are enough batches to be worth while.
+        if group_test and n_batches > 2:
+            cluster_groups = [set(cluster_ids[i::n_batches]) for i in range(n_batches)]
+
+            group_features = {}
+            group_feature_checks = {}
+
+            for group in cluster_groups:
+                group_key = tuple(sorted(group))
+                this_group_features = set.union(
+                    *(cluster_feature[key] for key in group_key)
+                )
+
+                group_features[group_key] = this_group_features
+                group_feature_checks[group_key] = movable_features
+
+                # Handle features in the current group specially by generating specific smaller
+                # groups excluding the self cluster.
+                for cluster_key in group_key:
+                    subgroup_key = tuple(sorted(group - set([cluster_key])))
+                    subgroup_features = (
+                        this_group_features - cluster_feature[cluster_key]
+                    )
+                    subgroup_feature_checks = (
+                        cluster_feature[cluster_key] & movable_features
+                    )
+
+                    group_features[subgroup_key] = subgroup_features
+                    group_feature_checks[subgroup_key] = subgroup_feature_checks
+
+            best_groups = self._calculate_best_feature_moves(
+                group_features,
+                group_feature_checks,
+                probe_query=probe_query,
+                top_k=top_k,
+            )
+
+            cluster_feature_checks = collections.defaultdict(set)
+
+            # Convert best group results into individual cluster checks
+            for feature, groups in best_groups.items():
+                for _, group_key in groups:
+                    for cluster_key in group_key:
+                        cluster_feature_checks[cluster_key].add(feature)
+
+        # The dense testing case is much much simpler, but also much slower!
+        else:
+            cluster_feature_checks = {c: movable_features for c in cluster_ids}
+
+        return self._calculate_best_feature_moves(
+            cluster_feature,
+            cluster_feature_checks,
+            probe_query=probe_query,
+            top_k=top_k,
+        )
+
+    def _create_subcluster(
+        self,
+        cluster_feature,
+        refine_parameters: Optional[dict] = None,
+        threads: int = 8,
+    ):
+        """
+        An extension to _refine_feature_groups that computes many feature_clusterings.
+
+        A small threadpool is created to manage running a couple of the
+        subclusterings in parallel - each required subclustering is performed
+        to completion in turn to ensure data locality.
+
+        """
+
+        refine_parameters = refine_parameters or {}
+
+        with cf.ThreadPoolExecutor(threads) as threadpool:
+            futures = []
+            cluster_order = []
+
+            for cluster_id, features in cluster_feature.items():
+                # TODO: skip small enough clusters.
+                target_clusters = math.ceil(len(features) ** 0.5)
+                refine_parameters["target_clusters"] = target_clusters
+                futures.append(
+                    threadpool.submit(
+                        self._refine_feature_groups,
+                        {cluster_id: features},
+                        **refine_parameters,
+                    )
+                )
+                cluster_order.append(cluster_id)
+
+            subclusters = {
+                cluster_id: f.result()[0]
+                for cluster_id, f in zip(cluster_order, futures)
+            }
+
+        return subclusters
+
     def _refine_feature_groups(
         self,
         cluster_feature: dict[int, set[int]],
         iterations: int = 10,
         group_test: bool = True,
         minimum_cluster_features: int = 1,
         pinned_features: Optional[Iterable[int]] = None,
         probe_query: Optional[AbstractBitMap] = None,
         target_clusters: Optional[int] = None,
-        tolerance: float = 0.01,
-        acceptance_probability: float = 0.75,
+        tolerance: float = 0.05,
+        acceptance_probability: float = 0.9,
+        top_k: int = 2,
     ) -> tuple[dict[int, set[int]], set[int]]:
         """
         Low level function for iteratively refining a feature clustering.
 
         cluster_features is a mapping from a cluster_key to a set of feature_ids.
 
         This is most useful if you want to explore specific clustering
@@ -1139,21 +1484,26 @@
         there are more clusters, the clusters that contribute least to the
         objective will be dissolved. Dissolves will be conducted evenly per
         iteration, rather than all at once. If there are fewer clusters than
         target, new clusters will be created and filled randomly.
 
         tolerance: specifies a termination tolerance. If fewer than
         tolerance * total_features features move in an iteration, terminate
-        early. The default is set at 0.01, or 1% - the model is considered
-        converged if less than 1% of the features have moved during an
+        early. The default is set at 0.05 - the model is considered
+        converged if less than 5% of the features have moved during an
         iteration.
 
         acceptance_probability: the probability a move that is estimated to
-            improve the score will be accepted.
+        improve the score will be accepted. This interacts with the top_k
+        parameter - the top_k possible moves will be processed in order from
+        best move to worst move. A lower acceptance_probability and a larger
+        top_k result in less greedy exploration of the solution space.
 
+        top_k: the number of nearest neighbour clusters to consider as move
+        candidates.
         """
 
         target_clusters = target_clusters or len(cluster_feature)
 
         # If cluster_feature is empty, return immediately
         if not len(cluster_feature.keys()):
             return cluster_feature, set()
@@ -1280,15 +1630,15 @@
             current_cluster_scores = self._measure_feature_cluster_contributions(
                 cluster_feature, probe_query=probe_query
             )
 
             total_objective = sum(r[2] for r in current_cluster_scores.values())
 
             self.logger.info(
-                f"Iteration {iteration}, current objective: {total_objective}"
+                f"Iteration {iteration + 1}, current objective: {total_objective}"
             )
 
             # Dissolve target low objective clusters for this iteration
             if dissolve_clusters:
                 n_dissolve = min(dissolve_clusters, dissolve_per_iteration)
                 dissolve_clusters -= n_dissolve
                 dissolve_cluster_ids = set(
@@ -1299,76 +1649,25 @@
                 )
                 self.logger.info(
                     f"Dissolving {len(dissolve_cluster_ids)} low objective clusters"
                 )
             else:
                 dissolve_cluster_ids = set()
 
-            assigned_cluster_ids -= dissolve_cluster_ids
-
-            # Group testing for which specific cluster to check against. Note
-            # that features are not tested against the group containing their
-            # current cluster.
-
-            # Start by generating the randomised cluster groups, accounting
-            # for the dissolving clusters
-            cluster_ids = list(current_cluster_scores.keys() - dissolve_cluster_ids)
-            self.random.shuffle(cluster_ids)
-
-            n_batches = math.ceil(len(cluster_ids) ** 0.5)
-
-            if group_test and n_batches > 2:
-                cluster_groups = [
-                    set(cluster_ids[i::n_batches]) for i in range(n_batches)
-                ]
-
-                group_features = {}
-                group_feature_checks = {}
-
-                for group in cluster_groups:
-                    group_key = tuple(sorted(group))
-                    this_group_features = set.union(
-                        *(cluster_feature[key] for key in group_key)
-                    )
-
-                    group_features[group_key] = this_group_features
-                    group_feature_checks[group_key] = movable_features
-
-                    # Handle features in the current group specially by generating specific smaller
-                    # groups excluding the self cluster.
-                    for cluster_key in group_key:
-                        subgroup_key = tuple(sorted(group - set([cluster_key])))
-                        subgroup_features = (
-                            this_group_features - cluster_feature[cluster_key]
-                        )
-                        subgroup_feature_checks = (
-                            cluster_feature[cluster_key] - pinned_features
-                        )
-
-                        group_features[subgroup_key] = subgroup_features
-                        group_feature_checks[subgroup_key] = subgroup_feature_checks
-
-                best_groups = self._calculate_best_feature_moves(
-                    group_features, group_feature_checks, probe_query=probe_query
-                )
-
-                cluster_feature_checks = collections.defaultdict(set)
-
-                # Convert best group results into individual cluster checks
-                for feature, groups in best_groups.items():
-                    for _, group_key in groups:
-                        for cluster_key in group_key:
-                            cluster_feature_checks[cluster_key].add(feature)
+            for cluster_id in dissolve_cluster_ids:
+                del cluster_feature[cluster_id]
 
-            else:
-                cluster_feature_checks = {c: movable_features for c in cluster_ids}
+            assigned_cluster_ids -= dissolve_cluster_ids
 
-            best_feature_clusters = self._calculate_best_feature_moves(
+            # Calculate possible moves given this clustering
+            best_feature_clusters = self._next_nearest_clusters(
                 cluster_feature,
-                cluster_feature_checks,
+                top_k=top_k,
+                group_test=group_test,
+                movable_features=movable_features,
                 probe_query=probe_query,
             )
 
             moved_features = 0
             features_with_possible_improvements = 0
             changed_clusters = set()
 
@@ -1376,67 +1675,72 @@
                 features, deltas, _ = current_cluster_scores[current_cluster]
 
                 # When a cluster is dissolved, just reassign to the best cluster
                 # immediately.
                 if current_cluster in dissolve_cluster_ids:
                     for feature_id, current_delta in zip(features, deltas):
                         new_cluster = best_feature_clusters[feature_id][0][1]
-                        cluster_feature[current_cluster].discard(feature_id)
                         cluster_feature[new_cluster].add(feature_id)
                         feature_cluster[feature_id] = new_cluster
 
                         changed_clusters.add(new_cluster)
 
                 else:
                     for feature_id, current_delta in zip(features, deltas):
                         if feature_id in pinned_features:
                             continue
 
                         comparison_delta, comparison_cluster = best_feature_clusters[
                             feature_id
                         ][0]
 
-                        if (
-                            comparison_delta >= current_delta
-                            and self.random.random() < acceptance_probability
-                        ):
-                            cluster_feature[current_cluster].discard(feature_id)
-                            cluster_feature[comparison_cluster].add(feature_id)
-                            feature_cluster[feature_id] = comparison_cluster
+                        comparisons = best_feature_clusters[feature_id]
+
+                        for comparison_delta, comparison_cluster in comparisons:
+                            # Because the comparisons are sorted in descending
+                            # order, there's no point checking anything
+                            # else.
+                            if comparison_delta <= current_delta:
+                                break
+
+                            elif self.random.random() < acceptance_probability:
+                                cluster_feature[current_cluster].discard(feature_id)
+                                cluster_feature[comparison_cluster].add(feature_id)
+                                feature_cluster[feature_id] = comparison_cluster
 
-                            changed_clusters.add(comparison_cluster)
+                                changed_clusters.add(comparison_cluster)
 
-                            moved_features += 1
+                                moved_features += 1
+                                break
 
             for cluster_id in dissolve_cluster_ids:
                 del current_cluster_scores[cluster_id]
-                del cluster_feature[cluster_id]
+
+            self.logger.info(
+                f"Finished iteration {iteration + 1}/{iterations}, changed "
+                f"{len(changed_clusters)} clusters, moved {moved_features} features."
+            )
 
             if not dissolve_cluster_ids:
                 if (moved_features / len(movable_features)) < tolerance:
                     self.logger.info(
                         "Terminating refinement due to small number of feature moves."
                     )
                     break
 
-            self.logger.info(
-                f"Finished iteration {iteration + 1}/{iterations}, changed "
-                f"{len(changed_clusters)} clusters, moved {moved_features} features."
-            )
-
         return cluster_feature, new_cluster_ids
 
     @atomic()
     def refine_clusters(
         self,
         iterations: int = 10,
         cluster_ids: Optional[Sequence[int]] = None,
         target_clusters: Optional[int] = None,
         minimum_cluster_features: int = 1,
-        tolerance: float = 0.01,
+        tolerance: float = 0.05,
     ):
         """
         Refine the feature clusters for the current model.
 
         Optionally provide a list of specific cluster_ids to refine.
 
         If target_clusters is larger than the current number of clusters in
@@ -1544,15 +1848,15 @@
 
         """
 
         # First update the feature counts, and remove empty clusters
         self.db.execute(
             """
             update cluster set feature_count = (
-                select count(*) 
+                select count(*)
                 from feature_cluster fc
                 where fc.cluster_id=cluster.cluster_id
             )
             where cluster_id in (select cluster_id from changed_cluster)
             """
         )
 
@@ -1588,324 +1892,274 @@
                 """,
                 (len(query), weight, query, cluster_id),
             )
 
         self.db.execute("delete from cluster where feature_count = 0")
         self.db.execute("delete from changed_cluster")
 
+    @atomic()
+    def create_cluster_cooccurrence_graph(self, top_k=5, include_field_in_label=True):
+        """
+        Create a networkx graph showing cluster-cluster relationships.
+
+        In this graph each cluster of features is a node, and the edges
+        between nodes show cluster overlap. Edges are weighted by the jaccard
+        similarity of documents belonging to each cluster.
 
-def _index_docs(corpus, doc_ids, doc_keys, temp_db_path, skipgram_window_size):
-    """Index all of the given docs into temp_db_path."""
+        Nodes are labelled with the top_k features from that node.
 
-    local_db = db_utilities.connect_sqlite(temp_db_path)
+        """
 
-    try:
-        local_db.execute("begin")
+        graph = nx.Graph()
+        clusters = self.top_cluster_features(top_k=top_k)
+        # First add basic node information
+        for cluster_id, doc_count, top_features in clusters:
+            if include_field_in_label:
+                label = ", ".join(
+                    f"{field}:{value}" for _, field, value, _ in top_features
+                )
+            else:
+                label = ", ".join(value for _, field, value, _ in top_features)
+
+            graph.add_node(cluster_id, document_count=doc_count, label=label)
+
+        # The compute all the pairwise cluster details, in parallel.
+        futures = set()
 
-        # This is {field: {value: doc_ids, value2: doc_ids}}
-        batch = collections.defaultdict(lambda: collections.defaultdict(BitMap))
-        # The structure is (distance, field, value_a, value_b: count)
-        skipgram_counts = [
-            collections.defaultdict(
-                lambda: collections.defaultdict(collections.Counter)
+        for i, (cluster_id, _, _) in enumerate(clusters):
+            query = self.cluster_docs(cluster_id)
+            comparison_clusters = [c[0] for c in clusters[i + 1 :]]
+            futures.add(
+                self.pool.submit(
+                    _calculate_query_cluster_cooccurrence,
+                    self.db_path,
+                    cluster_id,
+                    query,
+                    comparison_clusters,
+                )
             )
-            for _ in range(skipgram_window_size)
-        ]
 
-        docs = corpus.docs(doc_keys=doc_keys)
+        for future in cf.as_completed(futures):
+            cluster_id, weights = future.result()
 
-        for doc_id, (_, doc) in zip(doc_ids, docs):
-            features = corpus.index(doc)
-            for field, values in features.items():
-                # Only find bigrams in sequences - non sequence types such as
-                # a set don't make sense to do this.
-                if skipgram_window_size > 0 and isinstance(
-                    values, collections.abc.Sequence
-                ):
-                    bigrams = utilities.long_distance_bigrams(
-                        values, skipgram_window_size
-                    )
-                    for item_a, item_b, distance in bigrams:
-                        skipgram_counts[distance - 1][field][item_a][item_b] += 1
+            for o_cluster, sim, inter in weights:
+                graph.add_edge(cluster_id, o_cluster, weight=sim)
 
-                set_values = set(values)
+        return graph
 
-                for value in set_values:
-                    batch[field][value].add(doc_id)
 
-        local_db.execute(
-            """
-            CREATE table inverted_index_segment(
-                field text,
-                value,
-                docs_count,
-                doc_ids roaring_bitmap,
-                primary key (field, value)
-            ) without rowid
-            """
-        )
-        for field, values in batch.items():
-            local_db.executemany(
-                "insert into inverted_index_segment values(?, ?, ?, ?)",
-                (
-                    (field, value, len(doc_ids), doc_ids)
-                    for value, doc_ids in values.items()
-                    if value is not None
-                ),
-            )
+def _index_docs(
+    corpus, doc_ids, doc_keys, temp_db_path, position_window_size, write_lock
+):
+    """
+    Index all of the given docs into temp_db_path.
 
-        local_db.execute(
-            """
-            CREATE table skipgram_count(
-                field text,
-                value_a,
-                value_b,
-                distance integer,
-                docs_count integer,
-                primary key (field, value_a, value_b, distance)
-            )
-            """
+    position_window_size has two modes:
+
+    0 - disabled, no position information will be recorded.
+    > 0 - approximate position windows of the given half width will be
+      created. Coocurrence of values can be found exactly up to 2 *
+      position_window_size - note that edge effects mean that the position
+      windows will miss cooccurence across window boundaries which is why the
+      limit is 2*position_window_size not position_window_size. Note that
+      setting this to 1 computes an exact position index.
+
+    """
+
+    local_db = db_utilities.connect_sqlite(temp_db_path)
+
+    try:
+        if len(doc_ids) != len(doc_keys):
+            raise ValueError("There must be exactly one doc_id for every doc_key.")
+
+        # Mapping of {field: {value: (BitMap(), BitMap())}}
+        # One bitmap for document occurrence, the other other for recording
+        # positional information.
+        batch = collections.defaultdict(
+            lambda: collections.defaultdict(lambda: (BitMap(), BitMap()))
         )
 
-        for i, f in enumerate(skipgram_counts):
-            distance = i + 1
-            for field, item_as in f.items():
-                for item_a, item_bs in item_as.items():
-                    local_db.executemany(
-                        "INSERT into skipgram_count values(?, ?, ?, ?, ?)",
-                        (
-                            (field, item_a, item_b, distance, c)
-                            for item_b, c in sorted(item_bs.items())
-                        ),
-                    )
+        # Mapping of fields -> position ends for each document. Note that
+        # documents with an empty field present are dropped at this stage.
+        field_doc_position = collections.defaultdict(lambda: (BitMap(), BitMap([0])))
 
-        local_db.execute("commit")
+        docs = corpus.docs(doc_keys=doc_keys)
 
-    finally:
-        local_db.close()
+        first_doc_id = doc_ids[0]
+        last_doc_id = doc_ids[-1]
 
-    return temp_db_path, 0
+        for doc_id, (_, doc) in zip(doc_ids, docs):
+            features = corpus.index(doc)
 
+            for field, values in features.items():
+                # Only record position information if there is a
+                # position_window_size set, and the field is an ordered
+                # sequence type.
+                if position_window_size and isinstance(
+                    values, collections.abc.Sequence
+                ):
+                    batch_position = field_doc_position[field][1][-1]
 
-def _merge_indices(target_db_path, level, *to_merge):
-    """Merge the given indices into target_db_path."""
+                    # Make sure this is initilaised - values can be non-empty
+                    # but only contain sentinels that generate no positions.
+                    position = None
 
-    target_db = db_utilities.connect_sqlite(target_db_path)
+                    position_values = utilities.approximate_positions_with_sentinels(
+                        values, position_window_size
+                    )
 
-    try:
-        target_db.execute("begin")
+                    for position, value in position_values:
+                        batch[field][value][1].add(position + batch_position)
 
-        for i, db in enumerate(to_merge):
-            target_db.execute(f"attach ? as to_merge_{i}", [db])
+                    # Record offset for the start of the next positions in this
+                    # field for this batch.
+                    if position is None:
+                        continue
+                    else:
+                        field_doc_position[field][0].add(doc_id)
+                        field_doc_position[field][1].add(position + batch_position + 1)
 
-        target_db.execute(
-            """
-            CREATE table inverted_index_segment(
-                field text,
-                value,
-                docs_count,
-                doc_ids roaring_bitmap,
-                primary key (field, value)
-            ) without rowid
-            """
-        )
+                set_values = set(values)
+                set_values.discard(None)
 
-        union_all = "\nunion all\n".join(
-            f"SELECT * from to_merge_{i}.inverted_index_segment"
-            for i in range(len(to_merge))
-        )
+                for value in set_values:
+                    batch[field][value][0].add(doc_id)
 
-        target_db.execute(
-            f"""
-            INSERT into inverted_index_segment
-                select
-                    field,
+        with write_lock:
+            local_db.execute("pragma synchronous=0")
+            local_db.execute("begin")
+            local_db.execute(
+                """
+                CREATE table if not exists inverted_index_segment(
+                    field text,
                     value,
-                    sum(docs_count),
-                    roaring_union(doc_ids)
-                from (
-                    {union_all}
+                    docs_count,
+                    doc_ids roaring_bitmap,
+                    position_count,
+                    positions roaring_bitmap,
+                    first_doc_id
                 )
-                group by field, value
-            """
-        )
-
-        union_all = "\nunion all\n".join(
-            f"SELECT * from to_merge_{i}.skipgram_count" for i in range(len(to_merge))
-        )
-
-        target_db.execute(
-            """
-            CREATE table skipgram_count(
-                field text,
-                value_a,
-                value_b,
-                distance integer,
-                docs_count integer,
-                primary key (field, value_a, value_b, distance)
+                """
             )
-            """
-        )
 
-        target_db.execute(
-            f"""
-            INSERT into skipgram_count
-                select
+            local_db.execute(
+                """
+                CREATE table if not exists batch_position(
                     field,
-                    value_a,
-                    value_b,
-                    distance,
-                    sum(docs_count)
-                from (
-                    {union_all}
+                    first_doc_id,
+                    last_doc_id,
+                    docs_count,
+                    doc_ids roaring_bitmap,
+                    doc_position_starts roaring_bitmap,
+                    primary key (field, first_doc_id)
                 )
-                group by 1, 2, 3, 4
-            """
-        )
-
-        target_db.execute("commit")
-
-    finally:
-        target_db.close()
-        for path in to_merge:
-            os.remove(path)
-
-    return target_db_path, level
+                """
+            )
 
+            for field, (batch_doc_ids, position_starts) in field_doc_position.items():
+                local_db.execute(
+                    "insert into batch_position values(?, ?, ?, ?, ?, ?)",
+                    (
+                        field,
+                        first_doc_id,
+                        last_doc_id,
+                        len(batch_doc_ids),
+                        batch_doc_ids,
+                        position_starts[1:],
+                    ),
+                )
 
-def _pivot_cluster_by_query_jaccard(args):
-    index_db_path, query, cluster_id, top_k = args
-    index = Index(index_db_path)
+            # Ensure we do all the inserts in sorted order as far as possible
+            field_order = sorted(batch.keys())
 
-    results = [(0, -1, "", "")] * top_k
+            for field in field_order:
+                values = batch[field]
+                value_order = sorted(v for v in values if v is not None)
 
-    q = len(query)
+                local_db.executemany(
+                    "insert into inverted_index_segment values(?, ?, ?, ?, ?, ?, ?)",
+                    (
+                        (
+                            field,
+                            value,
+                            len(values[value][0]),
+                            values[value][0],
+                            len(values[value][1]),
+                            values[value][1] or None,
+                            first_doc_id,
+                        )
+                        for value in value_order
+                    ),
+                )
 
-    search_upper = index.db.execute(
-        """
-        select
-            feature_cluster.feature_id,
-            field,
-            value,
-            feature_cluster.docs_count,
-            doc_ids
-        from feature_cluster
-        inner join inverted_index using(feature_id)
-        where cluster_id = ?
-            and feature_cluster.docs_count >= ?
-        order by feature_cluster.docs_count
-        """,
-        [cluster_id, q],
-    )
+            local_db.execute("commit")
 
-    for feature_id, field, value, docs_count, docs in search_upper:
-        # Early break if the length threshold can't be reached.
-        if q / docs_count <= results[0][0]:
-            break
+    finally:
+        local_db.close()
 
-        heapq.heappushpop(
-            results, (query.jaccard_index(docs), feature_id, field, value)
-        )
+    return temp_db_path
 
-    search_upper = index.db.execute(
-        """
-        select
-            feature_cluster.feature_id,
-            field,
-            value,
-            feature_cluster.docs_count,
-            doc_ids
-        from feature_cluster
-        inner join inverted_index using(feature_id)
-        where cluster_id = ?
-            and feature_cluster.docs_count < ?
-        order by feature_cluster.docs_count desc
-        """,
-        [cluster_id, q],
-    )
 
-    for feature_id, field, value, docs_count, docs in search_upper:
-        # Early break if the length threshold can't be reached.
-        if docs_count / q <= results[0][0]:
-            break
+def _calculate_query_cluster_cooccurrence(index_db_path, key, query, cluster_ids):
+    idx = Index(index_db_path)
 
-        heapq.heappushpop(
-            results, (query.jaccard_index(docs), feature_id, field, value)
-        )
+    try:
+        idx.db.execute("begin")
 
-    results = sorted(
-        ((*r[1:], r[0]) for r in results if r[0] > 0), reverse=True, key=lambda r: r[3]
-    )
+        weights = []
 
-    # Finally compute the similarity of the query with the cluster_union.
-    cluster_union = list(
-        index.db.execute(
-            "select doc_ids from cluster where cluster_id = ?", [cluster_id]
-        )
-    )[0][0]
+        for cluster_id in cluster_ids:
+            cluster_docs = idx.cluster_docs(cluster_id)
+            inter = query.intersection_cardinality(cluster_docs)
 
-    similarity = query.jaccard_index(cluster_union)
+            if inter:
+                sim = query.jaccard_index(cluster_docs)
+                weights.append((cluster_id, sim, inter))
 
-    index.close()
+    finally:
+        idx.db.execute("commit")
 
-    return (similarity, cluster_id), results
+    return key, weights
 
 
-def _pivot_cluster_by_query_chi_squared(args):
-    index_db_path, query, cluster_id, top_k, N = args
-    index = Index(index_db_path)
+def _pivot_cluster_features_by_query_jaccard(
+    index_db_path, query, cluster_id, top_k, cluster_inter
+):
+    idx = Index(index_db_path)
 
     results = [(0, -1, "", "")] * top_k
 
     q = len(query)
 
-    search = index.db.execute(
-        """
-        select
-            feature_cluster.feature_id,
-            field,
-            value,
-            feature_cluster.docs_count,
-            doc_ids
-        from feature_cluster
-        inner join inverted_index using(feature_id)
-        where cluster_id = ?
-        """,
-        [cluster_id],
+    features = (
+        (min(f[-1], cluster_inter) / (q + f[-1] - min(f[-1], cluster_inter)), *f)
+        for f in idx.cluster_features(cluster_id)
     )
 
-    for feature_id, field, value, docs_count, docs in search:
-        f = docs_count
-
-        # These are the cells in the 2x2 contingency table
-        A = query.intersection_cardinality(docs)
-        B = q - A
-        C = f - A
-        D = N - q - f + A
+    search_order = sorted(features, reverse=True)
 
-        score = (((A * D) - (B * C)) ** 2) * N / ((A + B) * (C + D) * (B + D) * (A + C))
+    # TODO: find further ways to accelerate this - it seems like most features
+    # end up being checked when the similarity is low.
+    for max_threshold, f_id, field, value, docs_count in search_order:
+        # Early break if the length threshold can't be reached.
+        if max_threshold < results[0][0]:
+            break
 
-        heapq.heappushpop(results, (score, feature_id, field, value))
+        heapq.heappushpop(results, (query.jaccard_index(idx[f_id]), f_id, field, value))
 
     results = sorted(
-        ((*r[1:], r[0]) for r in results if r[1] >= 0), reverse=True, key=lambda r: r[3]
+        ((*r[1:], r[0]) for r in results if r[0] > 0), reverse=True, key=lambda r: r[3]
     )
 
-    # Finally compute the similarity of the query with the cluster_union.
-    cluster_union = list(
-        index.db.execute(
-            "select doc_ids from cluster where cluster_id = ?", [cluster_id]
-        )
-    )[0][0]
-
-    similarity = results[0][-1]
+    # Finally compute the similarity of the query with the cluster.
+    similarity = query.jaccard_index(idx.cluster_docs(cluster_id))
 
-    index.close()
+    idx.close()
 
-    return (similarity, cluster_id), results
+    return cluster_id, similarity, results
 
 
 def measure_feature_contribution_to_cluster(
     index_db_path,
     group_key,
     feature_group: set[int],
     probe_query: Optional[AbstractBitMap],
@@ -1955,15 +2209,15 @@
             covered_twice |= cluster_union & docs
             # All docs now covered
             cluster_union |= docs
 
         only_once = cluster_union - covered_twice
 
         c = len(cluster_union)
-        objective = hits / (c + n_features)
+        objective = hits / (c + n_features) - (hits / (hits + n_features))
 
         # SECOND PHASE: compute the incremental change in objective from removing each
         # feature (alone) from the current cluster.
         # Note: using an array to only manage two objects worth of de/serialisation
 
         feature_array = array.array("q", feature_group)
         delta_array = array.array("d", (0 for _ in feature_group))
@@ -1984,15 +2238,17 @@
             old_c = c - only_once_hits
 
             # Check if this feature intersects with any other feature in this cluster
             intersects_with_other_feature = only_once_hits < feature_hits
 
             # It's okay for the cluster to become empty - we'll just prune it.
             if old_c and intersects_with_other_feature:
-                old_objective = old_hits / (old_c + (n_features - 1))
+                old_objective = old_hits / (old_c + (n_features - 1)) - (
+                    old_hits / (old_hits + n_features - 1)
+                )
 
                 delta = objective - old_objective
 
             # Penalises features that don't intersect with other features in the cluster.
             elif old_c:
                 delta = -1
             # If it would otherwise be a singleton cluster, just mark it as no change
@@ -2048,15 +2304,15 @@
 
             hits += len(docs)
 
             # All docs now covered
             cluster_union |= docs
 
         c = len(cluster_union)
-        objective = hits / (c + n_features)
+        objective = hits / (c + n_features) - (hits / (hits + n_features))
 
         # PHASE 2: Incremental delta from adding new features to the cluster.
         # Note: using an array to only manage two objects worth of de/serialisation
         feature_array = array.array("q", sorted(add_features))
         delta_array = array.array("d", (0 for _ in feature_array))
 
         # All tokens that are adds (not already in the cluster)
@@ -2067,15 +2323,17 @@
                 docs &= probe_query
 
             feature_hits = len(docs)
 
             if docs.intersect(cluster_union):
                 new_hits = hits + feature_hits
                 new_c = docs.union_cardinality(cluster_union)
-                new_objective = new_hits / (new_c + (n_features + 1))
+                new_objective = new_hits / (new_c + (n_features + 1)) - (
+                    new_hits / (new_hits + n_features + 1)
+                )
 
                 delta = new_objective - objective
 
             # If the feature doesn't intersect with the cluster at all,
             # give it a bad delta.
             else:
                 delta = -1
@@ -2090,19 +2348,21 @@
 
 
 def _union_query(args):
     index_db_path, query_key, feature_ids = args
 
     try:
         index = Index(index_db_path)
+        index.db.execute("begin")
         query = BitMap()
         weight = 0
 
         for feature_id in feature_ids:
             docs = index[feature_id]
             query |= docs
             weight += len(docs)
 
     finally:
+        index.db.execute("commit")
         index.close()
 
     return query_key, query, weight
```

### Comparing `hyperreal-0.3.1/hyperreal/server.py` & `hyperreal-0.4.0/hyperreal/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,19 +90,21 @@
             filter_cluster_id = int(filter_cluster_id)
             if query:
                 query &= cherrypy.request.index.cluster_docs(filter_cluster_id)
             else:
                 query = cherrypy.request.index.cluster_docs(filter_cluster_id)
 
         if query:
-            sorted_features = cherrypy.request.index.pivot_clusters_by_query(
-                query,
-                cluster_ids=[cluster_id],
-                top_k=n_features,
-                scoring=scoring,
+            sorted_features = list(
+                cherrypy.request.index.pivot_clusters_by_query(
+                    query,
+                    cluster_ids=[cluster_id],
+                    top_k=n_features,
+                    scoring=scoring,
+                )
             )
 
             # Make sure that there are actually matching features.
             if sorted_features:
                 features = sorted_features[0][-1]
 
             # Make sure to only show the intersection of the requested feature with
@@ -113,15 +115,15 @@
 
         else:
             retrieve_docs = cherrypy.request.index.cluster_docs(cluster_id)
             visible_features = None
 
         # Retrieve matching documents if we have a corpus to render them.
         if cherrypy.request.index.corpus is not None:
-            rendered_docs = cherrypy.request.index.render_docs(
+            rendered_docs = cherrypy.request.index.render_docs_html(
                 retrieve_docs, random_sample_size=int(exemplar_docs)
             )
 
         total_docs = len(retrieve_docs)
 
         pinned = int(cluster_id in cherrypy.request.index.pinned_cluster_ids)
 
@@ -266,88 +268,73 @@
 @cherrypy.tools.cleanup_index()
 @cherrypy.tools.lookup_index()
 class Index:
     cluster = ClusterOverview()
     feature = FeatureOverview()
 
     @cherrypy.expose
+    @cherrypy.config(**{"response.stream": True})
     def index(
         self,
         index_id,
         feature_id=None,
         cluster_id=None,
         exemplar_docs="5",
         top_k_features="40",
         scoring="jaccard",
     ):
         template = templates.get_template("index.html")
 
         rendered_docs = []
+        total_docs = 0
+        query = None
         highlight_cluster_id = None
         highlight_feature_id = None
 
         # Redirect to the index overview page to create a new model if no
         # index has been created.
         if not cherrypy.request.index.cluster_ids:
             raise cherrypy.HTTPRedirect(f"/index/{index_id}/details")
 
         if feature_id is not None:
             query = cherrypy.request.index[int(feature_id)]
-            clusters = cherrypy.request.index.pivot_clusters_by_query(
-                query, scoring=scoring, top_k=int(top_k_features)
-            )
-
-            if cherrypy.request.index.corpus is not None:
-                rendered_docs = cherrypy.request.index.render_docs(
-                    query, random_sample_size=int(exemplar_docs)
-                )
-
-            total_docs = len(query)
             highlight_feature_id = int(feature_id)
 
-            visible_features = [
-                feature[0] for _, _, features in clusters for feature in features
-            ]
-
         elif cluster_id is not None:
             query = cherrypy.request.index.cluster_docs(int(cluster_id))
+            highlight_cluster_id = int(cluster_id)
+
+        if query:
             clusters = cherrypy.request.index.pivot_clusters_by_query(
                 query, scoring=scoring, top_k=int(top_k_features)
             )
 
             if cherrypy.request.index.corpus is not None:
-                rendered_docs = cherrypy.request.index.render_docs(
+                rendered_docs = cherrypy.request.index.render_docs_html(
                     query, random_sample_size=int(exemplar_docs)
                 )
 
             total_docs = len(query)
-            highlight_cluster_id = int(cluster_id)
-
-            visible_features = [
-                feature[0] for _, _, features in clusters for feature in features
-            ]
 
         else:
             clusters = cherrypy.request.index.top_cluster_features(
                 top_k=int(top_k_features)
             )
             total_docs = 0
-            visible_features = None
 
-        return template.render(
+        return template.generate(
             clusters=clusters,
             total_docs=total_docs,
             rendered_docs=rendered_docs,
             # Design note: might be worth letting templates grab the request
             # context, and avoid passing this around for everything that
             # needs it?
             index_id=index_id,
             highlight_feature_id=highlight_feature_id,
             highlight_cluster_id=highlight_cluster_id,
-            visible_features=visible_features,
         )
 
     @cherrypy.expose
     def details(self, index_id):
         """
         Show the details of the index, including indexed fields and associated cardinalities.
```

### Comparing `hyperreal-0.3.1/hyperreal/templates/base.html` & `hyperreal-0.4.0/hyperreal/templates/base.html`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.1/hyperreal/templates/cluster.html` & `hyperreal-0.4.0/hyperreal/templates/cluster.html`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.1/hyperreal/templates/details.html` & `hyperreal-0.4.0/hyperreal/templates/details.html`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.1/hyperreal/templates/index.html` & `hyperreal-0.4.0/hyperreal/templates/index.html`

 * *Files 15% similar despite different names*

```diff
@@ -8,66 +8,41 @@
     <li><a href="/index/{{ index_id }}/details">Index Details</a></li>
     <li><a href="/index/{{ index_id }}">Model Overview</a></li>
     <li><a href="/index/{{ index_id }}/export_clusters">Export Clusters</a></li>
 {% endblock %}
 
 {% block content %}
 <details>
-    <summary>Edit Clusters</summary>
-    <form method="post" action="/index/{{ index_id }}/cluster/delete">
-        <label for="cluster_selection">Choose clusters:</label>
-        <select name="cluster_id" id="cluster_selection" multiple>
-            {% for cluster_id, _, features in clusters %}
-            <option value="{{ cluster_id }}">
-                {% for feature_id, field, value, count in features %}
-                {{ field }}: {{ value }}
-                {% endfor %}
-            </option>
-            {% endfor %}
-        </select>
+    <summary>Edit Selected Clusters</summary>
+    <form method="post" id="cluster_edit" action="/index/{{ index_id }}/cluster/delete">
         <input type="hidden" name="return_to" value="model">
         <label for="target_clusters">Refine selection into how many clusters:</label>
-        <input id="target_clusters" name="target_clusters" type="number" />
+        <input id="target_clusters" name="target_clusters" type="number">
         <button type="submit" formaction="/index/{{ index_id }}/cluster/refine" method="post">Refine Selected Clusters</button>
         <br>
         <button type="submit">Delete Clusters 🗑️</button>
         <button type="submit" formaction="/index/{{ index_id }}/cluster/merge" method="post">Merge Clusters</button>
     </form>
-
-    {% if visible_features %}
-    <form method="post" action="/index/{{ index_id }}/cluster/create">
-        {% for feature_id in visible_features %}
-        <input type="hidden" name="feature_id" value={{ feature_id }}>
-        {% endfor %}
-        <button type="submit">Create New Cluster From All Visible Features</button>
-    </form>
-    {% endif %}
 </details>
 
-<ul class="cluster-list">
-
-    {% for cluster_id, cluster_score, features in clusters[:1] %}
-        <li>
-            {{ render_cluster(index_id, cluster_id, features, cluster_score, highlight_cluster_id, highlight_feature_id) }}
-        </li>
-    {% endfor %}
 
+<ul class="cluster-list">
     {% if rendered_docs %}
     <li>
         <div class="cluster-header">
             {% if rendered_docs|length < total_docs %}Sample of {{ total_docs }} documents{% else %}All {{ total_docs }} matching documents.{% endif %}
         </div>
         <ul class="doc-list">
             {% for doc_id, doc in rendered_docs %}
             <li>{{ doc }}</li>
             {% endfor %}
         </ul>
     </li>
     {% endif %}
 
-    {% for cluster_id, cluster_score, features in clusters[1:] %}
+    {% for cluster_id, cluster_score, features in clusters %}
     <li>
         {{ render_cluster(index_id, cluster_id, features, cluster_score, highlight_cluster_id, highlight_feature_id) }}
     </li>
     {% endfor %}
 </ul>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,31 +1,20 @@
 {% extends "base.html" %} {% from 'macros.html' import render_cluster %} {%
 block title %}Feature Clustering{% endblock %} {% block nav %}
 Index_Details
 Model_Overview
 Export_Clusters
-{% endblock %} {% block content %}  Edit Clusters
-{% for cluster_id, _, features in clusters %}
-{% for feature_id, field, value, count in features %} {{ field }}: {{ value }}
-{% endfor %}
-{% endfor %}
-  Refine selection into how many clusters: [Unknown INPUT type] Refine Selected
+{% endblock %} {% block content %}  Edit Selected Clusters
+ Refine selection into how many clusters: [Unknown INPUT type] Refine Selected
 Clusters
 Delete Clusters ðï¸ Merge Clusters
-{% if visible_features %}
-{% for feature_id in visible_features %}
-}> {% endfor %} Create New Cluster From All Visible Features
-{% endif %}
-    * {% for cluster_id, cluster_score, features in clusters[:1] %}
-    * {{ render_cluster(index_id, cluster_id, features, cluster_score,
-      highlight_cluster_id, highlight_feature_id) }}
-    * {% endfor %} {% if rendered_docs %}
+    * {% if rendered_docs %}
     * {% if rendered_docs|length < total_docs %}Sample of {{ total_docs }}
       documents{% else %}All {{ total_docs }} matching documents.{% endif %}
           o {% for doc_id, doc in rendered_docs %}
           o {{ doc }}
           o {% endfor %}
-    * {% endif %} {% for cluster_id, cluster_score, features in clusters[1:] %}
+    * {% endif %} {% for cluster_id, cluster_score, features in clusters %}
     * {{ render_cluster(index_id, cluster_id, features, cluster_score,
       highlight_cluster_id, highlight_feature_id) }}
     * {% endfor %}
 {% endblock %}
```

### Comparing `hyperreal-0.3.1/hyperreal/templates/macros.html` & `hyperreal-0.4.0/hyperreal/templates/macros.html`

 * *Files 16% similar despite different names*

```diff
@@ -22,20 +22,23 @@
             {{ render_feature(index_id, cluster_id, feature_id, field, value, score, context, highlight_feature_id=highlight_feature_id)}}
         </li>
         {% endfor %}
     </ul>
 
     {% if context == "index" %}
     <div class="cluster-footer">
-        <a href="/index/{{ index_id }}/cluster/{{ cluster_id }}{{ '/?feature_id={}'.format(highlight_feature_id) if highlight_feature_id else '' }}">See all</a>
+        {% if highlight_feature_id is not none %}
+        <a href="/index/{{ index_id }}/cluster/{{ cluster_id }}/?feature_id={{ highlight_feature_id }}">Intersect selected feature</a>
+        {% elif highlight_cluster_id is not none %}
+        <a href="/index/{{ index_id }}/cluster/{{ cluster_id }}/?filter_cluster_id={{ highlight_cluster_id }}">Intersect selected cluster</a>
+        {% else %}
+        <a href="/index/{{ index_id }}/cluster/{{ cluster_id }}"/>See  all in cluster</a>
+        {% endif %}
         <a href="/index/{{ index_id }}/?cluster_id={{ cluster_id }}">Pivot</a>
-        <details>
-            <summary>Edit</summary>
-            <form method="post" action="/index/{{ index_id }}/cluster/delete">
-                <input type="hidden" name="cluster_id" value="{{ cluster_id }}">
-                <button class="inline-button" type="submit">Delete 🗑️</button>
-            </form>
-        </details>
+        <label>
+            Select for editing:
+            <input type="checkbox" form="cluster_edit" name="cluster_id" value="{{ cluster_id }}">
+        </label>
     </div>
     {% endif %}
 </div>
 {%- endmacro %}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -9,11 +9,12 @@
 Cluster {{ cluster_id }} {% if cluster_score is not none %}- {{ "{:.2e}".format
 (cluster_score) }}{% endif %}
     * {% for feature_id, field, value, score in features %}
     * {{ render_feature(index_id, cluster_id, feature_id, field, value, score,
       context, highlight_feature_id=highlight_feature_id)}}
     * {% endfor %}
 {% if context == "index" %}
-See_all Pivot  Edit
- Delete ðï¸
+{% if highlight_feature_id is not none %} Intersect_selected_feature {% elif
+highlight_cluster_id is not none %} Intersect_selected_cluster {% else %} See
+all_in_cluster {% endif %} Pivot  Select for editing: ⁰
 {% endif %}
 {%- endmacro %}
```

### Comparing `hyperreal-0.3.1/hyperreal/utilities.py` & `hyperreal-0.4.0/hyperreal/utilities.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+import heapq
 from html.parser import HTMLParser
 from io import StringIO
+import itertools
 import math
+import operator
 
 from pyroaring import BitMap
 import regex
 
 
 # Used to transform left/right sided curly quotes into their straight quote
 # equivalents. This is particularly important on social media as the IOS
@@ -41,57 +44,29 @@
 
 
 def social_media_tokens(entry):
     cleaned = social_media_cleaner.sub(
         "", entry.translate(curly_quote_translator).lower()
     )
     tokens = [token for token in word_tokenizer.split(cleaned) if token.strip()]
+    # This is a terminator token, to make sure that collocations aren't
+    # identified across textual boundaries.
     tokens.append(None)
     return tokens
 
 
 def tokens(entry):
     cleaned = entry.lower()
     tokens = [token for token in word_tokenizer.split(cleaned) if token.strip()]
+    # This is a terminator token, to make sure that collocations aren't
+    # identified across textual boundaries.
     tokens.append(None)
     return tokens
 
 
-class HTMLTextLines(HTMLParser):
-    """
-    Parser for extracting the text from the data elements of given HTML.
-
-    """
-
-    def __init__(self):
-        super().__init__()
-        self.reset()
-        self.strict = False
-        self.convert_charrefs = True
-        self.lines = []
-
-    def handle_data(self, d):
-        self.lines.append(d)
-
-    def get_lines(self):
-        return self.lines
-
-
-def text_from_html(html):
-    """
-    Returns a list of the text contained in the data elements of the given HTML string.
-
-    """
-    s = HTMLTextLines()
-    s.feed(html)
-    lines = s.get_lines()
-    s.close()
-    return lines
-
-
 def bstm(matching, bitslice, top_k):
     """
     Applies the bit sliced term matching procedure.
 
     """
 
     if len(matching) <= top_k:
@@ -205,7 +180,92 @@
             if not carry:
                 break
 
         if carry:
             bitslice.append(carry)
 
     return matching, bitslice
+
+
+def weight_bitslice(bitslice):
+    """
+    Return an iterator of weights for each document in the bitslice.
+
+    """
+
+    # Can't be a lambda as we need to capture the layer eagerly
+    def slice_gen(bm, layer):
+        weight = 2**layer
+        for doc_id in bm:
+            yield (doc_id, weight)
+
+    # Returns them in merged order
+    ordered = heapq.merge(*(slice_gen(bm, i) for i, bm in enumerate(bitslice)))
+
+    grouped = itertools.groupby(ordered, key=operator.itemgetter(0))
+
+    for key, group in grouped:
+        yield key, sum(g[1] for g in group)
+
+
+def approximate_positions_with_sentinels(values, position_window_size):
+    """
+    Turn a Sequence of values into a generator of (position_bucket, value).
+
+    This function handles None as sentinel values to enforce position breaks
+    and the rounding of position values.
+
+    Examples:
+
+    This is position_window_size = 1, which is the exact position case.
+
+    >>> list(approximate_positions_with_sentinels(['the', 'cat', 'sat'], 1))
+    [(0, 'the'), (1, 'cat'), (2, 'sat')]
+
+    Approximate positions (position_window_size > 1) accumulate multiple
+    values into the same position as in the following examples for 2, 3:
+
+    >>> list(approximate_positions_with_sentinels(['the', 'cat', 'sat'], 2))
+    [(0, 'the'), (0, 'cat'), (1, 'sat')]
+
+    >>> values = "the cat sat on the mat".split()
+    >>> list(approximate_positions_with_sentinels(values, 3))
+    [(0, 'the'), (0, 'cat'), (0, 'sat'), (1, 'on'), (1, 'the'), (1, 'mat')]
+
+    'None' values are sentinel markers to terminate the position bucket
+    earlier. This can be used to control breaking more finely in a stream
+    of tokens than would otherwise be possible.
+
+    >>> values.insert(3, None)
+    >>> list(approximate_positions_with_sentinels(values, 2))
+    [(0, 'the'), (0, 'cat'), (1, 'sat'), (2, 'on'), (2, 'the'), (3, 'mat')]
+
+    Lastly a negative position value only changes position at sentinel None's.
+    This allows you to control everything about the procedure.
+
+    >>> list(approximate_positions_with_sentinels(values, -2))
+    [(0, 'the'), (0, 'cat'), (0, 'sat'), (1, 'on'), (1, 'the'), (1, 'mat')]
+
+    """
+
+    current_position = 0
+    current_size = 0
+
+    for value in values:
+        if value is None:
+            # If we've placed anything in the current bucket, we
+            # need to advance the position counter - otherwise
+            # we can just keep advancing. This turns consecutive
+            # sentinels into a single sentinel.
+            if current_size:
+                current_position += 1
+                current_size = 0
+
+            continue
+
+        current_size += 1
+
+        yield (current_position, value)
+
+        if current_size == position_window_size:
+            current_position += 1
+            current_size = 0
```

### Comparing `hyperreal-0.3.1/hyperreal.egg-info/PKG-INFO` & `hyperreal-0.4.0/hyperreal.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: hyperreal
-Version: 0.3.1
+Version: 0.4.0
 Summary: Hyperreal is a library and tool for intepretive topic modelling.
 Home-page: https://github.com/SamHames/hyperreal/
 Author: Sam Hames
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: stackexchange
 License-File: LICENSE.txt
 
 # Hyperreal
 
 Hyperreal is a Python tool for interactive qualitative analysis of large
 collections of documents.
 
@@ -38,15 +39,15 @@
 ## Usage
 
 Hyperreal can be used in three different ways to flexibly support different
 use cases:
 
 - as a command line application
 - as a Python library
-- via the built in web application
+- as a local web application
 
 All of hyperreal's functionality is available from the Python library, but you
 will need to write Python code to use it directly. The command line interface
 allows for quick and repeatable experimentation and automation for standard
 data types - for example if you often work with Twitter data the command line
 will allow you to rapidly work with many different Twitter data collections.
 The web application is currently focused solely on creating and interactive
@@ -63,15 +64,15 @@
 If you haven't worked with the command line before, you might find the
 following resources useful:
 
 - [Software Carpentry resources for Mac](https://swcarpentry.github.io/shell-novice/)
 - [Open Water Foundation resources for Windows](https://learn.openwaterfoundation.org/owf-learn-windows-shell/)
 
 ```
-# Create a corpus database from the plaintext file
+# Create a corpus database from a plaintext file
 hyperreal plaintext-corpus create corpus.txt corpus.db
 
 # Create an index from the corpus
 hyperreal plaintext-corpus index corpus.db corpus_index.db
 
 # Create a model from that index, in this case with 128 clusters and
 # only include features present in 10 or more documents.
@@ -99,46 +100,48 @@
   # This will drop any line that has no text (such as a paragraph break)
   docs = (line for line in f if line.strip())
   c.replace_docs(docs)
 
 
 # Index that corpus - note that we need to pass the corpus object for
 # initialisation.
-i = index.Index('corpus_index.db', corpus=c)
+idx = index.Index('corpus_index.db', corpus=c)
 # This only needs to be done once, unless the corpus changes.
-i.index()
+idx.index()
 
 # Create a model on this index, with 128 clusters and only including features
 # that match at least 10 documents.
-i.initialise_clusters(n_clusters=128, min_docs=10)
+idx.initialise_clusters(n_clusters=128, min_docs=10)
 # Refine the model for 10 iterations. Note that you can continue to refine
 # the model without initialising the clusters.
-i.refine_clusters(iterations=10)
+idx.refine_clusters(iterations=10)
 
 # Inspect the output of the model using the index instance (currently quite
 # limited). This will print the top 10 most frequent features in each
 # cluster.
-for cluster_id in i.cluster_ids:
-    cluster_features = i.cluster_features(cluster_id)
+for cluster_id in idx.cluster_ids:
+    cluster_features = idx.cluster_features(cluster_id)
     for feature in cluster_features[:10]:
         print(feature)
 
 # Perform a boolean query on the corpus, looking for documents that contain
 # both apples AND oranges in the text field.
 q = i[('text', 'apples')] & i[('text', 'oranges')]
 # Lookup all of the documents in the corpus that match this query.
-docs = i.get_docs(q)
+docs = idx.get_docs(q)
 
 # 'Pivot' the features in the index with respect to all cluster in the model.
 #  This will show the top 10 features in each cluster that are similar to the
 #  query.
-i.pivot_clusters_by_query(query, top_k=10)
+for cluster_detail in idx.pivot_clusters_by_query(query, top_k=10):
+    print(cluster_detail)
 
 # This will show the top 10 features for a selected set of cluster_ids.
-i.pivot_clusters_by_query(query, cluster_ids=[3,5,7], top_k=10)
+for cluster_detail in idx.pivot_clusters_by_query(query, cluster_ids=[3,5,7], top_k=10):
+    print(cluster_detail)
 
 ```
 
 
 ## Development
 
 ### Installation
```

### Comparing `hyperreal-0.3.1/setup.py` & `hyperreal-0.4.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 requires = [
     "click>=8.1.0",
     "jinja2>=3.1.0",
     "pyroaring>=0.3.4",
     "regex>=2022.4.24",
     "cherrypy>=18.6.0",
     "python-dateutil>=2.8.0",
+    "networkx>=3.0.0",
 ]
 
-extras = {"test": ["pytest", "black", "tox"]}
+extras = {"test": ["pytest", "black", "tox"], "stackexchange": ["lxml"]}
 
 
 setup(
     name="hyperreal",
     use_scm_version=True,
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `hyperreal-0.3.1/tox.ini` & `hyperreal-0.4.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     tests_coverage
     check_format
 
 [testenv:tests_coverage]
 deps =
     pytest
     coverage
+    lxml
 passenv =
     RUNNING_IN_CI
 commands =
     coverage erase
     # Config is all specified in .coveragerc
     coverage run -m pytest --doctest-modules
     coverage combine
```

