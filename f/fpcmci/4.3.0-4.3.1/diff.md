# Comparing `tmp/fpcmci-4.3.0.tar.gz` & `tmp/fpcmci-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpcmci-4.3.0.tar", last modified: Sat Aug  5 11:04:10 2023, max compression
+gzip compressed data, was "fpcmci-4.3.1.tar", last modified: Sat Aug  5 11:20:41 2023, max compression
```

## Comparing `fpcmci-4.3.0.tar` & `fpcmci-4.3.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:04:10.777374 fpcmci-4.3.0/
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     8371 2023-08-05 11:04:10.777374 fpcmci-4.3.0/PKG-INFO
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     6657 2023-05-29 18:54:02.000000 fpcmci-4.3.0/README.md
-drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:04:10.777374 fpcmci-4.3.0/fpcmci/
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     1066 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/CPrinter.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)    11125 2023-07-26 08:29:42.000000 fpcmci-4.3.0/fpcmci/FPCMCI.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)    14739 2023-08-05 10:53:21.000000 fpcmci-4.3.0/fpcmci/PCMCI.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)      240 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/__init__.py
-drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:04:10.777374 fpcmci-4.3.0/fpcmci/basics/
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)       72 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/basics/__init__.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)      445 2023-08-05 10:43:49.000000 fpcmci-4.3.0/fpcmci/basics/constants.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)      506 2023-08-05 10:53:21.000000 fpcmci-4.3.0/fpcmci/basics/logger.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)      812 2023-08-05 10:44:32.000000 fpcmci-4.3.0/fpcmci/basics/utils.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     8790 2023-08-05 10:53:21.000000 fpcmci-4.3.0/fpcmci/causal_graph.py
-drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:04:10.777374 fpcmci-4.3.0/fpcmci/graph/
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)    15964 2023-08-05 10:53:21.000000 fpcmci-4.3.0/fpcmci/graph/DAG.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     3681 2023-08-05 10:53:21.000000 fpcmci-4.3.0/fpcmci/graph/Node.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)       43 2023-07-26 08:29:42.000000 fpcmci-4.3.0/fpcmci/graph/__init__.py
-drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:04:10.777374 fpcmci-4.3.0/fpcmci/preprocessing/
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     2304 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/preprocessing/Subsampler.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)        0 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/preprocessing/__init__.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     4568 2023-08-05 10:53:21.000000 fpcmci-4.3.0/fpcmci/preprocessing/data.py
-drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:04:10.777374 fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     3649 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/EntropyBasedMethod.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)      639 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/Static.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)      781 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/SubsamplingMethod.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     1798 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/WSDynamic.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     2600 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/WSFFTStatic.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     1765 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/WSStatic.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)      267 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/__init__.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     2493 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/moving_window.py
-drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:04:10.777374 fpcmci-4.3.0/fpcmci/selection_methods/
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     1400 2023-07-26 08:29:42.000000 fpcmci-4.3.0/fpcmci/selection_methods/Corr.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     2220 2023-07-26 08:29:42.000000 fpcmci-4.3.0/fpcmci/selection_methods/MI.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     2698 2023-07-26 08:29:42.000000 fpcmci-4.3.0/fpcmci/selection_methods/ParCorr.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     3457 2023-08-05 10:53:21.000000 fpcmci-4.3.0/fpcmci/selection_methods/SelectionMethod.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     3803 2023-07-26 08:29:42.000000 fpcmci-4.3.0/fpcmci/selection_methods/TE.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)      134 2023-07-26 08:29:42.000000 fpcmci-4.3.0/fpcmci/selection_methods/__init__.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)       17 2023-08-05 10:59:38.000000 fpcmci-4.3.0/fpcmci/version.py
-drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:04:10.777374 fpcmci-4.3.0/fpcmci.egg-info/
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     8371 2023-08-05 11:04:10.000000 fpcmci-4.3.0/fpcmci.egg-info/PKG-INFO
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     1204 2023-08-05 11:04:10.000000 fpcmci-4.3.0/fpcmci.egg-info/SOURCES.txt
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)        1 2023-08-05 11:04:10.000000 fpcmci-4.3.0/fpcmci.egg-info/dependency_links.txt
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)      154 2023-08-05 11:04:10.000000 fpcmci-4.3.0/fpcmci.egg-info/requires.txt
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)        7 2023-08-05 11:04:10.000000 fpcmci-4.3.0/fpcmci.egg-info/top_level.txt
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)       38 2023-08-05 11:04:10.777374 fpcmci-4.3.0/setup.cfg
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     1431 2023-08-05 10:54:20.000000 fpcmci-4.3.0/setup.py
+drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:20:41.917014 fpcmci-4.3.1/
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     8517 2023-08-05 11:20:41.917014 fpcmci-4.3.1/PKG-INFO
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     6787 2023-08-05 11:19:46.000000 fpcmci-4.3.1/README.md
+drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:20:41.917014 fpcmci-4.3.1/fpcmci/
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     1066 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/CPrinter.py
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)    11125 2023-08-05 11:14:12.000000 fpcmci-4.3.1/fpcmci/FPCMCI.py
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)    14739 2023-08-05 11:14:12.000000 fpcmci-4.3.1/fpcmci/PCMCI.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)      240 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/__init__.py
+drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:20:41.917014 fpcmci-4.3.1/fpcmci/basics/
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)       72 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/basics/__init__.py
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)      445 2023-08-05 11:14:12.000000 fpcmci-4.3.1/fpcmci/basics/constants.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)      506 2023-08-05 10:53:21.000000 fpcmci-4.3.1/fpcmci/basics/logger.py
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)      812 2023-08-05 11:14:12.000000 fpcmci-4.3.1/fpcmci/basics/utils.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     8790 2023-08-05 10:53:21.000000 fpcmci-4.3.1/fpcmci/causal_graph.py
+drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:20:41.917014 fpcmci-4.3.1/fpcmci/graph/
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)    15964 2023-08-05 11:14:12.000000 fpcmci-4.3.1/fpcmci/graph/DAG.py
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     3681 2023-08-05 11:14:12.000000 fpcmci-4.3.1/fpcmci/graph/Node.py
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)       43 2023-08-05 11:14:12.000000 fpcmci-4.3.1/fpcmci/graph/__init__.py
+drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:20:41.917014 fpcmci-4.3.1/fpcmci/preprocessing/
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     2304 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/preprocessing/Subsampler.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)        0 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/preprocessing/__init__.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     4568 2023-08-05 10:53:21.000000 fpcmci-4.3.1/fpcmci/preprocessing/data.py
+drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:20:41.917014 fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     3649 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/EntropyBasedMethod.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)      639 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/Static.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)      781 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/SubsamplingMethod.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     1798 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/WSDynamic.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     2600 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/WSFFTStatic.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     1765 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/WSStatic.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)      267 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/__init__.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     2493 2023-05-29 18:54:02.000000 fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/moving_window.py
+drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:20:41.917014 fpcmci-4.3.1/fpcmci/selection_methods/
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     1400 2023-08-05 11:14:12.000000 fpcmci-4.3.1/fpcmci/selection_methods/Corr.py
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     2220 2023-08-05 11:14:12.000000 fpcmci-4.3.1/fpcmci/selection_methods/MI.py
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     2698 2023-08-05 11:14:12.000000 fpcmci-4.3.1/fpcmci/selection_methods/ParCorr.py
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     3457 2023-08-05 11:14:12.000000 fpcmci-4.3.1/fpcmci/selection_methods/SelectionMethod.py
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     3803 2023-08-05 11:14:12.000000 fpcmci-4.3.1/fpcmci/selection_methods/TE.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)      134 2023-07-26 08:29:42.000000 fpcmci-4.3.1/fpcmci/selection_methods/__init__.py
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)       17 2023-08-05 11:19:32.000000 fpcmci-4.3.1/fpcmci/version.py
+drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:20:41.917014 fpcmci-4.3.1/fpcmci.egg-info/
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     8517 2023-08-05 11:20:41.000000 fpcmci-4.3.1/fpcmci.egg-info/PKG-INFO
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     1204 2023-08-05 11:20:41.000000 fpcmci-4.3.1/fpcmci.egg-info/SOURCES.txt
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)        1 2023-08-05 11:20:41.000000 fpcmci-4.3.1/fpcmci.egg-info/dependency_links.txt
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)      154 2023-08-05 11:20:41.000000 fpcmci-4.3.1/fpcmci.egg-info/requires.txt
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)        7 2023-08-05 11:20:41.000000 fpcmci-4.3.1/fpcmci.egg-info/top_level.txt
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)       38 2023-08-05 11:20:41.917014 fpcmci-4.3.1/setup.cfg
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     1431 2023-08-05 11:14:13.000000 fpcmci-4.3.1/setup.py
```

### Comparing `fpcmci-4.3.0/PKG-INFO` & `fpcmci-4.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fpcmci
-Version: 4.3.0
+Version: 4.3.1
 Summary: A causal discovery Python package
 Home-page: https://github.com/lcastri/fpcmci
 Author: Luca Castri
 Author-email: lucacastri94@gmail.com
 License: UNKNOWN
 Description: # <img src="https://github.com/lcastri/fpcmci/raw/developer/docs/assets/icon.png" width="25"> FPCMCI - Filtered PCMCI
         
