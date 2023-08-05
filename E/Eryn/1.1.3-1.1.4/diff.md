# Comparing `tmp/Eryn-1.1.3.tar.gz` & `tmp/Eryn-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Eryn-1.1.3.tar", last modified: Wed May 24 18:45:31 2023, max compression
+gzip compressed data, was "Eryn-1.1.4.tar", last modified: Sat Aug  5 00:54:31 2023, max compression
```

## Comparing `Eryn-1.1.3.tar` & `Eryn-1.1.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2023-05-24 18:45:31.339148 Eryn-1.1.3/
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2023-05-24 18:45:31.318135 Eryn-1.1.3/Eryn.egg-info/
--rw-r--r--   0 mlkatz1    (502) staff       (20)     4616 2023-05-24 18:45:31.000000 Eryn-1.1.3/Eryn.egg-info/PKG-INFO
--rw-r--r--   0 mlkatz1    (502) staff       (20)      857 2023-05-24 18:45:31.000000 Eryn-1.1.3/Eryn.egg-info/SOURCES.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)        1 2023-05-24 18:45:31.000000 Eryn-1.1.3/Eryn.egg-info/dependency_links.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)        5 2023-05-24 18:45:31.000000 Eryn-1.1.3/Eryn.egg-info/top_level.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)     4616 2023-05-24 18:45:31.338844 Eryn-1.1.3/PKG-INFO
--rw-r--r--   0 mlkatz1    (502) staff       (20)     4301 2023-05-24 18:44:18.000000 Eryn-1.1.3/README.md
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2023-05-24 18:45:31.322759 Eryn-1.1.3/eryn/
--rw-r--r--   0 mlkatz1    (502) staff       (20)       38 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/__init__.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)       21 2023-05-24 18:45:31.000000 Eryn-1.1.3/eryn/_version.py
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2023-05-24 18:45:31.325210 Eryn-1.1.3/eryn/backends/
--rw-r--r--   0 mlkatz1    (502) staff       (20)      380 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/backends/__init__.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    39175 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/backends/backend.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    26715 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/backends/hdfbackend.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    68537 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/ensemble.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)      284 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/model.py
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2023-05-24 18:45:31.334623 Eryn-1.1.3/eryn/moves/
--rw-r--r--   0 mlkatz1    (502) staff       (20)     1081 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/__init__.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     4547 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/combine.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     7670 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/delayedrejection.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     3935 2023-05-16 22:44:45.000000 Eryn-1.1.3/eryn/moves/distgen.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     9133 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/distgenrj.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     6728 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/gaussian.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     8767 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/group.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     3493 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/groupstretch.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     6425 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/mh.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    28232 2023-05-24 18:44:18.000000 Eryn-1.1.3/eryn/moves/move.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     5347 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/mtdistgen.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     8102 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/mtdistgenrj.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    29678 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/multipletry.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    12932 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/red_blue.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    15910 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/rj.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     8072 2023-05-24 18:44:18.000000 Eryn-1.1.3/eryn/moves/stretch.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    23812 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/moves/tempering.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     1330 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/pbar.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    11254 2023-05-16 22:44:45.000000 Eryn-1.1.3/eryn/prior.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    23945 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/state.py
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2023-05-24 18:45:31.338312 Eryn-1.1.3/eryn/utils/
--rw-r--r--   0 mlkatz1    (502) staff       (20)      250 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/utils/__init__.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     3983 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/utils/periodic.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     5095 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/utils/stopping.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     8895 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/utils/transform.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     2137 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/utils/updates.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     6692 2023-05-16 15:38:51.000000 Eryn-1.1.3/eryn/utils/utility.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)       72 2023-05-16 15:38:51.000000 Eryn-1.1.3/pyproject.toml
--rw-r--r--   0 mlkatz1    (502) staff       (20)       38 2023-05-24 18:45:31.339248 Eryn-1.1.3/setup.cfg
--rw-r--r--   0 mlkatz1    (502) staff       (20)     1037 2023-05-16 15:38:51.000000 Eryn-1.1.3/setup.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2023-08-05 00:54:31.664803 Eryn-1.1.4/
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2023-08-05 00:54:31.613206 Eryn-1.1.4/Eryn.egg-info/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     4838 2023-08-05 00:54:31.000000 Eryn-1.1.4/Eryn.egg-info/PKG-INFO
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      857 2023-08-05 00:54:31.000000 Eryn-1.1.4/Eryn.egg-info/SOURCES.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        1 2023-08-05 00:54:31.000000 Eryn-1.1.4/Eryn.egg-info/dependency_links.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        5 2023-08-05 00:54:31.000000 Eryn-1.1.4/Eryn.egg-info/top_level.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     4838 2023-08-05 00:54:31.663249 Eryn-1.1.4/PKG-INFO
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     4523 2023-08-05 00:53:53.000000 Eryn-1.1.4/README.md
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2023-08-05 00:54:31.620864 Eryn-1.1.4/eryn/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       38 2023-05-16 15:38:51.000000 Eryn-1.1.4/eryn/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       21 2023-08-05 00:54:31.000000 Eryn-1.1.4/eryn/_version.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2023-08-05 00:54:31.624735 Eryn-1.1.4/eryn/backends/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      380 2023-05-16 15:38:51.000000 Eryn-1.1.4/eryn/backends/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    43784 2023-08-05 00:53:53.000000 Eryn-1.1.4/eryn/backends/backend.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    26715 2023-05-16 15:38:51.000000 Eryn-1.1.4/eryn/backends/hdfbackend.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    67776 2023-06-08 01:07:59.000000 Eryn-1.1.4/eryn/ensemble.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      284 2023-05-16 15:38:51.000000 Eryn-1.1.4/eryn/model.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2023-08-05 00:54:31.649418 Eryn-1.1.4/eryn/moves/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     1081 2023-05-16 15:38:51.000000 Eryn-1.1.4/eryn/moves/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     4547 2023-05-16 15:38:51.000000 Eryn-1.1.4/eryn/moves/combine.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     7670 2023-05-16 15:38:51.000000 Eryn-1.1.4/eryn/moves/delayedrejection.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     3935 2023-05-16 22:44:45.000000 Eryn-1.1.4/eryn/moves/distgen.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     9133 2023-05-16 15:38:51.000000 Eryn-1.1.4/eryn/moves/distgenrj.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     6723 2023-08-05 00:53:53.000000 Eryn-1.1.4/eryn/moves/gaussian.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     8767 2023-05-16 15:38:51.000000 Eryn-1.1.4/eryn/moves/group.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     3493 2023-05-16 15:38:51.000000 Eryn-1.1.4/eryn/moves/groupstretch.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     6425 2023-05-16 15:38:51.000000 Eryn-1.1.4/eryn/moves/mh.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    28232 2023-05-24 18:44:18.000000 Eryn-1.1.4/eryn/moves/move.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     5347 2023-05-16 15:38:51.000000 Eryn-1.1.4/eryn/moves/mtdistgen.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     8102 2023-05-16 15:38:51.000000 Eryn-1.1.4/eryn/moves/mtdistgenrj.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    29678 2023-05-16 15:38:51.000000 Eryn-1.1.4/eryn/moves/multipletry.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    12943 2023-08-05 00:53:53.000000 Eryn-1.1.4/eryn/moves/red_blue.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    15915 2023-06-07 23:55:44.000000 Eryn-1.1.4/eryn/moves/rj.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     8025 2023-06-07 23:55:44.000000 Eryn-1.1.4/eryn/moves/stretch.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    23812 2023-05-16 15:38:51.000000 Eryn-1.1.4/eryn/moves/tempering.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     1330 2023-05-16 15:38:51.000000 Eryn-1.1.4/eryn/pbar.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    11254 2023-05-16 22:44:45.000000 Eryn-1.1.4/eryn/prior.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    23945 2023-05-16 15:38:51.000000 Eryn-1.1.4/eryn/state.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2023-08-05 00:54:31.661007 Eryn-1.1.4/eryn/utils/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      250 2023-05-16 15:38:51.000000 Eryn-1.1.4/eryn/utils/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     3983 2023-05-16 15:38:51.000000 Eryn-1.1.4/eryn/utils/periodic.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     5095 2023-05-16 15:38:51.000000 Eryn-1.1.4/eryn/utils/stopping.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     8895 2023-05-16 15:38:51.000000 Eryn-1.1.4/eryn/utils/transform.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     2137 2023-05-16 15:38:51.000000 Eryn-1.1.4/eryn/utils/updates.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    11173 2023-08-05 00:53:53.000000 Eryn-1.1.4/eryn/utils/utility.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       72 2023-05-16 15:38:51.000000 Eryn-1.1.4/pyproject.toml
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       38 2023-08-05 00:54:31.665459 Eryn-1.1.4/setup.cfg
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     1037 2023-05-16 15:38:51.000000 Eryn-1.1.4/setup.py
```

### Comparing `Eryn-1.1.3/Eryn.egg-info/PKG-INFO` & `Eryn-1.1.4/Eryn.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Eryn
-Version: 1.1.3
+Version: 1.1.4
 Summary: An all purpose MCMC sampler
 Home-page: https://github.com/mikekatz04/Eryn
 Author: Michael Katz, Nikos Karnesis
 Author-email: mikekatz04@gmail.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -55,15 +55,15 @@
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
 
 ## Versioning
 
 We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/BlackHolePerturbationToolkit/FastEMRIWaveforms/tags).
 
