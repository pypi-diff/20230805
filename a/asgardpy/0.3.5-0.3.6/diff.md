# Comparing `tmp/asgardpy-0.3.5.tar.gz` & `tmp/asgardpy-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgardpy-0.3.5.tar", last modified: Mon Jul 17 00:34:03 2023, max compression
+gzip compressed data, was "asgardpy-0.3.6.tar", last modified: Sat Aug  5 14:13:25 2023, max compression
```

## Comparing `asgardpy-0.3.5.tar` & `asgardpy-0.3.6.tar`

### file list

```diff
@@ -1,39 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:34:03.164307 asgardpy-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-17 00:33:45.000000 asgardpy-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-17 00:34:03.164307 asgardpy-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-17 00:33:45.000000 asgardpy-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:34:03.164307 asgardpy-0.3.5/asgardpy/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:34:03.164307 asgardpy-0.3.5/asgardpy/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/analysis/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:34:03.164307 asgardpy-0.3.5/asgardpy/base/
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/base/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/base/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/base/reduction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:34:03.164307 asgardpy-0.3.5/asgardpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/config/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:34:03.164307 asgardpy-0.3.5/asgardpy/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/data/dataset_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    25065 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/data/dataset_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/data/dl4.py
--rw-r--r--   0 runner    (1001) docker     (123)    38087 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/data/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:34:03.164307 asgardpy-0.3.5/asgardpy/io/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/io/io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:34:03.164307 asgardpy-0.3.5/asgardpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-17 00:34:03.000000 asgardpy-0.3.5/asgardpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-17 00:34:03.000000 asgardpy-0.3.5/asgardpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 00:34:03.000000 asgardpy-0.3.5/asgardpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-17 00:34:03.000000 asgardpy-0.3.5/asgardpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 00:34:03.000000 asgardpy-0.3.5/asgardpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-17 00:33:45.000000 asgardpy-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-17 00:34:03.164307 asgardpy-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-17 00:33:45.000000 asgardpy-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:34:03.164307 asgardpy-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-17 00:33:45.000000 asgardpy-0.3.5/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:13:25.127241 asgardpy-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-08-05 14:13:00.000000 asgardpy-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-05 14:13:25.127241 asgardpy-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-08-05 14:13:00.000000 asgardpy-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:13:25.119241 asgardpy-0.3.6/asgardpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-05 14:13:00.000000 asgardpy-0.3.6/asgardpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:13:25.127241 asgardpy-0.3.6/asgardpy/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-05 14:13:00.000000 asgardpy-0.3.6/asgardpy/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-08-05 14:13:00.000000 asgardpy-0.3.6/asgardpy/analysis/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-05 14:13:00.000000 asgardpy-0.3.6/asgardpy/analysis/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-05 14:13:00.000000 asgardpy-0.3.6/asgardpy/analysis/step_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:13:25.127241 asgardpy-0.3.6/asgardpy/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-08-05 14:13:00.000000 asgardpy-0.3.6/asgardpy/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-08-05 14:13:00.000000 asgardpy-0.3.6/asgardpy/base/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-08-05 14:13:00.000000 asgardpy-0.3.6/asgardpy/base/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18962 2023-08-05 14:13:00.000000 asgardpy-0.3.6/asgardpy/base/reduction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:13:25.127241 asgardpy-0.3.6/asgardpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-05 14:13:00.000000 asgardpy-0.3.6/asgardpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-08-05 14:13:00.000000 asgardpy-0.3.6/asgardpy/config/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:13:25.127241 asgardpy-0.3.6/asgardpy/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-05 14:13:00.000000 asgardpy-0.3.6/asgardpy/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9191 2023-08-05 14:13:00.000000 asgardpy-0.3.6/asgardpy/data/dataset_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25722 2023-08-05 14:13:00.000000 asgardpy-0.3.6/asgardpy/data/dataset_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-08-05 14:13:00.000000 asgardpy-0.3.6/asgardpy/data/dl4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23318 2023-08-05 14:13:00.000000 asgardpy-0.3.6/asgardpy/data/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:13:25.127241 asgardpy-0.3.6/asgardpy/gammapy/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-05 14:13:00.000000 asgardpy-0.3.6/asgardpy/gammapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-08-05 14:13:00.000000 asgardpy-0.3.6/asgardpy/gammapy/interoperate_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:13:25.127241 asgardpy-0.3.6/asgardpy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-05 14:13:00.000000 asgardpy-0.3.6/asgardpy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-08-05 14:13:00.000000 asgardpy-0.3.6/asgardpy/io/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 14:13:00.000000 asgardpy-0.3.6/asgardpy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:13:25.127241 asgardpy-0.3.6/asgardpy/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-05 14:13:00.000000 asgardpy-0.3.6/asgardpy/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-08-05 14:13:00.000000 asgardpy-0.3.6/asgardpy/stats/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-05 14:13:00.000000 asgardpy-0.3.6/asgardpy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:13:25.119241 asgardpy-0.3.6/asgardpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-05 14:13:25.000000 asgardpy-0.3.6/asgardpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-08-05 14:13:25.000000 asgardpy-0.3.6/asgardpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 14:13:25.000000 asgardpy-0.3.6/asgardpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-05 14:13:25.000000 asgardpy-0.3.6/asgardpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 14:13:25.000000 asgardpy-0.3.6/asgardpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-05 14:13:00.000000 asgardpy-0.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-08-05 14:13:25.127241 asgardpy-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-08-05 14:13:00.000000 asgardpy-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:13:25.127241 asgardpy-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-05 14:13:00.000000 asgardpy-0.3.6/tests/test_basic.py
```

### Comparing `asgardpy-0.3.5/LICENSE` & `asgardpy-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.5/PKG-INFO` & `asgardpy-0.3.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: asgardpy
-Version: 0.3.5
+Version: 0.3.6
 Summary: Gammapy-based pipeline for easy joint analysis of different gamma-ray datasets
 Home-page: https://github.com/chaimain/asgardpy
