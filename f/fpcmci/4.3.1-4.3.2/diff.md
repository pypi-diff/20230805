# Comparing `tmp/fpcmci-4.3.1.tar.gz` & `tmp/fpcmci-4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpcmci-4.3.1.tar", last modified: Sat Aug  5 11:20:41 2023, max compression
+gzip compressed data, was "fpcmci-4.3.2.tar", last modified: Sat Aug  5 13:45:18 2023, max compression
```

## Comparing `fpcmci-4.3.1.tar` & `fpcmci-4.3.2.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:20:41.917014 fpcmci-4.3.1/
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     8517 2023-08-05 11:20:41.917014 fpcmci-4.3.1/PKG-INFO
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     6787 2023-08-05 11:19:46.000000 fpcmci-4.3.1/README.md
-drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:20:41.917014 fpcmci-4.3.1/fpcmci/
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     1066 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/CPrinter.py
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)    11125 2023-08-05 11:14:12.000000 fpcmci-4.3.1/fpcmci/FPCMCI.py
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)    14739 2023-08-05 11:14:12.000000 fpcmci-4.3.1/fpcmci/PCMCI.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)      240 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/__init__.py
-drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:20:41.917014 fpcmci-4.3.1/fpcmci/basics/
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)       72 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/basics/__init__.py
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)      445 2023-08-05 11:14:12.000000 fpcmci-4.3.1/fpcmci/basics/constants.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)      506 2023-08-05 10:53:21.000000 fpcmci-4.3.1/fpcmci/basics/logger.py
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)      812 2023-08-05 11:14:12.000000 fpcmci-4.3.1/fpcmci/basics/utils.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     8790 2023-08-05 10:53:21.000000 fpcmci-4.3.1/fpcmci/causal_graph.py
-drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:20:41.917014 fpcmci-4.3.1/fpcmci/graph/
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)    15964 2023-08-05 11:14:12.000000 fpcmci-4.3.1/fpcmci/graph/DAG.py
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     3681 2023-08-05 11:14:12.000000 fpcmci-4.3.1/fpcmci/graph/Node.py
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)       43 2023-08-05 11:14:12.000000 fpcmci-4.3.1/fpcmci/graph/__init__.py
-drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:20:41.917014 fpcmci-4.3.1/fpcmci/preprocessing/
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     2304 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/preprocessing/Subsampler.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)        0 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/preprocessing/__init__.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     4568 2023-08-05 10:53:21.000000 fpcmci-4.3.1/fpcmci/preprocessing/data.py
-drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:20:41.917014 fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     3649 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/EntropyBasedMethod.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)      639 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/Static.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)      781 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/SubsamplingMethod.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     1798 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/WSDynamic.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     2600 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/WSFFTStatic.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     1765 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/WSStatic.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)      267 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/__init__.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     2493 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/moving_window.py
-drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:20:41.917014 fpcmci-4.3.1/fpcmci/selection_methods/
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     1400 2023-08-05 11:14:12.000000 fpcmci-4.3.1/fpcmci/selection_methods/Corr.py
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     2220 2023-08-05 11:14:12.000000 fpcmci-4.3.1/fpcmci/selection_methods/MI.py
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     2698 2023-08-05 11:14:12.000000 fpcmci-4.3.1/fpcmci/selection_methods/ParCorr.py
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     3457 2023-08-05 11:14:12.000000 fpcmci-4.3.1/fpcmci/selection_methods/SelectionMethod.py
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     3803 2023-08-05 11:14:12.000000 fpcmci-4.3.1/fpcmci/selection_methods/TE.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)      134 2023-07-26 08:29:42.000000 fpcmci-4.3.1/fpcmci/selection_methods/__init__.py
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)       17 2023-08-05 11:19:32.000000 fpcmci-4.3.1/fpcmci/version.py
-drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:20:41.917014 fpcmci-4.3.1/fpcmci.egg-info/
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     8517 2023-08-05 11:20:41.000000 fpcmci-4.3.1/fpcmci.egg-info/PKG-INFO
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     1204 2023-08-05 11:20:41.000000 fpcmci-4.3.1/fpcmci.egg-info/SOURCES.txt
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)        1 2023-08-05 11:20:41.000000 fpcmci-4.3.1/fpcmci.egg-info/dependency_links.txt
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)      154 2023-08-05 11:20:41.000000 fpcmci-4.3.1/fpcmci.egg-info/requires.txt
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)        7 2023-08-05 11:20:41.000000 fpcmci-4.3.1/fpcmci.egg-info/top_level.txt
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)       38 2023-08-05 11:20:41.917014 fpcmci-4.3.1/setup.cfg
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     1431 2023-08-05 11:14:13.000000 fpcmci-4.3.1/setup.py
+drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 13:45:18.531322 fpcmci-4.3.2/
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     8560 2023-08-05 13:45:18.531322 fpcmci-4.3.2/PKG-INFO
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     6822 2023-08-05 13:31:12.000000 fpcmci-4.3.2/README.md
+drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 13:45:18.527322 fpcmci-4.3.2/fpcmci/
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     1066 2023-05-29 18:54:02.000000 fpcmci-4.3.2/fpcmci/CPrinter.py
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)    11125 2023-08-05 13:25:12.000000 fpcmci-4.3.2/fpcmci/FPCMCI.py
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)    14519 2023-08-05 13:24:08.000000 fpcmci-4.3.2/fpcmci/PCMCI.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)      240 2023-05-29 18:54:02.000000 fpcmci-4.3.2/fpcmci/__init__.py
+drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 13:45:18.527322 fpcmci-4.3.2/fpcmci/basics/
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)       72 2023-05-29 18:54:02.000000 fpcmci-4.3.2/fpcmci/basics/__init__.py
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)      445 2023-08-05 11:14:12.000000 fpcmci-4.3.2/fpcmci/basics/constants.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)      506 2023-08-05 10:53:21.000000 fpcmci-4.3.2/fpcmci/basics/logger.py
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)      812 2023-08-05 11:14:12.000000 fpcmci-4.3.2/fpcmci/basics/utils.py
+drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 13:45:18.527322 fpcmci-4.3.2/fpcmci/graph/
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)    17896 2023-08-05 13:41:19.000000 fpcmci-4.3.2/fpcmci/graph/DAG.py
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     4059 2023-08-05 13:29:08.000000 fpcmci-4.3.2/fpcmci/graph/Node.py
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)       38 2023-08-05 12:46:04.000000 fpcmci-4.3.2/fpcmci/graph/__init__.py
+drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 13:45:18.527322 fpcmci-4.3.2/fpcmci/preprocessing/
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     2304 2023-05-29 18:54:02.000000 fpcmci-4.3.2/fpcmci/preprocessing/Subsampler.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)        0 2023-05-29 18:54:02.000000 fpcmci-4.3.2/fpcmci/preprocessing/__init__.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     4568 2023-08-05 10:53:21.000000 fpcmci-4.3.2/fpcmci/preprocessing/data.py
+drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 13:45:18.527322 fpcmci-4.3.2/fpcmci/preprocessing/subsampling_methods/
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     3649 2023-05-29 18:54:02.000000 fpcmci-4.3.2/fpcmci/preprocessing/subsampling_methods/EntropyBasedMethod.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)      639 2023-05-29 18:54:02.000000 fpcmci-4.3.2/fpcmci/preprocessing/subsampling_methods/Static.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)      781 2023-05-29 18:54:02.000000 fpcmci-4.3.2/fpcmci/preprocessing/subsampling_methods/SubsamplingMethod.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     1798 2023-05-29 18:54:02.000000 fpcmci-4.3.2/fpcmci/preprocessing/subsampling_methods/WSDynamic.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     2600 2023-05-29 18:54:02.000000 fpcmci-4.3.2/fpcmci/preprocessing/subsampling_methods/WSFFTStatic.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     1765 2023-05-29 18:54:02.000000 fpcmci-4.3.2/fpcmci/preprocessing/subsampling_methods/WSStatic.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)      267 2023-05-29 18:54:02.000000 fpcmci-4.3.2/fpcmci/preprocessing/subsampling_methods/__init__.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     2493 2023-05-29 18:54:02.000000 fpcmci-4.3.2/fpcmci/preprocessing/subsampling_methods/moving_window.py
+drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 13:45:18.531322 fpcmci-4.3.2/fpcmci/selection_methods/
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     1400 2023-08-05 11:14:12.000000 fpcmci-4.3.2/fpcmci/selection_methods/Corr.py
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     2220 2023-08-05 11:14:12.000000 fpcmci-4.3.2/fpcmci/selection_methods/MI.py
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     2698 2023-08-05 11:14:12.000000 fpcmci-4.3.2/fpcmci/selection_methods/ParCorr.py
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     3457 2023-08-05 11:14:12.000000 fpcmci-4.3.2/fpcmci/selection_methods/SelectionMethod.py
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     3803 2023-08-05 11:14:12.000000 fpcmci-4.3.2/fpcmci/selection_methods/TE.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)      134 2023-07-26 08:29:42.000000 fpcmci-4.3.2/fpcmci/selection_methods/__init__.py
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)       17 2023-08-05 13:30:52.000000 fpcmci-4.3.2/fpcmci/version.py
+drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 13:45:18.527322 fpcmci-4.3.2/fpcmci.egg-info/
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     8560 2023-08-05 13:45:18.000000 fpcmci-4.3.2/fpcmci.egg-info/PKG-INFO
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     1181 2023-08-05 13:45:18.000000 fpcmci-4.3.2/fpcmci.egg-info/SOURCES.txt
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)        1 2023-08-05 13:45:18.000000 fpcmci-4.3.2/fpcmci.egg-info/dependency_links.txt
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)      154 2023-08-05 13:45:18.000000 fpcmci-4.3.2/fpcmci.egg-info/requires.txt
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)        7 2023-08-05 13:45:18.000000 fpcmci-4.3.2/fpcmci.egg-info/top_level.txt
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)       38 2023-08-05 13:45:18.531322 fpcmci-4.3.2/setup.cfg
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     1431 2023-08-05 11:14:13.000000 fpcmci-4.3.2/setup.py
```

### Comparing `fpcmci-4.3.1/PKG-INFO` & `fpcmci-4.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fpcmci
-Version: 4.3.1
+Version: 4.3.2
 Summary: A causal discovery Python package
 Home-page: https://github.com/lcastri/fpcmci
 Author: Luca Castri
 Author-email: lucacastri94@gmail.com
 License: UNKNOWN
 Description: # <img src="https://github.com/lcastri/fpcmci/raw/developer/docs/assets/icon.png" width="25"> FPCMCI - Filtered PCMCI
         
