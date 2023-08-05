# Comparing `tmp/compositional-2022.8.31.tar.gz` & `tmp/compositional-2023.7.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compositional-2022.8.31.tar", last modified: Thu Sep  1 01:45:11 2022, max compression
+gzip compressed data, was "compositional-2023.7.20.tar", last modified: Thu Jul 20 22:08:26 2023, max compression
```

## Comparing `compositional-2022.8.31.tar` & `compositional-2023.7.20.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2022-09-01 01:45:11.904551 compositional-2022.8.31/
--rw-------   0 jespinoz  (3456) staff       (20)     2017 2020-05-14 00:14:55.000000 compositional-2022.8.31/LICENSE.txt
--rw-r--r--   0 jespinoz  (3456) staff       (20)      259 2022-09-01 01:45:11.904211 compositional-2022.8.31/PKG-INFO
--rw-------   0 jespinoz  (3456) staff       (20)     7023 2021-01-11 23:55:24.000000 compositional-2022.8.31/README.md
-drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2022-09-01 01:45:11.899797 compositional-2022.8.31/compositional/
--rw-------   0 jespinoz  (3456) staff       (20)     2610 2022-09-01 01:19:59.000000 compositional-2022.8.31/compositional/__init__.py
--rw-------   0 jespinoz  (3456) staff       (20)    25466 2022-09-01 01:23:55.000000 compositional-2022.8.31/compositional/compositional.py
-drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2022-09-01 01:45:11.903736 compositional-2022.8.31/compositional.egg-info/
--rw-------   0 jespinoz  (3456) staff       (20)        0 2022-08-30 21:34:11.000000 compositional-2022.8.31/compositional.egg-info/Icon
--rw-------   0 jespinoz  (3456) staff       (20)      259 2022-09-01 01:45:11.000000 compositional-2022.8.31/compositional.egg-info/PKG-INFO
--rw-------   0 jespinoz  (3456) staff       (20)      300 2022-09-01 01:45:11.000000 compositional-2022.8.31/compositional.egg-info/SOURCES.txt
--rw-------   0 jespinoz  (3456) staff       (20)        1 2022-09-01 01:45:11.000000 compositional-2022.8.31/compositional.egg-info/dependency_links.txt
--rw-------   0 jespinoz  (3456) staff       (20)       13 2022-09-01 01:45:11.000000 compositional-2022.8.31/compositional.egg-info/requires.txt
--rw-------   0 jespinoz  (3456) staff       (20)       14 2022-09-01 01:45:11.000000 compositional-2022.8.31/compositional.egg-info/top_level.txt
--rw-r--r--   0 jespinoz  (3456) staff       (20)       38 2022-09-01 01:45:11.904666 compositional-2022.8.31/setup.cfg
--rw-------   0 jespinoz  (3456) staff       (20)      693 2020-05-14 09:20:41.000000 compositional-2022.8.31/setup.py
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-07-20 22:08:26.101521 compositional-2023.7.20/
+-rw-------   0 jespinoz  (3456) staff       (20)     1563 2023-07-20 21:39:20.000000 compositional-2023.7.20/LICENSE
+-rw-r--r--   0 jespinoz  (3456) staff       (20)      283 2023-07-20 22:08:26.101187 compositional-2023.7.20/PKG-INFO
+-rw-------   0 jespinoz  (3456) staff       (20)     7475 2023-07-20 22:07:50.000000 compositional-2023.7.20/README.md
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-07-20 22:08:26.097963 compositional-2023.7.20/compositional/
+-rw-------   0 jespinoz  (3456) staff       (20)      780 2023-07-20 21:38:17.000000 compositional-2023.7.20/compositional/__init__.py
+-rw-------   0 jespinoz  (3456) staff       (20)    35699 2023-07-20 21:38:53.000000 compositional-2023.7.20/compositional/compositional.py
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-07-20 22:08:26.100670 compositional-2023.7.20/compositional.egg-info/
+-rw-------   0 jespinoz  (3456) staff       (20)      283 2023-07-20 22:08:26.000000 compositional-2023.7.20/compositional.egg-info/PKG-INFO
+-rw-------   0 jespinoz  (3456) staff       (20)      267 2023-07-20 22:08:26.000000 compositional-2023.7.20/compositional.egg-info/SOURCES.txt
+-rw-------   0 jespinoz  (3456) staff       (20)        1 2023-07-20 22:08:26.000000 compositional-2023.7.20/compositional.egg-info/dependency_links.txt
+-rw-------   0 jespinoz  (3456) staff       (20)       13 2023-07-20 22:08:26.000000 compositional-2023.7.20/compositional.egg-info/requires.txt
+-rw-------   0 jespinoz  (3456) staff       (20)       14 2023-07-20 22:08:26.000000 compositional-2023.7.20/compositional.egg-info/top_level.txt
+-rw-r--r--   0 jespinoz  (3456) staff       (20)       38 2023-07-20 22:08:26.101654 compositional-2023.7.20/setup.cfg
+-rw-------   0 jespinoz  (3456) staff       (20)      693 2020-05-14 09:20:41.000000 compositional-2023.7.20/setup.py
```

### Comparing `compositional-2022.8.31/LICENSE.txt` & `compositional-2023.7.20/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# ==============
-# compositional
-# ==============
-# Compositional data analysis in Python
-# ------------------------------------
-# GitHub: https://github.com/jolespin/compositional
-# PyPI: https://pypi.org/project/compositional
-# ------------------------------------
-# =======
-# Contact
-# =======
-# Producer: Josh L. Espinoza
-# Contact: jespinoz@jcvi.org, jol.espinoz@gmail.com
-# Google Scholar: https://scholar.google.com/citations?user=r9y1tTQAAAAJ&hl
 # =======
 # License BSD-3
 # =======
 # https://opensource.org/licenses/BSD-3-Clause
 #
 # Copyright 2018 Josh L. Espinoza
 #
