# Comparing `tmp/scgraphne-0.1.0.tar.gz` & `tmp/scgraphne-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scgraphne-0.1.0.tar", last modified: Tue Jul 25 05:45:51 2023, max compression
+gzip compressed data, was "scgraphne-0.1.1.tar", last modified: Sat Aug  5 08:00:20 2023, max compression
```

## Comparing `scgraphne-0.1.0.tar` & `scgraphne-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 05:45:51.637686 scgraphne-0.1.0/
--rw-rw-rw-   0        0        0     2824 2023-07-25 05:45:51.636602 scgraphne-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1830 2023-07-23 12:47:02.000000 scgraphne-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 05:45:51.608374 scgraphne-0.1.0/scgraphne/
--rw-rw-rw-   0        0        0      473 2023-07-23 13:03:58.000000 scgraphne-0.1.0/scgraphne/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 05:45:51.621478 scgraphne-0.1.0/scgraphne/data/
--rw-rw-rw-   0        0        0       89 2023-07-23 08:25:36.000000 scgraphne-0.1.0/scgraphne/data/__init__.py
--rw-rw-rw-   0        0        0     2854 2023-07-24 06:14:16.000000 scgraphne-0.1.0/scgraphne/data/data_utils.py
--rw-rw-rw-   0        0        0     1932 2023-07-23 12:03:42.000000 scgraphne-0.1.0/scgraphne/data/graph.py
-drwxrwxrwx   0        0        0        0 2023-07-25 05:45:51.627561 scgraphne-0.1.0/scgraphne/model/
--rw-rw-rw-   0        0        0       90 2023-07-23 13:00:36.000000 scgraphne-0.1.0/scgraphne/model/__init__.py
--rw-rw-rw-   0        0        0     4817 2023-07-23 15:37:28.000000 scgraphne-0.1.0/scgraphne/model/decoder.py
--rw-rw-rw-   0        0        0     8398 2023-07-23 15:35:06.000000 scgraphne-0.1.0/scgraphne/model/scgraphne.py
--rw-rw-rw-   0        0        0    14372 2023-07-25 02:46:36.000000 scgraphne-0.1.0/scgraphne/run_scgraphne.py
-drwxrwxrwx   0        0        0        0 2023-07-25 05:45:51.633928 scgraphne-0.1.0/scgraphne/utils/
--rw-rw-rw-   0        0        0      151 2023-07-23 12:54:42.000000 scgraphne-0.1.0/scgraphne/utils/__init__.py
--rw-rw-rw-   0        0        0     1877 2023-07-07 13:24:34.000000 scgraphne-0.1.0/scgraphne/utils/metric.py
--rw-rw-rw-   0        0        0    13875 2023-07-24 07:51:34.000000 scgraphne-0.1.0/scgraphne/utils/read.py
--rw-rw-rw-   0        0        0     1828 2023-07-07 13:35:40.000000 scgraphne-0.1.0/scgraphne/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-25 05:45:51.616338 scgraphne-0.1.0/scgraphne.egg-info/
--rw-rw-rw-   0        0        0     2824 2023-07-25 05:45:51.000000 scgraphne-0.1.0/scgraphne.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      498 2023-07-25 05:45:51.000000 scgraphne-0.1.0/scgraphne.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 05:45:51.000000 scgraphne-0.1.0/scgraphne.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-25 05:45:51.000000 scgraphne-0.1.0/scgraphne.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-25 05:45:51.000000 scgraphne-0.1.0/scgraphne.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 05:45:51.637686 scgraphne-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1220 2023-07-23 12:51:36.000000 scgraphne-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 08:00:20.116386 scgraphne-0.1.1/
+-rw-rw-rw-   0        0        0     2824 2023-08-05 08:00:20.115326 scgraphne-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1830 2023-08-05 07:28:26.000000 scgraphne-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 08:00:20.096234 scgraphne-0.1.1/scgraphne/
+-rw-rw-rw-   0        0        0      477 2023-08-05 07:44:47.000000 scgraphne-0.1.1/scgraphne/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 08:00:20.105435 scgraphne-0.1.1/scgraphne/data/
+-rw-rw-rw-   0        0        0       89 2023-07-23 08:25:36.000000 scgraphne-0.1.1/scgraphne/data/__init__.py
+-rw-rw-rw-   0        0        0     2855 2023-08-05 07:44:47.000000 scgraphne-0.1.1/scgraphne/data/data_utils.py
+-rw-rw-rw-   0        0        0     1928 2023-08-05 07:44:47.000000 scgraphne-0.1.1/scgraphne/data/graph.py
+drwxrwxrwx   0        0        0        0 2023-08-05 08:00:20.108455 scgraphne-0.1.1/scgraphne/model/
+-rw-rw-rw-   0        0        0       92 2023-08-05 07:44:47.000000 scgraphne-0.1.1/scgraphne/model/__init__.py
+-rw-rw-rw-   0        0        0     5525 2023-08-05 07:44:47.000000 scgraphne-0.1.1/scgraphne/model/decoder.py
+-rw-rw-rw-   0        0        0     8199 2023-08-05 07:44:47.000000 scgraphne-0.1.1/scgraphne/model/scgraphne.py
+-rw-rw-rw-   0        0        0    14165 2023-08-05 07:44:47.000000 scgraphne-0.1.1/scgraphne/run_scgraphne.py
+drwxrwxrwx   0        0        0        0 2023-08-05 08:00:20.114252 scgraphne-0.1.1/scgraphne/utils/
+-rw-rw-rw-   0        0        0      151 2023-07-23 12:54:42.000000 scgraphne-0.1.1/scgraphne/utils/__init__.py
+-rw-rw-rw-   0        0        0     1887 2023-08-05 07:44:47.000000 scgraphne-0.1.1/scgraphne/utils/metric.py
+-rw-rw-rw-   0        0        0     4053 2023-08-05 07:44:47.000000 scgraphne-0.1.1/scgraphne/utils/read.py
+-rw-rw-rw-   0        0        0     1829 2023-08-05 07:44:47.000000 scgraphne-0.1.1/scgraphne/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-05 08:00:20.102301 scgraphne-0.1.1/scgraphne.egg-info/
+-rw-rw-rw-   0        0        0     2824 2023-08-05 08:00:19.000000 scgraphne-0.1.1/scgraphne.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      498 2023-08-05 08:00:20.000000 scgraphne-0.1.1/scgraphne.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 08:00:19.000000 scgraphne-0.1.1/scgraphne.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-08-05 08:00:19.000000 scgraphne-0.1.1/scgraphne.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-05 08:00:19.000000 scgraphne-0.1.1/scgraphne.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 08:00:20.116386 scgraphne-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1220 2023-08-05 07:34:57.000000 scgraphne-0.1.1/setup.py
```

### Comparing `scgraphne-0.1.0/PKG-INFO` & `scgraphne-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: scgraphne
-Version: 0.1.0
+Version: 0.1.1
 Summary: scGraphNE: a novel scRNA-seq representation learning method based on graph node embedding
 Home-page: https://github.com/sldyns/scGraphNE
 Author: Kun Qian, Ting Li
 Author-email: kun_qian@foxmail.com
 Maintainer: Kun Qian
 Maintainer-email: kun_qian@foxmail.com
 License: MIT Licence
 Description: # scGraphNE: a novel scRNA-seq representation learning method based on graph node embedding
         
         ## Overview
         