@@ -136,14 +136,15 @@
         ```
         
         
         ## Recent changes
         
         | Version | Changes |
         | :---: | ----------- |
+        | 4.3.2 | documentation improved |
         | 4.3.1 | README and index.md updated |
         | 4.3.0 | alpha level fix in PCMCI<br>timeseries_dag fix<br>adaptation to DAG structure |
         | 4.2.1 | fixed dependency error in setup.py |
         | 4.2.0 | causal model with only selected features fix<br>adapted to tigramite 5.2<br>get_causal_matrix FPCMCI method added<br>f_alpha and pcmci_alpha instead of alpha<br>requirements changed<br>tutorials adapted to new version |
         | 4.1.2 | tutorials adapted to 4.1.1 and get_SCM method added in FPCMCI |
         | 4.1.1 | PCMCI dependencies fix: FPCMCI causal model field added, FPCMCI.run() and .run_pcmci() outputs the selected variables and the corresponding causal model |
         | 4.1.0 | FSelector and FValidator turned into FPCMCI and PCMCI<br>show_edge_label removed and dag optimized<br>new package included in the setup.py<br>added tutorials<br>new example in README.md |
```

### Comparing `fpcmci-4.3.1/README.md` & `fpcmci-4.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,15 @@
 ```
 
 
 ## Recent changes
 
 | Version | Changes |
 | :---: | ----------- |
+| 4.3.2 | documentation improved |
 | 4.3.1 | README and index.md updated |
 | 4.3.0 | alpha level fix in PCMCI<br>timeseries_dag fix<br>adaptation to DAG structure |
 | 4.2.1 | fixed dependency error in setup.py |
 | 4.2.0 | causal model with only selected features fix<br>adapted to tigramite 5.2<br>get_causal_matrix FPCMCI method added<br>f_alpha and pcmci_alpha instead of alpha<br>requirements changed<br>tutorials adapted to new version |
 | 4.1.2 | tutorials adapted to 4.1.1 and get_SCM method added in FPCMCI |
 | 4.1.1 | PCMCI dependencies fix: FPCMCI causal model field added, FPCMCI.run() and .run_pcmci() outputs the selected variables and the corresponding causal model |
 | 4.1.0 | FSelector and FValidator turned into FPCMCI and PCMCI<br>show_edge_label removed and dag optimized<br>new package included in the setup.py<br>added tutorials<br>new example in README.md |
```