@@ -136,14 +136,16 @@
         ```
         
         
         ## Recent changes
         
         | Version | Changes |
         | :---: | ----------- |
+        | 4.3.1 | README and index.md updated |
+        | 4.3.0 | alpha level fix in PCMCI<br>timeseries_dag fix<br>adaptation to DAG structure |
         | 4.2.1 | fixed dependency error in setup.py |
         | 4.2.0 | causal model with only selected features fix<br>adapted to tigramite 5.2<br>get_causal_matrix FPCMCI method added<br>f_alpha and pcmci_alpha instead of alpha<br>requirements changed<br>tutorials adapted to new version |
         | 4.1.2 | tutorials adapted to 4.1.1 and get_SCM method added in FPCMCI |
         | 4.1.1 | PCMCI dependencies fix: FPCMCI causal model field added, FPCMCI.run() and .run_pcmci() outputs the selected variables and the corresponding causal model |
         | 4.1.0 | FSelector and FValidator turned into FPCMCI and PCMCI<br>show_edge_label removed and dag optimized<br>new package included in the setup.py<br>added tutorials<br>new example in README.md |
         | 4.0.1 | online documentation and paths fixes |
         | 4.0.0 | package published |
```

### Comparing `fpcmci-4.3.0/README.md` & `fpcmci-4.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -128,14 +128,16 @@
 ```
 
 
 ## Recent changes
 
 | Version | Changes |
 | :---: | ----------- |
+| 4.3.1 | README and index.md updated |
+| 4.3.0 | alpha level fix in PCMCI<br>timeseries_dag fix<br>adaptation to DAG structure |
 | 4.2.1 | fixed dependency error in setup.py |
 | 4.2.0 | causal model with only selected features fix<br>adapted to tigramite 5.2<br>get_causal_matrix FPCMCI method added<br>f_alpha and pcmci_alpha instead of alpha<br>requirements changed<br>tutorials adapted to new version |
 | 4.1.2 | tutorials adapted to 4.1.1 and get_SCM method added in FPCMCI |
 | 4.1.1 | PCMCI dependencies fix: FPCMCI causal model field added, FPCMCI.run() and .run_pcmci() outputs the selected variables and the corresponding causal model |
 | 4.1.0 | FSelector and FValidator turned into FPCMCI and PCMCI<br>show_edge_label removed and dag optimized<br>new package included in the setup.py<br>added tutorials<br>new example in README.md |
 | 4.0.1 | online documentation and paths fixes |
 | 4.0.0 | package published |
```