-Current Version: 1.1.3
+Current Version: 1.1.4
 
 ## Citation
 
 When using this package, please cite at minimum the following sources:
 
 ```
 @article{Karnesis:2023ras,
@@ -124,8 +124,9 @@
 
 ## License
 
 This project is licensed under the GNU License - see the [LICENSE.md](LICENSE.md) file for details.
 
 ## Acknowledgments
 
-* TODO: add acknowledgements
+* We wish to thank S. Babak, M. Le Jeune, S. Marsat, T. Littenberg, and N. Cornish for their useful comments and very fruitful discussions. 
+* N Stergioulas and N Karnesis acknowledge  support from the Gr-PRODEX 2019 funding program (PEA 4000132310).
```

### Comparing `Eryn-1.1.3/Eryn.egg-info/SOURCES.txt` & `Eryn-1.1.4/Eryn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.3/PKG-INFO` & `Eryn-1.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Eryn
-Version: 1.1.3
+Version: 1.1.4
 Summary: An all purpose MCMC sampler
 Home-page: https://github.com/mikekatz04/Eryn
 Author: Michael Katz, Nikos Karnesis
 Author-email: mikekatz04@gmail.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -55,15 +55,15 @@
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
 
 ## Versioning
 
 We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/BlackHolePerturbationToolkit/FastEMRIWaveforms/tags).
 
-Current Version: 1.1.3
+Current Version: 1.1.4
 
 ## Citation
 
 When using this package, please cite at minimum the following sources:
 
 ```
 @article{Karnesis:2023ras,
@@ -124,8 +124,9 @@
 
 ## License
 
 This project is licensed under the GNU License - see the [LICENSE.md](LICENSE.md) file for details.
 
 ## Acknowledgments
 
-* TODO: add acknowledgements
+* We wish to thank S. Babak, M. Le Jeune, S. Marsat, T. Littenberg, and N. Cornish for their useful comments and very fruitful discussions. 
+* N Stergioulas and N Karnesis acknowledge  support from the Gr-PRODEX 2019 funding program (PEA 4000132310).
```

### Comparing `Eryn-1.1.3/README.md` & `Eryn-1.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
 
 ## Versioning
 
 We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/BlackHolePerturbationToolkit/FastEMRIWaveforms/tags).
 
-Current Version: 1.1.3
+Current Version: 1.1.4
 
 ## Citation
 
 When using this package, please cite at minimum the following sources:
 
 ```
 @article{Karnesis:2023ras,
@@ -113,8 +113,9 @@
 
 ## License
 
 This project is licensed under the GNU License - see the [LICENSE.md](LICENSE.md) file for details.
 
 ## Acknowledgments
 
-* TODO: add acknowledgements
+* We wish to thank S. Babak, M. Le Jeune, S. Marsat, T. Littenberg, and N. Cornish for their useful comments and very fruitful discussions. 
+* N Stergioulas and N Karnesis acknowledge  support from the Gr-PRODEX 2019 funding program (PEA 4000132310).
```

### Comparing `Eryn-1.1.3/eryn/backends/backend.py` & `Eryn-1.1.4/eryn/backends/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 import numpy as np
 
-from ..utils.utility import get_integrated_act, thermodynamic_integration_log_evidence
+from ..utils.utility import get_integrated_act, thermodynamic_integration_log_evidence, stepping_stone_log_evidence, psrf
 from ..state import State
 
 __all__ = ["Backend"]
 
 
 class Backend(object):
     """A simple default backend that stores the chain in memory
@@ -597,29 +597,32 @@
         out = get_integrated_act(x, **kwargs)
 
         # apply thinning factor if desired
         thin_factor = thin if multiply_thin else 1
 
         return {name: values * thin_factor for name, values in out.items()}
 
-    def get_evidence_estimate(self, discard=0, thin=1, return_error=True):
+    def get_evidence_estimate(self, discard=0, thin=1, return_error=True, method="therodynamic", **ss_kwargs):
         """Get an estimate of the evidence
 
         This function gets the sample information and uses 
-        :func:`thermodynamic_integration_log_evidence` to compute the evidence estimate.
+        :func:`thermodynamic_integration_log_evidence` or 
+        :func:`stepping_stone_log_evidence` to compute the evidence estimate.
 
         Args:
             discard (int, optional): Discard the first ``discard`` steps in
                 the chain as burn-in. (default: ``0``)
             thin (int, optional): Use only every ``thin`` steps from the
                 chain. The returned estimate is multiplied by ``thin`` so the
                 estimated time is in units of steps, not thinned steps.
                 (default: ``1``)
             return_error (bool, optional): If True, return the error associated
                 with the log evidence estimate. (default: ``True``)