### Comparing `fpcmci-4.3.1/fpcmci/CPrinter.py` & `fpcmci-4.3.2/fpcmci/CPrinter.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.1/fpcmci/FPCMCI.py` & `fpcmci-4.3.2/fpcmci/FPCMCI.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,16 +258,16 @@
     
     
     def __print_differences(self, old_dag : DAG, new_dag : DAG):
         """
         Print difference between old and new dependencies
 
         Args:
-            old_dep (DAG): old dag
-            new_dep (DAG): new dag
+            old_dag (DAG): old dag
+            new_dag (DAG): new dag
         """
         # Check difference(s) between validator and filter dependencies
         list_diffs = list()
         tmp = copy.deepcopy(old_dag)
         for t in tmp.g:
             if t not in new_dag.g:
                 list_diffs.append(t)
```

### Comparing `fpcmci-4.3.1/fpcmci/PCMCI.py` & `fpcmci-4.3.2/fpcmci/PCMCI.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,21 +108,20 @@
                                                 tau_min = self.min_lag,
                                                 # pc_alpha = self.alpha,
                                                 )
     
         return self.__PC_to_DAG(parents, data.features)
     
     
-    def __my_mci(self, autodep_dag: DAG):#, link_assumptions=None, parents=None):
+    def __my_mci(self, autodep_dag: DAG):
         """
         Performs MCI test
 
         Args:
-            link_assumptions (dict, optional): link assumptions. Defaults to None.
-            parents (dict, optional): parents dictionary. Defaults to None.
+            autodep_dag (DAG): current DAG to check via MCI
 
         Returns:
             (dict): MCI result
         """
         _int_link_assumptions = self.val_method._set_link_assumptions(autodep_dag.get_link_assumptions(autodep_ok = True), 
                                                                       self.min_lag, self.max_lag)
 