-        ![alt](overview.svg)
+        ![alt](overview.png)
         
         scGraphNE is a graph autoencoder network where the encoder based on multi-layer graph convolutional networks extracts high-order representations of cells and genes from the cell-gene bipartite graph, and the decoder based on the ZINB model uses these representations to reconstruct the gene expression matrix. By virtue of a model-driven self-supervised training paradigm, scGraphNE can effectively learn low-dimensional representations of both cells and genes, amenable to diverse downstream analytical tasks.
         
         ## Installation
         
         Please install `scGraphNE` from pypi with:
```

### Comparing `scgraphne-0.1.0/README.md` & `scgraphne-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # scGraphNE: a novel scRNA-seq representation learning method based on graph node embedding
 
 ## Overview
 
-![alt](overview.svg)
+![alt](overview.png)
 
 scGraphNE is a graph autoencoder network where the encoder based on multi-layer graph convolutional networks extracts high-order representations of cells and genes from the cell-gene bipartite graph, and the decoder based on the ZINB model uses these representations to reconstruct the gene expression matrix. By virtue of a model-driven self-supervised training paradigm, scGraphNE can effectively learn low-dimensional representations of both cells and genes, amenable to diverse downstream analytical tasks.
 
 ## Installation
 
 Please install `scGraphNE` from pypi with:
```

### Comparing `scgraphne-0.1.0/scgraphne/data/data_utils.py` & `scgraphne-0.1.1/scgraphne/data/data_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-import scanpy as sc
+import dgl
 import numpy as np
 import pandas as pd
-import dgl
+import scanpy as sc
 import torch
+
 from .graph import construct_gene_graph, add_degree
 
+
 def preprocess(adata, filter_min_counts=True, size_factors=True, normalize_input=False, logtrans_input=True):
     if size_factors or normalize_input or logtrans_input:
         adata.raw = adata.copy()
     else:
         adata.raw = adata
 
     if filter_min_counts:
@@ -28,14 +30,15 @@
     adata.var['gs_factor'] = gs_factor.reshape(-1)
 
     if normalize_input:
         sc.pp.scale(adata)
 
     return adata
 
+
 def make_graph(adata, raw_exp=False, gene_similarity=False):
     X = adata.X
     num_cells, num_genes = X.shape
 
     # Make expressioin/train graph
     num_nodes_dict = {'cell': num_cells, 'gene': num_genes}
     exp_train_cell, exp_train_gene = np.where(X > 0)
@@ -47,31 +50,31 @@
         ('gene', 'reverse-exp', 'cell'): (exp_train_gene, exp_train_cell)
     }
 
     coexp_edges, uncoexp_edges = None, None
     if gene_similarity:
         coexp_edges, uncoexp_edges = construct_gene_graph(X)
         exp_edge_dict[('gene', 'co-exp', 'gene')] = coexp_edges
-    
+
     # expression encoder/decoder graph
     enc_graph = dgl.heterograph(exp_edge_dict, num_nodes_dict=num_nodes_dict)
 
     exp_edge_dict.pop(('gene', 'reverse-exp', 'cell'))
     dec_graph = dgl.heterograph(exp_edge_dict, num_nodes_dict=num_nodes_dict)
-    
+
     # add degree to cell/gene nodes
     add_degree(enc_graph, ['exp'] + (['co-exp'] if gene_similarity else []))
 
     # If use ZINB decoder, add size factor to cell/gene nodes
     if raw_exp:
         Raw = pd.DataFrame(adata.raw.X, index=list(adata.raw.obs_names), columns=list(adata.raw.var_names))
         X = Raw[list(adata.var_names)].values
-        exp_value = X[exp_train_cell, exp_train_gene].reshape(-1,1)
+        exp_value = X[exp_train_cell, exp_train_gene].reshape(-1, 1)
         dec_graph.nodes['cell'].data['cs_factor'] = torch.Tensor(adata.obs['cs_factor']).reshape(-1, 1)
         dec_graph.nodes['gene'].data['gs_factor'] = torch.Tensor(adata.var['gs_factor']).reshape(-1, 1)
 
     else:
         ## Deflate the edge values of the bipartite graph to between 0 and 1
         X = X / adata.var['gs_factor'].values
         exp_value = X[exp_train_cell, exp_train_gene].reshape(-1, 1)
 
-    return adata, exp_value, enc_graph, dec_graph, unexp_edges, coexp_edges, uncoexp_edges
+    return adata, exp_value, enc_graph, dec_graph, unexp_edges, coexp_edges, uncoexp_edges
```

### Comparing `scgraphne-0.1.0/scgraphne/data/graph.py` & `scgraphne-0.1.1/scgraphne/data/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
-from sklearn.metrics.pairwise import cosine_similarity
 import torch