+            method (string, optional): Method to compute the evidence. Available
+                methods are the 'thermodynamic' and 'stepping-stone' (default: ``thermodynamic``)
 
         Returns:
             double or tuple: Evidence estimate
                 If requesting the error on the estimate, will receive a tuple:
                 ``(logZ, dlogZ)``. Otherwise, just a double value of logZ.
 
         """
@@ -632,23 +635,100 @@
             raise ValueError(
                 """Cannot compute evidence estimation if betas are allowed to vary. Use stop_adaptation 
                 kwarg in temperature settings."""
             )
 
         # setup information
         betas = betas_all[0]
-        logls = np.mean(logls_all, axis=(0, -1))
 
         # get log evidence and error
-        logZ, dlogZ = thermodynamic_integration_log_evidence(betas, logls)
-
+        if method.lower() in ["therodynamic", "thermodynamic integration", "thermo", "ti"]:
+            logls = np.mean(logls_all, axis=(0, -1))
+            logZ, dlogZ = thermodynamic_integration_log_evidence(betas, logls)
+        elif method.lower() in ["stepping stone", "ss", "step", "stone", "stepping-stone"]:
+            logZ, dlogZ = stepping_stone_log_evidence(betas, logls_all, **ss_kwargs)
+        else:
+            raise ValueError(
+                """Please choose only between 'thermodynamic' and 'stepping-stone' methods.""")
+            
         if return_error:
             return (logZ, dlogZ)
         else:
             return logZ
+        
+    def get_gelman_rubin_convergence_diagnostic(self, discard=0, thin=1, doprint=True, **psrf_kwargs):
+        """
+        The Gelman - Rubin convergence diagnostic. 
+        A general approach to monitoring convergence of MCMC output of multiple walkers. 
+        The function makes a comparison of within-chain and between-chain variances. 
+        A large deviation between these two variances indicates non-convergence, and 
+        the output [Rhat] deviates from unity.
+        
+        Based on 
+        a. Brooks, SP. and Gelman, A. (1998) General methods for monitoring convergence 
+        of iterative simulations. Journal of Computational and Graphical Statistics, 7, 434-455
+        b. Gelman, A and Rubin, DB (1992) Inference from iterative simulation using multiple sequences, 
+        Statistical Science, 7, 457-511.
+        
+        Args:
+            C (np.ndarray[nwalkers, nsamples, ndim]): The parameter traces. The MCMC chains. 
+            doprint (bool, optional): Flag to print the results on screen.
+        discard (int, optional): Discard the first ``discard`` steps in
+                the chain as burn-in. (default: ``0``)
+        thin (int, optional): Use only every ``thin`` steps from the
+                chain. The returned estimate is multiplied by ``thin`` so the
+                estimated time is in units of steps, not thinned steps.
+                (default: ``1``)
+        doprint (bool, optional): Flag to print a table with the results, per temperature.
+
+        Returns
+            dict:   ``Rhat_all_branches``: 
+                Returns an estimate of the Gelman-Rubin convergence diagnostic ``Rhat``,
+                per temperature, stored in a dictionary, per branch name.
+        
+        """
+        Rhat_all_branches = dict()
+        # Loop over the different models
+        for branch in self.branch_names:
+            
+            Rhat = dict() # Initialize
+            # Loop over the temperatures
+            for temp in range(self.ntemps):
+                
+                # Get all the chains per branch
+                chains = self.get_chain(discard=discard, thin=thin)[branch][:, temp]
+                
+                # Handle the cases of multiple leaves on a given branch
+                if chains.shape[2] == 1:
+                    # If no multiple leaves, we squeeze and transpose to the 
+                    # right shape to pass to the psrf function, which is  (nwalkers, nsamples, ndim)
+                    chains_in = chains.squeeze().transpose((1, 0, 2))
+                else:
+                    # Project onto the model dim all chains [in case of RJ and multiple leaves per branch]
+                    inds = self.get_inds(discard=discard, thin=thin)[branch][:, temp] # [t, w, nleavesmax, dim]
+                    min_leaves = inds.sum(axis=(0,2)).min()
+                    tmp = [inds[:, w].flatten() for w in range(self.nwalkers)]
+                    keep = [np.where( tmp[w] )[0][:min_leaves] for w in range(len(tmp)) ]
+                    chains_in = np.asarray([chains[:,w].reshape(-1, self.ndims[branch])[keep[w]] for w in range(self.nwalkers)])
+                                
+                Rhat[temp] = psrf(chains_in, self.ndims[branch], **psrf_kwargs)
+            Rhat_all_branches[branch] = Rhat # Store the Rhat per branch
+
+        if doprint: # Print table of results
+            print("  Gelman-Rubin diagnostic \n  <R̂>: Mean value for all parameters\n")
+            print("  --------------")
+            for branch in self.branch_names:
+                print(" Model: {}".format(branch))
+                print("   T \t <R̂>")
+                print("  --------------")
+                for temp in range(self.ntemps):
+                    print("   {:01d}\t{:3.2f}".format(temp, np.mean(Rhat_all_branches[branch][temp])))
+                print("\n")
+
+        return Rhat_all_branches
 
     @property
     def shape(self):
         """The dimensions of the ensemble
 
         Returns:
             dict: Shape of samples
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Eryn-1.1.3/eryn/backends/hdfbackend.py` & `Eryn-1.1.4/eryn/backends/hdfbackend.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.3/eryn/ensemble.py` & `Eryn-1.1.4/eryn/ensemble.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,92 +30,92 @@
 
 class EnsembleSampler(object):
     """An ensemble MCMC sampler
 
     The class controls the entire sampling run. It can handle
     everything from a basic non-tempered MCMC to a parallel-tempered,
     global fit containing multiple branches (models) and a variable
-    number of leaves (sources) per branch. 
+    number of leaves (sources) per branch.
     See `here <https://mikekatz04.github.io/Eryn/html/tutorial/Eryn_tutorial.html#The-Tree-Metaphor>`_
     for a basic explainer.
 
     Parameters related to parallelization can be controlled via the ``pool`` argument.
 
     Args:
         nwalkers (int): The number of walkers in the ensemble per temperature.
         ndims (int, list of ints, or dict): The number of dimensions for each branch. If
                 ``dict``, keys should be the branch names and values the associated dimensionality.
         log_like_fn (callable): A function that returns the natural logarithm of the
             likelihood for that position. The inputs to ``log_like_fn`` depend on whether
-            the function is vectorized (kwarg ``vectorize`` below), if you are using reversible jump, 
-            and how many branches you have. 
-            
-                In the simplest case where ``vectorize == False``, no reversible jump, and only one 
+            the function is vectorized (kwarg ``vectorize`` below), if you are using reversible jump,
+            and how many branches you have.
+
+                In the simplest case where ``vectorize == False``, no reversible jump, and only one
                 type of model, the inputs are just the array of parameters for one walker, so shape is ``(ndim,)``.
 
-                If ``vectorize == True``, no reversible jimp, and only one type of model, the inputs will 
+                If ``vectorize == True``, no reversible jimp, and only one type of model, the inputs will
                 be a 2D array of parameters of all the walkers going in. Shape: ``(num positions, ndim)``.
 
                 If using reversible jump, the leaves that go together in the same Likelihood will be grouped
                 together into a single function call. If ``vectorize == False``, then each group is sent as
-                an individual computation. With ``N`` different branches (``N > 1``), inputs would be a list 
+                an individual computation. With ``N`` different branches (``N > 1``), inputs would be a list
                 of 2D arrays of the coordinates for all leaves within each branch: ``([x0, x1,...,xN])``
                 where ``xi`` is 2D with shape ``(number of leaves in this branch, ndim)``. If ``N == 1``, then
                 a list is not provided, just x0, the 2D array of coordinates for the one branch considered.
 
                 If using reversible jump and ``vectorize == True``, then the arrays of parameters will be output
                 with information as regards the grouping of branch and leaf set. Inputs will be
                 ``([X0, X1,..XN], [group0, group1,...,groupN])`` where ``Xi`` is a 2D array of all
                 leaves in the sampler for branch ``i``. ``groupi`` is an index indicating which unique group
                 that sources belongs. For example, if we have 3 walkers with (1, 2, 1) leaves for model ``i``,
-                respectively, we wil have an ``Xi = array([params0, params1, params2, params3])`` and 
-                ``groupsi = array([0, 1, 1, 2])``. 
-                If ``N == 1``, then the lists are removed and the inputs become ``(X0, group0)``. 
+                respectively, we wil have an ``Xi = array([params0, params1, params2, params3])`` and
+                ``groupsi = array([0, 1, 1, 2])``.
+                If ``N == 1``, then the lists are removed and the inputs become ``(X0, group0)``.
 
-                Extra ``args`` and ``kwargs`` for the Likelihood function can be added with the kwargs 
+                Extra ``args`` and ``kwargs`` for the Likelihood function can be added with the kwargs
                 ``args`` and ``kwargs`` below.
 
-                Please see the 
-                `tutorial <https://mikekatz04.github.io/Eryn/html/tutorial/Eryn_tutorial.html#>`_ 
-                for more information. 
+                Please see the
+                `tutorial <https://mikekatz04.github.io/Eryn/html/tutorial/Eryn_tutorial.html#>`_
+                for more information.
 
         priors (dict): The prior dictionary can take four forms.
             1) A dictionary with keys as int or tuple containing the int or tuple of int
             that describe the parameter number over which to assess the prior, and values that
             are prior probability distributions that must have a ``logpdf`` class method.
             2) A :class:`eryn.prior.ProbDistContainer` object.
             3) A dictionary with keys that are ``branch_names`` and values that are dictionaries for
             each branch as described for (1).
             4) A dictionary with keys that are ``branch_names`` and values are
             :class:`eryn.prior.ProbDistContainer` objects.
             If the priors dictionary has the specific key ``"all_models_together"`` in it, then a special
             prior must be input by the user that can produce the prior ``logpdf`` information that can depend on all of the models
             together rather than handling them separately as is the default. In this case, the user must input
             as the item attached to this special key a class object with a ``logpdf`` method that takes as input
-            two arguments: ``(coords, inds)``, which are the coordinate and index dictionaries across all models with 
-            shapes of ``(ntemps, nwalkers, nleaves_max, ndim)`` and ``(ntemps, nwalkers, nleaves_max)`` for each 
-            individual model, respectively. This function must then return the numpy array of logpdf values for the 
-            prior value with shape ``(ntemps, nwalkers)``. 
+            two arguments: ``(coords, inds)``, which are the coordinate and index dictionaries across all models with
+            shapes of ``(ntemps, nwalkers, nleaves_max, ndim)`` and ``(ntemps, nwalkers, nleaves_max)`` for each
+            individual model, respectively. This function must then return the numpy array of logpdf values for the
+            prior value with shape ``(ntemps, nwalkers)``.
         provide_groups (bool, optional): If ``True``, provide groups as described in ``log_like_fn`` above.
             A group parameter is added for each branch. (default: ``False``)
-        provide_supplimental (bool, optional): If ``True``, it will provide keyword arguments to 
+        provide_supplimental (bool, optional): If ``True``, it will provide keyword arguments to
             the Likelihood function: ``supps`` and ``branch_supps``. Please see the `Tutorial <https://mikekatz04.github.io/Eryn/html/tutorial/Eryn_tutorial.html#>`_
             and :class:`eryn.state.BranchSupplimental` for more information.
         tempering_kwargs (dict, optional): Keyword arguments for initialization of the
             tempering class: :class:`eryn.moves.tempering.TemperatureControl`.  (default: ``{}``)
         branch_names (list, optional): List of branch names. If ``None``, models will be assigned
             names as ``f"model_{index}"`` based on ``nbranches``. (default: ``None``)
-        nbranches (int, optional): Number of branches (models) tested. 
+        nbranches (int, optional): Number of branches (models) tested.
             Only used if ``branch_names is None``.
             (default: ``1``)
-        nleaves_max (int, list of ints, or dict, optional): Maximum allowable leaf count for each branch. 
-            It should have the same length as the number of branches. 
+        nleaves_max (int, list of ints, or dict, optional): Maximum allowable leaf count for each branch.
+            It should have the same length as the number of branches.
             If ``dict``, keys should be the branch names and values the associated maximal leaf value.
             (default: ``1``)
-        nleaves_min (int, list of ints, or dict, optional): Minimum allowable leaf count for each branch. 
+        nleaves_min (int, list of ints, or dict, optional): Minimum allowable leaf count for each branch.
             It should have the same length as the number of branches. Only used with Reversible Jump.
             If ``dict``, keys should be the branch names and values the associated maximal leaf value.
             If ``None`` and using Reversible Jump, will fill all branches with zero.
             (default: ``0``)
         pool (object, optional): An object with a ``map`` method that follows the same
             calling sequence as the built-in ``map`` function. This is
             generally used to compute the log-probabilities for the ensemble
@@ -148,65 +148,53 @@
             (like :class:`backends.HDFBackend`) that is used to store and
             serialize the state of the chain. By default, the chain is stored
             as a set of numpy arrays in memory, but new backends can be
             written to support other mediums.
         vectorize (bool, optional): If ``True``, ``log_like_fn`` is expected
             to accept an array of position vectors instead of just one. Note
             that ``pool`` will be ignored if this is ``True``. See ``log_like_fn`` information
-            above to understand the arguments of ``log_like_fn`` based on whether 
-            ``vectorize`` is ``True``. 
+            above to understand the arguments of ``log_like_fn`` based on whether
+            ``vectorize`` is ``True``.
             (default: ``False``)
-        plot_iterations (int, optional): If ``plot_iterations == -1``, then the
-            diagnostic plots will not be constructed. Otherwise, the diagnostic
-            plots will be constructed every ``plot_iterations`` sampler iterations.
-            (default: -1)
-        plot_generator (optional): # TODO: add class object that controls
-            the diagnostic plotting updates. If not provided and ``plot_iterations > 0``,
-            the ensemble will initialize a default plotting setup.
-            (default: None)
-        plot_name (str, optional): Name of file to save diagnostic plots to. This only
-            applies if ``plot_generator == None`` and ``plot_iterations > 0``.
-            (default: ``None``)
         periodic (dict, optional): Keys are ``branch_names``. Values are dictionaries
             that have (key: value) pairs as (index to parameter: period). Periodic
             parameters are treated as having periodic boundary conditions in proposals.
         update_fn (callable, optional): :class:`eryn.utils.updates.AdjustStretchProposalScale`
             object that allows the user to update the sampler in any preferred way
             every ``update_iterations`` sampler iterations. The callable must have signature:
-            ``(sampler iteration, last sample state object, EnsembleSampler object)``. 
+            ``(sampler iteration, last sample state object, EnsembleSampler object)``.
         update_iterations (int, optional): Number of iterations between sampler
-            updates using ``update_fn``. Updates are only performed at the thinning rate. 
+            updates using ``update_fn``. Updates are only performed at the thinning rate.
             If ``thin_by>1`` when :func:`EnsembleSampler.run_mcmc` is used, the sampler
-            is updated every ``thin_by * update_iterations`` iterations. 
+            is updated every ``thin_by * update_iterations`` iterations.
         stopping_fn (callable, optional): :class:`eryn.utils.stopping.Stopping` object that
             allows the user to end the sampler if specified criteria are met.
             The callable must have signature:
-            ``(sampler iteration, last sample state object, EnsembleSampler object)``. 
+            ``(sampler iteration, last sample state object, EnsembleSampler object)``.
         stopping_iterations (int, optional): Number of iterations between sampler
-            attempts to evaluate the ``stopping_fn``. Stopping checks are only performed at the thinning rate. 
+            attempts to evaluate the ``stopping_fn``. Stopping checks are only performed at the thinning rate.
             If ``thin_by>1`` when :func:`EnsembleSampler.run_mcmc` is used, the sampler
             is checked for the stopping criterion every ``thin_by * stopping_iterations`` iterations.
         fill_zero_leaves_val (double, optional): When there are zero leaves in a
             given walker (across all branches), fill the likelihood value with
             ``fill_zero_leaves_val``. If wanting to keep zero leaves as a possible
             model, this should be set to the value of the contribution to the Likelihood
             from the data. (Default: ``-1e300``).
         num_repeats_in_model (int, optional): Number of times to repeat the in-model step
-            within in one sampler iteration. When analyzing the acceptance fraction, you must 
+            within in one sampler iteration. When analyzing the acceptance fraction, you must
             include the value of ``num_repeats_in_model`` to get the proper denominator.
-        num_repeats_rj (int, optional): Number of time to repeat the reversible jump step 
-            within in one sampler iteration. When analyzing the acceptance fraction, you must 
+        num_repeats_rj (int, optional): Number of time to repeat the reversible jump step
+            within in one sampler iteration. When analyzing the acceptance fraction, you must
             include the value of ``num_repeats_rj`` to get the proper denominator.
         track_moves (bool, optional): If ``True``, track acceptance fraction of each move
-            in the backend. If ``False``, no tracking is done. If ``True`` and run is interrupted, it will check 
-            that the move configuration has not changed. It will not allow the run to go on 
-            if it is changed. In this case, the user should declare a new backend and use the last 
+            in the backend. If ``False``, no tracking is done. If ``True`` and run is interrupted, it will check
+            that the move configuration has not changed. It will not allow the run to go on
+            if it is changed. In this case, the user should declare a new backend and use the last
             state from the previous backend. **Warning**: If the order of moves of the same move class
             is changed, the check may not catch it, so the tracking may mix move acceptance fractions together.
-        verbose (int, optional): # TODO
         info (dict, optional): Key and value pairs reprenting any information
             the user wants to add to the backend if the user is not inputing
             their own backend.
 
     Raises:
         ValueError: Any startup issues.
 
@@ -243,18 +231,16 @@
         update_iterations=-1,
         stopping_fn=None,
         stopping_iterations=-1,
         fill_zero_leaves_val=-1e300,
         num_repeats_in_model=1,
         num_repeats_rj=1,
         track_moves=True,
-        verbose=False,
         info={},
     ):
-
         # store priors
         self.priors = priors
 
         # store some kwargs
         self.provide_groups = provide_groups
         self.provide_supplimental = provide_supplimental
         self.fill_zero_leaves_val = fill_zero_leaves_val
@@ -288,15 +274,17 @@
             assert len(branch_names) == len(ndims)
             ndims = {bn: nd for bn, nd in zip(branch_names, ndims)}
 
         elif isinstance(ndims, dict):
             assert len(list(ndims.keys())) == len(branch_names)
             for key in ndims:
                 if key not in branch_names:
-                    raise ValueError(f"{key} is in ndims but does not appear in branch_names: {branch_names}.")
+                    raise ValueError(
+                        f"{key} is in ndims but does not appear in branch_names: {branch_names}."
+                    )
         else:
             raise ValueError("ndims is to be a scalar int, list or dict.")
 
         if isinstance(nleaves_max, int):
             assert len(branch_names) == 1
             nleaves_max = {branch_names[0]: nleaves_max}
 
@@ -304,15 +292,17 @@
             assert len(branch_names) == len(nleaves_max)
             nleaves_max = {bn: nl for bn, nl in zip(branch_names, nleaves_max)}
 
         elif isinstance(nleaves_max, dict):
             assert len(list(nleaves_max.keys())) == len(branch_names)
             for key in nleaves_max:
                 if key not in branch_names:
-                    raise ValueError(f"{key} is in nleaves_max but does not appear in branch_names: {branch_names}.")
+                    raise ValueError(
+                        f"{key} is in nleaves_max but does not appear in branch_names: {branch_names}."
+                    )
         else:
             raise ValueError("nleaves_max is to be a scalar int, list, or dict.")
 
         self.nbranches = len(branch_names)
 
         self.branch_names = branch_names
         self.ndims = ndims
@@ -332,15 +322,15 @@
                 total_ndim, nwalkers, **tempering_kwargs
             )
             self.ntemps = self.temperature_control.ntemps
 
         # set basic variables for sampling settings
         self.nwalkers = nwalkers
         self.nbranches = nbranches
-        
+
         # eryn wraps periodic parameters
         if periodic is not None:
             if not isinstance(periodic, PeriodicContainer) and not isinstance(
                 periodic, dict
             ):
                 raise ValueError(
                     "periodic must be PeriodicContainer or dict if not None."
@@ -388,25 +378,31 @@
             if self.has_reversible_jump:
                 if nleaves_min is None:
                     nleaves_min = {bn: 0 for bn in branch_names}
                 elif isinstance(nleaves_min, int):
                     assert len(branch_names) == 1
                     nleaves_min = {branch_names[0]: nleaves_min}
 
-                elif isinstance(nleaves_min, list) or isinstance(nleaves_min, np.ndarray):
+                elif isinstance(nleaves_min, list) or isinstance(
+                    nleaves_min, np.ndarray
+                ):
                     assert len(branch_names) == len(nleaves_min)
                     nleaves_min = {bn: nl for bn, nl in zip(branch_names, nleaves_min)}
 
                 elif isinstance(nleaves_min, dict):
                     assert len(list(nleaves_min.keys())) == len(branch_names)
                     for key in nleaves_min:
                         if key not in branch_names:
-                            raise ValueError(f"{key} is in nleaves_min but does not appear in branch_names: {branch_names}.")
+                            raise ValueError(
+                                f"{key} is in nleaves_min but does not appear in branch_names: {branch_names}."
+                            )
                 else:
-                    raise ValueError("If providing nleaves_min, nleaves_min is to be a scalar int, list, or dict.")
+                    raise ValueError(
+                        "If providing nleaves_min, nleaves_min is to be a scalar int, list, or dict."
+                    )
 
                 self.nleaves_min = nleaves_min
 
                 # default to DistributionGenerateRJ
                 rj_move = DistributionGenerateRJ(
                     self.priors,
                     nleaves_max=self.nleaves_max,
@@ -506,53 +502,52 @@
                 if move_name not in current_indices_move_keys:
                     current_indices_move_keys[move_name] = 0
 
                 else:
                     current_indices_move_keys[move_name] += 1
 
                 # get the full name including the index
-                full_move_name = (
-                    move_name + f"_{current_indices_move_keys[move_name]}"
-                )
+                full_move_name = move_name + f"_{current_indices_move_keys[move_name]}"
                 self.all_moves[full_move_name] = move
 
             # get move keys out
             move_keys = list(self.all_moves.keys())
 
         else:
-            move_keys = None 
+            move_keys = None
 
         self.move_keys = move_keys
 
         # Deal with re-used backends
         if not self.backend.initialized:
             self._previous_state = None
             self.reset(
                 branch_names=branch_names,
                 ntemps=self.ntemps,
                 nleaves_max=nleaves_max,
                 rj=self.has_reversible_jump,
                 moves=move_keys,
-                **info
+                **info,
             )
             state = np.random.get_state()
         else:
-
             if self.track_moves:
                 moves_okay = True
                 if len(self.move_keys) != len(self.backend.move_keys):
                     moves_okay = False
 
                 for key in self.move_keys:
                     if key not in self.backend.move_keys:
                         moves_okay = False
 
                 if not moves_okay:
-                    raise ValueError("Configuration of moves has changed. Cannot use the same backend. Declare a new backend and start from the previous state. If you would prefer not to track move acceptance fraction, set track_moves to False in the EnsembleSampler.")
-            
+                    raise ValueError(
+                        "Configuration of moves has changed. Cannot use the same backend. Declare a new backend and start from the previous state. If you would prefer not to track move acceptance fraction, set track_moves to False in the EnsembleSampler."
+                    )
+
             # Check the backend shape
             for i, (name, shape) in enumerate(self.backend.shape.items()):
                 test_shape = (
                     self.ntemps,
                     self.nwalkers,
                     self.nleaves_max[name],
                     self.ndims[name],
@@ -581,15 +576,14 @@
         self._random.set_state(state)
 
         # Do a little bit of _magic_ to make the likelihood call with
         # ``args`` and ``kwargs`` pickleable.
         self.log_like_fn = _FunctionWrapper(log_like_fn, args, kwargs)
 
         self.all_walkers = self.nwalkers * self.ntemps
-        self.verbose = verbose
 
         # prepare plotting
         # TODO: adjust plotting maybe?
         self.plot_iterations = plot_iterations
 
         if plot_generator is None and self.plot_iterations > 0:
             raise NotImplementedError
@@ -644,20 +638,19 @@
 
         """
         return self._priors
 
     @priors.setter
     def priors(self, priors):
         """Set priors information.
-        
+
         This performs checks to make sure the inputs are okay.
 
         """
         if isinstance(priors, dict):