@@ -264,16 +263,15 @@
     
     def run_mci(self, data: Data, autodep_dag:DAG):#, link_assumptions, parents):
         """
         Run MCI test on observational data using the causal structure computed by the validator 
 
         Args:
             data (Data): Data obj to analyse
-            link_assumptions (dict): prior assumptions on causal model links. Defaults to None.
-            parents (dict): causal structure
+            autodep_dag (DAG): current DAG to check via MCI
 
         Returns:
             (DAG): estimated causal model
         """
         
         CP.info("\n##")
         CP.info("## MCI test analysis")
```

### Comparing `fpcmci-4.3.1/fpcmci/basics/utils.py` & `fpcmci-4.3.2/fpcmci/basics/utils.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.1/fpcmci/graph/DAG.py` & `fpcmci-4.3.2/fpcmci/graph/DAG.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,102 +5,169 @@
 from matplotlib import pyplot as plt
 import networkx as nx
 from netgraph import Graph
 
 
 class DAG():
     def __init__(self, var_names, min_lag, max_lag, neglect_autodep = False, scm = None):
+        """
+        DAG constructor
+
+        Args:
+            var_names (list): _description_
+            min_lag (int): _description_
+            max_lag (int): _description_
+            neglect_autodep (bool, optional): _description_. Defaults to False.
+            scm (dict, optional): _description_. Defaults to None.
+        """
         self.g = {var: Node(var, neglect_autodep) for var in var_names}
         self.neglect_autodep = neglect_autodep
         self.sys_context = dict()
         self.min_lag = min_lag
         self.max_lag = max_lag
         
         if scm is not None:
             for t in scm:
                 for s in scm[t]: self.add_source(t, s[0], 0.3, 0, s[1])
 
 
     @property