+from sklearn.metrics.pairwise import cosine_similarity
+
 
 def construct_gene_graph(gex_features, corr_method='cosine', corr_threshold=0.8):
     """Generate nodes, edges and edge weights for dataset.
 
     Parameters
     ----------
     gex_features: anndata.AnnData
@@ -47,10 +48,7 @@
     cell_cj, gene_cj = _calc_norm(graph['exp'].out_degrees()), _calc_norm(graph['reverse-exp'].out_degrees())
     graph.nodes['cell'].data.update({'ci': cell_ci, 'cj': cell_cj})
     graph.nodes['gene'].data.update({'ci': gene_ci, 'cj': gene_cj})
 
     if 'co-exp' in edge_types:
         gene_cii, gene_cjj = _calc_norm(graph['co-exp'].in_degrees()), _calc_norm(graph['co-exp'].out_degrees())
         graph.nodes['gene'].data.update({'cii': gene_cii, 'cjj': gene_cjj})
-
-
-
```

### Comparing `scgraphne-0.1.0/scgraphne/model/decoder.py` & `scgraphne-0.1.1/scgraphne/model/decoder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
+import dgl.function as fn
 import torch
 import torch.nn as nn
-
-import dgl.function as fn
 import torch.nn.functional as F
 
 class DotDecoder(nn.Module):
     def __init__(self):
         super().__init__()
         """Dotproduct decoder for link prediction
         predict link existence (not edge type)
@@ -17,29 +16,33 @@
         Paramters
         ---------
         graph : dgl.homograph
         c_feat : torch.FloatTensor
             cell features
         g_feat : torch.FloatTensor
             gene features
+        g_last : torch.FloatTensor
+            gene features of the last layer
+        ckey, gkey : str
+            target node types
 
         Returns
         -------
         pred : torch.FloatTensor
-            shape : (n_cells, 1)
+            shape : (n_edges, 1)
         """
 
         with graph.local_scope():
             graph.nodes[ckey].data['h'] = c_feat
             graph.nodes[gkey].data['h'] = g_feat
             graph.apply_edges(fn.u_dot_v('h', 'h', 'score'))
             pred = self.act(graph.edata['score'])
 
         return pred
-    
+
 
 class GMFDecoder(nn.Module):
     def __init__(self, feats_dim):
         super().__init__()
         """Dotproduct decoder for link prediction
         predict link existence (not edge type)
         """
@@ -50,19 +53,23 @@
         Paramters
         ---------
         graph : dgl.homograph
         c_feat : torch.FloatTensor
             cell features
         g_feat : torch.FloatTensor
             gene features
+        g_last : torch.FloatTensor
+            gene features of the last layer
+        ckey, gkey : str
+            target node types
 
         Returns
         -------
         pred : torch.FloatTensor
-            shape : (n_cells, 1)
+            shape : (n_edges, 1)
         """
 
         with graph.local_scope():
             graph.nodes[ckey].data['h'] = c_feat
             graph.nodes[gkey].data['h'] = g_feat
             graph.apply_edges(fn.u_mul_v('h', 'h', 'score'))
             pred = self.out(graph.edata['score'])
@@ -71,76 +78,87 @@
 
 
 class MeanAct(nn.Module):
     def __init__(self):
         super(MeanAct, self).__init__()
 
     def forward(self, x):
-        return torch.clamp(torch.exp(x)-1., min=1e-5, max=1e6)
+        return torch.clamp(torch.exp(x) - 1., min=1e-5, max=1e6)
+
 
 class DispAct(nn.Module):
     def __init__(self):
         super(DispAct, self).__init__()
 
     def forward(self, x):
         return torch.clamp(F.softplus(x), min=1e-4, max=1e4)
 
+
 class ZINBDecoder(nn.Module):
     def __init__(self, feats_dim, gene_similarity=False):
         super().__init__()
         """ZINB decoder for link prediction
         predict link existence (not edge type)
         """
         self.dec_mean = nn.Sequential(nn.Linear(feats_dim, 1), nn.Sigmoid())
         self.dec_disp = nn.Linear(feats_dim, 1)
         self.dec_disp_act = DispAct()
         self.dec_pi = nn.Sequential(nn.Linear(feats_dim, 1), nn.Sigmoid())
         self.dec_mean_act = MeanAct()
         self.gene_similarity = gene_similarity
-        
-    def forward(self, graph, c_feat, g_feat, g_last=None, ckey='cell', gkey='gene'):
 
+    def forward(self, graph, c_feat, g_feat, g_last=None, ckey='cell', gkey='gene'):
         """
         Paramters
         ---------
         graph : dgl.homograph
         c_feat : torch.FloatTensor
             cell features
         g_feat : torch.FloatTensor
             gene features
+        g_last : torch.FloatTensor
+            gene features of the last laye
+        ckey, gkey : str
+            target node types
 
         Returns
         -------
-        pred : torch.FloatTensor
-            shape : (n_cells, 1)
+        mu : torch.FloatTensor
+            the estimated mean of ZINB model shape : (n_edges, 1)
+        disp : torch.FloatTensor
+            the estimated dispersion of ZINB model shape : (n_edges, 1)
+        pi : torch.FloatTensor
+            the estimated dropout rate of ZINB model shape : (n_edges, 1)
+        ge_score : torch.FloatTensor
+            the predicted values of highly correlated gene edges when considering gene massage
         """
         ge_score = None
-        
+
         with graph.local_scope():
             graph.nodes[ckey].data['h'], graph.nodes[gkey].data['h'] = c_feat, g_feat
             graph.nodes[ckey].data['one'] = torch.ones([c_feat.shape[0], 1], device=c_feat.device)
             graph.nodes[gkey].data['one'] = torch.ones([g_feat.shape[0], 1], device=g_feat.device)
 
             exp_graph = graph['cell', 'exp', 'gene'] if self.gene_similarity else graph
-            
+
             exp_graph.apply_edges(fn.u_mul_v('h', 'h', 'h_d'))
             exp_graph.apply_edges(fn.u_mul_v('one', 'gs_factor', 'gs_factor'))
             exp_graph.apply_edges(fn.u_mul_v('cs_factor', 'one', 'cs_factor'))
-            
+
             h_d = exp_graph.edata['h_d']
             mu_ = self.dec_mean(h_d)
             disp_ = self.dec_disp(h_d)
             pi = self.dec_pi(h_d)