-
             self._priors = {}
 
             for key in priors.keys():
                 test = priors[key]
                 if isinstance(test, dict):
                     # check all dists
                     for ind, dist in test.items():
@@ -751,16 +744,16 @@
         """Advance the chain as a generator
 
         Args:
             initial_state (State or ndarray[ntemps, nwalkers, nleaves_max, ndim] or dict): The initial
                 :class:`State` or positions of the walkers in the
                 parameter space. If multiple branches used, must be dict with keys
                 as the ``branch_names`` and values as the positions. If ``betas`` are
-                provided in the state object, they will be loaded into the 
-                ``temperature_control``. 
+                provided in the state object, they will be loaded into the
+                ``temperature_control``.
             iterations (int or None, optional): The number of steps to generate.
                 ``None`` generates an infinite stream (requires ``store=False``).
                 (default: 1)
             tune (bool, optional): If ``True``, the parameters of some moves
                 will be automatically tuned. (default: ``False``)
             thin_by (int, optional): If you only want to store and yield every
                 ``thin_by`` samples in the chain, set ``thin_by`` to an
@@ -775,15 +768,15 @@
                 be shown as the sampler progresses. If a string, will select a
                 specific ``tqdm`` progress bar - most notable is
                 ``'notebook'``, which shows a progress bar suitable for
                 Jupyter notebooks.  If ``False``, no progress bar will be
                 shown. (default: ``False``)
             skip_initial_state_check (bool, optional): If ``True``, a check
                 that the initial_state can fully explore the space will be
-                skipped. If using reversible jump, the user needs to ensure this on their own 
+                skipped. If using reversible jump, the user needs to ensure this on their own
                 (``skip_initial_state_check``is set to ``False`` in this case.
                 (default: ``True``)
 
         Returns:
             State: Every ``thin_by`` steps, this generator yields the :class:`State` of the ensemble.
 
         Raises:
@@ -880,15 +873,14 @@
         with get_progress_bar(progress, total) as pbar:
             i = 0
             for _ in count() if iterations is None else range(iterations):
                 for _ in range(yield_step):
                     # in model moves
                     accepted = np.zeros((self.ntemps, self.nwalkers))
                     for repeat in range(self.num_repeats_in_model):
-
                         # Choose a random move
                         move = self._random.choice(self.moves, p=self.weights)
 
                         # Propose (in model)
                         state, accepted_out = move.propose(model, state)
                         accepted += accepted_out
                         if self.ntemps > 1:
@@ -925,18 +917,18 @@
 
                     else:
                         rj_accepted = None
                         rj_swaps = None
 
                     # Save the new step
                     if store and (i + 1) % checkpoint_step == 0:
-
                         if self.track_moves:
-                            moves_accepted_fraction = {key:
-                                move_tmp.acceptance_fraction for key, move_tmp in self.all_moves.items()
+                            moves_accepted_fraction = {
+                                key: move_tmp.acceptance_fraction
+                                for key, move_tmp in self.all_moves.items()
                             }
                         else:
                             moves_accepted_fraction = None
 
                         self.backend.save_step(
                             state,
                             accepted,
@@ -959,19 +951,19 @@
         Iterate :func:`sample` for ``nsteps`` iterations and return the result.
 
         Args:
             initial_state (State or ndarray[ntemps, nwalkers, nleaves_max, ndim] or dict): The initial
                 :class:`State` or positions of the walkers in the
                 parameter space. If multiple branches used, must be dict with keys
                 as the ``branch_names`` and values as the positions. If ``betas`` are
-                provided in the state object, they will be loaded into the 
-                ``temperature_control``. 
+                provided in the state object, they will be loaded into the
+                ``temperature_control``.
             nsteps (int): The number of steps to generate. The total number of proposals is ``nsteps * thin_by``.
             burn (int, optional): Number of burn steps to run before storing information. The ``thin_by`` kwarg is ignored when counting burn steps since there is no storage (equivalent to ``thin_by=1``).
-            post_burn_update (bool, optional): If ``True``, run ``update_fn`` after burn in. 
+            post_burn_update (bool, optional): If ``True``, run ``update_fn`` after burn in.
 
         Other parameters are directly passed to :func:`sample`.
 
         Returns:
             State: This method returns the most recent result from :func:`sample`.
 
         Raises:
@@ -987,17 +979,14 @@
             initial_state = self._previous_state
 
         # setup thin_by info
         thin_by = 1 if "thin_by" not in kwargs else kwargs["thin_by"]
 
         # run burn in
         if burn is not None and burn != 0:
-            if self.verbose:
-                print("Start burn")
-
             # prepare kwargs that relate to burn
             burn_kwargs = deepcopy(kwargs)
             burn_kwargs["store"] = False
             burn_kwargs["thin_by"] = 1
             i = 0
             for results in self.sample(initial_state, iterations=burn, **burn_kwargs):
                 # if updating and using burn_in, need to make sure it does not use
@@ -1011,25 +1000,22 @@
                 i += 1
 
             # run post-burn update
             if post_burn_update and self.update_fn is not None:
                 self.update_fn(i, results, self)
 
             initial_state = results
-            if self.verbose:
-                print("Finish burn")
 
         if nsteps == 0:
             return initial_state
 
         results = None
 
         i = 0
         for results in self.sample(initial_state, iterations=nsteps, **kwargs):
-
             # diagnostic plots
             # TODO: adjust diagnostic plots
             if self.plot_iterations > 0 and (i + 1) % (self.plot_iterations) == 0:
                 self.plot_generator.generate_plot_info()  # TODO: remove defaults
 
             # check for stopping before updating
             if (
@@ -1091,15 +1077,14 @@
 
         # for completely customizable priors
         if "all_models_together" in self.priors:
             prior_out = self.priors["all_models_together"].logpdf(coords, inds)
             assert prior_out.shape == (ntemps, nwalkers)
 
         elif self.provide_groups:
-
             # get group information from the inds dict
             groups = groups_from_inds(inds)
 
             # get the coordinates that are used
             for i, (name, coords_i) in enumerate(coords.items()):
                 x_in[name] = coords_i[inds[name]]
 
@@ -1292,15 +1277,14 @@
             groups_in = groups_in[0]
 
         # list of paramter arrays
         params_in = list(x_in.values())
 
         # Likelihoods are vectorized across groups
         if self.vectorize:
-
             # prepare args list
             args_in = []
 
             # when vectorizing, if params_in has one entry, take out of list
             if len(params_in) == 1:
                 params_in = params_in[0]
 
@@ -1331,26 +1315,24 @@
             args_and_kwargs = (args_in, kwargs_in)
 
             # get vectorized results
             results = self.log_like_fn(args_and_kwargs)
 
         # each Likelihood is computed individually
         else:
-
             # if groups in is an array, need to put it in a list.
             if isinstance(groups_in, np.ndarray):
                 groups_in = [groups_in]
 
             # prepare input args for all Likelihood calls
             # to be spread out with map functions below
             args_in = []
 
             # each individual group in the groups_map
             for group_i in groups_map:
-
                 # args and kwargs for the individual Likelihood
                 arg_i = [None for _ in self.branch_names]
                 kwarg_i = {}
 
                 # iterate over the group information from the branches
                 for branch_i, groups_in_set in enumerate(groups_in):
                     # which entries in this branch are in the overall group tested
@@ -1558,26 +1540,29 @@
     """
     This is a hack to make the likelihood function pickleable when ``args``
     or ``kwargs`` are also included.
 
     """
 
     def __init__(
-        self, f, args, kwargs,
+        self,
+        f,
+        args,
+        kwargs,
     ):
         self.f = f
         self.args = [] if args is None else args
         self.kwargs = {} if kwargs is None else kwargs
 
     def __call__(self, args_and_kwargs):
         """
         Internal function that takes a tuple (args, kwargs) for entrance into the Likelihood.
 
         ``self.args`` and ``self.kwargs`` are added to these inputs.
