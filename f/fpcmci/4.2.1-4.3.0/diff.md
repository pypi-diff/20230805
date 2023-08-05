# Comparing `tmp/fpcmci-4.2.1.tar.gz` & `tmp/fpcmci-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpcmci-4.2.1.tar", last modified: Wed May 17 11:16:50 2023, max compression
+gzip compressed data, was "fpcmci-4.3.0.tar", last modified: Sat Aug  5 11:04:10 2023, max compression
```

## Comparing `fpcmci-4.2.1.tar` & `fpcmci-4.3.0.tar`

### file list

```diff
@@ -1,43 +1,47 @@
-drwxrwxr-x   0 lucacastri  (1000) lucacastri  (1000)        0 2023-05-17 11:16:50.872811 fpcmci-4.2.1/
--rw-rw-r--   0 lucacastri  (1000) lucacastri  (1000)     8371 2023-05-17 11:16:50.872811 fpcmci-4.2.1/PKG-INFO
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     6657 2023-05-17 11:14:30.000000 fpcmci-4.2.1/README.md
-drwxrwxr-x   0 lucacastri  (1000) lucacastri  (1000)        0 2023-05-17 11:16:50.868811 fpcmci-4.2.1/fpcmci/
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     1066 2023-03-03 16:48:10.000000 fpcmci-4.2.1/fpcmci/CPrinter.py
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)    16932 2023-05-17 09:58:42.000000 fpcmci-4.2.1/fpcmci/FPCMCI.py
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)    10260 2023-05-17 09:34:09.000000 fpcmci-4.2.1/fpcmci/PCMCI.py
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)      240 2023-03-03 16:48:10.000000 fpcmci-4.2.1/fpcmci/__init__.py
-drwxrwxr-x   0 lucacastri  (1000) lucacastri  (1000)        0 2023-05-17 11:16:50.868811 fpcmci-4.2.1/fpcmci/basics/
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)       72 2023-03-03 16:48:10.000000 fpcmci-4.2.1/fpcmci/basics/__init__.py
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)      401 2023-03-03 16:48:10.000000 fpcmci-4.2.1/fpcmci/basics/constants.py
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)      506 2023-03-03 16:48:10.000000 fpcmci-4.2.1/fpcmci/basics/logger.py
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     1235 2023-03-03 16:48:10.000000 fpcmci-4.2.1/fpcmci/basics/utils.py
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     8598 2023-03-03 16:48:10.000000 fpcmci-4.2.1/fpcmci/causal_graph.py
-drwxrwxr-x   0 lucacastri  (1000) lucacastri  (1000)        0 2023-05-17 11:16:50.868811 fpcmci-4.2.1/fpcmci/preprocessing/
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     2304 2023-03-03 16:48:10.000000 fpcmci-4.2.1/fpcmci/preprocessing/Subsampler.py
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)        0 2023-03-03 16:48:10.000000 fpcmci-4.2.1/fpcmci/preprocessing/__init__.py
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     4568 2023-03-03 16:48:10.000000 fpcmci-4.2.1/fpcmci/preprocessing/data.py
-drwxrwxr-x   0 lucacastri  (1000) lucacastri  (1000)        0 2023-05-17 11:16:50.868811 fpcmci-4.2.1/fpcmci/preprocessing/subsampling_methods/
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     3649 2023-03-03 16:48:10.000000 fpcmci-4.2.1/fpcmci/preprocessing/subsampling_methods/EntropyBasedMethod.py
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)      639 2023-03-03 16:48:10.000000 fpcmci-4.2.1/fpcmci/preprocessing/subsampling_methods/Static.py
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)      781 2023-03-03 16:48:10.000000 fpcmci-4.2.1/fpcmci/preprocessing/subsampling_methods/SubsamplingMethod.py
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     1798 2023-03-03 16:48:10.000000 fpcmci-4.2.1/fpcmci/preprocessing/subsampling_methods/WSDynamic.py
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     2600 2023-03-03 16:48:10.000000 fpcmci-4.2.1/fpcmci/preprocessing/subsampling_methods/WSFFTStatic.py
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     1765 2023-03-03 16:48:10.000000 fpcmci-4.2.1/fpcmci/preprocessing/subsampling_methods/WSStatic.py
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)      267 2023-03-03 16:48:10.000000 fpcmci-4.2.1/fpcmci/preprocessing/subsampling_methods/__init__.py
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     2493 2023-03-03 16:48:10.000000 fpcmci-4.2.1/fpcmci/preprocessing/subsampling_methods/moving_window.py
-drwxrwxr-x   0 lucacastri  (1000) lucacastri  (1000)        0 2023-05-17 11:16:50.872811 fpcmci-4.2.1/fpcmci/selection_methods/
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     1402 2023-03-03 16:48:10.000000 fpcmci-4.2.1/fpcmci/selection_methods/Corr.py
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     2222 2023-03-03 16:48:10.000000 fpcmci-4.2.1/fpcmci/selection_methods/MI.py
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     2700 2023-03-03 16:48:10.000000 fpcmci-4.2.1/fpcmci/selection_methods/ParCorr.py
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     3791 2023-03-03 16:48:10.000000 fpcmci-4.2.1/fpcmci/selection_methods/SelectionMethod.py
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     3805 2023-03-03 16:48:10.000000 fpcmci-4.2.1/fpcmci/selection_methods/TE.py
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)      134 2023-03-03 16:48:10.000000 fpcmci-4.2.1/fpcmci/selection_methods/__init__.py
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)       17 2023-05-17 11:13:20.000000 fpcmci-4.2.1/fpcmci/version.py
-drwxrwxr-x   0 lucacastri  (1000) lucacastri  (1000)        0 2023-05-17 11:16:50.868811 fpcmci-4.2.1/fpcmci.egg-info/
--rw-rw-r--   0 lucacastri  (1000) lucacastri  (1000)     8371 2023-05-17 11:16:50.000000 fpcmci-4.2.1/fpcmci.egg-info/PKG-INFO
--rw-rw-r--   0 lucacastri  (1000) lucacastri  (1000)     1138 2023-05-17 11:16:50.000000 fpcmci-4.2.1/fpcmci.egg-info/SOURCES.txt
--rw-rw-r--   0 lucacastri  (1000) lucacastri  (1000)        1 2023-05-17 11:16:50.000000 fpcmci-4.2.1/fpcmci.egg-info/dependency_links.txt
--rw-rw-r--   0 lucacastri  (1000) lucacastri  (1000)      154 2023-05-17 11:16:50.000000 fpcmci-4.2.1/fpcmci.egg-info/requires.txt
--rw-rw-r--   0 lucacastri  (1000) lucacastri  (1000)        7 2023-05-17 11:16:50.000000 fpcmci-4.2.1/fpcmci.egg-info/top_level.txt
--rw-rw-r--   0 lucacastri  (1000) lucacastri  (1000)       38 2023-05-17 11:16:50.872811 fpcmci-4.2.1/setup.cfg
--rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     1415 2023-05-17 11:02:42.000000 fpcmci-4.2.1/setup.py
+drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:04:10.777374 fpcmci-4.3.0/
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     8371 2023-08-05 11:04:10.777374 fpcmci-4.3.0/PKG-INFO
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     6657 2023-05-29 18:54:02.000000 fpcmci-4.3.0/README.md
+drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:04:10.777374 fpcmci-4.3.0/fpcmci/
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     1066 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/CPrinter.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)    11125 2023-07-26 08:29:42.000000 fpcmci-4.3.0/fpcmci/FPCMCI.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)    14739 2023-08-05 10:53:21.000000 fpcmci-4.3.0/fpcmci/PCMCI.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)      240 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/__init__.py
+drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:04:10.777374 fpcmci-4.3.0/fpcmci/basics/
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)       72 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/basics/__init__.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)      445 2023-08-05 10:43:49.000000 fpcmci-4.3.0/fpcmci/basics/constants.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)      506 2023-08-05 10:53:21.000000 fpcmci-4.3.0/fpcmci/basics/logger.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)      812 2023-08-05 10:44:32.000000 fpcmci-4.3.0/fpcmci/basics/utils.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     8790 2023-08-05 10:53:21.000000 fpcmci-4.3.0/fpcmci/causal_graph.py
+drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:04:10.777374 fpcmci-4.3.0/fpcmci/graph/
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)    15964 2023-08-05 10:53:21.000000 fpcmci-4.3.0/fpcmci/graph/DAG.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     3681 2023-08-05 10:53:21.000000 fpcmci-4.3.0/fpcmci/graph/Node.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)       43 2023-07-26 08:29:42.000000 fpcmci-4.3.0/fpcmci/graph/__init__.py
+drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:04:10.777374 fpcmci-4.3.0/fpcmci/preprocessing/
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     2304 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/preprocessing/Subsampler.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)        0 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/preprocessing/__init__.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     4568 2023-08-05 10:53:21.000000 fpcmci-4.3.0/fpcmci/preprocessing/data.py
+drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:04:10.777374 fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     3649 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/EntropyBasedMethod.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)      639 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/Static.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)      781 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/SubsamplingMethod.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     1798 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/WSDynamic.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     2600 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/WSFFTStatic.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     1765 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/WSStatic.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)      267 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/__init__.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     2493 2023-05-29 18:54:02.000000 fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/moving_window.py
+drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:04:10.777374 fpcmci-4.3.0/fpcmci/selection_methods/
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     1400 2023-07-26 08:29:42.000000 fpcmci-4.3.0/fpcmci/selection_methods/Corr.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     2220 2023-07-26 08:29:42.000000 fpcmci-4.3.0/fpcmci/selection_methods/MI.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     2698 2023-07-26 08:29:42.000000 fpcmci-4.3.0/fpcmci/selection_methods/ParCorr.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     3457 2023-08-05 10:53:21.000000 fpcmci-4.3.0/fpcmci/selection_methods/SelectionMethod.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     3803 2023-07-26 08:29:42.000000 fpcmci-4.3.0/fpcmci/selection_methods/TE.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)      134 2023-07-26 08:29:42.000000 fpcmci-4.3.0/fpcmci/selection_methods/__init__.py
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)       17 2023-08-05 10:59:38.000000 fpcmci-4.3.0/fpcmci/version.py
+drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-08-05 11:04:10.777374 fpcmci-4.3.0/fpcmci.egg-info/
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     8371 2023-08-05 11:04:10.000000 fpcmci-4.3.0/fpcmci.egg-info/PKG-INFO
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     1204 2023-08-05 11:04:10.000000 fpcmci-4.3.0/fpcmci.egg-info/SOURCES.txt
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)        1 2023-08-05 11:04:10.000000 fpcmci-4.3.0/fpcmci.egg-info/dependency_links.txt
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)      154 2023-08-05 11:04:10.000000 fpcmci-4.3.0/fpcmci.egg-info/requires.txt
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)        7 2023-08-05 11:04:10.000000 fpcmci-4.3.0/fpcmci.egg-info/top_level.txt
+-rw-rw-r--   0 lcastri   (1000) lcastri   (1000)       38 2023-08-05 11:04:10.777374 fpcmci-4.3.0/setup.cfg
+-rw-r--r--   0 lcastri   (1000) lcastri   (1000)     1431 2023-08-05 10:54:20.000000 fpcmci-4.3.0/setup.py
```

### Comparing `fpcmci-4.2.1/PKG-INFO` & `fpcmci-4.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fpcmci
-Version: 4.2.1
+Version: 4.3.0
 Summary: A causal discovery Python package
 Home-page: https://github.com/lcastri/fpcmci
 Author: Luca Castri
 Author-email: lucacastri94@gmail.com
 License: UNKNOWN
 Description: # <img src="https://github.com/lcastri/fpcmci/raw/developer/docs/assets/icon.png" width="25"> FPCMCI - Filtered PCMCI