-            
+
             disp = self.dec_disp_act(exp_graph.edata['gs_factor'] * disp_)
             mu_ = exp_graph.edata['gs_factor'] * mu_
             mu = exp_graph.edata['cs_factor'] * self.dec_mean_act(mu_)
-            
+
             if self.gene_similarity:
                 co_exp_graph = graph['gene', 'co-exp', 'gene']
                 co_exp_graph.nodes[gkey].data['hh'] = g_last
                 co_exp_graph.apply_edges(fn.u_dot_v('hh', 'hh', 'h_d'))
                 h_d = co_exp_graph.edata['h_d']
-    
+
                 ge_score = F.sigmoid(h_d)
-                
-        return mu, disp, pi, ge_score
+
+        return mu, disp, pi, ge_score
```

### Comparing `scgraphne-0.1.0/scgraphne/model/scgraphne.py` & `scgraphne-0.1.1/scgraphne/model/scgraphne.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import torch
-from torch import nn
-
 import dgl
+import torch
 from dgl import function as fn
+from torch import nn
 from .decoder import DotDecoder, GMFDecoder, ZINBDecoder
 
-
 class LightGraphConv(nn.Module):
-    def __init__(self, drop_out = 0.1, gene2gene=False):
+    def __init__(self, drop_out=0.1, gene2gene=False):
         """Light Graph Convolution
 
         Paramters
         ---------
         drop_out : float
             dropout rate (neighborhood dropout)
+        gene2gene : boolean
+            whether to add gene massage to cell-gene bipartite graph
         """
         super().__init__()
         self.dropout = nn.Dropout(drop_out)
         self.gene2gene = gene2gene
 
     def forward(self, graph, feats):
         """Apply Light Graph Convoluiton to specific edge type {r}
@@ -62,48 +62,46 @@
             graph.srcdata['h'] = weighted_feats
 
             graph.update_all(fn.copy_src('h', 'm'), fn.sum('m', 'out'))
             out = torch.mul(graph.dstdata['out'], ci)
 
         return out
 
-class LightGCNLayer(nn.Module):
-    def __init__(self, drop_out = 0.1, alpha=None):
+
+class lightgraphconvlayer(nn.Module):
+    def __init__(self, drop_out=0.1, alpha=None):
         super().__init__()
-        """LightGCN Layer
+        """lightgraphconv layer
 
-        edge_types : list
-            all edge types
         drop_out : float
             dropout rate (feature dropout)
         alpha: float
             weight for gene massage
         """
         self.alpha = alpha
         conv = {}
 
         cell_to_gene_key = 'exp'
         gene_to_cell_key = 'reverse-exp'
         gene_to_gene_key = 'co-exp'
 
-
         # convolution on cell -> gene graph
         conv[cell_to_gene_key] = LightGraphConv(drop_out=drop_out)
 
         # convolution on gene -> cell graph
         conv[gene_to_cell_key] = LightGraphConv(drop_out=drop_out)
 
         # convolution on gene -> gene graph
         if self.alpha is not None:
             conv[gene_to_gene_key] = LightGraphConv(drop_out=drop_out, gene2gene=True)
 
         self.conv = dgl.nn.HeteroGraphConv(conv, aggregate='stack')
         self.feature_dropout = nn.Dropout(drop_out)
 
-    def forward(self, graph, c_feat, g_feat, ckey = 'cell', gkey = 'gene'):
+    def forward(self, graph, c_feat, g_feat, ckey='cell', gkey='gene'):
         """
         Paramters
         ---------
         graph : dgl.graph
         c_feat, g_feat : torch.FloatTensor
             node features
         ckey, gkey : str
@@ -124,42 +122,53 @@
         feats = {
             ckey: c_feat,
             gkey: g_feat
         }
 
         out = self.conv(graph, feats)
         c_feat = out[ckey].squeeze()
-        g_feat = self.alpha * out[gkey][:,0] + (1 - self.alpha) * out[gkey][:,1] if self.alpha is not None else out[gkey].squeeze()
+        g_feat = self.alpha * out[gkey][:, 0] + (1 - self.alpha) * out[gkey][:, 1] if self.alpha is not None else out[
+            gkey].squeeze()
 
         return c_feat, g_feat
 
+
 class scGraphNE(nn.Module):
     def __init__(self,
                  n_layers,
                  n_cells,
                  n_genes,
                  drop_out,
                  feats_dim,
-                 decoder = 'Dot',
-                 learnable_weight = False,
-                 gene_similarity = False,
+                 decoder='ZINB',
+                 learnable_weight=False,
+                 gene_similarity=False,
                  alpha=0.9):
         super().__init__()
-        """LightGCN: Simplifying and Powering Graph Convolution Network for Recommendation
-        paper : https://arxiv.org/pdf/2002.02126.pdf
+        """scGraphNE: a novel scRNA-seq representation learning method based on graph node embedding
 
         n_layers : int
-            number of GCMC layers
-        edge_types : list
-            all edge types
+            number of GCN layers
+        n_cells : int
+            number of cells
+        n_genes : int
+            number of genes   
         drop_out : float
             dropout rate (neighbors)
+        feats_dim : int
+            node feature dimension
+        decoder = 'ZINB'
+            structure of decoder. default is 'ZINB', optionally input 'Dot', 'GMF' or 'ZINB'
         learnable_weight : boolean
-            whether to learn weights for embedding aggregation
-            if False, use 1/n_layers
+            whether to learn weights for embedding aggregation, if False, use 1/n_layers
+        gene_similarity : boolean
+           whether to consider gene massage
+        alpha: float
+            weight for gene massage
+        
         """
         self.gene_similarity = gene_similarity
         self.alpha = alpha if gene_similarity else None
 
         self.n_cells = n_cells
         self.n_genes = n_genes
 
@@ -168,20 +177,20 @@
 
         nn.init.xavier_uniform_(self.cell_feature)
         nn.init.xavier_uniform_(self.gene_feature)
 
         self.n_layers = n_layers
         self.encoders = nn.ModuleList()
         for _ in range(n_layers):