-        
+
         """
 
         args_in_add, kwargs_in_add = args_and_kwargs
 
         try:
             args_in = args_in_add + type(args_in_add)(self.args)
             kwargs_in = {**kwargs_in_add, **self.kwargs}
@@ -1598,21 +1583,21 @@
             raise
 
 
 def walkers_independent(coords_in):
     """Determine if walkers are independent
 
     Orginall from ``emcee``.
-    
+
     Args:
         coords_in (np.ndarray[ntemps, nwalkers, nleaves_max, ndim]): Coordinates of the walkers.
 
     Returns:
         bool: If walkers are independent.
-    
+
     """
     # make sure it is 4-dimensional and reshape
     # so it groups by temperature and walker
     assert coords_in.ndim == 4
     ntemps, nwalkers, nleaves_max, ndim = coords_in.shape
     coords = coords_in.reshape(ntemps * nwalkers, nleaves_max * ndim)
 
@@ -1622,10 +1607,10 @@
 
     # roughly determine covariance information
     C = coords - np.mean(coords, axis=0)[None, :]
     C_colmax = np.amax(np.abs(C), axis=0)
     if np.any(C_colmax == 0):
         return False
     C /= C_colmax
-    C_colsum = np.sqrt(np.sum(C ** 2, axis=0))
+    C_colsum = np.sqrt(np.sum(C**2, axis=0))
     C /= C_colsum
     return np.linalg.cond(C.astype(float)) <= 1e8
```

### Comparing `Eryn-1.1.3/eryn/moves/__init__.py` & `Eryn-1.1.4/eryn/moves/__init__.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.3/eryn/moves/combine.py` & `Eryn-1.1.4/eryn/moves/combine.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.3/eryn/moves/delayedrejection.py` & `Eryn-1.1.4/eryn/moves/delayedrejection.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.3/eryn/moves/distgen.py` & `Eryn-1.1.4/eryn/moves/distgen.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.3/eryn/moves/distgenrj.py` & `Eryn-1.1.4/eryn/moves/distgenrj.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.3/eryn/moves/gaussian.py` & `Eryn-1.1.4/eryn/moves/gaussian.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 __all__ = ["GaussianMove"]
 
 
 class GaussianMove(MHMove):
     """A Metropolis step with a Gaussian proposal function.
 