```

### Comparing `fpcmci-4.2.1/README.md` & `fpcmci-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fpcmci-4.2.1/fpcmci/CPrinter.py` & `fpcmci-4.3.0/fpcmci/CPrinter.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.2.1/fpcmci/FPCMCI.py` & `fpcmci-4.3.0/fpcmci/PCMCI.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,455 +1,348 @@
-import copy
-import pickle
-import matplotlib.pyplot as plt
-import numpy as np
+from tigramite.pcmci import PCMCI as VAL
 from tigramite.independence_tests.independence_tests_base import CondIndTest
-import sys
-from fpcmci.selection_methods.SelectionMethod import SelectionMethod
+import tigramite.data_processing as pp
+import numpy as np
 from fpcmci.CPrinter import CPLevel, CP
 from fpcmci.basics.constants import *
-from fpcmci.basics.logger import Logger
-import fpcmci.basics.utils as utils
-from fpcmci.PCMCI import PCMCI
-from fpcmci.preprocessing.data import Data 
+from fpcmci.graph.DAG import DAG
+from fpcmci.preprocessing.data import Data
 
 
-class FPCMCI():
+class PCMCI():
     """
-    FPCMCI class.
+    PCMCI class.
 
-    FPCMCI is a causal feature selector framework for large-scale time series
-    datasets. Sarting from a Data object and it selects the main features
-    responsible for the evolution of the analysed system. Based on the selected features,
-    the framework outputs a causal model.
+    PCMCI works with FSelector in order to find the causal 
+    model starting from a prefixed set of variables and links.
     """
