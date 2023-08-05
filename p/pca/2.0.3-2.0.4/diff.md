# Comparing `tmp/pca-2.0.3.tar.gz` & `tmp/pca-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pca-2.0.3.tar", last modified: Wed May 31 20:47:32 2023, max compression
+gzip compressed data, was "pca-2.0.4.tar", last modified: Sat Aug  5 18:45:10 2023, max compression
```

## Comparing `pca-2.0.3.tar` & `pca-2.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 20:47:32.001826 pca-2.0.3/
--rw-rw-rw-   0        0        0     1094 2022-05-07 12:53:27.000000 pca-2.0.3/LICENSE
--rw-rw-rw-   0        0        0      100 2022-05-07 12:53:27.000000 pca-2.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0    10335 2023-05-31 20:47:31.995837 pca-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     9811 2023-05-28 19:59:46.000000 pca-2.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 20:47:31.921043 pca-2.0.3/pca/
--rw-rw-rw-   0        0        0     1272 2023-05-31 20:46:18.000000 pca-2.0.3/pca/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 20:47:31.990049 pca-2.0.3/pca/data/
--rw-rw-rw-   0        0        0        0 2022-05-07 12:53:27.000000 pca-2.0.3/pca/data/__init__.py
--rw-rw-rw-   0        0        0    33480 2023-04-28 11:42:55.000000 pca-2.0.3/pca/examples.py
--rw-rw-rw-   0        0        0    75101 2023-05-31 20:43:53.000000 pca-2.0.3/pca/pca.py
-drwxrwxrwx   0        0        0        0 2023-05-31 20:47:31.993843 pca-2.0.3/pca/tests/
--rw-rw-rw-   0        0        0        0 2022-05-07 12:53:27.000000 pca-2.0.3/pca/tests/__init__.py
--rw-rw-rw-   0        0        0    10683 2023-05-31 19:00:16.000000 pca-2.0.3/pca/tests/test_pca.py
-drwxrwxrwx   0        0        0        0 2023-05-31 20:47:31.987856 pca-2.0.3/pca.egg-info/
--rw-rw-rw-   0        0        0    10335 2023-05-31 20:47:31.000000 pca-2.0.3/pca.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-05-31 20:47:31.000000 pca-2.0.3/pca.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 20:47:31.000000 pca-2.0.3/pca.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2023-05-31 20:47:31.000000 pca-2.0.3/pca.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-31 20:47:31.000000 pca-2.0.3/pca.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 20:47:32.002044 pca-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1700 2023-05-31 20:38:42.000000 pca-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:45:10.221260 pca-2.0.4/
+-rw-rw-rw-   0        0        0     1094 2022-05-07 12:53:27.000000 pca-2.0.4/LICENSE
+-rw-rw-rw-   0        0        0      100 2022-05-07 12:53:27.000000 pca-2.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    10335 2023-08-05 18:45:10.221260 pca-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9811 2023-05-28 19:59:46.000000 pca-2.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 18:45:10.204301 pca-2.0.4/pca/
+-rw-rw-rw-   0        0        0     1246 2023-08-05 18:40:55.000000 pca-2.0.4/pca/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:45:10.219260 pca-2.0.4/pca/data/
+-rw-rw-rw-   0        0        0        0 2022-05-07 12:53:27.000000 pca-2.0.4/pca/data/__init__.py
+-rw-rw-rw-   0        0        0    33480 2023-04-28 11:42:55.000000 pca-2.0.4/pca/examples.py
+-rw-rw-rw-   0        0        0    78754 2023-08-05 18:42:02.000000 pca-2.0.4/pca/pca.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:45:10.220254 pca-2.0.4/pca/tests/
+-rw-rw-rw-   0        0        0        0 2022-05-07 12:53:27.000000 pca-2.0.4/pca/tests/__init__.py
+-rw-rw-rw-   0        0        0    10683 2023-05-31 19:00:16.000000 pca-2.0.4/pca/tests/test_pca.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:45:10.218286 pca-2.0.4/pca.egg-info/
+-rw-rw-rw-   0        0        0    10335 2023-08-05 18:45:10.000000 pca-2.0.4/pca.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-08-05 18:45:10.000000 pca-2.0.4/pca.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 18:45:10.000000 pca-2.0.4/pca.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2023-08-05 18:45:10.000000 pca-2.0.4/pca.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-05 18:45:10.000000 pca-2.0.4/pca.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 18:45:10.222259 pca-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1700 2023-08-05 14:53:39.000000 pca-2.0.4/setup.py
```

### Comparing `pca-2.0.3/LICENSE` & `pca-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pca-2.0.3/PKG-INFO` & `pca-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pca
-Version: 2.0.3
+Version: 2.0.4
 Summary: pca: A Python Package for Principal Component Analysis.
 Home-page: https://erdogant.github.io/pca