-    def features(self):
+    def features(self) -> list:
+        """
+        Features list
+
+        Returns:
+            list: Features list
+        """
         return list(self.g)
 
     
     @property
-    def autodep_nodes(self):
+    def autodep_nodes(self) -> list:
+        """
+        Autodependent nodes list
+
+        Returns:
+            list: Autodependent nodes list
+        """
         autodeps = list()
         for t in self.g:
             # NOTE: I commented this because I want to check all the auto-dep nodes with obs data
             # if self.g[t].is_autodependent and self.g[t].intervention_node: autodeps.append(t)
             if self.g[t].is_autodependent: autodeps.append(t)
         return autodeps
     
     
     @property
-    def interventions_links(self):
+    def interventions_links(self) -> list:
+        """
+        Intervention links list
+
+        Returns:
+            list: Intervention link list
+        """
         int_links = list()
         for t in self.g:
             for s in self.g[t].sources:
                 if self.g[s[0]].intervention_node:
                     int_links.append((s[0], s[1], t))
         return int_links
     
     
     def fully_connected_dag(self):
+        """
+        Build a fully connected DAG
+        """
         for t in self.g:
             for s in self.g:
                 for l in range(1, self.max_lag + 1): self.add_source(t, s, 1, 0, l)
     
     
     def add_source(self, t, s, score, pval, lag):
+        """
+        Adds source node to a target node
+
+        Args:
+            t (str): target node name
+            s (str): source node name
+            score (float): dependency score
+            pval (float): dependency p-value
+            lag (int): dependency lag
+        """
         self.g[t].sources[(s, abs(lag))] = {SCORE: score, PVAL: pval}
         self.g[s].children.append(t)
        
         
     def del_source(self, t, s, lag):
+        """
+        Removes source node from a target node
+
+        Args:
+            t (str): target node name
+            s (str): source node name
+            lag (int): dependency lag
+        """
         del self.g[t].sources[(s, lag)]
         self.g[s].children.remove(t)
         
         
     def remove_unneeded_features(self):
+        """
+        Removes isolated nodes
+        """
         tmp = copy.deepcopy(self.g)
         for t in self.g.keys():
             if self.g[t].is_isolated: 
                 if self.g[t].intervention_node: del tmp[self.g[t].associated_context] # FIXME: last edit to be tested
                 del tmp[t]
         self.g = tmp
             
             
     def add_context(self):
+        """
+        Adds context variables
+        """
         for sys_var, context_var in self.sys_context.items():
             if sys_var in self.features:
                 
                 # Adding context var to the graph
                 self.g[context_var] = Node(context_var, self.neglect_autodep)
                 
                 # Adding context var to sys var
                 self.g[sys_var].intervention_node = True
                 self.g[sys_var].associated_context = context_var
                 self.add_source(sys_var, context_var, 1, 0, 1)
                 
     
     def remove_context(self):
+        """
+        Remove context variables
+        """
         for sys_var, context_var in self.sys_context.items():
             if sys_var in self.g:
                 
                 # Removing context var from sys var
                 # self.g[sys_var].intervention_node = False
                 self.g[sys_var].associated_context = None
                 self.del_source(sys_var, context_var, 1)
                 
                 # Removing context var from dag
                 del self.g[context_var]
                 
                 