-
-    def __init__(self, 
-                 data: Data, 
-                 min_lag, max_lag, 
-                 sel_method: SelectionMethod, val_condtest: CondIndTest, 
-                 verbosity: CPLevel, 
-                 f_alpha = 0.05, 
-                 pcmci_alpha = 0.05, 
-                 resfolder = None,
-                 neglect_only_autodep = False):
+    def __init__(self, alpha, min_lag, max_lag, val_condtest: CondIndTest, verbosity: CPLevel, sys_context = dict()):
         """
-        FPCMCI class contructor
+        PCMCI class constructor
 
         Args:
-            data (Data): data to analyse
+            alpha (float): significance level
             min_lag (int): minimum time lag
             max_lag (int): maximum time lag
-            sel_method (SelectionMethod): selection method
             val_condtest (CondIndTest): validation method
             verbosity (CPLevel): verbosity level
-            f_alpha (float, optional): filter significance level. Defaults to 0.05.
-            pcmci_alpha (float, optional): PCMCI significance level. Defaults to 0.05.
-            resfolder (string, optional): result folder to create. Defaults to None.
-            neglect_only_autodep (bool, optional): Bit for neglecting variables with only autodependency. Defaults to False.
         """
-        
-        self.data = data
-        self.f_alpha = f_alpha
-        self.pcmci_alpha = pcmci_alpha
+        self.alpha = alpha
         self.min_lag = min_lag
         self.max_lag = max_lag
-        self.sel_method = sel_method
-        self.filter_dependencies = None
-        self.o_filter_dependencies = None
-        self.causal_model = None
         self.result = None
-        self.neglect_only_autodep = neglect_only_autodep
-
-        self.dependency_path = None
-        if resfolder is not None:
-            utils.create_results_folder()
-            logpath, self.dependency_path = utils.get_selectorpath(resfolder)
-            sys.stdout = Logger(logpath)
+        self.dependencies = None
+        self.val_method = None
+        self.val_condtest = val_condtest
+        self.verbosity = verbosity.value
+        self.sys_context = sys_context
         
-        self.validator = PCMCI(data, self.pcmci_alpha, min_lag, max_lag, val_condtest, resfolder, verbosity)       
-        CP.set_verbosity(verbosity)
-
 
-    def run_filter(self):
+    def run(self, data: Data, link_assumptions = None):
         """
-        Run filter method
-        """
-        CP.info("\n")
-        CP.info(DASH)
-        CP.info("Selecting relevant features among: " + str(self.data.features))
-        CP.info("Selection method: " + self.sel_method.name)
-        CP.info("Significance level: " + str(self.f_alpha))
-        CP.info("Max lag time: " + str(self.max_lag))
-        CP.info("Min lag time: " + str(self.min_lag))
-        CP.info("Data length: " + str(self.data.T))
-
-        self.sel_method.initialise(self.data, self.f_alpha, self.min_lag, self.max_lag)
-        self.filter_dependencies = self.sel_method.compute_dependencies()
-        self.o_filter_dependecies = copy.deepcopy(self.filter_dependencies)
+        Run causal discovery algorithm
 
+        Args:
+            data (Data): Data obj to analyse
+            link_assumptions (dict, optional): prior assumptions on causal model links. Defaults to None.
 
-    def run_pcmci(self):
-        """
-        Run PCMCI
-        
         Returns:
-            list(str): list of selected variable names
-            dict(str:list(tuple)): causal model
+            (DAG): estimated causal model
         """
-        CP.info("Significance level: " + str(self.pcmci_alpha))
-        CP.info("Max lag time: " + str(self.max_lag))
-        CP.info("Min lag time: " + str(self.min_lag))
-        CP.info("Data length: " + str(self.data.T))
-
-        # causal model
-        self.validator.data = self.data
-        self.validator.run()
-        self.causal_model = self.validator.dependencies
-        
-        self.result = self.data.features
         
-        self.save_validator_res()
-        
-        return self.result, self.causal_model
+        CP.info('\n')
+        CP.info(DASH)
+        CP.info("Running Causal Discovery Algorithm")
 
-    
-    def run(self):
-        """
-        Run Selector and Validator
-        
-        Returns:
-            list(str): list of selected variable names
-            dict(str:list(tuple)): causal model
-        """
+        # build tigramite dataset
+        vector = np.vectorize(float)
+        d = vector(data.d)
+        dataframe = pp.DataFrame(data = d, var_names = data.features)
         
-        self.run_filter()        
-            
-        # list of selected features based on dependencies
-        tmp_sel_features = self.get_selected_features()
-        if not tmp_sel_features:
-            return self.result
+        # init and run pcmci
+        self.val_method = VAL(dataframe = dataframe,
+                              cond_ind_test = self.val_condtest,
+                              verbosity = self.verbosity)
 
-        # shrink dataframe d and dependencies by the selector result
-        self.shrink(tmp_sel_features)
+        self.result = self.val_method.run_pcmci(link_assumptions = link_assumptions,
+                                                tau_max = self.max_lag,
+                                                tau_min = self.min_lag,
+                                                alpha_level = self.alpha,
+                                                # pc_alpha = self.alpha
+                                                )
         
-        # selected links to check by the validator
-        link_assumptions = self.__get_link_assumptions()
-            
-        # causal model on selected links
-        self.validator.data = self.data
-        pcmci_result = self.validator.run(link_assumptions)
+        self.result['var_names'] = data.features
+        self.result['pretty_var_names'] = data.pretty_features
         
-        # application of the validator result to the filter_dependencies field
-        self.__apply_validator_result(pcmci_result)
-        
-        self.result = self.get_selected_features()
-        # shrink dataframe d and dependencies by the validator result
-        self.shrink(self.result)
-        
-        # final causal model
-        self.causal_model = self.validator.dependencies
-        self.save_validator_res()
-        
-        CP.info("\nFeature selected: " + str(self.result))
-        return self.result, self.causal_model
+        self.dependencies = self.__PCMCI_to_DAG()
+        return self.dependencies
     
     
-    def get_causal_matrix(self):
+    def run_pc(self, data: Data, link_assumptions = None):
         """
-        Returns a dictionary with keys the lags and values the causal matrix containing the causal weights between targets (rows) and sources (columns)
+        Run PC causal discovery algorithm
 
-        Returns:
-            dict/np.ndarray: causal matrix per 
-        """
-        cm_per_lag = {lag : np.zeros((len(self.result), len(self.result))) for lag in range(self.min_lag, self.max_lag + 1)}
-        vars = ['$' + var +'$' for var in self.result]
-        for lag in cm_per_lag:
-            for var in vars:
-                for source in self.causal_model[var]:
-                    if source[LAG] == lag: cm_per_lag[lag][vars.index(var)][vars.index(source[SOURCE])] = source[SCORE]
-        if len(cm_per_lag) == 1: return list(cm_per_lag.values())[0]
-        return cm_per_lag
-    
-    
-    def get_SCM(self):
-        """
-        Return Structural Causal Model
-
-        Raises:
-            ValueError: "Causal Model not estimated yet" if self.causal_model is None
+        Args:
+            data (Data): Data obj to analyse
+            link_assumptions (dict, optional): prior assumptions on causal model links. Defaults to None.
 
         Returns:
-            dict(str:list(tuple)): SCM of the causal model in the format "target": [(source, lag) ...] (e.g. "$X0$" : [("$X0$", -1), ("$X1$", -2)]) 
+            (DAG): estimated parents
         """
