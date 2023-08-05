# Comparing `tmp/scmomat-0.2.1.tar.gz` & `tmp/scmomat-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scmomat-0.2.1.tar", last modified: Thu Jul 27 18:47:06 2023, max compression
+gzip compressed data, was "scmomat-0.2.2.tar", last modified: Sat Aug  5 01:48:57 2023, max compression
```

## Comparing `scmomat-0.2.1.tar` & `scmomat-0.2.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-sr-x   0 zzhang834 (1059113) coc-xzhanglab-access (372345)        0 2023-07-27 18:47:06.393109 scmomat-0.2.1/
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)     1066 2023-02-21 22:18:42.000000 scmomat-0.2.1/LICENSE
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)       25 2023-02-21 22:18:42.000000 scmomat-0.2.1/MANIFEST.in
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)     7829 2023-07-27 18:47:06.392109 scmomat-0.2.1/PKG-INFO
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)     7008 2023-02-21 22:18:42.000000 scmomat-0.2.1/README.md
-drwxr-sr-x   0 zzhang834 (1059113) coc-xzhanglab-access (372345)        0 2023-07-27 18:47:06.344108 scmomat-0.2.1/scmomat/
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)      188 2023-02-21 22:21:48.000000 scmomat-0.2.1/scmomat/__init__.py
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)       62 2023-02-21 22:21:48.000000 scmomat-0.2.1/scmomat/__version__.py
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    21371 2023-02-21 22:21:48.000000 scmomat-0.2.1/scmomat/bmk.py
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    33204 2023-02-21 22:21:48.000000 scmomat-0.2.1/scmomat/model.py
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)   120615 2023-02-21 22:21:48.000000 scmomat-0.2.1/scmomat/umap_batch.py
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    33574 2023-07-27 18:11:22.000000 scmomat-0.2.1/scmomat/utils.py
-drwxr-sr-x   0 zzhang834 (1059113) coc-xzhanglab-access (372345)        0 2023-07-27 18:47:06.357109 scmomat-0.2.1/scmomat.egg-info/
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)     7829 2023-07-27 18:47:06.000000 scmomat-0.2.1/scmomat.egg-info/PKG-INFO
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)      639 2023-07-27 18:47:06.000000 scmomat-0.2.1/scmomat.egg-info/SOURCES.txt
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)        1 2023-07-27 18:47:06.000000 scmomat-0.2.1/scmomat.egg-info/dependency_links.txt
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)      129 2023-07-27 18:47:06.000000 scmomat-0.2.1/scmomat.egg-info/requires.txt
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)        8 2023-07-27 18:47:06.000000 scmomat-0.2.1/scmomat.egg-info/top_level.txt
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)       38 2023-07-27 18:47:06.394109 scmomat-0.2.1/setup.cfg
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)     4117 2023-07-27 18:45:30.000000 scmomat-0.2.1/setup.py
-drwxr-sr-x   0 zzhang834 (1059113) coc-xzhanglab-access (372345)        0 2023-07-27 18:47:06.389109 scmomat-0.2.1/test/
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    50946 2023-02-21 22:18:42.000000 scmomat-0.2.1/test/test_bmmc_healthy.py
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    14250 2023-02-21 22:18:42.000000 scmomat-0.2.1/test/test_hyperparams.py
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    20900 2023-02-21 22:18:42.000000 scmomat-0.2.1/test/test_marker_detection.py
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    48633 2023-02-21 22:18:42.000000 scmomat-0.2.1/test/test_mop_5batches.py
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    27229 2023-02-21 22:18:42.000000 scmomat-0.2.1/test/test_pancreas.py
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    73157 2023-02-21 22:18:42.000000 scmomat-0.2.1/test/test_pbmc.py
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    36300 2023-02-21 22:18:42.000000 scmomat-0.2.1/test/test_simulated_2modalities.py
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    36689 2023-02-21 22:18:42.000000 scmomat-0.2.1/test/test_simulated_3modalities.py
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    34257 2023-02-21 22:18:42.000000 scmomat-0.2.1/test/test_simulated_imbalanced.py
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    17211 2023-02-21 22:18:42.000000 scmomat-0.2.1/test/test_simulated_nopseudo.py
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    37474 2023-02-21 22:18:42.000000 scmomat-0.2.1/test/test_spleen.py
--rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    46027 2023-02-21 22:18:42.000000 scmomat-0.2.1/test/test_spleen_subsample.py
+drwxr-sr-x   0 zzhang834 (1059113) coc-xzhanglab-access (372345)        0 2023-08-05 01:48:57.064524 scmomat-0.2.2/
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)     1066 2023-02-21 22:18:42.000000 scmomat-0.2.2/LICENSE
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)       25 2023-02-21 22:18:42.000000 scmomat-0.2.2/MANIFEST.in
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)     7829 2023-08-05 01:48:57.063524 scmomat-0.2.2/PKG-INFO
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)     7008 2023-02-21 22:18:42.000000 scmomat-0.2.2/README.md
+drwxr-sr-x   0 zzhang834 (1059113) coc-xzhanglab-access (372345)        0 2023-08-05 01:48:57.005524 scmomat-0.2.2/scmomat/
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)      159 2023-08-05 01:40:10.000000 scmomat-0.2.2/scmomat/__init__.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)       62 2023-08-05 01:47:23.000000 scmomat-0.2.2/scmomat/__version__.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    21371 2023-02-21 22:21:48.000000 scmomat-0.2.2/scmomat/bmk.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    33204 2023-02-21 22:21:48.000000 scmomat-0.2.2/scmomat/model.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)   121168 2023-08-05 01:13:16.000000 scmomat-0.2.2/scmomat/umap_batch.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    34687 2023-08-05 01:38:12.000000 scmomat-0.2.2/scmomat/utils.py
+drwxr-sr-x   0 zzhang834 (1059113) coc-xzhanglab-access (372345)        0 2023-08-05 01:48:57.021524 scmomat-0.2.2/scmomat.egg-info/
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)     7829 2023-08-05 01:48:56.000000 scmomat-0.2.2/scmomat.egg-info/PKG-INFO
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)      661 2023-08-05 01:48:56.000000 scmomat-0.2.2/scmomat.egg-info/SOURCES.txt
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)        1 2023-08-05 01:48:56.000000 scmomat-0.2.2/scmomat.egg-info/dependency_links.txt
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)      129 2023-08-05 01:48:56.000000 scmomat-0.2.2/scmomat.egg-info/requires.txt
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)        8 2023-08-05 01:48:56.000000 scmomat-0.2.2/scmomat.egg-info/top_level.txt
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)       38 2023-08-05 01:48:57.064524 scmomat-0.2.2/setup.cfg
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)     4117 2023-08-05 01:45:43.000000 scmomat-0.2.2/setup.py
+drwxr-sr-x   0 zzhang834 (1059113) coc-xzhanglab-access (372345)        0 2023-08-05 01:48:57.060524 scmomat-0.2.2/test/
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)     3423 2023-08-05 01:39:13.000000 scmomat-0.2.2/test/test_10x_pbmc.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    50946 2023-02-21 22:18:42.000000 scmomat-0.2.2/test/test_bmmc_healthy.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    14250 2023-02-21 22:18:42.000000 scmomat-0.2.2/test/test_hyperparams.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    20900 2023-02-21 22:18:42.000000 scmomat-0.2.2/test/test_marker_detection.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    48633 2023-02-21 22:18:42.000000 scmomat-0.2.2/test/test_mop_5batches.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    27229 2023-02-21 22:18:42.000000 scmomat-0.2.2/test/test_pancreas.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    73157 2023-02-21 22:18:42.000000 scmomat-0.2.2/test/test_pbmc.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    36300 2023-02-21 22:18:42.000000 scmomat-0.2.2/test/test_simulated_2modalities.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    36689 2023-02-21 22:18:42.000000 scmomat-0.2.2/test/test_simulated_3modalities.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    34257 2023-02-21 22:18:42.000000 scmomat-0.2.2/test/test_simulated_imbalanced.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    17211 2023-02-21 22:18:42.000000 scmomat-0.2.2/test/test_simulated_nopseudo.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    37474 2023-02-21 22:18:42.000000 scmomat-0.2.2/test/test_spleen.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    46027 2023-02-21 22:18:42.000000 scmomat-0.2.2/test/test_spleen_subsample.py
```

### Comparing `scmomat-0.2.1/LICENSE` & `scmomat-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.1/PKG-INFO` & `scmomat-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmomat
-Version: 0.2.1
+Version: 0.2.2
 Summary: scmomat: a single-cell multi-omics mosaic integration method
 Home-page: https://github.com/PeterZZQ/scMoMaT
 Author: Ziqi Zhang
 Author-email: zhangziqibuaa@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `scmomat-0.2.1/README.md` & `scmomat-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.1/scmomat/bmk.py` & `scmomat-0.2.2/scmomat/bmk.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.1/scmomat/model.py` & `scmomat-0.2.2/scmomat/model.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.1/scmomat/umap_batch.py` & `scmomat-0.2.2/scmomat/umap_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1737,15 +1737,17 @@
                 self._inverse_distance_func = None
                 warn(
                     "custom distance metric does not return gradient; inverse_transform will be unavailable. "
                     "To enable using inverse_transform method method, define a distance function that returns "
                     "a tuple of (distance [float], gradient [np.array])"
                 )
         elif self.metric == "precomputed":
+            # self.unique is set to be unique, the default is False
             if self.unique:
+                # if self.unique is true, raise error
                 raise ValueError("unique is poorly defined on a precomputed metric")
             warn(
                 "using precomputed metric; transform will be unavailable for new data and inverse_transform "
                 "will be unavailable for all data"
             )
             self._input_distance_func = self.metric
             self._inverse_distance_func = None
@@ -2211,14 +2213,15 @@
         # This will save special cases later.
         else:
             print("not unique")
             index = list(range(X.shape[0]))
             inverse = list(range(X.shape[0]))
 
         # Error check n_neighbors based on data size
+        # if not unique, X[index] is X itself, larger than self.n_neighbors, and self._n_neighbors is set to self.n_neighbors
         if X[index].shape[0] <= self.n_neighbors:
             if X[index].shape[0] == 1:
                 self.embedding_ = np.zeros(
                     (1, self.n_components)
                 )  # needed to sklearn comparability
                 return self
 
@@ -2233,14 +2236,15 @@
             self._n_neighbors = self.n_neighbors
 
         # Note: unless it causes issues for setting 'index', could move this to
         # initial sparsity check above
         if self._sparse_data and not X.has_sorted_indices:
             X.sort_indices()
 
+        # generate random state given seed
         random_state = check_random_state(self.random_state)
 
         if self.verbose:
             print("Construct fuzzy simplicial set")
 
         if self.metric == "precomputed" and self._sparse_data:
             print("using precompute")
@@ -2268,14 +2272,15 @@
                         raise ValueError(
                             "Some rows contain fewer than n_neighbors distances!"
                         )
                     row_nn_data_indices = np.argsort(row_data)[: self._n_neighbors]
                     self._knn_indices[row_id] = row_indices[row_nn_data_indices]
                     self._knn_dists[row_id] = row_data[row_nn_data_indices]
             else:
+                # knn don't need to be calculated, as we have already calculated knn
                 print("Provided KNN...")
                 # use the provided knn in the initialization
                 self._knn_indices = self.knn_indices
                 self._knn_dists = self.knn_dists
 
             # Disconnect any vertices farther apart than _disconnection_distance
             # np.inf
@@ -2569,15 +2574,17 @@
 
         if self.densmap or self.output_dens:
             self._densmap_kwds["graph_dists"] = self.graph_dists_
 
         if self.verbose:
             print(ts(), "Construct embedding")
 
+        # Transforming into embedding
         if self.transform_mode == "embedding":
+            # when we have graph and the init is random, self._raw_data[index] is a place-holder
             self.embedding_, aux_data = self._fit_embed_data(
                 self._raw_data[index], n_epochs, init, random_state,  # JH why raw data?
             )
             # Assign any points that are fully disconnected from our manifold(s) to have embedding
             # coordinates of np.nan.  These will be filtered by our plotting functions automatically.
             # They also prevent users from being deceived a distance query to one of these points.
             # Might be worth moving this into simplicial_set_embedding or _fit_embed_data
@@ -2597,14 +2604,15 @@
 
         return self
 
     def _fit_embed_data(self, X, n_epochs, init, random_state):
         """A method wrapper for simplicial_set_embedding that can be
         replaced by subclasses.
         """
+        print(init + " intialization...")
         return simplicial_set_embedding(
             X,
             self.graph_,
             self.n_components,
             self._initial_alpha,
             self._a,
             self._b,
```