-    def get_link_assumptions(self, autodep_ok = False):
+    def get_link_assumptions(self, autodep_ok = False) -> dict:
+        """
+        Returnes link assumption dictionary
+
+        Args:
+            autodep_ok (bool, optional): If true, autodependecy link assumption = -->. Otherwise -?>. Defaults to False.
+
+        Returns:
+            dict: link assumption dictionary
+        """
         link_assump = {self.features.index(f): dict() for f in self.features}
         for t in self.g:
             for s in self.g[t].sources:
                 if autodep_ok and s[0] == t: # NOTE: new condition added in order to not control twice the autodependency links
                     link_assump[self.features.index(t)][(self.features.index(s[0]), -abs(s[1]))] = '-->'
                     
                 elif s[0] not in list(self.sys_context.values()):
@@ -108,23 +175,35 @@
                     
                 elif t in self.sys_context.keys() and s[0] == self.sys_context[t]:
                     link_assump[self.features.index(t)][(self.features.index(s[0]), -abs(s[1]))] = '-->'
                     
         return link_assump
 
 
-    def get_SCM(self):   
+    def get_SCM(self) -> dict:   
+        """
+        Returns SCM
+
+        Returns:
+            dict: SCM
+        """
         scm = {v: list() for v in self.features}
         for t in self.g:
             for s in self.g[t].sources:
                 scm[t].append((s[0], -abs(s[1]))) 
         return scm
     
     
-    def get_parents(self):        
+    def get_parents(self) -> dict:
+        """
+        Returns Parents dict
+
+        Returns:
+            dict: Parents dict
+        """
         scm = {self.features.index(v): list() for v in self.features}
         for t in self.g:
             for s in self.g[t].sources:
                 scm[self.features.index(t)].append((self.features.index(s[0]), -abs(s[1]))) 
         return scm
     
     
@@ -140,15 +219,21 @@
             for t in self.g:
                 for s in self.g[t].sources:
                     if s[1] == lag: cm_per_lag[lag][self.features.index(t)][self.features.index(s[0])] = self.g[t].sources[s][SCORE]
         if len(cm_per_lag) == 1: return list(cm_per_lag.values())[0]
         return cm_per_lag
     
     
-    def make_pretty(self):
+    def make_pretty(self) -> dict:
+        """
+        Makes variables' names pretty, i.e. $ varname $
+
+        Returns:
+            dict: pretty DAG
+        """
         pretty = dict()
         for t in self.g:
             p_t = '$' + t + '$'
             pretty[p_t] = copy.deepcopy(self.g[t])
             pretty[p_t].name = p_t
             pretty[p_t].children = ['$' + c + '$' for c in self.g[t].children]
             for s in self.g[t].sources:
@@ -168,15 +253,14 @@
             label_type = LabelType.Lag,
             save_name = None,
             img_extention = ImageExt.PNG):
         """
         build a dag
 
         Args:
-            res (DAG): causal model
             node_layout (str, optional): Node layout. Defaults to 'dot'.
             min_width (int, optional): minimum linewidth. Defaults to 1.
             max_width (int, optional): maximum linewidth. Defaults to 5.
             min_score (int, optional): minimum score range. Defaults to 0.
             max_score (int, optional): maximum score range. Defaults to 1.
             node_size (int, optional): node size. Defaults to 8.
             node_color (str, optional): node color. Defaults to 'orange'.
@@ -287,15 +371,14 @@
                font_size = 12,
                save_name = None,
                img_extention = ImageExt.PNG):
         """
         build a timeseries dag
 
         Args:
-            res (DAG): causal model
             tau (int): max time lag
             min_width (int, optional): minimum linewidth. Defaults to 1.
             max_width (int, optional): maximum linewidth. Defaults to 5.
             min_score (int, optional): minimum score range. Defaults to 0.
             max_score (int, optional): maximum score range. Defaults to 1.
             node_size (int, optional): node size. Defaults to 8.
             node_color (str, optional): node color. Defaults to 'orange'.