-        if self.causal_model is None:
-            raise ValueError("Causal Model not estimated yet.")
-        scm = {v: list() for v in self.data.pretty_features}
-        for t in self.causal_model.keys():
-            for s in self.causal_model[t]:
-                scm[t].append((s[SOURCE], -s[LAG])) 
-        return scm
-    
-
-    def shrink(self, sel_features):
-        """
-        Wrapper in order to shrink data.d and dependencies
+        
+        CP.info('\n')
+        CP.info(DASH)
+        CP.info("Running Causal Discovery Algorithm")
 
-        Args:
-            sel_features (list(str)): list of selected features
-        """
-        self.data.shrink(sel_features)
-        self.__shrink_dependencies()
-    
+        # build tigramite dataset
+        vector = np.vectorize(float)
+        d = vector(data.d)
+        dataframe = pp.DataFrame(data = d, var_names = data.features)
+        
+        # init and run pcmci
+        self.val_method = VAL(dataframe = dataframe,
+                              cond_ind_test = self.val_condtest,
+                              verbosity = self.verbosity)
+        
+        parents = self.val_method.run_pc_stable(link_assumptions = link_assumptions,
+                                                tau_max = self.max_lag,
+                                                tau_min = self.min_lag,
+                                                # pc_alpha = self.alpha,
+                                                )
     
-    def save_validator_res(self):
-        """
-        Saves dag plot if resfolder has been set otherwise it shows the figure
-        """
-        if self.result:
-            self.validator.save_result()
-        else:
-            CP.warning("Result impossible to save: no feature selected")
+        return self.__PC_to_DAG(parents, data.features)
     
     
-    def dag(self,
-            node_layout = 'dot',
-            min_width = 1,
-            max_width = 5,
-            min_score = 0,
-            max_score = 1,
-            node_size = 8,
-            node_color = 'orange',
-            edge_color = 'grey',
-            font_size = 12,
-            label_type = LabelType.Lag):
-        """
-        Saves dag plot if resfolder has been set otherwise it shows the figure
-        
-        Args:
-            node_layout (str, optional): Node layout. Defaults to 'dot'.
-            min_width (int, optional): minimum linewidth. Defaults to 1.
-            max_width (int, optional): maximum linewidth. Defaults to 5.
-            min_score (int, optional): minimum score range. Defaults to 0.
-            max_score (int, optional): maximum score range. Defaults to 1.
-            node_size (int, optional): node size. Defaults to 8.
-            node_color (str, optional): node color. Defaults to 'orange'.
-            edge_color (str, optional): edge color. Defaults to 'grey'.
-            font_size (int, optional): font size. Defaults to 12.
-            label_type (LabelType, optional): enum to set whether to show the lag time (LabelType.Lag) or the strength (LabelType.Score) of the dependencies on each link/node or not showing the labels (LabelType.NoLabels). Default LabelType.Lag.
-        """
-        
-        if self.result:
-            self.validator.build_dag(node_layout,
-                                     min_width, 
-                                     max_width,
-                                     min_score,
-                                     max_score,
-                                     node_size,
-                                     node_color,
-                                     edge_color,
-                                     font_size,
-                                     label_type)
-        else:
-            CP.warning("Dag impossible to create: no feature selected")
-    
-        
-    def timeseries_dag(self,
-                       min_width = 1,
-                       max_width = 5,
-                       min_score = 0,
-                       max_score = 1,
-                       node_size = 8,
-                       font_size = 12,
-                       node_color = 'orange',
-                       edge_color = 'grey'):
+    def __my_mci(self, autodep_dag: DAG):#, link_assumptions=None, parents=None):
         """
-        Saves timeseries dag plot if resfolder has been set otherwise it shows the figure
-        
-        Args:
-            min_width (int, optional): minimum linewidth. Defaults to 1.
-            max_width (int, optional): maximum linewidth. Defaults to 5.
-            min_score (int, optional): minimum score range. Defaults to 0.
-            max_score (int, optional): maximum score range. Defaults to 1.
-            node_size (int, optional): node size. Defaults to 8.
-            node_color (str, optional): node color. Defaults to 'orange'.
-            edge_color (str, optional): edge color. Defaults to 'grey'.
-            font_size (int, optional): font size. Defaults to 12.
-        """
-        
-        if self.result:
-            self.validator.build_ts_dag(min_width,
-                                        max_width,
-                                        min_score,
-                                        max_score,
-                                        node_size,
-                                        node_color,
-                                        edge_color,
-                                        font_size)
-        else:
-            CP.warning("Timeseries dag impossible to create: no feature selected")
+        Performs MCI test
 
-
-    def get_selected_features(self):
-        """
-        Defines the list of selected variables for d
+        Args:
+            link_assumptions (dict, optional): link assumptions. Defaults to None.
+            parents (dict, optional): parents dictionary. Defaults to None.
 
         Returns:
-            list(str): list of selected variable names
+            (dict): MCI result
         """
-        f_list = list()
-        for t in self.filter_dependencies:
-            sources_t = self.__get_dependencies_for_target(t)
-            if self.neglect_only_autodep and self.__is_only_autodep(sources_t, t):
-                sources_t.remove(t)
-            if sources_t: sources_t.append(t)
-            f_list = list(set(f_list + sources_t))
-        res = [f for f in self.data.features if f in f_list]
+        _int_link_assumptions = self.val_method._set_link_assumptions(autodep_dag.get_link_assumptions(autodep_ok = True), 
+                                                                      self.min_lag, self.max_lag)
 