### Comparing `scmomat-0.2.1/scmomat/utils.py` & `scmomat-0.2.2/scmomat/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 
 import numpy as np
 from scipy import stats
 import scipy.sparse as sp
 from umap.utils import fast_knn_indices
 import time
+import scmomat.umap_batch as umap_batch
 try:
     from adjustText import adjust_text
     adjust_text_flag = True
 except ImportError:
     adjust_text_flag = False
 
 # ----------------------------------------------------- # 
@@ -627,29 +628,28 @@
 
     partition_kwargs['weights'] = np.array(g.es['weight']).astype(np.float64)
     part = leidenalg.find_partition(g, partition_type, **partition_kwargs)
     groups = np.array(part.membership)
 
     return groups
 
-def post_process(X, n_neighbors, r = None, njobs = 1, return_sparse_dist = False):
+def calc_post_graph(X, n_neighbors, r = None, njobs = 1, return_sparse_dist = False):
     """\
     Description:
     ------------
-        The post-processing steps of scMoMaT.
+        Post-processing scMoMaT cell factor into neighborhood graph.
     Parameters:
     ------------
         X: the matrix format latent embedding.
         n_neighors: number of nearest neighbors.
         r: radius parameter of neighborhood size, between 0 and 1.
         njobs: number of jobs to run in parallel, speed up the calculation.
         return_sparse_dist: calculate the sparse pairwise distance or not in the end.
     Return:
     -------------
-        pair_dist: pairwise distance
         knn_indices: the knn indices of the post-processed embedding graph.
         knn_dists: the knn distance of the post-processed embedding graph.
     """
     # get a pairwise distance matrix for all batches
     from sklearn.metrics import pairwise_distances
     start_time = time.time()
     pair_dist = pairwise_distances(np.concatenate(X, axis = 0), n_jobs = njobs)