-    This class is heavily based on the same class in ``emcee``. 
+    This class is heavily based on the same class in ``emcee``.
 
     Args:
-        cov (dict): The covariance of the proposal function. The keys are branch names and the 
+        cov (dict): The covariance of the proposal function. The keys are branch names and the
             values are covariance information. This information can be provided as a scalar,
             vector, or matrix and the proposal will be assumed isotropic,
             axis-aligned, or general, respectively.
         mode (str, optional): Select the method used for updating parameters. This
             can be one of ``"vector"``, ``"random"``, or ``"sequential"``. The
             ``"vector"`` mode updates all dimensions simultaneously,
             ``"random"`` randomly selects a dimension and only updates that
@@ -32,15 +32,14 @@
     Raises:
         ValueError: If the proposal dimensions are invalid or if any of any of
             the other arguments are inconsistent.
 
     """
 
     def __init__(self, cov_all, mode="vector", factor=None, **kwargs):
-
         self.all_proposal = {}
         for name, cov in cov_all.items():
             # Parse the proposal type.
             try:
                 float(cov)
 
             except TypeError:
@@ -123,15 +122,14 @@
                 for name, tmp in q.items()
             }
 
         return q, np.zeros((ntemps, nwalkers))
 
 
 class _isotropic_proposal(object):
-
     allowed_modes = ["vector", "random", "sequential"]
 
     def __init__(self, scale, factor, mode):
         self.index = 0
         self.scale = scale
         self.invscale = np.linalg.inv(np.linalg.cholesky(scale))
         if factor is None:
@@ -174,14 +172,13 @@
 
 class _diagonal_proposal(_isotropic_proposal):
     def get_updated_vector(self, rng, x0):
         return x0 + self.get_factor(rng) * self.scale * rng.randn(*(x0.shape))
 
 
 class _proposal(_isotropic_proposal):
-
     allowed_modes = ["vector"]
 
     def get_updated_vector(self, rng, x0):
         return x0 + self.get_factor(rng) * rng.multivariate_normal(
             np.zeros(len(self.scale)), self.scale, size=len(x0)
         )
```

### Comparing `Eryn-1.1.3/eryn/moves/group.py` & `Eryn-1.1.4/eryn/moves/group.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.3/eryn/moves/groupstretch.py` & `Eryn-1.1.4/eryn/moves/groupstretch.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.3/eryn/moves/mh.py` & `Eryn-1.1.4/eryn/moves/mh.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.3/eryn/moves/move.py` & `Eryn-1.1.4/eryn/moves/move.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.3/eryn/moves/mtdistgen.py` & `Eryn-1.1.4/eryn/moves/mtdistgen.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.3/eryn/moves/mtdistgenrj.py` & `Eryn-1.1.4/eryn/moves/mtdistgenrj.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.3/eryn/moves/multipletry.py` & `Eryn-1.1.4/eryn/moves/multipletry.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.3/eryn/moves/red_blue.py` & `Eryn-1.1.4/eryn/moves/red_blue.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 class RedBlueMove(Move, ABC):
     """
     An abstract red-blue ensemble move with parallelization as described in
     `Foreman-Mackey et al. (2013) <https://arxiv.org/abs/1202.3665>`_.
 