-        return res
+        # Set the maximum condition dimension for Y and X
+        max_conds_py = self.val_method._set_max_condition_dim(None, self.min_lag, self.max_lag)
+        max_conds_px = self.val_method._set_max_condition_dim(None, self.min_lag, self.max_lag)
+        
+        # Get the parents that will be checked
+        _int_parents = self.val_method._get_int_parents(autodep_dag.get_parents())
+        
+        # Initialize the return values
+        val_matrix = np.zeros((self.val_method.dataframe.N, self.val_method.dataframe.N, self.max_lag + 1))
+        p_matrix = np.ones((self.val_method.dataframe.N, self.val_method.dataframe.N, self.max_lag + 1))
+        # Initialize the optional return of the confidance matrix
+        conf_matrix = None
+        if self.val_method.cond_ind_test.confidence is not None:
+            conf_matrix = np.zeros((self.val_method.dataframe.N, self.val_method.dataframe.N, self.max_lag + 1, 2))
+
+        # Get the conditions as implied by the input arguments
+        for j, i, tau, Z in self.val_method._iter_indep_conds(_int_parents,
+                                                              _int_link_assumptions,
+                                                              max_conds_py,
+                                                              max_conds_px):
+            # Set X and Y (for clarity of code)
+            X = [(i, tau)]
+            Y = [(j, 0)]
+
+            if ((i, -abs(tau)) in _int_link_assumptions[j] and _int_link_assumptions[j][(i, -abs(tau))] in ['-->', 'o-o']):
+                if autodep_dag.g[autodep_dag.features[j]].is_autodependent:
+                    val = autodep_dag.g[autodep_dag.features[j]].sources[(autodep_dag.features[i], abs(tau))][SCORE]
+                    pval = autodep_dag.g[autodep_dag.features[j]].sources[(autodep_dag.features[i], abs(tau))][PVAL]
+                else:
+                    val = 1. 
+                    pval = 0.
+            else:
+                val, pval = self.val_method.cond_ind_test.run_test(X, Y, Z=Z, tau_max=self.max_lag)
+            val_matrix[i, j, abs(tau)] = val
+            p_matrix[i, j, abs(tau)] = pval
+            CP.info("\t|val = " + str(round(val,3)) + " |pval = " + str(str(round(pval,3))))
+
+
+            # Get the confidence value, returns None if cond_ind_test.confidence
+            # is False
+            conf = self.val_method.cond_ind_test.get_confidence(X, Y, Z=Z, tau_max=self.max_lag)
+            # Record the value if the conditional independence requires it
+            if self.val_method.cond_ind_test.confidence:
+                conf_matrix[i, j, abs(tau)] = conf
+
+        # Threshold p_matrix to get graph
+        final_graph = p_matrix <= self.alpha
+
+        # Convert to string graph representation
+        graph = self.val_method.convert_to_string_graph(final_graph)
+
+        # Symmetrize p_matrix and val_matrix
+        symmetrized_results = self.val_method.symmetrize_p_and_val_matrix(
+                            p_matrix=p_matrix, 
+                            val_matrix=val_matrix, 
+                            link_assumptions=_int_link_assumptions,
+                            conf_matrix=conf_matrix)
+
+        if self.verbosity > 0:
+            self.val_method.print_significant_links(graph = graph,
+                                                    p_matrix = symmetrized_results['p_matrix'], 
+                                                    val_matrix = symmetrized_results['val_matrix'],
+                                                    conf_matrix = symmetrized_results['conf_matrix'],
+                                                    alpha_level = self.alpha)
+
+        # Return the values as a dictionary and store in class
+        results = {
+            'graph': graph,
+            'p_matrix': symmetrized_results['p_matrix'],
+            'val_matrix': symmetrized_results['val_matrix'],
+            'conf_matrix': symmetrized_results['conf_matrix'],
+                   }
+        self.results = results
+        return results
     
     
-    def show_dependencies(self):
-        """
-        Saves dependencies graph if resfolder is set otherwise it shows the figure
-        """
-        # FIXME: LAG not considered
-        dependencies_matrix = self.__get_dependencies_matrix()
-
-        fig, ax = plt.subplots()
-        im = ax.imshow(dependencies_matrix, cmap=plt.cm.Greens, interpolation='nearest', vmin=0, vmax=1, origin='lower')
-        fig.colorbar(im, orientation='vertical', label="score")
-
-        plt.xlabel("Sources")
-        plt.ylabel("Targets")
-        plt.xticks(ticks = range(0, self.data.orig_N), labels = self.data.orig_pretty_features, fontsize = 8)
-        plt.yticks(ticks = range(0, self.data.orig_N), labels = self.data.orig_pretty_features, fontsize = 8)
-        plt.title("Dependencies")
-
-        if self.dependency_path is not None:
-            plt.savefig(self.dependency_path, dpi = 300)
-        else:
-            plt.show()
-
-
-    def print_dependencies(self):
-        """
-        Print dependencies found by the selector
-        """
-        for t in self.o_filter_dependecies:
-            print()
-            print()
-            print(DASH)
-            print("Target", t)
-            print(DASH)
-            print('{:<10s}{:>15s}{:>15s}{:>15s}'.format('SOURCE', 'SCORE', 'PVAL', 'LAG'))
-            print(DASH)
-            for s in self.o_filter_dependecies[t]:
-                print('{:<10s}{:>15.3f}{:>15.3f}{:>15d}'.format(s[SOURCE], s[SCORE], s[PVAL], s[LAG]))      
-
-
-    def load_result(self, res_path):
-        with open(res_path, 'rb') as f:
-            self.validator.result = pickle.load(f)
-
-
-    def __shrink_dependencies(self):
-        """
-        Shrinks dependencies based on the selected features
-        """
-        difference_set = self.filter_dependencies.keys() - self.data.features
-        for d in difference_set: 
-            del self.filter_dependencies[d]
-            if self.validator.dependencies is not None: del self.validator.dependencies['$' + d + '$']
- 
-
-    def __get_dependencies_for_target(self, t):
+    def check_autodependency(self, data: Data, dag:DAG, link_assumptions) -> DAG:
         """
-        Returns list of sources for a specified target
+        Run MCI test on observational data using the causal structure computed by the validator 
 
         Args:
-            t (str): target variable name
+            data (Data): Data obj to analyse
+            dag (DAG): causal model
+            link_assumptions (dict): prior assumptions on causal model links. Defaults to None.
 
         Returns:
-            list(str): list of sources for target t
+            (DAG): estimated causal model
         """
-        return [s[SOURCE] for s in self.filter_dependencies[t]]
-    
+        
+        CP.info("\n##")
+        CP.info("## Auto-dependency check on observational data")
+        CP.info("##")
+        
+        # build tigramite dataset
+        vector = np.vectorize(float)
+        d = vector(data.d)
+        dataframe = pp.DataFrame(data = d, var_names = data.features)
+        
+        # init and run pcmci
+        self.val_method = VAL(dataframe = dataframe,
+                              cond_ind_test = self.val_condtest,
+                              verbosity = 0)
+        
+        _int_link_assumptions = self.val_method._set_link_assumptions(link_assumptions, self.min_lag, self.max_lag)
+
+        # Set the maximum condition dimension for Y and X
+        max_conds_py = self.val_method._set_max_condition_dim(None, self.min_lag, self.max_lag)
+        max_conds_px = self.val_method._set_max_condition_dim(None, self.min_lag, self.max_lag)
+        
+        # Get the parents that will be checked
+        _int_parents = self.val_method._get_int_parents(dag.get_parents())
+
+        # Get the conditions as implied by the input arguments
+        links_tocheck = self.val_method._iter_indep_conds(_int_parents, _int_link_assumptions, max_conds_py, max_conds_px)
+        for j, i, tau, Z in links_tocheck:
+            if data.features[j] not in dag.autodep_nodes or j != i: continue
+            else:
+                # Set X and Y (for clarity of code)
+                X = [(i, tau)]
+                Y = [(j, 0)]
+                
+                CP.info("\tlink: (" + data.features[i] + " " + str(tau) + ") -?> (" + data.features[j] + "):")
+                # Run the independence tests and record the results
+                val, pval = self.val_method.cond_ind_test.run_test(X, Y, Z = Z, tau_max = self.max_lag)
+                if pval > self.alpha:
+                    dag.del_source(data.features[j], data.features[j], abs(tau))
+                    CP.info("\t|val = " + str(round(val,3)) + " |pval = " + str(str(round(pval,3))) + " -- removed")
+
+                else:
+                    dag.g[data.features[j]].sources[(data.features[i], abs(tau))][SCORE] = val
+                    dag.g[data.features[j]].sources[(data.features[i], abs(tau))][PVAL] = pval
+                    CP.info("\t|val = " + str(round(val,3)) + " |pval = " + str(str(round(pval,3))) + " -- ok")
+                
+        return dag
+ 
     