@@ -737,31 +737,56 @@
     for batch_i in range(len(X)):
         ref_block = knn_dists[start_point[batch_i]:(end_point[batch_i] + 1), sum(b_neighbors[0:batch_i]):sum(b_neighbors[0:(batch_i+1)])]
         for batch_j in range(len(X)):
             if batch_i != batch_j:
                 block = knn_dists[start_point[batch_i]:(end_point[batch_i] + 1), sum(b_neighbors[0:batch_j]):sum(b_neighbors[0:(batch_j+1)])]
                 knn_dists[start_point[batch_i]:(end_point[batch_i] + 1), sum(b_neighbors[0:batch_j]):sum(b_neighbors[0:(batch_j+1)])] = block/(np.mean(block, axis = 1, keepdims = True) + 1e-6) * np.mean(ref_block, axis = 1, keepdims = True)
     end_time = time.time()
-    print("modify distance 1, time used {:.4f}s".format(end_time - start_time))
+    print("modify distance, time used {:.4f}s".format(end_time - start_time))
 
-    start_time = time.time()
+    # start_time = time.time()
     # Modify pairwise distance matrix where the elements are changed due to knn_dists, 
     # pairwise_distance does not affect the UMAP visualization and leiden clustering
 
 
     # NEW, UMAP
-    if return_sparse_dist:
-        pairwise_distances = np.zeros_like(pair_dist)
-        pairwise_distances[np.arange(pairwise_distances.shape[0])[:, None], knn_indices] = knn_dists
-        pairwise_distances = pairwise_distances + pairwise_distances.T - pairwise_distances * pairwise_distances.T
-
-        end_time = time.time()
-        print("modify distance 2, time used {:.4f}s".format(end_time - start_time))
-
-        # start_time = time.time()     
-        pair_dist = sp.csr_matrix(pairwise_distances)
-    else:
-        pair_dist = sp.csr_matrix(pair_dist)
+    # if return_sparse_dist:
+    #     pairwise_distances = np.zeros_like(pair_dist)
+    #     pairwise_distances[np.arange(pairwise_distances.shape[0])[:, None], knn_indices] = knn_dists
+    #     pairwise_distances = pairwise_distances + pairwise_distances.T - pairwise_distances * pairwise_distances.T
+
+    #     end_time = time.time()
+    #     print("modify distance 2, time used {:.4f}s".format(end_time - start_time))
+
+    #     # start_time = time.time()     
+    #     pair_dist = sp.csr_matrix(pairwise_distances)
+    # else:
+        # pair_dist = sp.csr_matrix(pair_dist)
     # end_time = time.time()
     # print("make sparse, time used {:.4f}s".format(end_time - start_time))
     # pairwise_distances = pair_dist