```

### Comparing `compositional-2022.8.31/README.md` & `compositional-2023.7.20/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 ```	
 	
 
 		
 
 #### Install:
 ```
-# "Stable" release (still developmental)
+# Stable release (Preferred)
 pip install compositional
-# Current release
+
+# Developmental release
 pip install git+https://github.com/jolespin/compositional
 ```
 
 #### Proportionality methods adapted from the following source:
 * [propr: An R package to calculate proportionality between vectors of compositional data
  (Thomm Quinn)](https://github.com/tpq/propr)
  
@@ -85,26 +86,41 @@
 
 #### Loading package and obtaining data
 ```python
 import compositional as coda
 import pandas as pd
 
 # Load abundances (Gomez and Espinoza et al. 2017)
-X = pd.read_csv("https://github.com/jolespin/supragingival_plaque_microbiome/blob/master/16S_amplicons/Data/X.tsv.gz?raw=true", 
+X = pd.read_csv("https://github.com/jolespin/projects/raw/main/supragingival_plaque_microbiome/16S_amplicons/Data/X.tsv.gz", 
                 sep="\t",
                 index_col=0,
                 compression="gzip",
 )
 # Add pseudocount
 delta = 1/X.shape[1]**2 # http://scikit-bio.org/docs/latest/generated/skbio.stats.composition.multiplicative_replacement.html
 X = X + delta
 # print("X.shape: (n={} samples, m={} OTUs)| delta={}".format(*X.shape, delta))
 # X.shape: (n=473 samples, m=481 OTUs) | delta=4.322249644494967e-06
 ```
 
+#### (Highpass) Filtering of compositional data
+Here we are going to first remove all samples with less than 10,000 total counts, then all features that aren't in at least 50% of the samples, and then samples that don't have at least 50 detected components.
+
+```
+X_filtered = coda.filter_data_highpass(
+    X=X, 
+    minimum_total_counts=10000,
+    minimum_prevalence=0.5,
+    minimum_components=50,
+)
+
+X.shape, X_filtered.shape
+# ((473, 481), (401, 93))
+```
+
 #### Pairwise operations
 ```
 # Pairwise variance log-ratio
 vlr = coda.pairwise_vlr(X)
 # print(vlr.iloc[:4,:4])
 #            Otu000514  Otu000001  Otu000038  Otu000003
 # Otu000514   0.000000   2.158950   3.763323   3.453961
```

### Comparing `compositional-2022.8.31/compositional/compositional.py` & `compositional-2023.7.20/compositional/compositional.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from __future__ import print_function, division
 
 # Built-ins
-import sys,warnings,functools
+import sys,warnings,functools, operator
 from collections.abc import Mapping 
 from importlib import import_module
 
 # Version specific
 if sys.version_info.major == 2:
     from StringIO import StringIO
 if sys.version_info.major == 3:
@@ -16,14 +16,36 @@
 import numpy as np
 import pandas as pd
 from pandas._libs.algos import nancorr
 
 # =========
 # Utilities
 # =========
+def assert_acceptable_arguments(query, target, operation="le", message="Invalid option provided.  Please refer to the following for acceptable arguments:"):
+    """
+    le: operator.le(a, b) : <=
+    eq: operator.eq(a, b) : ==
+    ge: operator.ge(a, b) : >=
+    """
+    def is_nonstring_iterable(obj):
+        condition_1 = hasattr(obj, "__iter__")
+        condition_2 =  not type(obj) == str
+        return all([condition_1,condition_2])
+    
+    # If query is not a nonstring iterable or a tuple
+    if any([
+            not is_nonstring_iterable(query),
+            isinstance(query,tuple),
+            ]):
+        query = [query]
+    query = set(query)
+    target = set(target)
+    func_operation = getattr(operator, operation)
+    assert func_operation(query,target), "{}\n{}".format(message, target)
+
 # Check packages
 def check_packages(packages, namespace=None, import_into_backend=True, verbose=False):
     """
     Check if packages are available (and import into global namespace)
     If package is a tuple then imports as follows: ("numpy", "np") where "numpy" is full package name and "np" is abbreviation
     To import packages into current namespace: namespace = globals()
     To import packages in backend, e.g. if this is used in a module/script, use `import_into_backend`
@@ -69,17 +91,166 @@
                         print("Cannot import {}:".format(pkg_name), False, file=sys.stderr)
             assert not missing_packages, "Please install the following packages to use this function:\n{}".format( ", ".join(missing_packages))
             return func(*args, **kwargs)
 
         return wrapper
     return decorator
 
+def check_compositional(X, n_dimensions:int=None, acceptable_dimensions:set={1,2}):
+    """
+    # Description
+    Check that 1D and 2D NumPy/Pandas objects are the correct shape and >= 0
+
+    # Parameters
+        * X:
+            - Compositional data
+            (1D): pd.Series or 1D np.array
+            (2D): pd.DataFrame or 2D np.array
+        * n_dimensions: int   
+    """
+    if n_dimensions is None:
+        n_dimensions = len(X.shape)
+    if not hasattr(acceptable_dimensions, "__iter__"):
+        acceptable_dimensions = {acceptable_dimensions}
+    assert n_dimensions in acceptable_dimensions, "`X` must be {}".format(" or ".join(map(lambda d: f"{d}D", acceptable_dimensions)))
+    assert np.all(X >= 0), "`X` cannot contain negative values."
+
+# ===========================
+# Summary metrics
+# ===========================
+def sparsity(X, checks=True):
+    """
+    # Description
+    Calculates the sparsity (i.e., ratio of zeros) in a NumPy or Pandas object
+
+    # Parameters
+        * X:
+            - Compositional data
+            (1D): pd.Series or 1D np.array
+            (2D): pd.DataFrame or 2D np.array
+        * checks:
+            Check whether or not dimmensions are correct and data is >= 0
+    * Output
+        Ratio zeros
+    """
+    n_dimensions = len(X.shape)
+    if checks:
+        check_compositional(X, n_dimensions)
+
+    if n_dimensions == 2:
+        if isinstance(X, pd.DataFrame):
+            X = X.values
+        X = X.ravel()
+    number_of_zeros = np.sum(X == 0)
+    number_of_values = X.size
+    return number_of_zeros/number_of_values
+
+def number_of_components(X, checks=True):
+    """
+    # Description
+    Calculates the number of detected components (i.e., richness) in a NumPy or Pandas object
+
+    # Parameters
+        * X:
+            - Compositional data
+            (1D): pd.Series or 1D np.array of a composition (i.e., sample)
+            (2D): pd.DataFrame or 2D np.array (rows=samples/compositions, columns=features/components)
+        * checks:
+            Check whether or not dimmensions are correct and data is >= 0
+    * Output
+        Number of components per composition (i.e., sample)
+    """
+    n_dimensions = len(X.shape)
+    
+    if checks:
+        check_compositional(X, n_dimensions)
+    
+    if n_dimensions == 2:
+        return (X > 0).sum(axis=1)
+        
+    else:
+        return (X > 0).sum()
+
+def prevalence_of_components(X, checks=True):
+    """
+    # Description
+    Calculates the prevalence of detected components in a NumPy or Pandas object
+
+    # Parameters
+        * X:
+            - Compositional data
+            (1D): pd.Series or 1D np.array of a component vector
+            (2D): pd.DataFrame or 2D np.array (rows=samples/compositions, columns=features/components)
+        * checks:
+            Check whether or not dimmensions are correct and data is >= 0
+    * Output
+        Number of compositions where a component was detected
+    """
+    
+    n_dimensions = len(X.shape)
+    
+    if checks:
+        check_compositional(X, n_dimensions)
+    
+    if n_dimensions == 2:
+        return (X > 0).sum(axis=0)
+        
+    else:
+        return (X > 0).sum()
 # ===========================
 # Compositional data analysis
 # ===========================
+def transform_closure(X, checks=True):
+    """
+    # Description
+    Closure (e.g., total sum scaling, relative abundance) that can handle 1D and 2D NumPy  and Pandas objects
+
+    # Parameters
+        * X:
+            - Compositional data
+            (1D): pd.Series or 1D np.array
+            (2D): pd.DataFrame or 2D np.array
+        * checks:
+            Check whether or not dimmensions are correct and data is >= 0
+    * Output
+        Closure transformed matching input object class
+    """
+    
+    n_dimensions = len(X.shape)
+
+    if checks:
+        check_compositional(X, n_dimensions)
+    
+    if n_dimensions == 2:
+        
+        index = None
+        components = None
+        
+        if isinstance(X, pd.DataFrame):
+            index = X.index
+            components = X.columns
+            X = X.values
+            
+        X_closure = X/X.sum(axis=1).reshape(-1,1)
+        
+        if index is not None:
+            X_closure = pd.DataFrame(X_closure, index=index, columns=components)
+        
+    else:
+        components = None
+        if isinstance(X, pd.Series):
+            components = X.index
+            X = X.values
+            
+        X_closure = X/X.sum()
+        if components is not None:
+            X_closure = pd.Series(X_closure, index=components)
+
+    return X_closure
+
 # Extension of CLR to use custom centroids, references, and zeros without pseudocounts
 def transform_xlr(X, reference_components=None, centroid="mean", return_zeros_as_neginfinity=False, zeros_ok=True):
     """
     # Description
     Extension of CLR to incorporate custom centroids, reference components (iqlr), and handle missing values.
     This implementation is more versatile than skbio's implementation but that makes it slower if it done iteratively.
 
@@ -102,16 +273,16 @@
             True: Returns zeros as -np.inf 
             False: Returns zeros as np.nan
         * zeros_ok:
             True: Mask zeros with np.nan with warning
             False: Error
     """
     n_dimensions = len(X.shape)
-    assert n_dimensions in {1,2}, "`X` must be 1D or 2D"
-    assert np.all(X >= 0), "`X` cannot contain negative values because of log-transformation step."
+    check_compositional(X, n_dimensions)
+
     assert not isinstance(reference_components, tuple), "`reference_components` cannot be type tuple"
     # 1-Dimensional
     if n_dimensions == 1:
         # Check for labels
         components = None
         if isinstance(X, pd.Series):
             components = X.index
@@ -291,16 +462,15 @@
         * centroid, return_zeros_as_neginfinity, and zeros_ok: See `transform_xlr`
 
     Adapted from the following source:
         * https://github.com/tpq/propr/blob/2bd7c44bf59eaac6b4d329d38afd40ac83e2089a/R/2-proprCall.R#L31
     """
     # Checks
     n_dimensions = len(X.shape)
-    assert n_dimensions in {2}, "`X` must be 2D"
-    assert np.all(X >= 0), "`X` cannot contain negative values because of log-transformation step."
+    check_compositional(X, n_dimensions)
     assert interval_type in {"closed", "open"}, "`interval_type` must be in the following: {closed, open}"
     percentile_range = tuple(sorted(percentile_range))
     assert len(percentile_range) == 2, "percentile_range must have 2 elements"
     
     index=None
     components=None
     if isinstance(X, pd.DataFrame):
@@ -338,16 +508,15 @@
     Adapted from the following source:
     * https://github.com/tpq/propr
     ddof=1 for compatibility with propr package in R
     To properly handle missing values and optimize speed, nancorr from pandas must be used which does not take ddof
     """
     # Checks
     n_dimensions = len(X.shape)
-    assert n_dimensions in {2}, "`X` must be 2D"
-    assert np.all(X >= 0), "`X` cannot contain negative values because of log-transformation step."
+    check_compositional(X, n_dimensions, acceptable_dimensions={2})
 
     components = None
     if isinstance(X, pd.DataFrame):
         components = X.columns
         X = X.values
     X = X.astype("float64")
     n,m = X.shape
@@ -594,8 +763,144 @@
 
     # Without tree
     if tree is None:
         return _ilr_without_tree(X=X)
     # With tree
     else:
         return _ilr_with_tree(X=X, tree=tree)
+    
+# =========    
+# Filtering
+# =========
+def _filter_data(
+    X:pd.DataFrame,
+    total_counts,
+    prevalence,
+    components,
+    mode,
+    order_of_operations:list=["total_counts", "prevalence", "components"],
+    interval_type="closed",
+    ):
+
+    check_compositional(X, acceptable_dimensions=2)
+    assert_acceptable_arguments(query=order_of_operations,target=["total_counts", "prevalence", "components"], operation="le")
+    assert_acceptable_arguments(query=[mode],target=["highpass", "lowpass"], operation="le")
+    assert_acceptable_arguments(query=[interval_type],target=["closed", "open"], operation="le")
+
+
+    def _get_elements(data,tol,operation):
+        return data[lambda x: operation(x,tol)].index
+
+    def _filter_total_counts(X, tol, operation):
+        data = X.sum(axis=1)
+        return X.loc[_get_elements(data, tol, operation),:]
+
+    def _filter_prevalence(X, tol, operation):
+        conditions = [
+            isinstance(tol, float),
+            0.0 < tol <= 1.0,
+        ]
+
+        if all(conditions):
+            tol = round(X.shape[0]*tol)
+        data = (X > 0).sum(axis=0)
+        assert tol <= X.shape[0], "If prevalence is an integer ({}), it cannot be larger than the number of samples ({}) in the index".format(tol, X.shape[0])
+        return X.loc[:,_get_elements(data, tol, operation)]
+
+    def _filter_components(X, tol, operation):
+        data = (X > 0).sum(axis=1)
+        return X.loc[_get_elements(data, tol, operation),:]
+
+    if interval_type == "closed":
+        operations = {"highpass":operator.ge, "lowpass":operator.le}
+    if interval_type == "open":
+        operations = {"highpass":operator.gt, "lowpass":operator.lt}
+
+    # Defaults
+    if mode == "highpass":
+        if components is None:
+            components = 0
+        if total_counts is None:
+            total_counts = 0
+        if prevalence is None:
+            prevalence = 0
+    if mode == "lowpass":
+        if components in {None, np.inf}:
+            components = X.shape[1]
+        if total_counts in {None, np.inf}:
+            total_counts = np.inf
+        if prevalence in {None, np.inf}:
+            prevalence = X.shape[0]
+            
+    functions = dict(zip(["total_counts", "prevalence", "components"], [_filter_total_counts, _filter_prevalence, _filter_components]))
+    thresholds = dict(zip(["total_counts", "prevalence", "components"], [total_counts, prevalence, components]))
+
+    for strategy in order_of_operations:
+        tol = thresholds[strategy]
+        if tol is not None:
+            X = functions[strategy](X=X,tol=tol, operation=operations[mode])
+
+    return X
+        
+def filter_data_highpass(
+    X:pd.DataFrame,
+    minimum_total_counts=1,
+    minimum_prevalence=1,
+    minimum_components=1,
+    order_of_operations:list=["minimum_total_counts", "minimum_prevalence", "minimum_components"],
+    interval_type="closed",
+    ):
+
+    """
+    # Description
+    Highpass filter compositional table to include data higher than a minimum
+    
+    # Parameters
+        * X: pd.DataFrame or 2D np.array of compositional data (rows=compositions/samples, columns=components/features)
+        * minimum_total_counts:  The minimum total counts in a composition (sum per row) (axis=0)
+        * minimum_prevalence: The minimum number of compositions that must contain the components (axis=1)
+        * minimum_components: The minimum number of detected components (axis=0)
+        * order_of_operations: Order of filtering scheme.  Choose between: ["minimum_total_counts", "minimum_prevalence", "minimum_components"]
+
+    Adapted from the following source:
+    * https://github.com/jolespin/soothsayer
+ 
+    """
+    assert_acceptable_arguments(query=order_of_operations,target=["minimum_total_counts", "minimum_prevalence", "minimum_components"], operation="le")
+        
+    order_of_operations = list(map(lambda x: "_".join(x.split("_")[1:]), order_of_operations))
+
+    return _filter_data(
+        X=X,
+        total_counts=minimum_total_counts,
+        prevalence=minimum_prevalence,
+        components=minimum_components,
+        mode="highpass",
+        order_of_operations=order_of_operations,
+        interval_type=interval_type,
+        )
+
+# def filter_data_lowpass(
+#     X:pd.DataFrame,
+#     maximum_total_counts=np.inf,
+#     maximum_prevalence=np.inf,
+#     maximum_components=np.inf,
+#     order_of_operations:list=["maximum_total_counts", "maximum_prevalence", "maximum_components"],
+#     interval_type="closed",
+#     ):
+
+#     """
+#     # Description
+#     Lowpass filter compositional table to include data lower than a maximum
+    
+#     # Parameters
+#         * X: pd.DataFrame or 2D np.array of compositional data (rows=compositions/samples, columns=components/features)
+#         * maximum_total_counts:  The maximum total counts in a composition (sum per row) (axis=0)
+#         * maximum_prevalence: The maximum number of compositions that must contain the components (axis=1)
+#         * maximum_components: The maximum number of detected components (axis=0)
+#         * order_of_operations: Order of filtering scheme.  Choose between: ["maximum_total_counts", "maximum_prevalence", "maximum_components"]
+
+#     Adapted from the following source:
+#     * https://github.com/jolespin/soothsayer
+ 
+#     """
```

### Comparing `compositional-2022.8.31/setup.py` & `compositional-2023.7.20/setup.py`

 * *Files identical despite different names*