-    def __is_only_autodep(self, sources, t):
+    def run_mci(self, data: Data, autodep_dag:DAG):#, link_assumptions, parents):
         """
-        Returns list of sources for a specified target
+        Run MCI test on observational data using the causal structure computed by the validator 
 
         Args:
-            sources (list(str)): list of sources for the selected target
-            t (str): target variable name
+            data (Data): Data obj to analyse
+            link_assumptions (dict): prior assumptions on causal model links. Defaults to None.
+            parents (dict): causal structure
 
         Returns:
-            (bool): True if sources list contains only the target. False otherwise
+            (DAG): estimated causal model
         """
-        if len(sources) == 1 and sources[0] == t: return True
-        return False
+        
+        CP.info("\n##")
+        CP.info("## MCI test analysis")
+        CP.info("##")
 
+        # build tigramite dataset
+        vector = np.vectorize(float)
+        d = vector(data.d)
+        dataframe = pp.DataFrame(data = d, var_names = data.features)
+        
+        # init and run pcmci
+        self.val_method = VAL(dataframe = dataframe,
+                              cond_ind_test = self.val_condtest,
+                              verbosity = self.verbosity)
 
-    def __get_dependencies_matrix(self):
+        # self.result = self.__my_mci(link_assumptions = autodep_dag.get_link_assumptions(autodep_ok = True),
+        #                             parents = autodep_dag.get_parents())
+        self.result = self.__my_mci(autodep_dag)
+        
+        self.result['var_names'] = data.features
+        self.result['pretty_var_names'] = data.pretty_features
+        
+        self.dependencies = self.__PCMCI_to_DAG()
+        return self.dependencies
+    
+    
+    def __PC_to_DAG(self, parents, features):
         """
-        Returns a matrix composed by scores for each target
+        Re-elaborates the PC result in a dag
+
+        Args:
+            parents (dict): causal structure
+            features (list): feature list
 
         Returns:
-            (np.array): score matrix
+            (DAG): pc result re-elaborated
         """
-        dep_mat = list()
-        for t in self.o_filter_dependecies:
-            dep_vet = [0] * self.data.orig_N
-            for s in self.o_filter_dependecies[t]:
-                dep_vet[self.data.orig_features.index(s[SOURCE])] = s[SCORE]
-            dep_mat.append(dep_vet)
-
-        dep_mat = np.array(dep_mat)
-        inf_mask = np.isinf(dep_mat)
-        neginf_mask = np.isneginf(dep_mat)
-        max_dep_mat = np.max(dep_mat[(dep_mat != -np.inf) & (dep_mat != np.inf)])
-        min_dep_mat = np.min(dep_mat[(dep_mat != -np.inf) & (dep_mat != np.inf)])
-
-        dep_mat[inf_mask] = max_dep_mat
-        dep_mat[neginf_mask] = min_dep_mat
-        dep_mat = (dep_mat - min_dep_mat) / (max_dep_mat - min_dep_mat)
-        return dep_mat
-
-
-    def __get_link_assumptions(self):
+        tmp_dag = DAG(features, self.min_lag, self.max_lag)
+        tmp_dag.sys_context = self.sys_context
+        for t in parents:
+            for s in parents[t]:
+                if features[t] in self.sys_context.keys() and features[s[0]] == self.sys_context[features[t]]:
+                    tmp_dag.g[features[t]].intervention_node = True
+                    tmp_dag.g[features[t]].associated_context = features[s[0]]
+                tmp_dag.add_source(features[t], features[s[0]], 1.0, 0.0, s[1])
+        return tmp_dag
+    
+    
+    def __PCMCI_to_DAG(self):
         """
-        Return selected links found by the selector
-        in this form: {0: {(0,-1) : "-?>", (2,-1) : "-?>"}}
+        Re-elaborates the PCMCI result in a new dictionary
 
         Returns:
-            (dict): selected links
+            (DAG): pcmci result re-elaborated
         """
-        sel_links = {self.data.features.index(f):dict() for f in self.data.features}
-        for t in self.filter_dependencies:
-            
-            # add links
-            for s in self.filter_dependencies[t]:
-                sel_links[self.data.features.index(t)][(self.data.features.index(s[SOURCE]), -s[LAG])] = '-?>'
-
-        return sel_links
-    
-    
-    def __apply_validator_result(self, causal_model):
-        """
-        Exclude dependencies based on validator result
-        It does not overwrite the filter_dependencies' inference/p-values matrix with the ones found by the validator
-        """
-        list_diffs = list()
-        tmp_dependencies = copy.deepcopy(self.filter_dependencies)
-        for t in tmp_dependencies:
-            for s in tmp_dependencies[t]:
-                if (self.data.features.index(s[SOURCE]), -s[LAG]) not in causal_model[self.data.features.index(t)]:
-                    list_diffs.append((s[SOURCE], str(s[LAG]), t))
-                    self.filter_dependencies[t].remove(s)
-        if list_diffs:
-            CP.debug(DASH)
-            CP.debug("Difference(s)")
-            CP.debug(DASH)
-            for diff in list_diffs:
-                CP.debug("Removing (" + diff[0] + " -" + diff[1] +") --> (" + diff[2] + ")")
-    
+        vars = self.result['var_names']
+        tmp_dag = DAG(vars, self.min_lag, self.max_lag)
+        tmp_dag.sys_context = self.sys_context
+        N, lags = self.result['graph'][0].shape
+        for s in range(len(self.result['graph'])):
+            for t in range(N):
+                for lag in range(lags):
+                    if self.result['graph'][s][t,lag] == '-->':
+                        if vars[t] in self.sys_context.keys() and vars[s] == self.sys_context[vars[t]]:
+                            tmp_dag.g[vars[t]].intervention_node = True
+                            tmp_dag.g[vars[t]].associated_context = vars[s]
+                        tmp_dag.add_source(vars[t], 
+                                           vars[s],
+                                           self.result['val_matrix'][s][t,lag],
+                                           self.result['p_matrix'][s][t,lag],
+                                           lag)
+        return tmp_dag
```

### Comparing `fpcmci-4.2.1/fpcmci/basics/utils.py` & `fpcmci-4.3.0/fpcmci/basics/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,32 +14,18 @@
     """
     Return log file path
 
     Args:
         resfolder (str): result folder
 
     Returns:
-        (str, str): log file path, dependency image file path
+        (str): log file path
     """
     Path(SEP.join([RESULTS_FILENAME, resfolder])).mkdir(parents=True, exist_ok=True)