-Download-URL: https://github.com/erdogant/pca/archive/2.0.3.tar.gz
+Download-URL: https://github.com/erdogant/pca/archive/2.0.4.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pca Version: 2.0.3 Summary: pca: A Python Package
+Metadata-Version: 2.1 Name: pca Version: 2.0.4 Summary: pca: A Python Package
 for Principal Component Analysis. Home-page: https://erdogant.github.io/pca
-Download-URL: https://github.com/erdogant/pca/archive/2.0.3.tar.gz Author:
+Download-URL: https://github.com/erdogant/pca/archive/2.0.4.tar.gz Author:
 Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3
 Description-Content-Type: text/markdown License-File: LICENSE
    [https://github.com/erdogant/pca/blob/master/docs/figs/iris_density.png]
 [![Python](https://img.shields.io/pypi/pyversions/pca)](https://img.shields.io/
 pypi/pyversions/pca) [![Pypi](https://img.shields.io/pypi/v/pca)](https://
```

### Comparing `pca-2.0.3/README.md` & `pca-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pca-2.0.3/pca/__init__.py` & `pca-2.0.4/pca/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,23 +5,21 @@
     hotellingsT2,
     spe_dmodx,
     )
 
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '2.0.3'
+__version__ = '2.0.4'
 
 # module level doc-string
 __doc__ = """
 pca
 =====================================================================
 
-Description
------------
 pca: A Python Package for Principal Component Analysis.
 
 Examples
 --------
 >>> from pca import pca
 >>>
 >>> Initialize
```

### Comparing `pca-2.0.3/pca/examples.py` & `pca-2.0.4/pca/examples.py`

 * *Files identical despite different names*

### Comparing `pca-2.0.3/pca/pca.py` & `pca-2.0.4/pca/pca.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,23 @@
 import scipy.sparse as sp
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 from adjustText import adjust_text
 import statsmodels.stats.multitest as multitest
 from typing import Union
+# import logging
+
+# logger = logging.getLogger('')
+# [logger.removeHandler(handler) for handler in logger.handlers[:]]
+# console = logging.StreamHandler()
+# formatter = logging.Formatter('[pca] >%(levelname)s> %(message)s')
+# console.setFormatter(formatter)
+# logger.addHandler(console)
+# logger = logging.getLogger(__name__)
 
 
 # %% Association learning across all variables
 class pca:
     """pca module.
 
     Parameters
@@ -80,19 +89,25 @@
                  alpha=0.05,
                  multipletests='fdr_bh',
                  n_std=3,
                  onehot=False,
                  normalize=False,
                  detect_outliers=['ht2', 'spe'],
                  random_state=None,
-                 verbose=3):
+                 verbose='info'):
         """Initialize pca with user-defined parameters."""
         if isinstance(detect_outliers, str): detect_outliers = [detect_outliers]
         if detect_outliers is not None: detect_outliers=list(map(str.lower, detect_outliers))
 
+        verbose = convert_verbose_to_old(verbose)
+        # Convert to new verbose
+        # verbose = convert_verbose_to_new(verbose)
+        # Set the logger
+        # set_logger(verbose=verbose)
+
         if onehot:
             if verbose>=3: print('[pca] >Method is set to: [sparse_pca] because onehot=True.')
             method = 'sparse_pca'
 
         # Store in object
         self.n_components = n_components
         self.method = method.lower()
@@ -1634,12 +1649,107 @@
         getsizes = getsizes.ravel()
     # Max digits is 4
     getsizes = np.array(list(map(lambda x: round(x, 4), getsizes)))
 
     return getsizes
 
 
+# %%
+def convert_verbose_to_old(verbose):
+    """Convert new verbosity to the old ones."""
+    # In case the new verbosity is used, convert to the old one.
+    if verbose is None: verbose=0
+    if isinstance(verbose, str) or verbose>=10:
+        status_map = {
+            60: 0, 'silent': 0, 'off': 0, 'no': 0, None: 0,
+            40: 1, 'error': 1, 'critical': 1,
+            30: 2, 'warning': 2,
+            20: 3, 'info': 3,
+            10: 4, 'debug': 4}
+        return status_map.get(verbose, 0)
+    else:
+        return verbose
+
+
+# def convert_verbose_to_new(verbose):
+#     """Convert old verbosity to the new."""
+#     # In case the new verbosity is used, convert to the old one.
+#     if verbose is None: verbose=0
+#     if not isinstance(verbose, str) and verbose<10:
+#         status_map = {
+#             'None': 'silent',
+#             0: 'silent',
+#             6: 'silent',
+#             1: 'critical',
+#             2: 'warning',
+#             3: 'info',
+#             4: 'debug',
+#             5: 'debug'}
+#         if verbose>=2: print('[scatterd]> WARNING use the standardized verbose status. The status [1-6] will be deprecated in future versions.')
+#         return status_map.get(verbose, 0)
+#     else:
+#         return verbose
+
+
+# def get_logger():
+#     return logger.getEffectiveLevel()
+
+
+# def set_logger(verbose: [str, int] = 'info'):
+#     """Set the logger for verbosity messages.
+
+#     Parameters
+#     ----------
+#     verbose : [str, int], default is 'info' or 20
+#         Set the verbose messages using string or integer values.
+#         * [0, 60, None, 'silent', 'off', 'no']: No message.
+#         * [10, 'debug']: Messages from debug level and higher.
+#         * [20, 'info']: Messages from info level and higher.
+#         * [30, 'warning']: Messages from warning level and higher.
+#         * [50, 'critical']: Messages from critical level and higher.
+
+#     Returns
+#     -------
+#     None.
+
+#     > # Set the logger to warning
+#     > set_logger(verbose='warning')
+#     > # Test with different messages
+#     > logger.debug("Hello debug")
+#     > logger.info("Hello info")
+#     > logger.warning("Hello warning")
+#     > logger.critical("Hello critical")
+
+#     """
+#     # Set 0 and None as no messages.
+#     if (verbose==0) or (verbose is None):
+#         verbose=60
+#     # Convert to verbose
+#     verbose = convert_verbose_to_new(verbose)
+#     # Convert str to levels
+#     if isinstance(verbose, str):
+#         levels = {'silent': 60,
+#                   'off': 60,
+#                   'no': 60,
+#                   'debug': 10,
+#                   'info': 20,
+#                   'warning': 30,
+#                   'error': 50,
+#                   'critical': 50}
+#         verbose = levels[verbose]
+
+#     # Show examples
+#     logger.setLevel(verbose)
+#     logger.debug('Set verbose to %s' %(verbose))
+
+
+# def disable_tqdm():
+#     """Set the logger for verbosity messages."""
+#     return (True if (logger.getEffectiveLevel()>=30) else False)
+
+
+# %%
 def _show_deprecated_warning(label, y, verbose):
     if label is not None:
         if verbose>=2: print('[pca]> [WARNING]: De parameter <label> is deprecated and will not be supported in future version.')
     if y is not None:
         if verbose>=2: print('[pca]> [WARNING]: De parameter <y> is deprecated and will not be supported in future version. Use <labels> instead.')
```

### Comparing `pca-2.0.3/pca/tests/test_pca.py` & `pca-2.0.4/pca/tests/test_pca.py`

 * *Files identical despite different names*

### Comparing `pca-2.0.3/pca.egg-info/PKG-INFO` & `pca-2.0.4/pca.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pca
-Version: 2.0.3
+Version: 2.0.4
 Summary: pca: A Python Package for Principal Component Analysis.
 Home-page: https://erdogant.github.io/pca
-Download-URL: https://github.com/erdogant/pca/archive/2.0.3.tar.gz
+Download-URL: https://github.com/erdogant/pca/archive/2.0.4.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pca Version: 2.0.3 Summary: pca: A Python Package
+Metadata-Version: 2.1 Name: pca Version: 2.0.4 Summary: pca: A Python Package
 for Principal Component Analysis. Home-page: https://erdogant.github.io/pca
-Download-URL: https://github.com/erdogant/pca/archive/2.0.3.tar.gz Author:
+Download-URL: https://github.com/erdogant/pca/archive/2.0.4.tar.gz Author:
 Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3
 Description-Content-Type: text/markdown License-File: LICENSE
    [https://github.com/erdogant/pca/blob/master/docs/figs/iris_density.png]
 [![Python](https://img.shields.io/pypi/pyversions/pca)](https://img.shields.io/
 pypi/pyversions/pca) [![Pypi](https://img.shields.io/pypi/v/pca)](https://
```

### Comparing `pca-2.0.3/setup.py` & `pca-2.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 setuptools.setup(
      install_requires=['datazets',
                        'statsmodels',
                        'matplotlib',
                        'numpy',
                        'scikit-learn',
                        'scipy',
-                       'colourmap>=1.1.14',
+                       'colourmap>=1.1.15',
                        'pandas',
                        'scatterd>=1.3.1',
                        'adjusttext',
                        ],
      python_requires='>=3',
      name='pca',
      version=new_version,
```