-    This class is heavily based on the original from ``emcee``. 
+    This class is heavily based on the original from ``emcee``.
 
     Args:
         nsplits (int, optional): The number of sub-ensembles to use. Each
             sub-ensemble is updated in parallel using the other sets as the
             complementary ensemble. The default value is ``2`` and you
             probably won't need to change that.
         randomize_split (bool, optional): Randomly shuffle walkers between
@@ -43,30 +43,30 @@
     ):
         super(RedBlueMove, self).__init__(**kwargs)
         self.nsplits = int(nsplits)
         self.live_dangerously = live_dangerously
         self.randomize_split = randomize_split
 
     def setup(self, branches_coords):
-        """Any setup for the proposal. 
-        
+        """Any setup for the proposal.
+
         Args:
             branches_coords (dict): Keys are ``branch_names``. Values are
                 np.ndarray[ntemps, nwalkers, nleaves_max, ndim]. These are the curent
                 coordinates for all the walkers.
 
         """
 
     @classmethod
     def get_proposal(self, sample, complement, random, gibbs_ndim=None):
         """Make a proposal
 
         Args:
             sample (dict): Keys are ``branch_names``. Values are
-                np.ndarray[ntemps, nwalkers, nleaves_max, ndim]. 
+                np.ndarray[ntemps, nwalkers, nleaves_max, ndim].
             complement (dict): Keys are ``branch_names``. Values are lists of other
                 other np.ndarray[ntemps, nwalkers - subset size, nleaves_max, ndim] from
                 all other subsets. This is the compliment whose ``coords`` are
                 used to form the proposal for the ``sample`` subset.
             random (object): Current random state of the sampler.
             gibbs_ndim (int or np.ndarray, optional): If Gibbs sampling, this indicates
                 the true dimension. If given as an array, must have shape ``(ntemps, nwalkers)``.
@@ -123,18 +123,17 @@
             [np.random.shuffle(x) for x in inds]
 
         all_branch_names = list(state.branches.keys())
 
         ntemps, nwalkers, _, _ = state.branches[all_branch_names[0]].shape
 
         # get gibbs sampling information