-    return SEP.join([RESULTS_FILENAME, resfolder, LOG_FILENAME]), SEP.join([RESULTS_FILENAME, resfolder, DEP_FILENAME])
+    return SEP.join([RESULTS_FILENAME, resfolder, LOG_FILENAME]), SEP.join([RESULTS_FILENAME, resfolder, RES_FILENAME]), SEP.join([RESULTS_FILENAME, resfolder, DAG_FILENAME]), SEP.join([RESULTS_FILENAME, resfolder, TSDAG_FILENAME])
 
 
 def create_results_folder():
     """
     Creates results folder if doesn't exist
     """
-    Path(RESULTS_FILENAME).mkdir(parents=True, exist_ok=True)
-
-
-def get_validatorpaths(resfolder):
-    """
-    Creates resfolder if doesn't exist
-
-    Args:
-        resfolder (str): result folder name
-
-    Returns:
-        (str, str, str): result.pkl file path, dag file path, ts_dag file path
-    """
-    Path(SEP.join([RESULTS_FILENAME, resfolder])).mkdir(parents=True, exist_ok=True)
-    return SEP.join([RESULTS_FILENAME, resfolder, RES_FILENAME]), SEP.join([RESULTS_FILENAME, resfolder, DAG_FILENAME]), SEP.join([RESULTS_FILENAME, resfolder, TSDAG_FILENAME])
+    Path(RESULTS_FILENAME).mkdir(parents=True, exist_ok=True)
```

### Comparing `fpcmci-4.2.1/fpcmci/causal_graph.py` & `fpcmci-4.3.0/fpcmci/causal_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,18 +166,25 @@
     # edges definition
     edges = list()
     edge_width = dict()
     for t in res.keys():
         for s in res[t]:
             s_index = len(res.keys())-1 - list(res.keys()).index(s[SOURCE])
             t_index = len(res.keys())-1 - list(res.keys()).index(t)
-            s_node = (tau - s[LAG], s_index)
-            t_node = (tau, t_index)
-            edges.append((s_node, t_node))
-            edge_width[(s_node, t_node)] = __scale(s[SCORE], min_width, max_width, min_score, max_score)
+            
+            s_lag = tau - s[LAG]
+            t_lag = tau
+            while s_lag >= 0:
+                s_node = (s_lag, s_index)
+                t_node = (t_lag, t_index)
+                edges.append((s_node, t_node))
+                edge_width[(s_node, t_node)] = __scale(s[SCORE], min_width, max_width, min_score, max_score)
+                s_lag -= s[LAG]
+                t_lag -= s[LAG]
+                
     G.add_edges_from(edges)
 
     # label definition
     labeldict = {}
     for n in G.nodes():
         if n[0] == 0:
             labeldict[n] = list(res.keys())[len(res.keys()) - 1 - n[1]]
```

### Comparing `fpcmci-4.2.1/fpcmci/preprocessing/Subsampler.py` & `fpcmci-4.3.0/fpcmci/preprocessing/Subsampler.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.2.1/fpcmci/preprocessing/data.py` & `fpcmci-4.3.0/fpcmci/preprocessing/data.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.2.1/fpcmci/preprocessing/subsampling_methods/EntropyBasedMethod.py` & `fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/EntropyBasedMethod.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.2.1/fpcmci/preprocessing/subsampling_methods/Static.py` & `fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/Static.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.2.1/fpcmci/preprocessing/subsampling_methods/SubsamplingMethod.py` & `fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/SubsamplingMethod.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.2.1/fpcmci/preprocessing/subsampling_methods/WSDynamic.py` & `fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/WSDynamic.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.2.1/fpcmci/preprocessing/subsampling_methods/WSFFTStatic.py` & `fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/WSFFTStatic.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.2.1/fpcmci/preprocessing/subsampling_methods/WSStatic.py` & `fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/WSStatic.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.2.1/fpcmci/preprocessing/subsampling_methods/moving_window.py` & `fpcmci-4.3.0/fpcmci/preprocessing/subsampling_methods/moving_window.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.2.1/fpcmci/selection_methods/Corr.py` & `fpcmci-4.3.0/fpcmci/selection_methods/Corr.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,10 +34,10 @@
                 # Filter on pvalue
                 f = pval < self.alpha
 
                 # Result of the selection
                 sel_sources, sel_sources_score, sel_sources_pval = X.columns[f].tolist(), scores[f].tolist(), pval[f].tolist()
 
                 for s, score, pval in zip(sel_sources, sel_sources_score, sel_sources_pval):
-                    self._add_dependecies(target, s, score, pval, lag)
+                    self._add_dependecy(target, s, score, pval, lag)
 
         return self.result
```

### Comparing `fpcmci-4.2.1/fpcmci/selection_methods/MI.py` & `fpcmci-4.3.0/fpcmci/selection_methods/MI.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,10 +46,10 @@
         for t in results._single_target.keys():
             sel_sources = [s[0] for s in results._single_target[t]['selected_vars_sources']]
             if sel_sources:
                 sel_sources_lag = [s[1] for s in results._single_target[t]['selected_vars_sources']]
                 sel_sources_score = results._single_target[t]['selected_sources_mi']
                 sel_sources_pval = results._single_target[t]['selected_sources_pval']
                 for s, score, pval, lag in zip(sel_sources, sel_sources_score, sel_sources_pval, sel_sources_lag):
-                    self._add_dependecies(self.features[t], self.features[s], score, pval, lag)
+                    self._add_dependecy(self.features[t], self.features[s], score, pval, lag)
 
         return self.result
```

### Comparing `fpcmci-4.2.1/fpcmci/selection_methods/ParCorr.py` & `fpcmci-4.3.0/fpcmci/selection_methods/ParCorr.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,12 +72,12 @@
                     for candidate in candidates:
                         X = np.array(self.data.d[candidate][:-lag])
                         score, pval = self.partial_corr(X, Y, Z)
                         if pval < self.alpha and (tmp_res is None or abs(tmp_res[1]) < abs(score)):
                             tmp_res = (candidate, score, pval)
 
                     if tmp_res is not None: 
-                        self._add_dependecies(target, tmp_res[0], tmp_res[1], tmp_res[2], lag)
+                        self._add_dependecy(target, tmp_res[0], tmp_res[1], tmp_res[2], lag)
                         candidates.remove(tmp_res[0])
                     else:
                         break
         return self.result
```

### Comparing `fpcmci-4.2.1/fpcmci/selection_methods/SelectionMethod.py` & `fpcmci-4.3.0/fpcmci/selection_methods/SelectionMethod.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from abc import ABC, abstractmethod
 from enum import Enum
 from contextlib import contextmanager
 import sys, os
 from fpcmci.preprocessing.data import Data
 from fpcmci.basics.constants import *
+from fpcmci.CPrinter import CP
+from fpcmci.graph.DAG import DAG
 
 
 class CTest(Enum):
     Corr = "Correlation"
     MI = "Mutual Information"
     TE = "Transfer Entropy"
 