-            self.encoders.append(LightGCNLayer(drop_out=drop_out, alpha=self.alpha))
+            self.encoders.append(lightgraphconvlayer(drop_out=drop_out, alpha=self.alpha))
 
         if self.n_layers == 2:
             self.weights = torch.tensor([1., 1. / 2, 1. / 2])
         else:
-            self.weights = torch.ones([self.n_layers+1, 1]) / (self.n_layers+1)
+            self.weights = torch.ones([self.n_layers + 1, 1]) / (self.n_layers + 1)
 
         if learnable_weight:
             self.weights = nn.Parameter(self.weights)
 
         if decoder == 'Dot':
             self.decoder = DotDecoder()
         elif decoder == 'GMF':
@@ -198,48 +207,41 @@
     def encode(self, graph, ckey='cell', gkey='gene'):
         c_feat, g_feat = self.cell_feature, self.gene_feature
         c_hidden, g_hidden = self.weights[0] * c_feat, self.weights[0] * g_feat
         for w, encoder in zip(self.weights[1:], self.encoders):
             c_feat, g_feat = encoder(graph, c_feat, g_feat, ckey, gkey)
             c_hidden = c_hidden + w * c_feat
             g_hidden = g_hidden + w * g_feat
-        
+
         return c_hidden, g_hidden, c_feat, g_feat
 
     def decode(self, pos_graph, neg_graph, c_feat, g_feat, g_last, ckey, gkey):
         pos_pre = self.decoder(pos_graph, c_feat, g_feat, g_last, ckey, gkey)
         neg_pre = self.decoder(neg_graph, c_feat, g_feat, g_last, ckey, gkey)
         return pos_pre, neg_pre
 
     def forward(self,
                 enc_graph,
                 pos_graph,
-                neg_graph = None,
-                ckey = 'cell',
-                gkey = 'gene'):
+                neg_graph=None,
+                ckey='cell',
+                gkey='gene'):
         """
         Parameters
         ----------
-        enc_graph : dgl.graph
-        dec_graph : dgl.homograph
+        enc_graph, pos_graph, neg_graph: dgl.graph
+            constructed graphs
 
-        Notes
-        -----
-        1. LightGCN encoder
-            1 ) message passing
-                MP_{j -> i, r} = h_{j} / ( N_{i, r} * N_{j, r} )
-            2 ) aggregation
-                \sum_{j \in N(i), r} MP_{j -> i, r}
-
-        2. final features
-            cell_{i} = mean( h_{i, layerself.cell_feature = {Parameter: (943, 75)} Parameter containing:\ntensor([[ 0.0007, -0.0501,  0.0644,  ..., -0.0756,  0.0526, -0.0293],\n        [ 0.0743, -0.0693, -0.0382,  ..., -0.0612,  0.0300,  0.0068],\n        [-0.0341, -0.0038,  0.0670,  ..., -0.0470, -0.0631, -0.0403],\n        ...,\n        [-0… View_1}, h_{i, layer_2}, ... )
-            gene_{j} = mean( h_{j, layer_1}, h_{j, layer_2}, ... )
+        ckey, gkey : str
+            target node types
 
-        3. Bilinear decoder
-            logits_{i, j, r} = c_feat_{i} @ Q_r @ g_feat_{j}
+        Returns
+        -------
+        pos_pre, neg_pre : torch.FloatTensor
+            edge predictions of positive and negative graph in the decoder
         """
 
         c_feat, g_feat, c_last, g_last = self.encode(enc_graph, ckey, gkey)
         if neg_graph is not None:
             return self.decode(pos_graph, neg_graph, c_feat, g_feat, g_last, ckey, gkey)
 
         return self.decoder(pos_graph, c_feat, g_feat, g_last, ckey, gkey)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scgraphne-0.1.0/scgraphne/run_scgraphne.py` & `scgraphne-0.1.1/scgraphne/run_scgraphne.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,60 +1,62 @@
 #!/usr/bin/env python
 # coding: utf-8
+import gc
+
 import dgl
-import torch
-from torch import nn, optim
 import numpy as np
 import scanpy as sc
-import gc
+import torch
+from torch import nn, optim
 
-from .model import scGraphNE
 from .data import make_graph
+from .model import scGraphNE
 from .utils import calculate_metric, ZINBLoss, kmeans, louvain
 