```

### Comparing `fpcmci-4.3.1/fpcmci/graph/Node.py` & `fpcmci-4.3.2/fpcmci/graph/Node.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,116 +16,129 @@
         self.children = list()
         self.neglect_autodep = neglect_autodep
         self.intervention_node = False        
         self.associated_context = None        
     
     
     @property
-    def is_autodependent(self):
+    def is_autodependent(self) -> bool:
         """
         Returns True if the node is autodependent
 
         Returns:
             bool: Returns True if the node is autodependent. Otherwise False
         """
         return self.name in self.sourcelist
     
     
     @property
-    def is_isolated(self):
+    def is_isolated(self) -> bool:
         """
         Returns True if the node is isolated
 
         Returns:
             bool: Returns True if the node is isolated. Otherwise False
         """
         if self.neglect_autodep:
             return (self.is_exogenous or self.is_only_autodep or self.is_only_autodep_context) and not self.has_child
         
         return (self.is_exogenous or self.has_only_context) and not self.has_child
     
     
     @property
-    def is_only_autodep(self):
+    def is_only_autodep(self) -> bool:
         """
         Returns True if the node is ONLY auto-dependent
 
         Returns:
             bool: Returns True if the node is ONLY auto-dependent. Otherwise False
         """
         return len(self.sources) == 1 and self.name in self.sourcelist
     
     
     @property
-    def has_only_context(self):
+    def has_only_context(self) -> bool:
         """
         Returns True if the node has ONLY the context variable as parent
 
         Returns:
             bool: Returns True if the node has ONLY the context variable as parent. Otherwise False
         """
         return len(self.sources) == 1 and self.associated_context in self.sourcelist
     
     
     @property
-    def is_only_autodep_context(self):
+    def is_only_autodep_context(self) -> bool:
         """
         Returns True if the node has ONLY the context variable and itself as parent
 
         Returns:
             bool: Returns True if the node has ONLY the context variable and itself as parent. Otherwise False
         """
         return len(self.sources) == 2 and self.name in self.sourcelist and self.associated_context in self.sourcelist
     
     
     @property
-    def is_exogenous(self):
+    def is_exogenous(self) -> bool:
         """
         Returns True if the node has no parents
 
         Returns:
             bool: Returns True if the node has no parents. Otherwise False
         """
         return len(self.sources) == 0
         
         
     @property
-    def has_child(self):
+    def has_child(self) -> bool:
         """
         Returns True if the node has at least one child
 
         Returns:
             bool: Returns True if the node has at least one child. Otherwise False
         """
         return len(self.children) > 0
     
     
     @property
-    def sourcelist(self):
+    def sourcelist(self) -> list(str):
         """
         Returns list of source names
 
         Returns:
             list(str): Returns list of source names
         """
         return [s[0] for s in self.sources]
     
     
     @property
-    def autodependency_links(self):
+    def autodependency_links(self) -> list:
+        """
+        Returns list of autodependency links
+
+        Returns:
+            list: Returns list of autodependency links
+
+        """
         autodep_links = list()
         if self.is_autodependent:
             for s in self.sources: 
                 if s[0] == self.name: 
                     autodep_links.append(s)
         return autodep_links
     
     
     @property
-    def get_max_autodependent(self):
+    def get_max_autodependent(self) -> float:
+        """
+        Returns max score of autodependent link
+
+        Returns:
+            float: Returns max score of autodependent link
+        """
         max_score = 0
         max_s = None
         if self.is_autodependent:
             for s in self.sources: 
                 if s[0] == self.name:
                     if self.sources[s][SCORE] > max_score: max_s = s
         return max_s