-        for (branch_names_run, inds_run) in self.gibbs_sampling_setup_iterator(
+        for branch_names_run, inds_run in self.gibbs_sampling_setup_iterator(
             all_branch_names
         ):
-
             # setup proposals based on Gibbs sampling
             (
                 coords_going_for_proposal,
                 inds_going_for_proposal,
                 at_least_one_proposal,
             ) = self.setup_proposals(
                 branch_names_run, inds_run, state.branches_coords, state.branches_inds
@@ -142,27 +141,27 @@
 
             if not at_least_one_proposal:
                 continue
 
             # prepare accepted fraction
             accepted_here = np.zeros((ntemps, nwalkers), dtype=bool)
             for split in range(self.nsplits):
-
                 # get split information
                 S1 = inds == split
                 num_total_here = np.sum(inds == split)
                 nwalkers_here = np.sum(S1[0])
 
                 all_inds_shaped = all_inds[S1].reshape(ntemps, nwalkers_here)
-                fixed_inds_shaped = all_inds[~S1].reshape(ntemps, nwalkers_here)
 
                 # inds including gibbs information
                 new_inds = {
                     name: np.take_along_axis(
-                        state.branches[name].inds, all_inds_shaped[:, :, None], axis=1,
+                        state.branches[name].inds,
+                        all_inds_shaped[:, :, None],
+                        axis=1,
                     )
                     for name in state.branches
                 }
 
                 # the actual inds for the subset
                 real_inds_subset = {
                     name: new_inds[name] for name in inds_going_for_proposal
@@ -286,15 +285,18 @@
                 lnpdiff = factors + logP - prev_logP
 
                 keep = lnpdiff > np.log(model.random.rand(ntemps, nwalkers_here))
 
                 # if gibbs sampling, this will say it is accepted if
                 # any of the gibbs proposals were accepted
                 np.put_along_axis(
-                    accepted_here, all_inds_shaped, keep, axis=1,
+                    accepted_here,
+                    all_inds_shaped,
+                    keep,
+                    axis=1,
                 )
 
                 # readout for total
                 accepted = (accepted.astype(int) + accepted_here.astype(int)).astype(
                     bool
                 )
                 # new state
@@ -318,8 +320,7 @@
             self.num_proposals += 1
 
         # temp swaps
         if self.temperature_control is not None:
             state = self.temperature_control.temper_comps(state)
 
         return state, accepted
-
```

### Comparing `Eryn-1.1.3/eryn/moves/rj.py` & `Eryn-1.1.4/eryn/moves/rj.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 from .distgen import DistributionGenerate
 
 __all__ = ["ReversibleJumpMove"]
 
 
 class ReversibleJumpMove(Move):
     """
-    An abstract reversible jump move from # TODO: add citations.
+    An abstract reversible jump move.
 
     Args:
         nleaves_max (dict): Maximum number(s) of leaves for each model.
             Keys are ``branch_names`` and values are ``nleaves_max`` for each branch.
             This is a keyword argument, nut it is required.
         nleaves_min (dict): Minimum number(s) of leaves for each model.
             Keys are ``branch_names`` and values are ``nleaves_min`` for each branch.
             This is a keyword argument, nut it is required.
         tune (bool, optional): If True, tune proposal. (Default: ``False``)
-        fix_change (int or None, optional): Fix the change in the number of leaves. Make them all 
+        fix_change (int or None, optional): Fix the change in the number of leaves. Make them all
             add a leaf or remove a leaf. This can be useful for some search functions. Options
             are ``+1`` or ``-1``. (default: ``None``)
 
     """
 
     def __init__(
         self,
@@ -39,18 +39,22 @@
         fix_change=None,
         **kwargs
     ):
         # super(ReversibleJumpMove, self).__init__(**kwargs)
         Move.__init__(self, is_rj=True, **kwargs)
 
         if nleaves_max is None or nleaves_min is None:
-            raise ValueError("Must provide nleaves_min and nleaves_max keyword arguments for RJ.")
+            raise ValueError(
+                "Must provide nleaves_min and nleaves_max keyword arguments for RJ."
+            )
 
         if not isinstance(nleaves_max, dict) or not isinstance(nleaves_min, dict):
-            raise ValueError("nleaves_min and nleaves_max must be provided as dictionaries with keys as branch names and values as the max or min leaf count.")
+            raise ValueError(
+                "nleaves_min and nleaves_max must be provided as dictionaries with keys as branch names and values as the max or min leaf count."
+            )
         # store info
         self.nleaves_max = nleaves_max
         self.nleaves_min = nleaves_min
         self.tune = tune
         self.dr = dr
         self.fix_change = fix_change
         if self.fix_change not in [None, +1, -1]:
@@ -67,15 +71,15 @@
             else:
                 # Otherwise pass given input
                 dr_proposal = self.dr
 
             self.dr = DelayedRejection(dr_proposal, max_iter=dr_max_iter)
 
     def setup(self, branches_coords):
-        """Any setup for the proposal. 
+        """Any setup for the proposal.
 
         Args:
             branches_coords (dict): Keys are ``branch_names``. Values are
                 np.ndarray[ntemps, nwalkers, nleaves_max, ndim]. These are the curent
                 coordinates for all the walkers.
 
         """
@@ -88,18 +92,18 @@
         Args:
             all_coords (dict): Keys are ``branch_names``. Values are
                 np.ndarray[ntemps, nwalkers, nleaves_max, ndim]. These are the curent
                 coordinates for all the walkers.
             all_inds (dict): Keys are ``branch_names``. Values are
                 np.ndarray[ntemps, nwalkers, nleaves_max]. These are the boolean
                 arrays marking which leaves are currently used within each walker.
-            nleaves_min_all (dict): Minimum values of leaf ount for each model. Must have same order as ``all_cords``. 
-            nleaves_max_all (dict): Maximum values of leaf ount for each model. Must have same order as ``all_cords``. 
+            nleaves_min_all (dict): Minimum values of leaf ount for each model. Must have same order as ``all_cords``.
+            nleaves_max_all (dict): Maximum values of leaf ount for each model. Must have same order as ``all_cords``.
             random (object): Current random state of the sampler.
-            **kwargs (ignored): For modularity. 
+            **kwargs (ignored): For modularity.
 
         Returns:
             tuple: Tuple containing proposal information.
                 First entry is the new coordinates as a dictionary with keys
                 as ``branch_names`` and values as
                 ``double `` np.ndarray[ntemps, nwalkers, nleaves_max, ndim] containing
                 proposed coordinates. Second entry is the new ``inds`` array with
@@ -113,31 +117,31 @@
             NotImplementedError: If this proposal is not implemented by a subclass.
 
         """
         raise NotImplementedError("The proposal must be implemented by " "subclasses")
 
     def get_model_change_proposal(self, inds, random, nleaves_min, nleaves_max):
         """Helper function for changing the model count by 1.
-        
+
         This helper function works with nested models where you want to add or remove
-        one leaf at a time. 
+        one leaf at a time.
 
         Args:
-            inds (np.ndarray): ``inds`` values for this specific branch with shape 
+            inds (np.ndarray): ``inds`` values for this specific branch with shape
                 ``(ntemps, nwalkers, nleaves_max)``.
             random (object): Current random state of the sampler.
             nleaves_min (int): Minimum allowable leaf count for this branch.
             nleaves_max (int): Maximum allowable leaf count for this branch.
 
         Returns:
             dict: Keys are ``"+1"`` and ``"-1"``. Values are indexing information.
                     ``"+1"`` and ``"-1"`` indicate if a source is being added or removed, respectively.
                     The indexing information is a 2D array with shape ``(number changing, 3)``.
                     The length 3 is the index into each of the ``(ntemps, nwalkers, nleaves_max)``.
-        
+
         """
 
         raise NotImplementedError
 
     def propose(self, model, state):
         """Use the move to generate a proposal and compute the acceptance
 
@@ -158,18 +162,17 @@
 
         accepted = np.zeros((ntemps, nwalkers), dtype=bool)
 
         all_branch_names = list(state.branches.keys())
 
         ntemps, nwalkers, _, _ = state.branches[all_branch_names[0]].shape
 
-        for (branch_names_run, inds_run) in self.gibbs_sampling_setup_iterator(
+        for branch_names_run, inds_run in self.gibbs_sampling_setup_iterator(
             all_branch_names
         ):
-
             # gibbs sampling is only over branches so pick out that info
             coords_propose_in = {
                 key: state.branches_coords[key] for key in branch_names_run
             }
             inds_propose_in = {
                 key: state.branches_inds[key] for key in branch_names_run
             }
@@ -220,15 +223,15 @@
             # fix any ordering issues
             q, new_inds, branches_supps_new = self.ensure_ordering(
                 list(state.branches.keys()), q, new_inds, branches_supps_new
             )
 
             edge_factors = np.zeros((ntemps, nwalkers))
             # get factors for edges
-            for (name, branch) in state.branches.items():
+            for name, branch in state.branches.items():
                 nleaves_max = self.nleaves_max[name]
                 nleaves_min = self.nleaves_min[name]
 
                 if name not in branch_names_run:
                     continue
 
                 # get old and new values
```

### Comparing `Eryn-1.1.3/eryn/moves/stretch.py` & `Eryn-1.1.4/eryn/moves/stretch.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,16 +148,14 @@
         if self.use_gpu and not self.return_gpu:
             temp = temp.get()
         return temp
 
     def get_proposal(self, s_all, c_all, random, gibbs_ndim=None, **kwargs):
         """Generate stretch proposal
 
-        # TODO: add log proposal from ptemcee
-
         Args:
             s_all (dict): Keys are ``branch_names`` and values are coordinates
                 for which a proposal is to be generated.
             c_all (dict): Keys are ``branch_names`` and values are lists. These
                 lists contain all the complement array values.
             random (object): Random state object.
             gibbs_ndim (int or np.ndarray, optional): If Gibbs sampling, this indicates
```

### Comparing `Eryn-1.1.3/eryn/moves/tempering.py` & `Eryn-1.1.4/eryn/moves/tempering.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.3/eryn/pbar.py` & `Eryn-1.1.4/eryn/pbar.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.3/eryn/prior.py` & `Eryn-1.1.4/eryn/prior.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.3/eryn/state.py` & `Eryn-1.1.4/eryn/state.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.3/eryn/utils/periodic.py` & `Eryn-1.1.4/eryn/utils/periodic.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.3/eryn/utils/stopping.py` & `Eryn-1.1.4/eryn/utils/stopping.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.3/eryn/utils/transform.py` & `Eryn-1.1.4/eryn/utils/transform.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.3/eryn/utils/updates.py` & `Eryn-1.1.4/eryn/utils/updates.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.3/setup.py` & `Eryn-1.1.4/setup.py`

 * *Files identical despite different names*

