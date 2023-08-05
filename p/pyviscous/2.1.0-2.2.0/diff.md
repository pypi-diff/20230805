# Comparing `tmp/pyviscous-2.1.0.tar.gz` & `tmp/pyviscous-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyviscous-2.1.0.tar", last modified: Mon Jul 24 17:40:11 2023, max compression
+gzip compressed data, was "pyviscous-2.2.0.tar", last modified: Sat Aug  5 06:23:17 2023, max compression
```

## Comparing `pyviscous-2.1.0.tar` & `pyviscous-2.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hongliliu   (501) staff       (20)        0 2023-07-24 17:40:11.383361 pyviscous-2.1.0/
--rw-r--r--   0 hongliliu   (501) staff       (20)     1603 2023-07-24 17:30:37.000000 pyviscous-2.1.0/LICENSE
--rw-r--r--   0 hongliliu   (501) staff       (20)     2637 2023-07-24 17:40:11.382907 pyviscous-2.1.0/PKG-INFO
--rw-r--r--   0 hongliliu   (501) staff       (20)     1842 2023-07-24 17:30:37.000000 pyviscous-2.1.0/README.md
-drwxr-xr-x   0 hongliliu   (501) staff       (20)        0 2023-07-24 17:40:11.379304 pyviscous-2.1.0/pyviscous/
--rwxr-xr-x   0 hongliliu   (501) staff       (20)       85 2023-07-24 17:30:37.000000 pyviscous-2.1.0/pyviscous/__init__.py
--rw-r--r--   0 hongliliu   (501) staff       (20)    24534 2023-07-24 17:30:37.000000 pyviscous-2.1.0/pyviscous/plot.py
--rwxr-xr-x   0 hongliliu   (501) staff       (20)    22344 2023-07-24 17:30:37.000000 pyviscous-2.1.0/pyviscous/pyviscous.py
-drwxr-xr-x   0 hongliliu   (501) staff       (20)        0 2023-07-24 17:40:11.382341 pyviscous-2.1.0/pyviscous.egg-info/
--rw-r--r--   0 hongliliu   (501) staff       (20)     2637 2023-07-24 17:40:11.000000 pyviscous-2.1.0/pyviscous.egg-info/PKG-INFO
--rw-r--r--   0 hongliliu   (501) staff       (20)      321 2023-07-24 17:40:11.000000 pyviscous-2.1.0/pyviscous.egg-info/SOURCES.txt
--rw-r--r--   0 hongliliu   (501) staff       (20)        1 2023-07-24 17:40:11.000000 pyviscous-2.1.0/pyviscous.egg-info/dependency_links.txt
--rw-r--r--   0 hongliliu   (501) staff       (20)       49 2023-07-24 17:40:11.000000 pyviscous-2.1.0/pyviscous.egg-info/entry_points.txt
--rw-r--r--   0 hongliliu   (501) staff       (20)        1 2023-07-24 17:40:11.000000 pyviscous-2.1.0/pyviscous.egg-info/not-zip-safe
--rw-r--r--   0 hongliliu   (501) staff       (20)       59 2023-07-24 17:40:11.000000 pyviscous-2.1.0/pyviscous.egg-info/requires.txt
--rw-r--r--   0 hongliliu   (501) staff       (20)       10 2023-07-24 17:40:11.000000 pyviscous-2.1.0/pyviscous.egg-info/top_level.txt
--rw-r--r--   0 hongliliu   (501) staff       (20)       38 2023-07-24 17:40:11.383491 pyviscous-2.1.0/setup.cfg
--rwxr-xr-x   0 hongliliu   (501) staff       (20)     1697 2023-07-24 17:37:16.000000 pyviscous-2.1.0/setup.py
+drwxr-xr-x   0 hongliliu   (501) staff       (20)        0 2023-08-05 06:23:17.808021 pyviscous-2.2.0/
+-rw-r--r--   0 hongliliu   (501) staff       (20)     1603 2023-07-24 17:30:37.000000 pyviscous-2.2.0/LICENSE
+-rw-r--r--   0 hongliliu   (501) staff       (20)     4257 2023-08-05 06:23:17.807793 pyviscous-2.2.0/PKG-INFO
+-rw-r--r--   0 hongliliu   (501) staff       (20)     3442 2023-08-05 06:20:06.000000 pyviscous-2.2.0/README.md
+drwxr-xr-x   0 hongliliu   (501) staff       (20)        0 2023-08-05 06:23:17.805056 pyviscous-2.2.0/pyviscous/
+-rwxr-xr-x   0 hongliliu   (501) staff       (20)       85 2023-07-24 17:30:37.000000 pyviscous-2.2.0/pyviscous/__init__.py
+-rw-r--r--   0 hongliliu   (501) staff       (20)    24534 2023-07-24 17:30:37.000000 pyviscous-2.2.0/pyviscous/plot.py
+-rwxr-xr-x   0 hongliliu   (501) staff       (20)    22322 2023-08-05 05:24:23.000000 pyviscous-2.2.0/pyviscous/pyviscous.py
+drwxr-xr-x   0 hongliliu   (501) staff       (20)        0 2023-08-05 06:23:17.807302 pyviscous-2.2.0/pyviscous.egg-info/
+-rw-r--r--   0 hongliliu   (501) staff       (20)     4257 2023-08-05 06:23:17.000000 pyviscous-2.2.0/pyviscous.egg-info/PKG-INFO
+-rw-r--r--   0 hongliliu   (501) staff       (20)      321 2023-08-05 06:23:17.000000 pyviscous-2.2.0/pyviscous.egg-info/SOURCES.txt
+-rw-r--r--   0 hongliliu   (501) staff       (20)        1 2023-08-05 06:23:17.000000 pyviscous-2.2.0/pyviscous.egg-info/dependency_links.txt
+-rw-r--r--   0 hongliliu   (501) staff       (20)       49 2023-08-05 06:23:17.000000 pyviscous-2.2.0/pyviscous.egg-info/entry_points.txt
+-rw-r--r--   0 hongliliu   (501) staff       (20)        1 2023-07-24 17:40:11.000000 pyviscous-2.2.0/pyviscous.egg-info/not-zip-safe
+-rw-r--r--   0 hongliliu   (501) staff       (20)       59 2023-08-05 06:23:17.000000 pyviscous-2.2.0/pyviscous.egg-info/requires.txt
+-rw-r--r--   0 hongliliu   (501) staff       (20)       10 2023-08-05 06:23:17.000000 pyviscous-2.2.0/pyviscous.egg-info/top_level.txt
+-rw-r--r--   0 hongliliu   (501) staff       (20)       38 2023-08-05 06:23:17.808098 pyviscous-2.2.0/setup.cfg
+-rwxr-xr-x   0 hongliliu   (501) staff       (20)     1985 2023-08-05 06:21:35.000000 pyviscous-2.2.0/setup.py
```

### Comparing `pyviscous-2.1.0/LICENSE` & `pyviscous-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyviscous-2.1.0/PKG-INFO` & `pyviscous-2.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,46 @@
-Metadata-Version: 2.1
-Name: pyviscous
-Version: 2.1.0
-Summary: Python codes to implement the VISCOUSm global sensitivity analysis framework
-Home-page: https://github.com/CH-Earth/pyviscous
-Author: Hongli Liu
-Author-email: hongliliu68@gmail.com
-License: GNU General Public License v3
-Keywords: pyviscous
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ### Abstract
-pyVISCOUS is the open-source code of VISCOUS in Python. VISCOUS (VarIance-based Sensitivity analysis using COpUlaS) is a variance-based global sensitivity analysis framework. It was developed by Sheikholeslami et al. ([2021](https://doi.org/10.1029/2020WR028435)) and improved by Liu et al. (2023).The advantage of VISCOUS is that it can use existing model input-output data (e.g., water model parameters-responses) to estimate the first- and total-order Sobol’ sensitivity indices. 
+pyVISCOUS is the open-source code of VISCOUS in Python. VISCOUS (VarIance-based Sensitivity analysis using COpUlaS) is a variance-based global sensitivity analysis framework. It was developed by Sheikholeslami et al. ([2021](https://doi.org/10.1029/2020WR028435)) and improved by Liu et al. (2023).
+
+
+As a “given-data” method, VISCOUS uses existing model input and output data (e.g., model parameters and responses) to provide useful approximations of the first- and total-order Sobol’ sensitivity indices. The greatest advantage of VISCOUS over other given-data global sensitivity analysis methods is that VISCOUS does not require the input data follow any specific sampling strategies. The input-output data can be from the previous model runs generated from other modeling purposes, such as uncertainty propagation and model calibration.
+
 
 Within the VISCOUS framework, the following steps are included. Details can be found in Liu et al. (2023).
 
 ![flowchart](https://github.com/CH-Earth/pyviscous/assets/48458815/2e8f7575-41d4-4e6a-bac8-fadc2a5b9c7a)
 
-### Installation
-#### From PyPI
-```pip install pyviscous```
+### Install pyviscous
+**From PyPI**: ```pip install pyviscous```
 
-#### From source
+**From source**:
 
 Clone pyviscous with: ```git clone https://github.com/CH-Earth/pyviscous.git```
 
 Then navigate to the pyviscous directory and install with: ```python setup.py install```
 
+### Do not want to install pyviscous
+If you do not want to install pyviscous, you can still use it by adding the pyviscous source code to the system path. For example,
+
+```
+import sys
+sys.path.insert(<path_to_directory>)
+import pyviscous
+```
+
+<path_to_directory> is the path to the folder where the pyviscous repository is located on your computer. The first two lines add the path of the repository directory to the system path so that Python can also look for the package in that directory if it doesn’t find it in its current directory. 
+
+**Important note**: To use pyviscous in this way, please make sure that you have installed all the required Python packages listed in setup.py file (i.e., *numpy*, *pandas*, *scipy*, *scikit-learn*, *copulae*, *matplotlib*, *jupyter*). Please install copulae via pip, not conda. This is because the conda distribution of copulae does not properly include its full source code/functions. We will remind the developer of copulae to fix this. 
+
 ### Examples
 We provide four example notebooks in the example directory. In each example, there are scripts to generate input-output data, set up and run VISCOUS, and evaluate the sensitivity results.
 
+### How to cite pyVISCOUS code
+Hongli Liu, Martyn P. Clark, Shervan Gharari, Razi Sheikholeslami, Jim Freer, Wouter J. M. Knoben, Christopher B. Marsh, & Simon Michael Papalexiou. (2023). pyVISCOUS. Zenodo. https://doi.org/10.5281/zenodo.8179325
+
 ### References
-Liu, H., Clark, M. P., Gharari, S., Sheikholeslami, R., Knoben, W. J. M., Freer, J., Marsh C. B., & Papalexiou, S. M. (2023) pyVISCOUS: An open-source tool for computationally frugal global sensitivity analysis. (Submitted to Water Resources Research)
+Liu, H., Clark, M. P., Gharari, S., Sheikholeslami, R., Freer, J., Knoben, W. J. M., Marsh C. B., & Papalexiou, S. M. (2023) pyVISCOUS: An open-source tool for computationally frugal global sensitivity analysis. (Submitted to Water Resources Research)
 
 Sheikholeslami, R., Gharari, S., Papalexiou, S. M., & Clark, M. P. (2021) VISCOUS: A variance-based sensitivity analysis using copulas for efficient identification of dominant hydrological processes. Water Resources Research, 57, e2020WR028435, https://doi.org/10.1029/2020WR028435
 
 ---
 This package was created with Cookiecutter and the `https://github.com/audreyr/cookiecutter-pypackage` project template.
```

### Comparing `pyviscous-2.1.0/pyviscous/plot.py` & `pyviscous-2.2.0/pyviscous/plot.py`

 * *Files identical despite different names*

### Comparing `pyviscous-2.1.0/pyviscous/pyviscous.py` & `pyviscous-2.2.0/pyviscous/pyviscous.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,20 +197,20 @@
         while trial_id <= trial_max:
             
             # Initialize gmcm params
             n_clusters, n_dim = int(n_component), int(n_xvariables+1)              
             if trial_id==1:
                 try:
                     fit_summary = k_means(data, n_clusters, n_dim, ties='average',init='k-means++')
-                except ValueError:
+                except:
                     pass
             else:
                 try:
                     fit_summary = k_means(data, n_clusters, n_dim,  ties='average',init='random')
-                except ValueError:
+                except:
                     pass
             
             # If fit_summary is obtained, pass it to param_init. Otherwise, move to the next trial.
             try:
                 param_init = fit_summary.best_params
             except:
                 print('\tinitial %d: fitting fails due to k_means initialization ValueError.'%(trial_id))
```

### Comparing `pyviscous-2.1.0/setup.py` & `pyviscous-2.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,17 @@
     from setuptools import setup
 except:
     from distutils.core import setup
 
 from setuptools import find_packages
 
 requirements = ['numpy', 'pandas', 'scipy', 'scikit-learn', 'copulae', 'matplotlib', 'jupyter']
+# Important note: if users install the above required packages by themselves, please install copulae via pip, not conda. 
+# This is because the conda distribution of copulae does not properly include its full source code/functions. 
+# We will remind the developer of copulae to fix this.
 
 test_requirements = [ ]
 
 # read the contents of your README file for distribution on PyPI
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
@@ -43,14 +46,14 @@
     include_package_data=True,
     keywords='pyviscous',
     name='pyviscous',
     packages=find_packages(include=['pyviscous', 'pyviscous.*', 'plot.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/CH-Earth/pyviscous',
-    version='2.1.0',
+    version='2.2.0',
     zip_safe=False,
     long_description=long_description,
     long_description_content_type='text/markdown',
 )
```