```

### Comparing `fpcmci-4.3.1/fpcmci/preprocessing/Subsampler.py` & `fpcmci-4.3.2/fpcmci/preprocessing/Subsampler.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.1/fpcmci/preprocessing/data.py` & `fpcmci-4.3.2/fpcmci/preprocessing/data.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/EntropyBasedMethod.py` & `fpcmci-4.3.2/fpcmci/preprocessing/subsampling_methods/EntropyBasedMethod.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/Static.py` & `fpcmci-4.3.2/fpcmci/preprocessing/subsampling_methods/Static.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/SubsamplingMethod.py` & `fpcmci-4.3.2/fpcmci/preprocessing/subsampling_methods/SubsamplingMethod.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/WSDynamic.py` & `fpcmci-4.3.2/fpcmci/preprocessing/subsampling_methods/WSDynamic.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/WSFFTStatic.py` & `fpcmci-4.3.2/fpcmci/preprocessing/subsampling_methods/WSFFTStatic.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/WSStatic.py` & `fpcmci-4.3.2/fpcmci/preprocessing/subsampling_methods/WSStatic.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/moving_window.py` & `fpcmci-4.3.2/fpcmci/preprocessing/subsampling_methods/moving_window.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.1/fpcmci/selection_methods/Corr.py` & `fpcmci-4.3.2/fpcmci/selection_methods/Corr.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.1/fpcmci/selection_methods/MI.py` & `fpcmci-4.3.2/fpcmci/selection_methods/MI.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.1/fpcmci/selection_methods/ParCorr.py` & `fpcmci-4.3.2/fpcmci/selection_methods/ParCorr.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.1/fpcmci/selection_methods/SelectionMethod.py` & `fpcmci-4.3.2/fpcmci/selection_methods/SelectionMethod.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.1/fpcmci/selection_methods/TE.py` & `fpcmci-4.3.2/fpcmci/selection_methods/TE.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.1/fpcmci.egg-info/PKG-INFO` & `fpcmci-4.3.2/fpcmci.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fpcmci
-Version: 4.3.1
+Version: 4.3.2
 Summary: A causal discovery Python package
 Home-page: https://github.com/lcastri/fpcmci
 Author: Luca Castri
 Author-email: lucacastri94@gmail.com
 License: UNKNOWN
 Description: # <img src="https://github.com/lcastri/fpcmci/raw/developer/docs/assets/icon.png" width="25"> FPCMCI - Filtered PCMCI
         
@@ -136,14 +136,15 @@
         ```
         
         
         ## Recent changes
         
         | Version | Changes |
         | :---: | ----------- |
+        | 4.3.2 | documentation improved |
         | 4.3.1 | README and index.md updated |
         | 4.3.0 | alpha level fix in PCMCI<br>timeseries_dag fix<br>adaptation to DAG structure |
         | 4.2.1 | fixed dependency error in setup.py |
         | 4.2.0 | causal model with only selected features fix<br>adapted to tigramite 5.2<br>get_causal_matrix FPCMCI method added<br>f_alpha and pcmci_alpha instead of alpha<br>requirements changed<br>tutorials adapted to new version |
         | 4.1.2 | tutorials adapted to 4.1.1 and get_SCM method added in FPCMCI |
         | 4.1.1 | PCMCI dependencies fix: FPCMCI causal model field added, FPCMCI.run() and .run_pcmci() outputs the selected variables and the corresponding causal model |
         | 4.1.0 | FSelector and FValidator turned into FPCMCI and PCMCI<br>show_edge_label removed and dag optimized<br>new package included in the setup.py<br>added tutorials<br>new example in README.md |
```

### Comparing `fpcmci-4.3.1/fpcmci.egg-info/SOURCES.txt` & `fpcmci-4.3.2/fpcmci.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 README.md
 setup.py
 fpcmci/CPrinter.py
 fpcmci/FPCMCI.py
 fpcmci/PCMCI.py
 fpcmci/__init__.py
-fpcmci/causal_graph.py
 fpcmci/version.py
 fpcmci.egg-info/PKG-INFO
 fpcmci.egg-info/SOURCES.txt
 fpcmci.egg-info/dependency_links.txt
 fpcmci.egg-info/requires.txt
 fpcmci.egg-info/top_level.txt
 fpcmci/basics/__init__.py
```

### Comparing `fpcmci-4.3.1/setup.py` & `fpcmci-4.3.2/setup.py`

 * *Files identical despite different names*