### Comparing `fpcmci-4.3.0/fpcmci/CPrinter.py` & `fpcmci-4.3.1/fpcmci/CPrinter.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.0/fpcmci/FPCMCI.py` & `fpcmci-4.3.1/fpcmci/FPCMCI.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.0/fpcmci/PCMCI.py` & `fpcmci-4.3.1/fpcmci/PCMCI.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.0/fpcmci/basics/utils.py` & `fpcmci-4.3.1/fpcmci/basics/utils.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.0/fpcmci/causal_graph.py` & `fpcmci-4.3.1/fpcmci/causal_graph.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.0/fpcmci/graph/DAG.py` & `fpcmci-4.3.1/fpcmci/graph/DAG.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.0/fpcmci/graph/Node.py` & `fpcmci-4.3.1/fpcmci/graph/Node.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.0/fpcmci/preprocessing/Subsampler.py` & `fpcmci-4.3.1/fpcmci/preprocessing/Subsampler.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.0/fpcmci/preprocessing/data.py` & `fpcmci-4.3.1/fpcmci/preprocessing/data.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/EntropyBasedMethod.py` & `fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/EntropyBasedMethod.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/Static.py` & `fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/Static.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/SubsamplingMethod.py` & `fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/SubsamplingMethod.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/WSDynamic.py` & `fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/WSDynamic.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/WSFFTStatic.py` & `fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/WSFFTStatic.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/WSStatic.py` & `fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/WSStatic.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/moving_window.py` & `fpcmci-4.3.1/fpcmci/preprocessing/subsampling_methods/moving_window.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.0/fpcmci/selection_methods/Corr.py` & `fpcmci-4.3.1/fpcmci/selection_methods/Corr.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.0/fpcmci/selection_methods/MI.py` & `fpcmci-4.3.1/fpcmci/selection_methods/MI.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.0/fpcmci/selection_methods/ParCorr.py` & `fpcmci-4.3.1/fpcmci/selection_methods/ParCorr.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.0/fpcmci/selection_methods/SelectionMethod.py` & `fpcmci-4.3.1/fpcmci/selection_methods/SelectionMethod.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.0/fpcmci/selection_methods/TE.py` & `fpcmci-4.3.1/fpcmci/selection_methods/TE.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.0/fpcmci.egg-info/PKG-INFO` & `fpcmci-4.3.1/fpcmci.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fpcmci
-Version: 4.3.0
+Version: 4.3.1
 Summary: A causal discovery Python package
 Home-page: https://github.com/lcastri/fpcmci
 Author: Luca Castri
 Author-email: lucacastri94@gmail.com
 License: UNKNOWN
 Description: # <img src="https://github.com/lcastri/fpcmci/raw/developer/docs/assets/icon.png" width="25"> FPCMCI - Filtered PCMCI
         
