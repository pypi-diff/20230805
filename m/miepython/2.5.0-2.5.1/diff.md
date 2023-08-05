# Comparing `tmp/miepython-2.5.0.tar.gz` & `tmp/miepython-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miepython-2.5.0.tar", last modified: Fri Aug  4 18:51:01 2023, max compression
+gzip compressed data, was "miepython-2.5.1.tar", last modified: Sat Aug  5 21:12:04 2023, max compression
```

## Comparing `miepython-2.5.0.tar` & `miepython-2.5.1.tar`

### file list

```diff
@@ -1,61 +1,35 @@
-drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-04 18:51:01.672263 miepython-2.5.0/
-drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-04 18:51:01.642866 miepython-2.5.0/.github/
-drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-04 18:51:01.649114 miepython-2.5.0/.github/workflows/
--rw-r--r--   0 prahl      (501) staff       (20)      713 2022-01-27 02:10:04.000000 miepython-2.5.0/.github/workflows/test.yml
--rw-r--r--   0 prahl      (501) staff       (20)      164 2022-01-27 02:10:04.000000 miepython-2.5.0/.gitignore
--rw-r--r--   0 prahl      (501) staff       (20)      398 2021-08-16 19:03:47.000000 miepython-2.5.0/.readthedocs.yaml
--rw-r--r--   0 prahl      (501) staff       (20)       48 2022-01-26 16:03:16.000000 miepython-2.5.0/.testignore
--rw-r--r--   0 prahl      (501) staff       (20)     5698 2023-08-04 18:48:01.000000 miepython-2.5.0/CHANGELOG.rst
--rw-r--r--   0 prahl      (501) staff       (20)      328 2023-05-26 22:17:36.000000 miepython-2.5.0/CITATION.cff
--rw-r--r--   0 prahl      (501) staff       (20)     1055 2021-03-21 17:45:57.000000 miepython-2.5.0/LICENSE.txt
--rw-r--r--   0 prahl      (501) staff       (20)      161 2023-05-26 22:17:36.000000 miepython-2.5.0/MANIFEST.in
--rw-r--r--   0 prahl      (501) staff       (20)     1767 2023-06-10 21:55:43.000000 miepython-2.5.0/Makefile
--rw-r--r--   0 prahl      (501) staff       (20)     4094 2023-08-04 18:51:01.672703 miepython-2.5.0/PKG-INFO
--rw-r--r--   0 prahl      (501) staff       (20)     3314 2023-05-26 22:17:36.000000 miepython-2.5.0/README.rst
-drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-04 18:51:01.663404 miepython-2.5.0/docs/
--rw-r--r--   0 prahl      (501) staff       (20)   190191 2023-05-26 22:17:36.000000 miepython-2.5.0/docs/01_basics.ipynb
--rw-r--r--   0 prahl      (501) staff       (20)    34904 2021-01-18 22:54:10.000000 miepython-2.5.0/docs/01_plot.png
--rw-r--r--   0 prahl      (501) staff       (20)   123686 2023-05-26 22:17:36.000000 miepython-2.5.0/docs/02_efficiencies.ipynb
--rw-r--r--   0 prahl      (501) staff       (20)    47794 2021-01-18 22:55:06.000000 miepython-2.5.0/docs/02_plot.png
--rw-r--r--   0 prahl      (501) staff       (20)   478393 2022-01-30 19:54:28.000000 miepython-2.5.0/docs/03_angular_scattering.ipynb
--rw-r--r--   0 prahl      (501) staff       (20)    34095 2021-01-18 22:55:36.000000 miepython-2.5.0/docs/03_plot.png
--rw-r--r--   0 prahl      (501) staff       (20)   165954 2023-05-26 22:17:36.000000 miepython-2.5.0/docs/03a_normalization.ipynb
--rw-r--r--   0 prahl      (501) staff       (20)    54959 2022-03-13 17:44:50.000000 miepython-2.5.0/docs/04_plot.png
--rw-r--r--   0 prahl      (501) staff       (20)   133775 2021-04-25 22:33:21.000000 miepython-2.5.0/docs/04_rayleigh.ipynb
--rw-r--r--   0 prahl      (501) staff       (20)   264354 2021-04-25 22:33:21.000000 miepython-2.5.0/docs/05_fog.ipynb
--rw-r--r--   0 prahl      (501) staff       (20)    88000 2021-04-25 22:33:21.000000 miepython-2.5.0/docs/06_random_deviates.ipynb
--rw-r--r--   0 prahl      (501) staff       (20)    43928 2022-01-26 16:03:16.000000 miepython-2.5.0/docs/07_algorithm.ipynb
--rw-r--r--   0 prahl      (501) staff       (20)   565045 2021-04-25 22:33:21.000000 miepython-2.5.0/docs/08_large_spheres.ipynb
--rw-r--r--   0 prahl      (501) staff       (20)    33297 2021-04-25 22:33:21.000000 miepython-2.5.0/docs/09_backscattering.ipynb
--rw-r--r--   0 prahl      (501) staff       (20)    21271 2021-05-22 14:24:13.000000 miepython-2.5.0/docs/10_basic_tests.ipynb
--rw-r--r--   0 prahl      (501) staff       (20)   111396 2021-04-25 22:33:21.000000 miepython-2.5.0/docs/11_performance.ipynb
--rw-r--r--   0 prahl      (501) staff       (20)       29 2020-03-30 16:00:58.000000 miepython-2.5.0/docs/changelog.rst
--rw-r--r--   0 prahl      (501) staff       (20)     1953 2022-07-05 15:41:23.000000 miepython-2.5.0/docs/conf.py
--rw-r--r--   0 prahl      (501) staff       (20)     3113 2023-05-26 22:17:36.000000 miepython-2.5.0/docs/index.rst
--rw-r--r--   0 prahl      (501) staff       (20)      136 2022-01-27 02:10:43.000000 miepython-2.5.0/docs/miepython.rst
--rw-r--r--   0 prahl      (501) staff       (20)       76 2022-07-05 15:42:07.000000 miepython-2.5.0/docs/requirements.txt
-drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-04 18:51:01.664986 miepython-2.5.0/miepython/
--rw-r--r--   0 prahl      (501) staff       (20)     1498 2023-08-04 18:48:20.000000 miepython-2.5.0/miepython/__init__.py
-drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-04 18:51:01.669433 miepython-2.5.0/miepython/data/
--rw-r--r--   0 prahl      (501) staff       (20)     1337 2022-01-27 02:10:04.000000 miepython-2.5.0/miepython/data/Johnson.txt
--rw-r--r--   0 prahl      (501) staff       (20)     1337 2022-01-27 02:10:04.000000 miepython-2.5.0/miepython/data/ag-Johnson.txt
--rw-r--r--   0 prahl      (501) staff       (20)    36719 2022-01-27 02:10:04.000000 miepython-2.5.0/miepython/data/segelstein81_index.txt
-drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-04 18:51:01.671791 miepython-2.5.0/miepython/examples/
--rwxr-xr-x   0 prahl      (501) staff       (20)      684 2021-07-09 19:31:22.000000 miepython-2.5.0/miepython/examples/01_dielectric.py
--rwxr-xr-x   0 prahl      (501) staff       (20)      804 2021-07-09 19:33:51.000000 miepython-2.5.0/miepython/examples/02_glass.py
--rwxr-xr-x   0 prahl      (501) staff       (20)      921 2021-07-09 19:46:36.000000 miepython-2.5.0/miepython/examples/03_droplets.py
--rwxr-xr-x   0 prahl      (501) staff       (20)     2717 2022-03-12 23:14:57.000000 miepython-2.5.0/miepython/examples/04_gold.py
--rw-r--r--   0 prahl      (501) staff       (20)    28001 2023-08-04 18:43:45.000000 miepython-2.5.0/miepython/miepython.py
--rw-r--r--   0 prahl      (501) staff       (20)    25628 2023-08-04 18:17:11.000000 miepython-2.5.0/miepython/miepython_nojit.py
-drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-04 18:51:01.667904 miepython-2.5.0/miepython.egg-info/
--rw-r--r--   0 prahl      (501) staff       (20)     4094 2023-08-04 18:51:01.000000 miepython-2.5.0/miepython.egg-info/PKG-INFO
--rw-r--r--   0 prahl      (501) staff       (20)     1156 2023-08-04 18:51:01.000000 miepython-2.5.0/miepython.egg-info/SOURCES.txt
--rw-r--r--   0 prahl      (501) staff       (20)        1 2023-08-04 18:51:01.000000 miepython-2.5.0/miepython.egg-info/dependency_links.txt
--rw-r--r--   0 prahl      (501) staff       (20)       23 2023-08-04 18:51:01.000000 miepython-2.5.0/miepython.egg-info/requires.txt
--rw-r--r--   0 prahl      (501) staff       (20)       10 2023-08-04 18:51:01.000000 miepython-2.5.0/miepython.egg-info/top_level.txt
--rw-r--r--   0 prahl      (501) staff       (20)      569 2022-07-05 15:56:06.000000 miepython-2.5.0/pyproject.toml
--rw-r--r--   0 prahl      (501) staff       (20)      602 2022-03-12 18:25:05.000000 miepython-2.5.0/release.txt
--rw-r--r--   0 prahl      (501) staff       (20)      182 2021-05-22 21:35:05.000000 miepython-2.5.0/requirements-dev.txt
--rw-r--r--   0 prahl      (501) staff       (20)       22 2021-04-25 22:33:21.000000 miepython-2.5.0/requirements.txt
--rw-r--r--   0 prahl      (501) staff       (20)      986 2023-08-04 18:51:01.673884 miepython-2.5.0/setup.cfg
--rw-r--r--   0 prahl      (501) staff       (20)     1095 2022-03-12 23:40:23.000000 miepython-2.5.0/setup.py
+drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-05 21:12:04.819537 miepython-2.5.1/
+drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-05 21:12:04.808180 miepython-2.5.1/.github/
+drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-05 21:12:04.812775 miepython-2.5.1/.github/workflows/
+-rw-r--r--   0 prahl      (501) staff       (20)      762 2023-08-05 20:43:21.000000 miepython-2.5.1/.github/workflows/test.yml
+-rw-r--r--   0 prahl      (501) staff       (20)      164 2022-01-27 02:10:04.000000 miepython-2.5.1/.gitignore
+-rw-r--r--   0 prahl      (501) staff       (20)     5852 2023-08-05 20:59:04.000000 miepython-2.5.1/CHANGELOG.rst
+-rw-r--r--   0 prahl      (501) staff       (20)      328 2023-05-26 22:17:36.000000 miepython-2.5.1/CITATION.cff
+-rw-r--r--   0 prahl      (501) staff       (20)     1055 2021-03-21 17:45:57.000000 miepython-2.5.1/LICENSE.txt
+-rw-r--r--   0 prahl      (501) staff       (20)      314 2023-08-05 20:11:57.000000 miepython-2.5.1/MANIFEST.in
+-rw-r--r--   0 prahl      (501) staff       (20)     4246 2023-08-05 21:12:04.819795 miepython-2.5.1/PKG-INFO
+-rw-r--r--   0 prahl      (501) staff       (20)     3314 2023-05-26 22:17:36.000000 miepython-2.5.1/README.rst
+drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-05 21:12:04.814038 miepython-2.5.1/miepython/
+-rw-r--r--   0 prahl      (501) staff       (20)     1498 2023-08-05 19:47:53.000000 miepython-2.5.1/miepython/__init__.py
+drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-05 21:12:04.817303 miepython-2.5.1/miepython/data/
+-rw-r--r--   0 prahl      (501) staff       (20)     1337 2022-01-27 02:10:04.000000 miepython-2.5.1/miepython/data/Johnson.txt
+-rw-r--r--   0 prahl      (501) staff       (20)     1337 2022-01-27 02:10:04.000000 miepython-2.5.1/miepython/data/ag-Johnson.txt
+-rw-r--r--   0 prahl      (501) staff       (20)    36719 2022-01-27 02:10:04.000000 miepython-2.5.1/miepython/data/segelstein81_index.txt
+drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-05 21:12:04.819130 miepython-2.5.1/miepython/examples/
+-rwxr-xr-x   0 prahl      (501) staff       (20)      684 2021-07-09 19:31:22.000000 miepython-2.5.1/miepython/examples/01_dielectric.py
+-rwxr-xr-x   0 prahl      (501) staff       (20)      804 2021-07-09 19:33:51.000000 miepython-2.5.1/miepython/examples/02_glass.py
+-rwxr-xr-x   0 prahl      (501) staff       (20)      921 2021-07-09 19:46:36.000000 miepython-2.5.1/miepython/examples/03_droplets.py
+-rwxr-xr-x   0 prahl      (501) staff       (20)     2717 2022-03-12 23:14:57.000000 miepython-2.5.1/miepython/examples/04_gold.py
+-rw-r--r--   0 prahl      (501) staff       (20)    28001 2023-08-04 18:43:45.000000 miepython-2.5.1/miepython/miepython.py
+-rw-r--r--   0 prahl      (501) staff       (20)    25628 2023-08-04 18:17:11.000000 miepython-2.5.1/miepython/miepython_nojit.py
+drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-05 21:12:04.816269 miepython-2.5.1/miepython.egg-info/
+-rw-r--r--   0 prahl      (501) staff       (20)     4246 2023-08-05 21:12:04.000000 miepython-2.5.1/miepython.egg-info/PKG-INFO
+-rw-r--r--   0 prahl      (501) staff       (20)      635 2023-08-05 21:12:04.000000 miepython-2.5.1/miepython.egg-info/SOURCES.txt
+-rw-r--r--   0 prahl      (501) staff       (20)        1 2023-08-05 21:12:04.000000 miepython-2.5.1/miepython.egg-info/dependency_links.txt
+-rw-r--r--   0 prahl      (501) staff       (20)       23 2023-08-05 21:12:04.000000 miepython-2.5.1/miepython.egg-info/requires.txt
+-rw-r--r--   0 prahl      (501) staff       (20)       10 2023-08-05 21:12:04.000000 miepython-2.5.1/miepython.egg-info/top_level.txt
+-rw-r--r--   0 prahl      (501) staff       (20)      179 2023-08-05 20:38:12.000000 miepython-2.5.1/pyproject.toml
+-rw-r--r--   0 prahl      (501) staff       (20)      179 2023-08-05 20:42:09.000000 miepython-2.5.1/requirements-dev.txt
+-rw-r--r--   0 prahl      (501) staff       (20)       22 2021-04-25 22:33:21.000000 miepython-2.5.1/requirements.txt
+-rw-r--r--   0 prahl      (501) staff       (20)     1105 2023-08-05 21:12:04.820931 miepython-2.5.1/setup.cfg
+-rw-r--r--   0 prahl      (501) staff       (20)     1095 2022-03-12 23:40:23.000000 miepython-2.5.1/setup.py
```

### Comparing `miepython-2.5.0/.github/workflows/test.yml` & `miepython-2.5.1/.github/workflows/test.yml`

 * *Files 26% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 jobs:
   test:
     runs-on: ubuntu-latest
     name: Build and test
 
     strategy:
       matrix:
-        python-version: ['3.9']
+        python-version: ["3.9", "3.10", "3.11"]
     
     steps:
       - uses: actions/checkout@v2
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
@@ -26,8 +26,8 @@
       
       - name: Install package and dependencies
         run: |
           pip install -U pip setuptools wheel
           pip install -r requirements-dev.txt
         
       - name: Test with pytest
-        run: pytest -v --notebooks
+        run: python -m pytest tests/test_nojit.py tests/test_jit.py
```