@@ -29,52 +31,53 @@
     """
     def __init__(self, ctest):
         self.ctest = ctest
         self.data = None
         self.alpha = None
         self.min_lag = None
         self.max_lag = None
-        self.result = dict()
+        self.result = None
 
 
     @property
     def name(self):
         """
         Returns Selection Method name
 
         Returns:
             (str): Selection Method name
         """
         return self.ctest.value
 
 
-    def initialise(self, data: Data, alpha, min_lag, max_lag):
+    # def initialise(self, data: Data, alpha, min_lag, max_lag):
+    def initialise(self, data: Data, alpha, min_lag, max_lag, graph):
         """
         Initialises the selection method
 
         Args:
             data (Data): Data
             alpha (float): significance threshold
             min_lag (int): min lag time
             max_lag (int): max lag time
         """
         self.data = data
         self.alpha = alpha
         self.min_lag = min_lag
         self.max_lag = max_lag
-        self.result = {f:list() for f in self.data.features}
+        self.result = graph
 
 
     @abstractmethod
-    def compute_dependencies(self) -> dict:
+    def compute_dependencies(self) -> DAG:
         """
         abstract method
         """
         pass
-
+    
 
     def _prepare_ts(self, target, lag, apply_lag = True, consider_autodep = True):
         """
         prepare the dataframe to the analysis
 
         Args:
             target (str): name target var
@@ -97,42 +100,29 @@
                 X = self.data.d[:-lag]
             else:
                 Y = self.data.d[target]
                 X = self.data.d
         return X, Y
 
 
-    def _get_sources(self, t):
-        """
-        Return target sources
-
-        Args:
-            t (str): target variable name
-
-        Returns:
-            list(str): list of target sources
-        """
-        return [s[SOURCE] for s in self.result[t]]
-
-
-    def _add_dependecies(self, t, s, score, pval, lag):
+    def _add_dependecy(self, t, s, score, pval, lag):
         """
         Adds found dependency from source (s) to target (t) specifying the 
         score, pval and the lag
 
         Args:
             t (str): target feature name
             s (str): source feature name
             score (float): selection method score
             pval (float): pval associated to the dependency
             lag (int): lag time of the dependency
         """
-        self.result[t].append({SOURCE:s, 
-                               SCORE:score,
-                               PVAL:pval, 
-                               LAG:lag})
+        self.result.add_source(t, s, score, pval, lag)
+        
         str_s = "(" + s + " -" + str(lag) + ")"
-        str_arrow = " --> "
         str_t = "(" + t + ")"
-        str_score = "|score: " + "{:.3f}".format(score)
-        str_pval = "|pval: " + "{:.3f}".format(pval)
-        print('{:<20s}{:<10s}{:<10s}{:<20s}{:<20s}'.format(str_s, str_arrow, str_t, str_score, str_pval))
+
+        CP.info("\tlink: " + str_s + " -?> " + str_t)
+        CP.info("\t|val = " + str(round(score,3)) + " |pval = " + str(str(round(pval,3))))
+        # CP.info("\n")
+
+
```

### Comparing `fpcmci-4.2.1/fpcmci/selection_methods/TE.py` & `fpcmci-4.3.0/fpcmci/selection_methods/TE.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,22 +66,22 @@
             
             # Auto-dependency handling
             auto_lag = [s[1] for s in res_auto._single_target[0]['selected_vars_sources']]
             auto_score = res_auto._single_target[0]['selected_sources_mi']
             auto_pval = res_auto._single_target[0]['selected_sources_pval']
             if auto_score is not None:
                 for score, pval, lag in zip(auto_score, auto_pval, auto_lag):
-                    self._add_dependecies(self.data.features[t], self.data.features[t], score, pval, lag)
+                    self._add_dependecy(self.data.features[t], self.data.features[t], score, pval, lag)
             
             # Cross-dependencies handling    
             sel_sources = [s[0] for s in res_cross._single_target[t]['selected_vars_sources']]
             if sel_sources:
                 sel_sources_lag = [s[1] for s in res_cross._single_target[t]['selected_vars_sources']]
                 sel_sources_score = res_cross._single_target[t]['selected_sources_te']
                 sel_sources_pval = res_cross._single_target[t]['selected_sources_pval']
                 for s, score, pval, lag in zip(sel_sources, sel_sources_score, sel_sources_pval, sel_sources_lag):
-                    self._add_dependecies(self.data.features[t], self.data.features[s], score, pval, lag)
+                    self._add_dependecy(self.data.features[t], self.data.features[s], score, pval, lag)
             
             if auto_score is None and not sel_sources:
-                CP.info("no sources selected")
+                CP.info("\tno sources selected")
 
         return self.result
```

### Comparing `fpcmci-4.2.1/fpcmci.egg-info/PKG-INFO` & `fpcmci-4.3.0/fpcmci.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fpcmci
-Version: 4.2.1
+Version: 4.3.0
 Summary: A causal discovery Python package
 Home-page: https://github.com/lcastri/fpcmci
 Author: Luca Castri
 Author-email: lucacastri94@gmail.com
 License: UNKNOWN
 Description: # <img src="https://github.com/lcastri/fpcmci/raw/developer/docs/assets/icon.png" width="25"> FPCMCI - Filtered PCMCI
```

### Comparing `fpcmci-4.2.1/fpcmci.egg-info/SOURCES.txt` & `fpcmci-4.3.0/fpcmci.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 fpcmci.egg-info/dependency_links.txt
 fpcmci.egg-info/requires.txt
 fpcmci.egg-info/top_level.txt
 fpcmci/basics/__init__.py
 fpcmci/basics/constants.py
 fpcmci/basics/logger.py
 fpcmci/basics/utils.py
+fpcmci/graph/DAG.py
+fpcmci/graph/Node.py
+fpcmci/graph/__init__.py
 fpcmci/preprocessing/Subsampler.py
 fpcmci/preprocessing/__init__.py
 fpcmci/preprocessing/data.py
 fpcmci/preprocessing/subsampling_methods/EntropyBasedMethod.py
 fpcmci/preprocessing/subsampling_methods/Static.py
 fpcmci/preprocessing/subsampling_methods/SubsamplingMethod.py
 fpcmci/preprocessing/subsampling_methods/WSDynamic.py
```

### Comparing `fpcmci-4.2.1/setup.py` & `fpcmci-4.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     version = VERSION,    
     description = 'A causal discovery Python package',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/lcastri/fpcmci',
     author = 'Luca Castri',
     author_email = 'lucacastri94@gmail.com',
-    packages = ['fpcmci', "fpcmci.preprocessing", "fpcmci.preprocessing.subsampling_methods", "fpcmci.basics", "fpcmci.selection_methods"],
+    packages = ['fpcmci', "fpcmci.preprocessing", "fpcmci.preprocessing.subsampling_methods", "fpcmci.basics", "fpcmci.selection_methods", "fpcmci.graph"],
     python_requires='>=3',
     install_requires = INSTALL_REQUIRES,
 
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',  
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
```