@@ -136,14 +136,16 @@
         ```
         
         
         ## Recent changes
         
         | Version | Changes |
         | :---: | ----------- |
+        | 4.3.1 | README and index.md updated |
+        | 4.3.0 | alpha level fix in PCMCI<br>timeseries_dag fix<br>adaptation to DAG structure |
         | 4.2.1 | fixed dependency error in setup.py |
         | 4.2.0 | causal model with only selected features fix<br>adapted to tigramite 5.2<br>get_causal_matrix FPCMCI method added<br>f_alpha and pcmci_alpha instead of alpha<br>requirements changed<br>tutorials adapted to new version |
         | 4.1.2 | tutorials adapted to 4.1.1 and get_SCM method added in FPCMCI |
         | 4.1.1 | PCMCI dependencies fix: FPCMCI causal model field added, FPCMCI.run() and .run_pcmci() outputs the selected variables and the corresponding causal model |
         | 4.1.0 | FSelector and FValidator turned into FPCMCI and PCMCI<br>show_edge_label removed and dag optimized<br>new package included in the setup.py<br>added tutorials<br>new example in README.md |
         | 4.0.1 | online documentation and paths fixes |
         | 4.0.0 | package published |
```

### Comparing `fpcmci-4.3.0/fpcmci.egg-info/SOURCES.txt` & `fpcmci-4.3.1/fpcmci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fpcmci-4.3.0/setup.py` & `fpcmci-4.3.1/setup.py`

 * *Files identical despite different names*