-    return pair_dist, knn_indices, knn_dists
+    return knn_indices, knn_dists
+
+
+def calc_umap_embedding(knn_indices, knn_dists, n_components = 2, n_neighbors = 100, min_dist = 0.2, 
+                        random_state = 0, init = "random", **kwarg):
+    """
+    Description:
+    -------------
+        Calculating UMAP from knn graph (knn_indices, knn_dists)
+    Parameters:
+    -------------
+        knn_indices, knn_dists: the output of function calc_post_graph
+        n_components: number of components in UMAP
+        n_neighbors, min_dist, random_state, init: UMAP parameters
+    Return:
+    -------------
+        x_umap: umap embedding of (n_cells, n_components) 
+        
+    """
+    umap_op = umap_batch.UMAP(n_components = n_components, n_neighbors = n_neighbors, min_dist = min_dist, random_state = random_state, 
+                              metric = "precomputed", knn_dists = knn_dists, knn_indices = knn_indices, init = init, **kwarg)
+    # fill in an empty matrix as place-holder
+    empty_matrix = sp.csr_matrix(np.zeros((knn_indices.shape[0], knn_indices.shape[0])))
+    x_umap = umap_op.fit_transform(empty_matrix)
+
+    return x_umap
```

### Comparing `scmomat-0.2.1/scmomat.egg-info/PKG-INFO` & `scmomat-0.2.2/scmomat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmomat
-Version: 0.2.1
+Version: 0.2.2
 Summary: scmomat: a single-cell multi-omics mosaic integration method
 Home-page: https://github.com/PeterZZQ/scMoMaT
 Author: Ziqi Zhang
 Author-email: zhangziqibuaa@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `scmomat-0.2.1/scmomat.egg-info/SOURCES.txt` & `scmomat-0.2.2/scmomat.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 scmomat/umap_batch.py
 scmomat/utils.py
 scmomat.egg-info/PKG-INFO
 scmomat.egg-info/SOURCES.txt
 scmomat.egg-info/dependency_links.txt
 scmomat.egg-info/requires.txt
 scmomat.egg-info/top_level.txt
+test/test_10x_pbmc.py
 test/test_bmmc_healthy.py
 test/test_hyperparams.py
 test/test_marker_detection.py
 test/test_mop_5batches.py
 test/test_pancreas.py
 test/test_pbmc.py
 test/test_simulated_2modalities.py
```

