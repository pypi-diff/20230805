# Comparing `tmp/optimal_data_selector-1.0.2.tar.gz` & `tmp/optimal_data_selector-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimal_data_selector-1.0.2.tar", last modified: Fri Jul 14 06:26:58 2023, max compression
+gzip compressed data, was "optimal_data_selector-1.0.3.tar", last modified: Sat Aug  5 16:19:03 2023, max compression
```

## Comparing `optimal_data_selector-1.0.2.tar` & `optimal_data_selector-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 06:26:58.473168 optimal_data_selector-1.0.2/
--rw-rw-rw-   0        0        0        0 2023-07-13 10:41:27.000000 optimal_data_selector-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      899 2023-07-14 06:26:58.471170 optimal_data_selector-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-14 06:26:58.329643 optimal_data_selector-1.0.2/optimal_data_selector/
--rw-rw-rw-   0        0        0        0 2023-07-13 09:41:50.000000 optimal_data_selector-1.0.2/optimal_data_selector/__init__.py
--rw-rw-rw-   0        0        0     9647 2023-07-13 14:26:26.000000 optimal_data_selector-1.0.2/optimal_data_selector/optimal.py
--rw-rw-rw-   0        0        0        0 2023-07-13 09:28:13.000000 optimal_data_selector-1.0.2/optimal_data_selector/optimal_2.py
-drwxrwxrwx   0        0        0        0 2023-07-14 06:26:58.456892 optimal_data_selector-1.0.2/optimal_data_selector.egg-info/
--rw-rw-rw-   0        0        0      899 2023-07-14 06:26:56.000000 optimal_data_selector-1.0.2/optimal_data_selector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-07-14 06:26:56.000000 optimal_data_selector-1.0.2/optimal_data_selector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 06:26:56.000000 optimal_data_selector-1.0.2/optimal_data_selector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-14 06:26:56.000000 optimal_data_selector-1.0.2/optimal_data_selector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 06:26:58.474167 optimal_data_selector-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1199 2023-07-14 06:23:11.000000 optimal_data_selector-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 16:19:03.560299 optimal_data_selector-1.0.3/
+-rw-rw-rw-   0        0        0        0 2023-07-13 10:41:27.000000 optimal_data_selector-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      951 2023-08-05 16:19:03.558299 optimal_data_selector-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-05 16:19:03.535323 optimal_data_selector-1.0.3/optimal_data_selector/
+-rw-rw-rw-   0        0        0        0 2023-07-13 09:41:50.000000 optimal_data_selector-1.0.3/optimal_data_selector/__init__.py
+-rw-rw-rw-   0        0        0     9647 2023-07-13 14:26:26.000000 optimal_data_selector-1.0.3/optimal_data_selector/optimal.py
+-rw-rw-rw-   0        0        0        0 2023-07-13 09:28:13.000000 optimal_data_selector-1.0.3/optimal_data_selector/optimal_2.py
+-rw-rw-rw-   0        0        0        0 2023-08-05 15:01:10.000000 optimal_data_selector-1.0.3/optimal_data_selector/word.py
+drwxrwxrwx   0        0        0        0 2023-08-05 16:19:03.555301 optimal_data_selector-1.0.3/optimal_data_selector.egg-info/
+-rw-rw-rw-   0        0        0      951 2023-08-05 16:19:03.000000 optimal_data_selector-1.0.3/optimal_data_selector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-08-05 16:19:03.000000 optimal_data_selector-1.0.3/optimal_data_selector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 16:19:03.000000 optimal_data_selector-1.0.3/optimal_data_selector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-08-05 16:19:03.000000 optimal_data_selector-1.0.3/optimal_data_selector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 16:19:03.560299 optimal_data_selector-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1253 2023-08-05 16:17:36.000000 optimal_data_selector-1.0.3/setup.py
```

### Comparing `optimal_data_selector-1.0.2/PKG-INFO` & `optimal_data_selector-1.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: optimal_data_selector
-Version: 1.0.2
-Summary: A function for selecting optimal data combinations
+Version: 1.0.3
+Summary: A Package for to optimize models
 Author: Rohan Majumder
 Author-email: majumderrohan2001@gmail.com
-Keywords: get_best_data_combination,optimise_accuracy,lock_data_combination,gives_best_result,best_data_for_ML_models,works on text data
+Keywords: get_best_data_combination,optimise_accuracy,lock_data_combination,gives_best_result,best_data_for_ML_models,works on text data also,short word treatment
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-A package to increase the accuracy of ML models, gives you the best data for model training, works on text data
+A package to increase the accuracy of ML models, gives you the best data for model training, works on text data also, short word treatment for NLP problems
```

### Comparing `optimal_data_selector-1.0.2/optimal_data_selector/optimal.py` & `optimal_data_selector-1.0.3/optimal_data_selector/optimal.py`

 * *Files identical despite different names*

### Comparing `optimal_data_selector-1.0.2/optimal_data_selector.egg-info/PKG-INFO` & `optimal_data_selector-1.0.3/optimal_data_selector.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: optimal-data-selector
-Version: 1.0.2
-Summary: A function for selecting optimal data combinations
+Version: 1.0.3
+Summary: A Package for to optimize models
 Author: Rohan Majumder
 Author-email: majumderrohan2001@gmail.com
-Keywords: get_best_data_combination,optimise_accuracy,lock_data_combination,gives_best_result,best_data_for_ML_models,works on text data
+Keywords: get_best_data_combination,optimise_accuracy,lock_data_combination,gives_best_result,best_data_for_ML_models,works on text data also,short word treatment
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-A package to increase the accuracy of ML models, gives you the best data for model training, works on text data
+A package to increase the accuracy of ML models, gives you the best data for model training, works on text data also, short word treatment for NLP problems
```

### Comparing `optimal_data_selector-1.0.2/setup.py` & `optimal_data_selector-1.0.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.0.2'
-DESCRIPTION = 'A function for selecting optimal data combinations'
-LONG_DESCRIPTION = 'A package to increase the accuracy of ML models, gives you the best data for model training, works on text data'
+VERSION = '1.0.3'
+DESCRIPTION = 'A Package for to optimize models'
+LONG_DESCRIPTION = 'A package to increase the accuracy of ML models, gives you the best data for model training, works on text data also, short word treatment for NLP problems'
 
 # Setting up
 setup(
     name="optimal_data_selector",
     version=VERSION,
     author="Rohan Majumder",
     author_email="majumderrohan2001@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
-    keywords=['get_best_data_combination', 'optimise_accuracy', 'lock_data_combination', 'gives_best_result', 'best_data_for_ML_models', 'works on text data'],
+    keywords=['get_best_data_combination', 'optimise_accuracy', 'lock_data_combination', 'gives_best_result', 'best_data_for_ML_models', 'works on text data also','short word treatment'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         "Operating System :: Unix",
```