+
 def run_scgraphne(adata: sc.AnnData,
-                    n_clusters = None,
-                    cl_type = None,
-                    gene_similarity: bool = False,
-                    alpha=0.9,
-                    n_layers: int = 2,
-                    feats_dim: int = 64,
-                    drop_out: float = 0.,
-                    gamma: int = 1,
-                    decoder = 'ZINB',
-                    lr: float = 0.1,
-                    iteration: int = 200,
-                    log_interval: int = 5,
-                    resolution: float = 1,
-                    sample_rate: float = 0.1,
-                    use_rep: str = 'feat',
-                    verbose: bool = True,
-                    return_all: bool = False,
-                    impute: bool = False
-                    ):
+                  n_clusters=None,
+                  cl_type=None,
+                  gene_similarity: bool = False,
+                  alpha=0.9,
+                  n_layers: int = 2,
+                  feats_dim: int = 64,
+                  drop_out: float = 0.,
+                  gamma: int = 1,
+                  decoder='ZINB',
+                  lr: float = 0.1,
+                  iteration: int = 200,
+                  log_interval: int = 5,
+                  resolution: float = 1,
+                  sample_rate: float = 0.1,
+                  use_rep: str = 'feat',
+                  verbose: bool = True,
+                  return_all: bool = False,
+                  impute: bool = False
+                  ):
     """
         Train scGraphNE.
         Parameters
         ----------
         adata
             AnnData object of scanpy package.
         n_clusters
             Number of true cell type. If provided, you can select KMeans for clustering.
         cl_type
             Cell type information. If provided, calculate ARI and NMI after clustering.
+        gene_similarity
+            If True,consider correlation between genes and change bipartite graph structure.
+        alpha
+            When considering correlation between genes, set the proportional coefficient of BCE loss.
         n_layers
             Number of graph convolution layers in encoder.
         feats_dim
             The embedding dimensions of cells or genes in latent space.
         drop_out
             The probability of randomly dropping node embedding values.
-        gene_similarity
-            If True,consider correlation between genes and change bipartite graph structure.
-        alpha
-            When considering correlation between genes, set the proportional coefficient of BCE loss.
         gamma
             The proportional coefficient of ZINB loss.
         decoder
             Structure of decoder. Default is 'ZINB', optionally input 'Dot', 'GMF' or 'ZINB'.
         lr
             Learning rate for AdamOptimizer.
         iteration
@@ -62,21 +64,21 @@
         log_interval
             how many iterations to wait before logging training status.
         resolution
             The resolution parameter of sc.tl.louvain for clustering.Default is 1.
         sample_rate
             The edge sampling rate of bipartite graph in decoder.
         use_rep
-            Use the indicated representation. 'X' or any key for .obsm is valid. Here we
-            use the cell embedding in the hidden space and store it in adata.obsm['feat'].
-        record_time
+            Use the indicated representation. 'X' or any key for .obsm is valid. Here we use the cell embedding in the hidden space and store it in adata.obsm['feat'].
+        verbose
+            If True, show details when running.
+        return_all
             If True, no clustering is performed during model training to save runtime.
         impute
-            Whether to output reconstructed gene expression matrix(optional). If True,
-            return imputed expression value and store it in adata.obsm['imputed'].
+            Whether to output reconstructed gene expression matrix(optional). If True, return imputed expression value and store it in adata.obsm['imputed'].
 
         Returns
         -------
         adata
             AnnData object of scanpy package. Cell embedding and louvain clustering result will be stored
             in adata.obsm['feat'] and adata.obs['louvain']
         record
@@ -93,17 +95,18 @@
     cell_type = adata.obs[cl_type].values if cl_type else None
     raw_exp = True if decoder == 'ZINB' else False
     n_cells, n_genes = adata.X.shape
 
     if cell_type is not None:
         n_clusters = len(np.unique(cell_type))
 
-    adata, exp_value, enc_graph, exp_dec_graph_, unexp_edges, coexp_edges, uncoexp_edges = make_graph(adata, raw_exp, gene_similarity)
+    adata, exp_value, enc_graph, exp_dec_graph_, unexp_edges, coexp_edges, uncoexp_edges = make_graph(adata, raw_exp,
+                                                                                                      gene_similarity)
 
-    n_pos_edges, n_neg_edges = int(sample_rate*len(exp_value)), int(sample_rate*len(exp_value))
+    n_pos_edges, n_neg_edges = int(sample_rate * len(exp_value)), int(sample_rate * len(exp_value))
     n_neg_genes = len(coexp_edges[0]) if gene_similarity else None
     enc_graph, exp_value = enc_graph.to(device), torch.tensor(exp_value, device=device)
 
     #######################   Prepare models   #######################
     model = scGraphNE(n_layers=n_layers,
                       n_cells=n_cells,
                       n_genes=n_genes,
@@ -133,50 +136,48 @@
     all_uncoexp_index = np.arange(len(uncoexp_edges[0])) if gene_similarity else None
 
     if sample_rate == 1:
         pos_graph, pos_value = exp_dec_graph_.to(device), exp_value
 
     ### Save time by not performing clustering if time would be recorded during training.
     for iter_idx in range(iteration):
-        # if iter_idx % (log_interval * 5) == 0:
-        # if iter_idx % log_interval == 0:
-        # if verbose and (iter_idx + log_interval) % log_interval == 0:
-            # Sample un-expressed / un-co-expressed edges, construct negative graph
+        # Sample un-expressed / un-co-expressed edges, construct negative graph
         neg_edges = {}
 
         unexp_sample_index = np.random.choice(all_unexp_index, n_neg_edges)
         neg_edges[('cell', 'exp', 'gene')] = (unexp_edges[0][unexp_sample_index], unexp_edges[1][unexp_sample_index])
         if gene_similarity:
             uncoexp_sample_index = np.random.choice(all_uncoexp_index, n_neg_genes)
-            neg_edges[('gene', 'co-exp', 'gene')] = (uncoexp_edges[0][uncoexp_sample_index], uncoexp_edges[1][uncoexp_sample_index])
+            neg_edges[('gene', 'co-exp', 'gene')] = (
+            uncoexp_edges[0][uncoexp_sample_index], uncoexp_edges[1][uncoexp_sample_index])
 
         neg_graph = dgl.heterograph(neg_edges, num_nodes_dict={'cell': n_cells, 'gene': n_genes}).to(device)
         # Add cell/gene size factor to negative graph
         if decoder == 'ZINB':
             neg_graph.nodes['cell'].data['cs_factor'] = exp_dec_graph_.nodes['cell'].data['cs_factor'].to(device)
             neg_graph.nodes['gene'].data['gs_factor'] = exp_dec_graph_.nodes['gene'].data['gs_factor'].to(device)
 
         # Sample expressed, construct positive graph
         if sample_rate != 1:
             pos_edges = {}
 
             exp_sample_index = np.random.choice(all_exp_index, n_pos_edges)
             pos_value = exp_value[exp_sample_index]
             exp_dec_edges = exp_dec_graph_[('cell', 'exp', 'gene')].edges()
-            pos_edges[('cell', 'exp', 'gene')] = (exp_dec_edges[0][exp_sample_index], exp_dec_edges[1][exp_sample_index])
+            pos_edges[('cell', 'exp', 'gene')] = (
+            exp_dec_edges[0][exp_sample_index], exp_dec_edges[1][exp_sample_index])
             if gene_similarity: pos_edges[('gene', 'co-exp', 'gene')] = coexp_edges
 
             pos_graph = dgl.heterograph(pos_edges, num_nodes_dict={'cell': n_cells, 'gene': n_genes}).to(device)
 
             # Add cell/gene size factor to positive graph
             if decoder == 'ZINB':
                 pos_graph.nodes['cell'].data['cs_factor'] = exp_dec_graph_.nodes['cell'].data['cs_factor'].to(device)
                 pos_graph.nodes['gene'].data['gs_factor'] = exp_dec_graph_.nodes['gene'].data['gs_factor'].to(device)
 
-
         # Feed forward
         pos_pre, neg_pre = model(enc_graph, pos_graph, neg_graph)
 
         # Calculate loss for regularization
         reg_loss = (1 / 2) * (model.cell_feature.norm(2).pow(2) +
                               model.gene_feature.norm(2).pow(2)) / float(n_cells + n_genes)
 
@@ -185,20 +186,18 @@
             loss_exp = criterion(pos_pre, pos_value)
             loss_unexp = criterion(neg_pre, torch.zeros_like(neg_pre))
 
         else:
             loss_exp = criterion(pos_pre[0], pos_pre[1], pos_pre[2], pos_value)
             loss_unexp = criterion(neg_pre[0], neg_pre[1], neg_pre[2])
 
-            # ridge = torch.square(pos_pre[2]).mean() + torch.square(neg_pre[2]).mean()
-            # reg_loss = reg_loss + 10 * ridge
             ridge = torch.square(pos_pre[2]).mean() + torch.square(neg_pre[2]).mean()
             reg_loss = reg_loss + 1e-3 * ridge
 
-        loss = loss_exp + gamma * loss_unexp + 0.0001*reg_loss
+        loss = loss_exp + gamma * loss_unexp + 0.0001 * reg_loss
 
         # Calculate loss for (un)co-expressed gene
         if gene_similarity:
             loss_gene = gene_cls(pos_pre[3], torch.ones_like(pos_pre[3]))
             loss_ungene = gene_cls(neg_pre[3], torch.zeros_like(neg_pre[3]))
 
             loss = loss + loss_gene + loss_ungene
@@ -212,74 +211,72 @@
 
         all_loss.append(loss.item())
 
         optimizer.zero_grad()
         loss.backward()
         optimizer.step()
 
-
         if verbose and (iter_idx + 1) % log_interval == 0:
             print(
                 "[{}/{}-iter] | [train] exp loss : {:.4f}, unexp loss : {:.4f}"
                 .format(iter_idx + 1, iteration, count_loss_exp / log_interval, count_loss_unexp / log_interval) +
                 (", gene loss : {:.4f}, ungene loss : {:.4f}".
-                 format(count_loss_gene / log_interval, count_loss_unexp / log_interval)if gene_similarity else "")
-                )
+                 format(count_loss_gene / log_interval, count_loss_unexp / log_interval) if gene_similarity else "")
+            )
 
             count_loss_exp, count_loss_unexp, count_loss_gene, count_loss_ungene = 0, 0, 0, 0
 
-
-        if verbose and cell_type is not None and (iter_idx+1) % (log_interval * 5) == 0:
+        if verbose and cell_type is not None and (iter_idx + 1) % (log_interval * 5) == 0:
             model.eval()
             with torch.no_grad():
                 c_feat, g_feat, c_last, g_last = model.encode(enc_graph)
             model.train()
-            
+
             # Cell embeddings
             adata.obsm['e0'] = model.cell_feature.data.cpu().numpy()  # Return initial cell embedding
             adata.obsm['e2'] = c_last.cpu().numpy()  # Return the final layer of cell embedding
             adata.obsm['feat'] = c_feat.cpu().numpy()  # Return the weighted cell embeddings
-            
+
             # kmeans
-            adata = kmeans(adata, n_clusters, use_rep = use_rep)
+            adata = kmeans(adata, n_clusters, use_rep=use_rep)
             y_pred_k = np.array(adata.obs['kmeans'])
 
             # louvain
-            adata = louvain(adata, resolution = resolution,use_rep = use_rep)
+            adata = louvain(adata, resolution=resolution, use_rep=use_rep)
             y_pred_l = np.array(adata.obs['louvain'])
             print('Number of clusters identified by Louvain is {}'.format(len(np.unique(y_pred_l))))
 
             nmi_k, ari_k = calculate_metric(cell_type, y_pred_k)
-            print('Clustering Kmeans %d: NMI= %.4f, ARI= %.4f' % (iter_idx+1, nmi_k, ari_k))
+            print('Clustering Kmeans %d: NMI= %.4f, ARI= %.4f' % (iter_idx + 1, nmi_k, ari_k))
 
             nmi_l, ari_l = calculate_metric(cell_type, y_pred_l)
-            print('Clustering Louvain %d: NMI= %.4f, ARI= %.4f' % (iter_idx+1, nmi_l, ari_l))
+            print('Clustering Louvain %d: NMI= %.4f, ARI= %.4f' % (iter_idx + 1, nmi_l, ari_l))
 
             all_ari_k.append(ari_k)
             all_ari_l.append(ari_l)
             all_nmi_k.append(nmi_k)
             all_nmi_l.append(nmi_l)
 
             if ari_k > best_ari_k:
                 best_ari_k = ari_k
                 best_nmi_k = nmi_k
-                best_iter_k = iter_idx+1
+                best_iter_k = iter_idx + 1
 
             if ari_l > best_ari_l:
                 best_ari_l = ari_l
                 best_nmi_l = nmi_l
-                best_iter_l = iter_idx+1
+                best_iter_l = iter_idx + 1
 
     ## End of training
     model.eval()
     with torch.no_grad():
         c_feat, g_feat, c_last, g_last = model.encode(enc_graph)
-    
+
     adata.obsm['e0'] = model.cell_feature.data.cpu().numpy()  # Return initial cell embedding
-    adata.obsm['e2'] = c_last.cpu().numpy()     # Return the final layer of cell embedding
+    adata.obsm['e2'] = c_last.cpu().numpy()  # Return the final layer of cell embedding
     adata.obsm['feat'] = c_feat.cpu().numpy()  # Return the weighted cell embeddings
     adata.varm['feat'] = g_last.cpu().numpy()  # Return the final layer's gene embeddings
 
     if verbose and cell_type is not None:
         print(
             f'[END] For Kmeans, Best Iter : {best_iter_k} Best ARI : {best_ari_k:.4f}, Best NMI : {best_nmi_k:.4f}')
         print(
```

### Comparing `scgraphne-0.1.0/scgraphne/utils/metric.py` & `scgraphne-0.1.1/scgraphne/utils/metric.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,58 +1,63 @@
 import numpy as np
 import scanpy as sc
 from scipy.optimize import linear_sum_assignment
-from sklearn.cluster import KMeans
-from sklearn import metrics
 from scipy.stats import pearsonr
+from sklearn import metrics
+from sklearn.cluster import KMeans
 from sklearn.metrics.pairwise import cosine_similarity
 
+
 def pearsonr_error(y, h):
     res = []
     if len(y.shape) < 2:
         y = y.reshape((1, -1))
         h = h.reshape((1, -1))
 
     for i in range(y.shape[0]):
         res.append(pearsonr(y[i], h[i])[0])
     return np.mean(res)
 
+
 def cosine_similarity_score(y, h):
     if len(y.shape) < 2:
         y = y.reshape((1, -1))
         h = h.reshape((1, -1))
     cos = cosine_similarity(y, h)
     res = []
     for i in range(len(cos)):
         res.append(cos[i][i])
     return np.mean(res)
 
+
 def kmeans(adata, n_clusters, use_rep=None):
-    k_means = KMeans(n_clusters, n_init=20,random_state=0)
+    k_means = KMeans(n_clusters, n_init=20, random_state=0)
     y_pred = k_means.fit_predict(adata.obsm[use_rep])
     adata.obs['kmeans'] = y_pred
     adata.obs['kmeans'] = adata.obs['kmeans'].astype(str).astype('category')
     return adata
 
-def louvain(adata, resolution = None, use_rep=None):
+
+def louvain(adata, resolution=None, use_rep=None):
     sc.pp.neighbors(adata, use_rep=use_rep)
     sc.tl.louvain(adata, resolution=resolution)
     return adata
 
+
 def cluster_acc(y_true, y_pred):
     y_true = y_true.astype(np.float64).astype(np.int64)
     y_pred = y_pred.astype(np.float64).astype(np.int64)
     assert y_pred.size == y_true.size
     D = max(y_pred.max(), y_true.max()) + 1
     w = np.zeros((D, D), dtype=np.int64)
     for i in range(y_pred.size):
         w[y_pred[i], y_true[i]] += 1
 
-    row_ind,col_ind = linear_sum_assignment(w.max() - w)
+    row_ind, col_ind = linear_sum_assignment(w.max() - w)
     return w[row_ind, col_ind].sum() * 1.0 / y_pred.size
 
+
 def calculate_metric(pred, label):
     nmi = np.round(metrics.normalized_mutual_info_score(label, pred), 4)
     ari = np.round(metrics.adjusted_rand_score(label, pred), 4)
 
     return nmi, ari
-
```

### Comparing `scgraphne-0.1.0/scgraphne/utils/utils.py` & `scgraphne-0.1.1/scgraphne/utils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
-from sklearn import metrics
-from scipy.optimize import linear_sum_assignment
 import torch
+from scipy.optimize import linear_sum_assignment
+from sklearn import metrics
 from torch import nn
 
 
 class ZINBLoss(nn.Module):
     def __init__(self):
         super().__init__()
 
@@ -19,14 +19,15 @@
         t2 = (disp + x) * torch.log(1.0 + (mean / (disp + eps))) + (x * (torch.log(disp + eps) - torch.log(mean + eps)))
         nb_final = t1 + t2
 
         nb_case = nb_final - torch.log(1.0 - pi + eps)
 
         return nb_case.mean()
 
+
 def cluster_acc(y_true, y_pred):
     """
     Calculate clustering accuracy. Require scikit-learn installed
     # Arguments
         y: true labels, numpy.array with shape `(n_samples,)`
         y_pred: predicted labels, numpy.array with shape `(n_samples,)`
     # Return