-Download-URL: https://github.com/chaimain/asgardpy/archive/refs/tags/v0.3.1.tar.gz
+Download-URL: https://github.com/chaimain/asgardpy/archive/refs/tags/v0.3.6.tar.gz
 Author: Chaitanya Priyadarshi
 Author-email: chaitanya.p.astrphys@gmail.com
 License: Apache
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8106369.svg)](https://doi.org/10.5281/zenodo.8106369) ![PyPI](https://img.shields.io/pypi/v/asgardpy?label=pypi%20asgardpy) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](https://www.astropy.org/)
+# asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8106369.svg)](https://doi.org/10.5281/zenodo.8106369) ![PyPI](https://img.shields.io/pypi/v/asgardpy?label=pypi%20asgardpy) [![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7699/badge)](https://bestpractices.coreinfrastructure.org/projects/7699) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](https://www.astropy.org/)
+
 ## Analysis Software for GAmma-Ray Data in Python
 
 'User-friendly' configuration-centred pipeline built over [Gammapy](https://github.com/gammapy/gammapy) to allow for easy simultaneous analysis of various datasets of different formats.
 Example: 3D Fermi-LAT (with various source models in the Region of Interest stored in XML file) + 1D energy-dependent directional cuts MAGIC/LST [PointSkyRegion geometry for ON region] + 1D global directional cut VERITAS [CircleSkyRegion geometry for ON region].
 
 Follow the documentation at https://asgardpy.readthedocs.io/en/latest/ for the main functionality of this pipeline.
 Follow the [Gammapy v1.1](https://docs.gammapy.org/1.1/) documentation for understanding the core Gammapy objects.
```

### Comparing `asgardpy-0.3.5/README.md` & `asgardpy-0.3.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8106369.svg)](https://doi.org/10.5281/zenodo.8106369) ![PyPI](https://img.shields.io/pypi/v/asgardpy?label=pypi%20asgardpy) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](https://www.astropy.org/)
+# asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8106369.svg)](https://doi.org/10.5281/zenodo.8106369) ![PyPI](https://img.shields.io/pypi/v/asgardpy?label=pypi%20asgardpy) [![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7699/badge)](https://bestpractices.coreinfrastructure.org/projects/7699) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](https://www.astropy.org/)
+
 ## Analysis Software for GAmma-Ray Data in Python
 
 'User-friendly' configuration-centred pipeline built over [Gammapy](https://github.com/gammapy/gammapy) to allow for easy simultaneous analysis of various datasets of different formats.
 Example: 3D Fermi-LAT (with various source models in the Region of Interest stored in XML file) + 1D energy-dependent directional cuts MAGIC/LST [PointSkyRegion geometry for ON region] + 1D global directional cut VERITAS [CircleSkyRegion geometry for ON region].
 
 Follow the documentation at https://asgardpy.readthedocs.io/en/latest/ for the main functionality of this pipeline.
 Follow the [Gammapy v1.1](https://docs.gammapy.org/1.1/) documentation for understanding the core Gammapy objects.
```

### Comparing `asgardpy-0.3.5/asgardpy/analysis/analysis.py` & `asgardpy-0.3.6/asgardpy/analysis/analysis.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 Config-driven high level analysis interface.
 """
 import logging
 
 from gammapy.datasets import Datasets
 from gammapy.modeling.models import Models
 
-from asgardpy.base import AnalysisStep
-from asgardpy.config import AsgardpyConfig
-from asgardpy.data import set_models
+from asgardpy.analysis.step import AnalysisStep
+from asgardpy.config.generator import AsgardpyConfig, gammapy_to_asgardpy_model_config
+from asgardpy.data.target import set_models
+from asgardpy.stats.stats import get_goodness_of_fit_stats
 
 log = logging.getLogger(__name__)
 
 __all__ = ["AsgardpyAnalysis"]
 
 
 class AsgardpyAnalysis:
@@ -37,30 +38,45 @@
     """
 
     def __init__(self, config):
         self.log = log
         self.config = config
 
         if self.config.target.models_file.is_file():
-            other_config = AsgardpyConfig.read(self.config.target.models_file)
+            try:
+                if AsgardpyConfig.read(self.config.target.models_file):
+                    other_config = AsgardpyConfig.read(self.config.target.models_file)
+                else:
+                    other_config = gammapy_to_asgardpy_model_config(self.config.target.models_file)
+            except OSError:
+                self.log.error("Provided models file is not readable")
             self.config = self.config.update(other_config)
 
         self.config.set_logging()
         self.datasets = Datasets()
-        self.instrument_spectral_info = {"name": [], "spectral_energy_ranges": []}
+        self.instrument_spectral_info = {
+            "name": [],
+            "spectral_energy_ranges": [],
+            "en_bins": 0,
+            "free_params": 0,
+            "DoF": 0,
+        }
         self.dataset_name_list = []
 
         self.final_model = Models()
         self.final_data_products = ["fit", "fit_result", "flux_points"]
 
         for data_product in self.final_data_products:
             setattr(self, data_product, None)
 
     @property
     def models(self):
+        """
+        Display the assigned Models.
+        """
         if not self.datasets:
             raise RuntimeError("No datasets defined. Impossible to set models.")
         return self.datasets.models
 
     @property
     def config(self):
         """
@@ -74,14 +90,17 @@
             self._config = AsgardpyConfig(**value)
         elif isinstance(value, AsgardpyConfig):
             self._config = value
         else:
             raise TypeError("config must be dict or AsgardpyConfig.")
 
     def run(self, steps=None, overwrite=None, **kwargs):
+        """
+        Main function to run the AnalaysisSteps provided.
+        """
         if steps is None:
             steps = self.config.general.steps
             overwrite = self.config.general.overwrite
         else:
             if overwrite is None:
                 overwrite = True
 
@@ -100,52 +119,58 @@
                     # This step is only valid for 3D Datasets which have a list of models
                     target_source_model = models_list[self.config.target.source_name]
 
                     if target_source_model.spatial_model:
                         # If the target source has Spatial model included,
                         # only then (?) get all the models as final_model.
                         # Needs reconsideration.
-                        for m in models_list:
-                            self.final_model.append(m)
+                        for model_ in models_list:
+                            self.final_model.append(model_)
                     else:
                         self.log.info(
-                            f"The target source only has spectral model:{target_source_model}"
+                            "The target source %s only has spectral model",
+                            self.config.target.source_name,
                         )
 
                 # To get all datasets_names from the datasets and update the final datasets list
                 for data in datasets_list:
                     if data.name not in self.dataset_name_list:
                         self.dataset_name_list.append(data.name)
                     self.datasets.append(data)
 
-                # Update the name and spectral energy ranges for each
-                # instrument Datasets, to be used for the FluxPointsAnalysisStep.
+                # Update the name, DoF and spectral energy ranges for each
+                # instrument Datasets, to be used for the DL4 to DL5 processes.
                 for name in instrument_spectral_info["name"]:
                     self.instrument_spectral_info["name"].append(name)
 
                 for edges in instrument_spectral_info["spectral_energy_ranges"]:
                     self.instrument_spectral_info["spectral_energy_ranges"].append(edges)
 
-        self.datasets, self.final_model = set_models(
-            self.config.target,
-            self.datasets,
-            self.dataset_name_list,
-            models=self.final_model,
-        )
-
-        # Evaluate the total degree of freedom for the model fitting to the data
-        en_bins = 0
-        for data in self.datasets:
-            if data.mask:
-                en_bins += data.mask.geom.axes["energy"].nbin
-            else:
-                en_bins += data.counts.geom.axes["energy"].nbin
-
-        dof = en_bins + len(list(self.final_model.parameters.free_parameters))
-        self.instrument_spectral_info["DoF"] = dof
+                self.instrument_spectral_info["en_bins"] += instrument_spectral_info["en_bins"]
+                self.instrument_spectral_info["free_params"] += instrument_spectral_info[
+                    "free_params"
+                ]
+
+            self.datasets, self.final_model = set_models(
+                self.config.target,
+                self.datasets,
+                self.dataset_name_list,
+                models=self.final_model,
+            )
+            self.log.info("Models have been associated with the Datasets")
+
+            # Add to the total number of free model parameters
+            n_free_params = len(list(self.final_model.parameters.free_parameters))
+            self.instrument_spectral_info["free_params"] += n_free_params
+
+            # Get the final degrees of freedom as en_bins - free_params
+            self.instrument_spectral_info["DoF"] = (
+                self.instrument_spectral_info["en_bins"]
+                - self.instrument_spectral_info["free_params"]
+            )
 
         if len(dl4_dl5_steps) > 0:
             self.log.info("Perform DL4 to DL5 processes!")
 
             for step in dl4_dl5_steps:
                 analysis_step = AnalysisStep.create(step, self.config, **kwargs)
 
@@ -154,14 +179,20 @@
                 )
 
                 # Update the final data product objects
                 for data_product in self.final_data_products:
                     if hasattr(analysis_step, data_product):
                         setattr(self, data_product, getattr(analysis_step, data_product))
 
+        if self.fit_result:
+            self.instrument_spectral_info, message = get_goodness_of_fit_stats(
+                self.datasets, self.instrument_spectral_info
+            )
+            self.log.info(message)
+
     # keep these methods to be backward compatible
     def get_1d_dataset(self):
         """Produce stacked 1D datasets."""
         self.run(steps=["datasets-1d"])
 
     def get_3d_datasets(self):
         """Produce stacked 3D datasets."""
```

### Comparing `asgardpy-0.3.5/asgardpy/base/__init__.py` & `asgardpy-0.3.6/asgardpy/base/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,61 @@
+"""
+Base Module
+
+# order matters to prevent circular imports
+isort:skip_file
+"""
 from asgardpy.base.base import (
-    AnalysisStep,
-    AnalysisStepBase,
-    AnalysisStepEnum,
     AngleType,
     BaseConfig,
     EnergyRangeConfig,
     EnergyType,
     FrameEnum,
     PathType,
     TimeFormatEnum,
     TimeIntervalsConfig,
     TimeRangeConfig,
     TimeType,
 )
-from asgardpy.base.geom import (
-    EnergyAxisConfig,
-    EnergyEdgesCustomConfig,
-    GeomConfig,
-    MapAxesConfig,
-    MapFrameShapeConfig,
-    ProjectionEnum,
-    SelectionConfig,
-    SkyPositionConfig,
-    WcsConfig,
-    create_counts_map,
-    generate_geom,
-    get_energy_axis,
-    get_source_position,
-)
 from asgardpy.base.reduction import (
-    BackgroundConfig,
-    BackgroundMethodEnum,
-    ExclusionRegionsConfig,
-    MapSelectionEnum,
     ObservationsConfig,
     ReductionTypeEnum,
     RegionsConfig,
     RequiredHDUEnum,
+    BackgroundConfig,
+    BackgroundMethodEnum,
+    ExclusionRegionsConfig,
+    MapSelectionEnum,
     SafeMaskConfig,
     SafeMaskMethodsEnum,
     generate_dl4_dataset,
     get_bkg_maker,
     get_dataset_maker,
     get_dataset_reference,
     get_exclusion_region_mask,
     get_filtered_observations,
     get_safe_mask_maker,
 )
+from asgardpy.base.geom import (
+    MapAxesConfig,
+    MapFrameShapeConfig,
+    ProjectionEnum,
+    SelectionConfig,
+    SkyPositionConfig,
+    EnergyAxisConfig,
+    EnergyEdgesCustomConfig,
+    GeomConfig,
+    WcsConfig,
+    create_counts_map,
+    generate_geom,
+    get_energy_axis,
+    get_source_position,
+)
 
 __all__ = [
-    "AnalysisStep",
-    "AnalysisStepBase",
-    "AnalysisStepEnum",
     "AngleType",
     "BackgroundConfig",
     "BackgroundMethodEnum",
     "BaseConfig",
     "EnergyAxisConfig",
     "EnergyEdgesCustomConfig",
     "EnergyRangeConfig",
```

### Comparing `asgardpy-0.3.5/asgardpy/base/base.py` & `asgardpy-0.3.6/asgardpy/base/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 """
 Classes containing the Base for the Analysis steps and some Basic Config types.
 """
 
-import abc
-import logging
 from enum import Enum
 from pathlib import Path
 from typing import List
 
 from astropy import units as u
 from astropy.coordinates import Angle
 from astropy.time import Time
 from pydantic import BaseModel
 
 __all__ = [
-    "AnalysisStep",
-    "AnalysisStepBase",
-    "AnalysisStepEnum",
     "AngleType",
     "BaseConfig",
     "EnergyRangeConfig",
     "EnergyType",
     "FrameEnum",
     "PathType",
     "TimeFormatEnum",
@@ -28,47 +23,55 @@
     "TimeRangeConfig",
     "TimeType",
 ]
 
 
 # Basic Quantities Type for building the Config
 class AngleType(Angle):
+    """Base Angle Type Quantity"""
+
     @classmethod
     def __get_validators__(cls):
         yield cls.validate
 
     @classmethod
     def validate(cls, v):
         return Angle(v)
 
 
 class EnergyType(u.Quantity):
+    """Base Energy Type Quantity"""
+
     @classmethod
     def __get_validators__(cls):
         yield cls.validate
 
     @classmethod
     def validate(cls, v):
         v = u.Quantity(v)
         if v.unit.physical_type != "energy":
             raise ValueError(f"Invalid unit for energy: {v.unit!r}")
         return v
 
 
 class TimeType(Time):
+    """Base Time Type Quantity"""
+
     @classmethod
     def __get_validators__(cls):
         yield cls.validate
 
     @classmethod
     def validate(cls, v):
         return Time(v)
 
 
 class PathType(str):
+    """Base Path Type Quantity"""
+
     @classmethod
     def __get_validators__(cls):
         yield cls.validate
 
     @classmethod
     def validate(cls, v):
         if v == "None":
@@ -117,70 +120,14 @@
             Angle: lambda v: f"{v.value} {v.unit}",
             u.Quantity: lambda v: f"{v.value} {v.unit}",
             Time: lambda v: f"{v.value}",
             Path: lambda v: Path(v),
         }
 
 
-class AnalysisStepBase(abc.ABC):
-    """Config section for creating a basic AsgardpyAnalysis Step."""
-
-    tag = "analysis-step"
-
-    def __init__(self, config, log=None, overwrite=True):
-        self.config = config
-        self.overwrite = overwrite
-
-        self.datasets = None
-        self.instrument_spectral_info = None
-
-        if log is None:
-            log = logging.getLogger(__name__)
-            self.log = log
-
-    def run(self, datasets=None, instrument_spectral_info=None):
-        """
-        One can provide datasets and instrument_spectral_info to be used,
-        especially for the High-level Analysis steps.
-        """
-        self.datasets = datasets
-        self.instrument_spectral_info = instrument_spectral_info
-
-        final_product = self._run()
-        self.log.info(f"Analysis Step {self.tag} completed")
-
-        return final_product
-
-    @abc.abstractmethod
-    def _run(self):
-        pass
-
-
-class AnalysisStep:
-    """
-    Create one of the Analysis Step class listed in the Registry.
-    """
-
-    @staticmethod
-    def create(tag, config, **kwargs):
-        from asgardpy.data import ANALYSIS_STEP_REGISTRY
-
-        cls = ANALYSIS_STEP_REGISTRY.get_cls(tag)
-        return cls(config, **kwargs)
-
-
-class AnalysisStepEnum(str, Enum):
-    """Config section for list of Analysis Steps."""
-
-    datasets_1d = "datasets-1d"
-    datasets_3d = "datasets-3d"
-    fit = "fit"
-    flux_points = "flux-points"
-
-
 # Basic Quantity ranges Type for building the Config
 class TimeRangeConfig(BaseConfig):
     """
     Config section for getting a time range information for creating a Time
     object.
     """
```

### Comparing `asgardpy-0.3.5/asgardpy/base/geom.py` & `asgardpy-0.3.6/asgardpy/base/geom.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import List
 
 from astropy import units as u
 from astropy.coordinates import SkyCoord
 from gammapy.maps import Map, MapAxis, RegionGeom, WcsGeom
 from regions import CircleSkyRegion, PointSkyRegion
 
-from asgardpy.base import AngleType, BaseConfig, EnergyType, FrameEnum
+from asgardpy.base.base import AngleType, BaseConfig, EnergyType, FrameEnum
 
 __all__ = [
     "EnergyAxisConfig",
     "EnergyEdgesCustomConfig",
     "GeomConfig",
     "MapAxesConfig",
     "MapFrameShapeConfig",
@@ -228,15 +228,15 @@
     center_pos: dict
         Dict information on the central `astropy.coordinates.SkyCoord` position
         and `astropy.units.Quantity` angular radius.
 
     Return
     ------
     counts_map: `gammapy.maps.Map`
-        Map object of the Counts informatio.
+        Map object of the Counts information.
     """
     energy_axes = geom_config.axes[0]
     energy_axis = get_energy_axis(energy_axes)
     bin_size = geom_config.wcs.binsize.to_value(u.deg)
 
     # For fetching information from the events fits file to resize the Map size.
     if geom_config.from_events_file:
```

### Comparing `asgardpy-0.3.5/asgardpy/base/reduction.py` & `asgardpy-0.3.6/asgardpy/base/reduction.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,22 +23,16 @@
     RingBackgroundMaker,
     SafeMaskMaker,
     SpectrumDatasetMaker,
     WobbleRegionsFinder,
 )
 from regions import CircleAnnulusSkyRegion, CircleSkyRegion
 
-from asgardpy.base import (
-    AngleType,
-    BaseConfig,
-    PathType,
-    SkyPositionConfig,
-    TimeIntervalsConfig,
-)
-from asgardpy.base.geom import generate_geom, get_energy_axis
+from asgardpy.base.base import AngleType, BaseConfig, PathType, TimeIntervalsConfig
+from asgardpy.base.geom import SkyPositionConfig, generate_geom, get_energy_axis
 
 __all__ = [
     "BackgroundConfig",
     "BackgroundMethodEnum",
     "BackgroundRegionFinderMethodEnum",
     "ExclusionRegionsConfig",
     "generate_dl4_dataset",
@@ -270,15 +264,17 @@
             "lat": obs_cone.lat,
             "radius": obs_cone.radius,
             "border": 0 * u.deg,  # Default?
         }
         obs_table = obs_table.select_observations(cone_select)
 
     filtered_obs_ids = obs_table["OBS_ID"].data
-    log.info(f"Observation ID list selected: {filtered_obs_ids}")
+
+    obs_ids_str = " ".join(map(str, filtered_obs_ids))
+    log.info("Observation ID list selected: %s", obs_ids_str)
 
     # IRFs selection
     irfs_selected = obs_config.required_irfs
     observations = datastore.get_observations(filtered_obs_ids, required_irf=irfs_selected)
 
     return observations
 
@@ -358,15 +354,15 @@
     return dataset_maker
 
 
 def get_safe_mask_maker(safe_config):
     """
     Generate Safe mask reduction maker as per the given config information.
 
-    Paramters
+    Parameters
     ---------
     safe_config: `asgardpy.base.reduction.SafeMaskConfig`
         Config information to create `gammapy.makers.SafeMaskMaker` object.
 
     Return
     ------
     safe_maker: `gammapy.makers.SafeMaskMaker`
```

### Comparing `asgardpy-0.3.5/asgardpy/config/generator.py` & `asgardpy-0.3.6/asgardpy/config/generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,35 @@
+"""
+Main AsgardpyConfig Generator Module
+"""
 import json
 import logging
 from enum import Enum
 from pathlib import Path
 from typing import List
 
 import yaml
+from gammapy.modeling.models import Models
 from gammapy.utils.scripts import make_path, read_yaml
 from pydantic.utils import deep_update
 
-from asgardpy.base import AnalysisStepEnum, BaseConfig, PathType
+from asgardpy.analysis.step_base import AnalysisStepEnum
+from asgardpy.base import BaseConfig, PathType
 from asgardpy.data import (
     Dataset1DConfig,
     Dataset3DConfig,
     FitConfig,
     FluxPointsConfig,
     Target,
 )
 
 __all__ = [
     "AsgardpyConfig",
+    "GeneralConfig",
+    "gammapy_to_asgardpy_model_config",
     "get_model_template",
     "recursive_merge_dicts",
 ]
 
 CONFIG_PATH = Path(__file__).resolve().parent
 
 log = logging.getLogger(__name__)
@@ -58,61 +65,88 @@
     stacked_dataset: bool = False
 
 
 def get_model_template(spec_model_tag):
     """
     Read a particular template model yaml file into AsgardpyConfig object.
     """
-    template_files = sorted(list(CONFIG_PATH.glob("model_template*yaml")))
+    template_files = sorted(list(CONFIG_PATH.glob("model_templates/model_template*yaml")))
     new_model_file = None
     for file in template_files:
         if spec_model_tag == file.name.split("_")[-1].split(".")[0]:
             new_model_file = file
     return new_model_file
 
 
-def recursive_merge_dicts(a, b):
+def recursive_merge_dicts(base_config, extra_config):
     """
     recursively merge two dictionaries.
-    Entries in b override entries in a. The built-in update function cannot be
-    used for hierarchical dicts.
+    Entries in extra_config override entries in base_config. The built-in
+    update function cannot be used for hierarchical dicts.
 
-    Also for the case when there is a list of dicts involved, one has to be more careful.
+    Also for the case when there is a list of dicts involved, one has to be
+    more careful.
 
     Combined here are 2 options from SO.
 
     See:
     http://stackoverflow.com/questions/3232943/update-value-of-a-nested-dictionary-of-varying-depth/3233356#3233356
     and also
     https://stackoverflow.com/questions/3232943/update-value-of-a-nested-dictionary-of-varying-depth/18394648#18394648
 
     Parameters
     ----------
-    a : dict
+    base_config : dict
         dictionary to be merged
-    b : dict
+    extra_config : dict
         dictionary to be merged
     Returns
     -------
-    c : dict
+    final_config : dict
         merged dict
     """
-    c = a.copy()
-    for k, v in b.items():
-        if k in c and isinstance(c[k], list):
-            new_c = []
-            for cc, vv in zip(c[k], v):
-                cc = recursive_merge_dicts(cc or {}, vv)
-                new_c.append(cc)
-            c[k] = new_c
-        elif k in c and isinstance(c[k], dict):
-            c[k] = recursive_merge_dicts(c.get(k) or {}, v)
+    final_config = base_config.copy()
+    for key, value in extra_config.items():
+        if key in final_config and isinstance(final_config[key], list):
+            new_config = []
+            for key_, value_ in zip(final_config[key], value):
+                key_ = recursive_merge_dicts(key_ or {}, value_)
+                new_config.append(key_)
+            final_config[key] = new_config
+        elif key in final_config and isinstance(final_config[key], dict):
+            final_config[key] = recursive_merge_dicts(final_config.get(key) or {}, value)
         else:
-            c[k] = v
-    return c
+            final_config[key] = value
+    return final_config
+
+
+def gammapy_to_asgardpy_model_config(gammapy_model, asgardpy_config_file=None):
+    """
+    Read the Gammapy Models YAML file and save it as AsgardpyConfig object.
+
+    Return
+    ------
+    asgardpy_config: `asgardpy.config.generator.AsgardpyConfig`
+        Updated AsgardpyConfig object
+    """
+    models_gpy = Models.read(gammapy_model)
+
+    if not asgardpy_config_file:
+        asgardpy_config = AsgardpyConfig()  # Default object
+    elif isinstance(asgardpy_config_file, str):  # File path
+        asgardpy_config = AsgardpyConfig.read(asgardpy_config_file)
+    # also for YAML object?
+
+    models_gpy_dict = models_gpy.to_dict()
+    asgardpy_config_target_dict = asgardpy_config.dict()["target"]
+
+    temp_target_dict = recursive_merge_dicts(asgardpy_config_target_dict, models_gpy_dict)
+    asgardpy_config.target = temp_target_dict
+
+    return asgardpy_config
 
 
 # Combine everything!
 class AsgardpyConfig(BaseConfig):
     """
     Asgardpy analysis configuration, based on Gammapy Analysis Config.
     """
```

### Comparing `asgardpy-0.3.5/asgardpy/data/__init__.py` & `asgardpy-0.3.6/asgardpy/data/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,13 @@
-from gammapy.utils.registry import Registry
+"""
+Data Module
 
+# order matters to prevent circular imports
+isort:skip_file
+"""
 from asgardpy.data.dataset_1d import (
     Dataset1DConfig,
     Dataset1DGeneration,
     Datasets1DAnalysisStep,
 )
 from asgardpy.data.dataset_3d import (
     Dataset3DConfig,
@@ -17,33 +21,19 @@
     FluxPointsConfig,
 )
 from asgardpy.data.target import (
     BrokenPowerLaw2SpectralModel,
     ExpCutoffLogParabolaSpectralModel,
     Target,
     apply_selection_mask_to_models,
-    check_model_preference_aic,
-    check_model_preference_lrt,
     config_to_dict,
     create_gal_diffuse_skymodel,
     create_iso_diffuse_skymodel,
     create_source_skymodel,
-    get_chi2_pval,
     set_models,
-    xml_spatial_model_to_gammapy,
-    xml_spectral_model_to_gammapy_params,
-)
-
-ANALYSIS_STEP_REGISTRY = Registry(
-    [
-        Datasets1DAnalysisStep,
-        Datasets3DAnalysisStep,
-        FitAnalysisStep,
-        FluxPointsAnalysisStep,
-    ]
 )
 
 __all__ = [
     "BrokenPowerLaw2SpectralModel",
     "Dataset1DConfig",
     "Dataset1DGeneration",
     "Dataset3DConfig",
@@ -53,18 +43,13 @@
     "ExpCutoffLogParabolaSpectralModel",
     "FitAnalysisStep",
     "FitConfig",
     "FluxPointsAnalysisStep",
     "FluxPointsConfig",
     "Target",
     "apply_selection_mask_to_models",
-    "check_model_preference_aic",
-    "check_model_preference_lrt",
     "config_to_dict",
     "create_gal_diffuse_skymodel",
     "create_iso_diffuse_skymodel",
     "create_source_skymodel",
-    "get_chi2_pval",
     "set_models",
-    "xml_spatial_model_to_gammapy",
-    "xml_spectral_model_to_gammapy_params",
 ]
```

### Comparing `asgardpy-0.3.5/asgardpy/data/dataset_1d.py` & `asgardpy-0.3.6/asgardpy/data/dataset_1d.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,29 +8,30 @@
 
 import numpy as np
 from astropy import units as u
 
 # from gammapy.analysis import Analysis, AnalysisConfig - no support for DL3 with RAD_MAX
 from gammapy.datasets import Datasets
 
-from asgardpy.base import (
-    AnalysisStepBase,
-    BackgroundConfig,
-    BaseConfig,
+from asgardpy.analysis.step_base import AnalysisStepBase
+from asgardpy.base.base import BaseConfig
+from asgardpy.base.geom import (
     GeomConfig,
     MapAxesConfig,
-    MapSelectionEnum,
-    ObservationsConfig,
-    ReductionTypeEnum,
-    SafeMaskConfig,
     SkyPositionConfig,
+    generate_geom,
     get_energy_axis,
+    get_source_position,
 )
-from asgardpy.base.geom import generate_geom, get_source_position
 from asgardpy.base.reduction import (
+    BackgroundConfig,
+    MapSelectionEnum,
+    ObservationsConfig,
+    ReductionTypeEnum,
+    SafeMaskConfig,
     generate_dl4_dataset,
     get_bkg_maker,
     get_dataset_maker,
     get_dataset_reference,
     get_exclusion_region_mask,
     get_filtered_observations,
     get_safe_mask_maker,
@@ -88,19 +89,22 @@
     Dataset1DGeneration function.
     """
 
     tag = "datasets-1d"
 
     def _run(self):
         instruments_list = self.config.dataset1d.instruments
-        self.log.info(f"{len(instruments_list)} number of 1D Datasets given")
+        self.log.info("%d number of 1D Datasets given", len(instruments_list))
 
         datasets_1d_final = Datasets()
         instrument_spectral_info = {"name": [], "spectral_energy_ranges": []}
 
+        # Calculate the total number of reconstructed energy bins used
+        en_bins = 0
+
         # Iterate over all instrument information given:
         for i in np.arange(len(instruments_list)):
             config_1d_dataset = instruments_list[i]
             instrument_spectral_info["name"].append(config_1d_dataset.name)
 
             generate_1d_dataset = Dataset1DGeneration(self.log, config_1d_dataset, self.config)
             dataset = generate_1d_dataset.run()
@@ -114,19 +118,35 @@
                     energy_axes,
                     only_edges=True,
                 )
             instrument_spectral_info["spectral_energy_ranges"].append(energy_bin_edges)
 
             if self.config.general.stacked_dataset:
                 dataset = dataset.stack_reduce(name=config_1d_dataset.name)
+
+                if dataset.mask:
+                    en_bins += dataset.mask.geom.axes["energy"].nbin
+                else:
+                    en_bins += dataset.counts.geom.axes["energy"].nbin
+
                 datasets_1d_final.append(dataset)
             else:
                 for data in dataset:
+                    if data.mask:
+                        en_bins += data.mask.geom.axes["energy"].nbin
+                    else:
+                        en_bins += data.counts.geom.axes["energy"].nbin
+
                     datasets_1d_final.append(data)
 
+        instrument_spectral_info["en_bins"] = en_bins
+
+        # No linked model parameters or other free model parameters taken here
+        instrument_spectral_info["free_params"] = 0
+
         return (
             datasets_1d_final,
             None,
             instrument_spectral_info,
         )
 
 
@@ -155,23 +175,27 @@
         self.config_target = config_full.target
         self.n_jobs = config_full.general.n_jobs
         self.parallel_backend = config_full.general.parallel_backend
         self.exclusion_regions = []
         self.datasets = Datasets()
 
     def run(self):
+        """
+        Main function to run the creation of 1D dataset.
+        """
         # First check for the given file list if they are readable or not.
-        file_list = {}
         dl3_info = DL3Files(
             self.config_1d_dataset_io[0],
-            file_list,
             log=self.log,
         )
         dl3_info.list_dl3_files()
 
+        if len(dl3_info.events_files) == 0:
+            self.log.error("No DL3 files found at %s", dl3_info.dl3_path)
+
         # Applying all provided filters to get the Observations object
         observations = get_filtered_observations(
             dl3_path=self.config_1d_dataset_io[0].input_dir,
             obs_config=self.config_1d_dataset_info.observation,
             log=self.log,
         )
         # Get dict information of the ON region, with its SkyCoord position and angular radius
```

### Comparing `asgardpy-0.3.5/asgardpy/data/dataset_3d.py` & `asgardpy-0.3.6/asgardpy/data/dataset_3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,29 +21,31 @@
 from gammapy.modeling.models import (
     Models,
     PowerLawNormSpectralModel,
     SkyModel,
     TemplateSpatialModel,
 )
 
-from asgardpy.base import (
-    AnalysisStepBase,
-    BackgroundConfig,
-    BaseConfig,
+from asgardpy.analysis.step_base import AnalysisStepBase
+from asgardpy.base.base import BaseConfig
+from asgardpy.base.geom import (
     GeomConfig,
     MapAxesConfig,
-    MapSelectionEnum,
-    ObservationsConfig,
-    ReductionTypeEnum,
-    SafeMaskConfig,
     SkyPositionConfig,
+    create_counts_map,
+    generate_geom,
     get_energy_axis,
+    get_source_position,
 )
-from asgardpy.base.geom import create_counts_map, generate_geom, get_source_position
 from asgardpy.base.reduction import (
+    BackgroundConfig,
+    MapSelectionEnum,
+    ObservationsConfig,
+    ReductionTypeEnum,
+    SafeMaskConfig,
     generate_dl4_dataset,
     get_bkg_maker,
     get_dataset_maker,
     get_dataset_reference,
     get_exclusion_region_mask,
     get_filtered_observations,
     get_safe_mask_maker,
@@ -109,28 +111,36 @@
     Dataset3DGeneration function.
     """
 
     tag = "datasets-3d"
 
     def _run(self):
         instruments_list = self.config.dataset3d.instruments
-        self.log.info(f"{len(instruments_list)} number of 3D Datasets given")
+        self.log.info("%d number of 3D Datasets given", len(instruments_list))
 
         datasets_3d_final = Datasets()
         models_final = Models()
         instrument_spectral_info = {"name": [], "spectral_energy_ranges": []}
 
+        # Calculate the total number of reconstructed energy bins used
+        # and the number of linked model parameters to incorporate in the
+        # total number of free model parameters, for the final estimation of
+        # total number of degrees of freedom
+        free_params = 0
+        en_bins = 0
+
         # Iterate over all instrument information given:
         for i in np.arange(len(instruments_list)):
             config_3d_dataset = instruments_list[i]
             instrument_spectral_info["name"].append(config_3d_dataset.name)
 
             key_names = config_3d_dataset.dataset_info.key
             if len(key_names) > 0:
-                self.log.info(f"The different keys used: {key_names}")
+                keys_str = " ".join(map(str, key_names))
+                self.log.info("The different keys used: %s", keys_str)
             else:
                 key_names = [None]
                 self.log.info("No distinct keys used for the 3D dataset")
 
             # Extra Datasets object to differentiate between datasets obtained
             # from various "keys" of each instrument.
             dataset_instrument = Datasets()
@@ -164,14 +174,16 @@
                         diffuse_models_names.append(model_name)
 
                 if len(diffuse_models_names) > 1:
                     for model_name in diffuse_models_names[1:]:
                         models_final[diffuse_models_names[0]].spectral_model.model2 = models_final[
                             model_name
                         ].spectral_model.model2
+                        # For each linked model parameter, reduce the number of DoF
+                        free_params -= 1
             else:
                 models_final = None
 
             # Get the spectral energy information for each Instrument Dataset
             energy_axes = config_3d_dataset.dataset_info.spectral_energy_range
             if len(energy_axes.axis_custom.edges) > 0:
                 energy_bin_edges = get_energy_axis(energy_axes, only_edges=True, custom_range=True)
@@ -180,16 +192,23 @@
                     energy_axes,
                     only_edges=True,
                 )
 
             instrument_spectral_info["spectral_energy_ranges"].append(energy_bin_edges)
 
             for data in dataset_instrument:
+                if data.mask:
+                    en_bins += data.mask.geom.axes["energy"].nbin
+                else:
+                    en_bins += data.counts.geom.axes["energy"].nbin
                 datasets_3d_final.append(data)
 
+        instrument_spectral_info["free_params"] = free_params
+        instrument_spectral_info["en_bins"] = en_bins
+
         return datasets_3d_final, models_final, instrument_spectral_info
 
 
 class Dataset3DGeneration:
     """
     Class for 3D dataset creation based on the config or AsgardpyConfig
     information provided on the 3D dataset and the target source.
@@ -223,14 +242,17 @@
 
         # For updating the main config file with target source position
         # information if necessary.
         self.config_full = config_full
         self.config_target = config_full.target
 
     def run(self, key_name):
+        """
+        Main function to run the creation of 3D dataset.
+        """
         # First check for the given file list if they are readable or not.
         file_list = self.read_to_objects(key_name)
 
         self.load_events(file_list["events_file"])
         exclusion_regions = []
 
         if self.config_3d_dataset.io[0].type == "gadf-dl3":
@@ -260,26 +282,16 @@
 
             # If there is no explicit list of models provided for the 3D data,
             # one can use one of the several catalogs available in Gammapy.
             # Reading them as Models will keep the procedure uniform.
             if len(self.list_sources) == 0:
                 # Read the SkyModel info from AsgardpyConfig.target section
                 if len(self.config_target.components) > 0:
-                    spectral_model, spatial_model = read_models_from_asgardpy_config(
-                        self.config_target
-                    )
-                    self.list_sources.append(
-                        Models(
-                            SkyModel(
-                                spectral_model=spectral_model,
-                                spatial_model=spatial_model,
-                                name=self.config_target.source_name,
-                            )
-                        )
-                    )
+                    models_ = read_models_from_asgardpy_config(self.config_target)
+                    self.list_sources.append(models_)
 
                 # If a catalog information is provided, use it to build up the list of models
                 # Check if a catalog data is given with selection radius
                 if self.config_target.use_catalog.selection_radius != 0 * u.deg:
                     catalog = CATALOG_REGISTRY.get_cls(self.config_target.use_catalog.name)()
 
                     # One can also provide a separate file, but one has to add
@@ -436,19 +448,20 @@
         """
         For a DL3 files type and tag of the 'mode of observations' or key
         (FRONT/00 and BACK/01 for Fermi-LAT in enrico/fermipy files),
         read the files to appropriate Object type for further analysis.
 
         If there are no distinct key types of files, the value is None.
         """
-        dl3_info = DL3Files(dl3_dir_dict, file_list, log=self.log)
+        dl3_info = DL3Files(dl3_dir_dict, log=self.log)
         object_list = []
 
         if dl3_dir_dict.type.lower() in ["gadf-dl3"]:
-            file_list = dl3_info.list_dl3_files()
+            dl3_info.list_dl3_files()
+            file_list = dl3_info.events_files
 
             return file_list, object_list
         else:
             file_list = dl3_info.prepare_lat_files(key, file_list)
 
             if dl3_dir_dict.type.lower() in ["lat"]:
                 exposure = Map.read(file_list["expmap_file"])
@@ -467,27 +480,30 @@
     def get_list_objects(self, aux_path, xml_file):
         """
         Read from the XML file to enlist the various objects and get their
         SkyModels
 
         Currently assuming this to be applicable only for Fermi-LAT data.
         """
-        with open(xml_file) as file:
+        with open(xml_file, encoding="utf-8") as file:
             data = xmltodict.parse(file.read())["source_library"]["source"]
 
         is_target_source = False
         for source in data:
             source_name = source["@name"]
             if source_name in ["IsoDiffModel", "isodiff"]:
                 source = self.diffuse_models["iso_diffuse"]
             elif source_name in ["GalDiffModel", "galdiff"]:
                 source = create_gal_diffuse_skymodel(self.diffuse_models["gal_diffuse"])
             else:
                 source, is_target_source = create_source_skymodel(
-                    self.config_target, source, aux_path
+                    self.config_target,
+                    source,
+                    aux_path,
+                    base_model_type="Fermi-XML",
                 )
             if is_target_source:
                 self.list_sources.insert(0, source)
                 is_target_source = False  # To not let it repeat
             else:
                 self.list_sources.append(source)
```

### Comparing `asgardpy-0.3.5/asgardpy/data/dl4.py` & `asgardpy-0.3.6/asgardpy/data/dl4.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from enum import Enum
 
 from astropy import units as u
 from gammapy.datasets import Datasets
 from gammapy.estimators import FluxPointsEstimator
 from gammapy.modeling import Fit
 
-from asgardpy.base import AnalysisStepBase, BaseConfig, EnergyRangeConfig
-from asgardpy.data.target import get_chi2_pval
+from asgardpy.analysis.step_base import AnalysisStepBase
+from asgardpy.base import BaseConfig, EnergyRangeConfig
 
 __all__ = [
     "FitAnalysisStep",
     "FitConfig",
     "FluxPointsAnalysisStep",
     "FluxPointsConfig",
 ]
@@ -58,29 +58,15 @@
     def _run(self):
         self.fit_params = self.config.fit_params
 
         self._setup_fit()
         final_dataset = self._set_datasets()
         self.fit_result = self.fit.run(datasets=final_dataset)
 
-        self.instrument_spectral_info["total_stat"] = self.fit_result.total_stat
-
-        chi2_, pval_ = get_chi2_pval(
-            self.instrument_spectral_info["total_stat"], self.instrument_spectral_info["DoF"]
-        )
-        self.instrument_spectral_info["chi2"] = chi2_
-        self.instrument_spectral_info["p-value"] = pval_
-
-        stat_message = (
-            f'The Chi2/dof value of the Fit is {chi2_:.2f}/{self.instrument_spectral_info["DoF"]}'
-        )
-        stat_message += f"\nand the p-value is {pval_:.3e}"
-
         self.log.info(self.fit_result)
-        self.log.info(stat_message)
 
     def _setup_fit(self):
         """
         Setup the Gammapy Fit function with all the provided parameters from
         the config.
         """
         self.fit = Fit(
```

### Comparing `asgardpy-0.3.5/asgardpy/io/io.py` & `asgardpy-0.3.6/asgardpy/io/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,27 +46,27 @@
     glob_pattern: dict = {}
 
 
 # Main Classes for I/O
 class DL3Files:
     """
     A general class to retrieve information from given DL3 files, along with
-    other auxillary files for neighbouring sources, if provided.
+    other auxiliary files for neighbouring sources, if provided.
     """
 
-    def __init__(self, dir_dict, file_list, log=None):
+    def __init__(self, dir_dict, log=None):
         if not log:
             self._set_logging()
         else:
             self.log = log
 
         if Path(dir_dict.input_dir).exists():
             self.dl3_path = Path(dir_dict.input_dir)
         else:
-            self.log.error(f"{dir_dict.input_dir} is not a valid file location")
+            self.log.error("%s is not a valid file location", dir_dict.input_dir)
 
         self.dl3_type = dir_dict.type
         self._check_dl3_type()
 
         self.glob_dict = dir_dict.glob_pattern
 
         self.events_files = None
@@ -82,15 +82,15 @@
 
     def _set_logging(self):
         self.log = logging.getLogger(__name__)
         self.log.setLevel(logging.INFO)
 
     def _check_dl3_type(self):
         if self.dl3_type.lower() not in EXPECTED_DL3_RANGE:
-            self.log.error(f"{self.dl3_type} is not in the expected range for DL3 files")
+            self.log.error("%s is not in the expected range for DL3 files", self.dl3_type)
 
     def prepare_lat_files(self, key, file_list):
         """
         Prepare a list of LAT files following a particular key. If there are no
         distinct key types of files, the value is None.
         """
         # Try to combine LAT and LAT-AUX files
@@ -162,15 +162,17 @@
                     filtered = [K for K in getattr(self, _v) if key in str(K.name)]
                     assert len(filtered) == 1
                 except TypeError:
                     self.log.info("No distinct key provided, selecting the first file in the list")
                     setattr(self, _v.replace("_files", "_f"), getattr(self, _v)[0])
                 except Exception:
                     self.log.error(
-                        f"Variable self.{_v} does not contain one element after filtering by {key}"
+                        "Variable {%s} does not contain one element after filtering by {%s}",
+                        self._v,
+                        key,
                     )
                 else:
-                    self.log.info(f"Selecting the file with name containing {key}")
+                    self.log.info("Selecting the file with name containing %s", key)
                     setattr(self, _v.replace("_files", "_f"), filtered[0])
                 file_list[_v.replace("files", "file")] = getattr(self, _v.replace("_files", "_f"))
 
         return file_list
```

### Comparing `asgardpy-0.3.5/asgardpy.egg-info/PKG-INFO` & `asgardpy-0.3.6/asgardpy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: asgardpy
-Version: 0.3.5
+Version: 0.3.6
 Summary: Gammapy-based pipeline for easy joint analysis of different gamma-ray datasets
 Home-page: https://github.com/chaimain/asgardpy
-Download-URL: https://github.com/chaimain/asgardpy/archive/refs/tags/v0.3.1.tar.gz
+Download-URL: https://github.com/chaimain/asgardpy/archive/refs/tags/v0.3.6.tar.gz
 Author: Chaitanya Priyadarshi
 Author-email: chaitanya.p.astrphys@gmail.com
 License: Apache
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8106369.svg)](https://doi.org/10.5281/zenodo.8106369) ![PyPI](https://img.shields.io/pypi/v/asgardpy?label=pypi%20asgardpy) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](https://www.astropy.org/)
+# asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8106369.svg)](https://doi.org/10.5281/zenodo.8106369) ![PyPI](https://img.shields.io/pypi/v/asgardpy?label=pypi%20asgardpy) [![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7699/badge)](https://bestpractices.coreinfrastructure.org/projects/7699) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](https://www.astropy.org/)
+
 ## Analysis Software for GAmma-Ray Data in Python
 
 'User-friendly' configuration-centred pipeline built over [Gammapy](https://github.com/gammapy/gammapy) to allow for easy simultaneous analysis of various datasets of different formats.
 Example: 3D Fermi-LAT (with various source models in the Region of Interest stored in XML file) + 1D energy-dependent directional cuts MAGIC/LST [PointSkyRegion geometry for ON region] + 1D global directional cut VERITAS [CircleSkyRegion geometry for ON region].
 
 Follow the documentation at https://asgardpy.readthedocs.io/en/latest/ for the main functionality of this pipeline.
 Follow the [Gammapy v1.1](https://docs.gammapy.org/1.1/) documentation for understanding the core Gammapy objects.
```

### Comparing `asgardpy-0.3.5/asgardpy.egg-info/SOURCES.txt` & `asgardpy-0.3.6/asgardpy.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -9,21 +9,27 @@
 asgardpy.egg-info/PKG-INFO
 asgardpy.egg-info/SOURCES.txt
 asgardpy.egg-info/dependency_links.txt
 asgardpy.egg-info/requires.txt
 asgardpy.egg-info/top_level.txt
 asgardpy/analysis/__init__.py
 asgardpy/analysis/analysis.py
+asgardpy/analysis/step.py
+asgardpy/analysis/step_base.py
 asgardpy/base/__init__.py
 asgardpy/base/base.py
 asgardpy/base/geom.py
 asgardpy/base/reduction.py
 asgardpy/config/__init__.py
 asgardpy/config/generator.py
 asgardpy/data/__init__.py
 asgardpy/data/dataset_1d.py
 asgardpy/data/dataset_3d.py
 asgardpy/data/dl4.py
 asgardpy/data/target.py
+asgardpy/gammapy/__init__.py
+asgardpy/gammapy/interoperate_models.py
 asgardpy/io/__init__.py
 asgardpy/io/io.py
+asgardpy/stats/__init__.py
+asgardpy/stats/stats.py
 tests/test_basic.py
```

### Comparing `asgardpy-0.3.5/setup.py` & `asgardpy-0.3.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,19 +41,19 @@
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
     keywords="",
     url="https://github.com/chaimain/asgardpy",
-    download_url="https://github.com/chaimain/asgardpy/archive/refs/tags/v0.3.1.tar.gz",
+    download_url="https://github.com/chaimain/asgardpy/archive/refs/tags/v0.3.6.tar.gz",
     author="Chaitanya Priyadarshi",
     author_email="chaitanya.p.astrphys@gmail.com",
     license="Apache",
     packages=find_packages(
         exclude=["*.tests", "*.tests.*", "tests.*", "tests"],
     ),
     package_data={"asgardpy": ["py.typed"]},
     install_requires=read_requirements("requirements.txt"),
     extras_require={"dev": read_requirements("dev-requirements.txt")},
-    python_requires=">=3.10",
+    python_requires=">=3.11",
 )
```