### Comparing `scmomat-0.2.1/setup.py` & `scmomat-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'scmomat'
 DESCRIPTION = 'scmomat: a single-cell multi-omics mosaic integration method'
 URL = 'https://github.com/PeterZZQ/scMoMaT'
 EMAIL = 'zhangziqibuaa@gmail.com'
 AUTHOR = 'Ziqi Zhang'
 REQUIRES_PYTHON = '>=3.8.10'
-VERSION = '0.2.1'
+VERSION = '0.2.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'torch>=1.11.0',
     'numpy>=1.19.5',
     'pandas>=1.4.0',
     'scipy>=1.7.3',
```

### Comparing `scmomat-0.2.1/test/test_bmmc_healthy.py` & `scmomat-0.2.2/test/test_bmmc_healthy.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.1/test/test_hyperparams.py` & `scmomat-0.2.2/test/test_hyperparams.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.1/test/test_marker_detection.py` & `scmomat-0.2.2/test/test_marker_detection.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.1/test/test_mop_5batches.py` & `scmomat-0.2.2/test/test_mop_5batches.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.1/test/test_pancreas.py` & `scmomat-0.2.2/test/test_pancreas.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.1/test/test_pbmc.py` & `scmomat-0.2.2/test/test_pbmc.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.1/test/test_simulated_2modalities.py` & `scmomat-0.2.2/test/test_simulated_2modalities.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.1/test/test_simulated_3modalities.py` & `scmomat-0.2.2/test/test_simulated_3modalities.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.1/test/test_simulated_imbalanced.py` & `scmomat-0.2.2/test/test_simulated_imbalanced.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.1/test/test_simulated_nopseudo.py` & `scmomat-0.2.2/test/test_simulated_nopseudo.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.1/test/test_spleen.py` & `scmomat-0.2.2/test/test_spleen.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.1/test/test_spleen_subsample.py` & `scmomat-0.2.2/test/test_spleen_subsample.py`

 * *Files identical despite different names*