@@ -38,17 +39,16 @@
     y_pred = y_pred.astype(np.float64).astype(np.int64)
     assert y_pred.size == y_true.size
     D = max(y_pred.max(), y_true.max()) + 1
     w = np.zeros((D, D), dtype=np.int64)
     for i in range(y_pred.size):
         w[y_pred[i], y_true[i]] += 1
 
-    row_ind,col_ind = linear_sum_assignment(w.max() - w)
+    row_ind, col_ind = linear_sum_assignment(w.max() - w)
     return w[row_ind, col_ind].sum() * 1.0 / y_pred.size
 
 
 def calculate_metric(pred, label):
     nmi = np.round(metrics.normalized_mutual_info_score(label, pred), 5)
     ari = np.round(metrics.adjusted_rand_score(label, pred), 5)
 
     return nmi, ari
-
```

### Comparing `scgraphne-0.1.0/scgraphne.egg-info/PKG-INFO` & `scgraphne-0.1.1/scgraphne.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: scgraphne
-Version: 0.1.0
+Version: 0.1.1
 Summary: scGraphNE: a novel scRNA-seq representation learning method based on graph node embedding
 Home-page: https://github.com/sldyns/scGraphNE
 Author: Kun Qian, Ting Li
 Author-email: kun_qian@foxmail.com
 Maintainer: Kun Qian
 Maintainer-email: kun_qian@foxmail.com
 License: MIT Licence
 Description: # scGraphNE: a novel scRNA-seq representation learning method based on graph node embedding
         
         ## Overview
         
-        ![alt](overview.svg)
+        ![alt](overview.png)
         
         scGraphNE is a graph autoencoder network where the encoder based on multi-layer graph convolutional networks extracts high-order representations of cells and genes from the cell-gene bipartite graph, and the decoder based on the ZINB model uses these representations to reconstruct the gene expression matrix. By virtue of a model-driven self-supervised training paradigm, scGraphNE can effectively learn low-dimensional representations of both cells and genes, amenable to diverse downstream analytical tasks.
         
         ## Installation
         
         Please install `scGraphNE` from pypi with:
```

### Comparing `scgraphne-0.1.0/setup.py` & `scgraphne-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     with open(os.path.join(path, 'README.md'), "r", encoding='utf-8') as f:
         long_description = f.read()
 except Exception as e:
     long_description = "scGraphNE: a novel scRNA-seq representation learning method based on graph node embedding"
 
 setup(
     name="scgraphne",
-    version="0.1.0",
+    version="0.1.1",
     keywords=["single-cell RNA-sequencing", "Graph node embedding", "Dimensionality reduction"],
     description="scGraphNE: a novel scRNA-seq representation learning method based on graph node embedding",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="MIT Licence",
 
     url="https://github.com/sldyns/scGraphNE",
```