### Comparing `miepython-2.5.0/CHANGELOG.rst` & `miepython-2.5.1/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+v2.5.1 (8/5/2023)
+-------------------
+*   change tests to accommodate conda-forge
+*   require python>=3.9 to accommodate latest numba
+*   get rid of tox
+
 v2.5.0 (8/4/2023)
 -------------------
 *   fix scattering function for very small spheres
 
 v2.4.0 (6/10/2023)
 -------------------
 *   add mie_phase_matrix() to calculate scattering (Mueller) matrix
```

### Comparing `miepython-2.5.0/LICENSE.txt` & `miepython-2.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `miepython-2.5.0/PKG-INFO` & `miepython-2.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: miepython
-Version: 2.5.0
+Version: 2.5.1
 Summary: Mie scattering of a plane wave by a sphere
 Home-page: https://github.com/scottprahl/miepython.git
 Author: Scott Prahl
 Author-email: scott.prahl@oit.edu
 License: MIT
 Keywords: mie,scattering,rainbow,droplet,backscatter,sphere,nanoparticle,sphere,cloud,phase function,efficiency,rayleigh,backscattering
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 miepython
 =========
 
 by Scott Prahl
```

### Comparing `miepython-2.5.0/README.rst` & `miepython-2.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `miepython-2.5.0/miepython/__init__.py` & `miepython-2.5.1/miepython/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     miepython.i_unpolarized(m, x, mu, norm='one')
 
 The scattering matrix
 
     miepython.mie_phase_matrix(m, x, mu)
 
 """
-__version__ = '2.5.0'
+__version__ = '2.5.1'
 __author__ = 'Scott Prahl'
 __email__ = 'scott.prahl@oit.edu'
 __copyright__ = 'Copyright 2017-23, Scott Prahl'
 __license__ = 'MIT'
 __url__ = 'https://github.com/scottprahl/miepython.git'
 
 from .miepython import *
```

### Comparing `miepython-2.5.0/miepython/data/Johnson.txt` & `miepython-2.5.1/miepython/data/Johnson.txt`

 * *Files identical despite different names*

### Comparing `miepython-2.5.0/miepython/data/ag-Johnson.txt` & `miepython-2.5.1/miepython/data/ag-Johnson.txt`

 * *Files identical despite different names*

### Comparing `miepython-2.5.0/miepython/data/segelstein81_index.txt` & `miepython-2.5.1/miepython/data/segelstein81_index.txt`

 * *Files identical despite different names*

### Comparing `miepython-2.5.0/miepython/examples/01_dielectric.py` & `miepython-2.5.1/miepython/examples/01_dielectric.py`

 * *Files identical despite different names*

### Comparing `miepython-2.5.0/miepython/examples/02_glass.py` & `miepython-2.5.1/miepython/examples/02_glass.py`

 * *Files identical despite different names*

### Comparing `miepython-2.5.0/miepython/examples/03_droplets.py` & `miepython-2.5.1/miepython/examples/03_droplets.py`

 * *Files identical despite different names*

### Comparing `miepython-2.5.0/miepython/examples/04_gold.py` & `miepython-2.5.1/miepython/examples/04_gold.py`

 * *Files identical despite different names*

### Comparing `miepython-2.5.0/miepython/miepython.py` & `miepython-2.5.1/miepython/miepython.py`

 * *Files identical despite different names*

### Comparing `miepython-2.5.0/miepython/miepython_nojit.py` & `miepython-2.5.1/miepython/miepython_nojit.py`

 * *Files identical despite different names*

### Comparing `miepython-2.5.0/miepython.egg-info/PKG-INFO` & `miepython-2.5.1/miepython.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: miepython
-Version: 2.5.0
+Version: 2.5.1
 Summary: Mie scattering of a plane wave by a sphere
 Home-page: https://github.com/scottprahl/miepython.git
 Author: Scott Prahl
 Author-email: scott.prahl@oit.edu
 License: MIT
 Keywords: mie,scattering,rainbow,droplet,backscatter,sphere,nanoparticle,sphere,cloud,phase function,efficiency,rayleigh,backscattering
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 miepython
 =========
 
 by Scott Prahl
```

### Comparing `miepython-2.5.0/setup.cfg` & `miepython-2.5.1/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	License :: OSI Approved :: MIT License
 	Intended Audience :: Science/Research
 	Programming Language :: Python
 	Topic :: Scientific/Engineering :: Physics
 	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 packages = miepython
 install_requires = 
 	numpy
 	matplotlib
 	numba
```

### Comparing `miepython-2.5.0/setup.py` & `miepython-2.5.1/setup.py`

 * *Files identical despite different names*

