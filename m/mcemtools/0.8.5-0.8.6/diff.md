# Comparing `tmp/mcemtools-0.8.5.tar.gz` & `tmp/mcemtools-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcemtools-0.8.5.tar", last modified: Thu Aug  3 10:44:53 2023, max compression
+gzip compressed data, was "mcemtools-0.8.6.tar", last modified: Sat Aug  5 12:13:15 2023, max compression
```

## Comparing `mcemtools-0.8.5.tar` & `mcemtools-0.8.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:44:53.505726 mcemtools-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-03 10:44:41.000000 mcemtools-0.8.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-08-03 10:44:41.000000 mcemtools-0.8.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-08-03 10:44:41.000000 mcemtools-0.8.5/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 10:44:41.000000 mcemtools-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-03 10:44:41.000000 mcemtools-0.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-08-03 10:44:53.505726 mcemtools-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-08-03 10:44:41.000000 mcemtools-0.8.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:44:53.501726 mcemtools-0.8.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-03 10:44:41.000000 mcemtools-0.8.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-03 10:44:41.000000 mcemtools-0.8.5/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-08-03 10:44:41.000000 mcemtools-0.8.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-03 10:44:41.000000 mcemtools-0.8.5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-03 10:44:41.000000 mcemtools-0.8.5/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-03 10:44:41.000000 mcemtools-0.8.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-03 10:44:41.000000 mcemtools-0.8.5/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-03 10:44:41.000000 mcemtools-0.8.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-03 10:44:41.000000 mcemtools-0.8.5/docs/mcemtools.denoise.rst
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-03 10:44:41.000000 mcemtools-0.8.5/docs/mcemtools.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-03 10:44:41.000000 mcemtools-0.8.5/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-03 10:44:41.000000 mcemtools-0.8.5/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:44:53.505726 mcemtools-0.8.5/mcemtools/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-03 10:44:41.000000 mcemtools-0.8.5/mcemtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-08-03 10:44:41.000000 mcemtools-0.8.5/mcemtools/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-03 10:44:41.000000 mcemtools-0.8.5/mcemtools/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12490 2023-08-03 10:44:41.000000 mcemtools-0.8.5/mcemtools/masking.py
--rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-08-03 10:44:41.000000 mcemtools-0.8.5/mcemtools/mcemtools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-08-03 10:44:41.000000 mcemtools-0.8.5/mcemtools/tensor_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9992 2023-08-03 10:44:41.000000 mcemtools-0.8.5/mcemtools/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:44:53.505726 mcemtools-0.8.5/mcemtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-08-03 10:44:53.000000 mcemtools-0.8.5/mcemtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-03 10:44:53.000000 mcemtools-0.8.5/mcemtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 10:44:53.000000 mcemtools-0.8.5/mcemtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 10:44:53.000000 mcemtools-0.8.5/mcemtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 10:44:53.000000 mcemtools-0.8.5/mcemtools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-03 10:44:53.000000 mcemtools-0.8.5/mcemtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 10:44:53.000000 mcemtools-0.8.5/mcemtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-03 10:44:41.000000 mcemtools-0.8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-03 10:44:53.505726 mcemtools-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-03 10:44:41.000000 mcemtools-0.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:44:53.505726 mcemtools-0.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-03 10:44:41.000000 mcemtools-0.8.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-03 10:44:41.000000 mcemtools-0.8.5/tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-08-03 10:44:41.000000 mcemtools-0.8.5/tests/test_masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-03 10:44:41.000000 mcemtools-0.8.5/tests/test_mcemtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-08-03 10:44:41.000000 mcemtools-0.8.5/tests/test_tensor_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-08-03 10:44:41.000000 mcemtools-0.8.5/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:13:15.456030 mcemtools-0.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-05 12:13:06.000000 mcemtools-0.8.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-08-05 12:13:06.000000 mcemtools-0.8.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-08-05 12:13:06.000000 mcemtools-0.8.6/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-05 12:13:06.000000 mcemtools-0.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-05 12:13:06.000000 mcemtools-0.8.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-08-05 12:13:15.456030 mcemtools-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-08-05 12:13:06.000000 mcemtools-0.8.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:13:15.452030 mcemtools-0.8.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-05 12:13:06.000000 mcemtools-0.8.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-05 12:13:06.000000 mcemtools-0.8.6/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-08-05 12:13:06.000000 mcemtools-0.8.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-05 12:13:06.000000 mcemtools-0.8.6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-05 12:13:06.000000 mcemtools-0.8.6/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-05 12:13:06.000000 mcemtools-0.8.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-05 12:13:06.000000 mcemtools-0.8.6/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-05 12:13:06.000000 mcemtools-0.8.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-05 12:13:06.000000 mcemtools-0.8.6/docs/mcemtools.denoise.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-05 12:13:06.000000 mcemtools-0.8.6/docs/mcemtools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-05 12:13:06.000000 mcemtools-0.8.6/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-05 12:13:06.000000 mcemtools-0.8.6/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:13:15.452030 mcemtools-0.8.6/mcemtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-05 12:13:06.000000 mcemtools-0.8.6/mcemtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-08-05 12:13:06.000000 mcemtools-0.8.6/mcemtools/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-05 12:13:06.000000 mcemtools-0.8.6/mcemtools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12490 2023-08-05 12:13:06.000000 mcemtools-0.8.6/mcemtools/masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11652 2023-08-05 12:13:06.000000 mcemtools-0.8.6/mcemtools/mcemtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-08-05 12:13:06.000000 mcemtools-0.8.6/mcemtools/tensor_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9992 2023-08-05 12:13:06.000000 mcemtools-0.8.6/mcemtools/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:13:15.456030 mcemtools-0.8.6/mcemtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-08-05 12:13:15.000000 mcemtools-0.8.6/mcemtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-05 12:13:15.000000 mcemtools-0.8.6/mcemtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 12:13:15.000000 mcemtools-0.8.6/mcemtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-05 12:13:15.000000 mcemtools-0.8.6/mcemtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 12:13:15.000000 mcemtools-0.8.6/mcemtools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-05 12:13:15.000000 mcemtools-0.8.6/mcemtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-05 12:13:15.000000 mcemtools-0.8.6/mcemtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-05 12:13:06.000000 mcemtools-0.8.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-05 12:13:15.456030 mcemtools-0.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-05 12:13:06.000000 mcemtools-0.8.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:13:15.456030 mcemtools-0.8.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-05 12:13:06.000000 mcemtools-0.8.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-05 12:13:06.000000 mcemtools-0.8.6/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-08-05 12:13:06.000000 mcemtools-0.8.6/tests/test_masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-05 12:13:06.000000 mcemtools-0.8.6/tests/test_mcemtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-08-05 12:13:06.000000 mcemtools-0.8.6/tests/test_tensor_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-08-05 12:13:06.000000 mcemtools-0.8.6/tests/test_transforms.py
```

### Comparing `mcemtools-0.8.5/CONTRIBUTING.rst` & `mcemtools-0.8.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.5/HISTORY.rst` & `mcemtools-0.8.6/HISTORY.rst`

 * *Files 12% similar despite different names*

```diff
@@ -57,8 +57,12 @@
 
 0.8.4 (2023-07-28)
 ------------------
 * critical bug was fixed in viewer_4D
 
 0.8.5 (2023-08-03)
 ------------------
-* bug fixed in image_by_windows
+* bug fixed in image_by_windows
+
+0.8.6 (2023-08-05)
+------------------
+* viewer_4D handles arrows to move the selected objects.
```

### Comparing `mcemtools-0.8.5/LICENSE` & `mcemtools-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.5/PKG-INFO` & `mcemtools-0.8.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.8.5
+Version: 0.8.6
 Summary: State of the art analysis tools for electron microscopy
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -124,7 +124,11 @@
 0.8.4 (2023-07-28)
 ------------------
 * critical bug was fixed in viewer_4D
 
 0.8.5 (2023-08-03)
 ------------------
 * bug fixed in image_by_windows
+
+0.8.6 (2023-08-05)
+------------------
+* viewer_4D handles arrows to move the selected objects.
```

### Comparing `mcemtools-0.8.5/README.rst` & `mcemtools-0.8.6/README.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.5/docs/Makefile` & `mcemtools-0.8.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.5/docs/conf.py` & `mcemtools-0.8.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.5/docs/installation.rst` & `mcemtools-0.8.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.5/docs/make.bat` & `mcemtools-0.8.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.5/mcemtools/__init__.py` & `mcemtools-0.8.6/mcemtools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for mcemtools."""
 
 __author__ = """Alireza Sadri"""
 __email__ = 'Alireza.Sadri@monash.edu'
-__version__ = '0.8.5'
+__version__ = '0.8.6'
 
 from .analysis import pyMSSE, cross_correlation_4D, SymmSTEM
 from .analysis import centre_of_mass_4D, sum_4D
 
 from .masking import annular_mask, image_by_windows, markimage, mask2D_to_4D
 
 from .tensor_svd import svd_fit, svd_eval
```

### Comparing `mcemtools-0.8.5/mcemtools/analysis.py` & `mcemtools-0.8.6/mcemtools/analysis.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.5/mcemtools/masking.py` & `mcemtools-0.8.6/mcemtools/masking.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.5/mcemtools/mcemtools.py` & `mcemtools-0.8.6/mcemtools/mcemtools.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 import pathlib
 import matplotlib.pyplot as plt
 from lognflow import printprogress, select_directory, lognflow
 from .analysis import sum_4D, swirl_and_sum
 from .masking import mask2D_to_4D
+import time
 
 def locate_atoms(data4D, min_distance = 3, filter_size = 3,
                  reject_too_close = False):
     from skimage.feature import peak_local_max
     import scipy.ndimage
     _, _, n_r, n_c = data4D.shape
     image_max = scipy.ndimage.maximum_filter(
@@ -116,38 +117,39 @@
 
         self.data4D_shape = self.data4D.shape
         self.data4D_shape_list = np.array(self.data4D_shape)
         self.viewers_list = [napari.Viewer(), napari.Viewer()]
         STEM_img, PACBED = self.statistics_4D(self.data4D)
         self.viewers_list[0].add_image(PACBED)
         self.viewers_list[1].add_image(STEM_img)
-
-        self.viewers_list[0].bind_key(
-            key = 'i', func = self.print_shape_info)
-        self.viewers_list[1].bind_key(
-            key = 'i', func = self.print_shape_info)
-        
-        self.viewers_list[0].bind_key(
-            key = 'm', func = self.show_mask)
-        self.viewers_list[1].bind_key(
-            key = 'm', func = self.show_mask)
-        
-        self.viewers_list[0].bind_key(
-            key = 'F5', func = self.update_by_masked_sum_4D)
-        self.viewers_list[1].bind_key(
-            key = 'F5', func = self.update_by_masked_sum_4D)
-        self.viewers_list[0].mouse_drag_callbacks.append(self.mouse_drag_event)
-        self.viewers_list[1].mouse_drag_callbacks.append(self.mouse_drag_event)
+        
+        #, Down, Left, Right
+        for viewer_cnt in range(2):
+            self.viewers_list[viewer_cnt].bind_key(
+                key = 'Up', func = self.move_up)
+            self.viewers_list[viewer_cnt].bind_key(
+                key = 'Down', func = self.move_down)
+            self.viewers_list[viewer_cnt].bind_key(
+                key = 'Left', func = self.move_left)
+            self.viewers_list[viewer_cnt].bind_key(
+                key = 'Right', func = self.move_right)
+            self.viewers_list[viewer_cnt].bind_key(
+                key = 'i', func = self.print_shape_info)
+            self.viewers_list[viewer_cnt].bind_key(
+                key = 'm', func = self.show_mask)
+            self.viewers_list[viewer_cnt].bind_key(
+                key = 'F5', func = self.update_by_masked_sum_4D)
+            self.viewers_list[viewer_cnt].mouse_drag_callbacks.append(self.mouse_drag_event)
         
         self.mask2D_list = []
         self.mask2D_list.append(np.ones(
             (self.data4D_shape[2], self.data4D_shape[3]), dtype='int8'))
         self.mask2D_list.append(np.ones(
             (self.data4D_shape[0], self.data4D_shape[1]), dtype='int8'))
-        
+        self.move_perv_time_time = 0
         napari.run()
     
     def show_mask(self, viewer):
         self.update_by_masked_sum_4D(viewer)
         viewer_index = self.viewers_list.index(viewer)
         plt.figure(), plt.imshow(self.mask2D_list[viewer_index])
         plt.title(f'mask for viewer {viewer_index}'), plt.show()
@@ -230,8 +232,35 @@
             yield
         if dragged:
             self.update_by_masked_sum_4D(viewer)
             
     def print_shape_info(self, viewer):
         self.logger(f'shape_type:{viewer.layers[1].shape_type}')
         self.logger(f'data:{viewer.layers[1].data}')
-        self.logger(f'edge_width:{viewer.layers[1].edge_width}')
+        self.logger(f'edge_width:{viewer.layers[1].edge_width}')
+        
+    def move(self, viewer, axis, sign):
+        time_since_last_move = time.time() - self.move_perv_time_time
+        shape_cnt_list = list(viewer.layers[1].selected_data)
+        if shape_cnt_list:
+            cdata = []
+            for shape_cnt in shape_cnt_list:
+                _cdata = viewer.layers[1].data[int(shape_cnt)]
+                _cdata[:, axis] += sign
+                cdata.append(_cdata)
+            viewer.layers[1].data = cdata
+            selected_data = set()
+            for shape_cnt in shape_cnt_list:
+                selected_data.add(shape_cnt)
+            viewer.layers[1].selected_data = selected_data
+        if time_since_last_move > 0.5:
+            self.update_by_masked_sum_4D(viewer)
+            self.move_perv_time_time = time.time()
+
+    def move_up(self, viewer):
+        self.move(viewer, axis = 0, sign = -1)
+    def move_down(self, viewer):
+        self.move(viewer, axis = 0, sign = 1)
+    def move_left(self, viewer):
+        self.move(viewer, axis = 1, sign = -1)
+    def move_right(self, viewer):
+        self.move(viewer, axis = 1, sign = 1)
```

### Comparing `mcemtools-0.8.5/mcemtools/tensor_svd.py` & `mcemtools-0.8.6/mcemtools/tensor_svd.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.5/mcemtools/transforms.py` & `mcemtools-0.8.6/mcemtools/transforms.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.5/mcemtools.egg-info/PKG-INFO` & `mcemtools-0.8.6/mcemtools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.8.5
+Version: 0.8.6
 Summary: State of the art analysis tools for electron microscopy
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -124,7 +124,11 @@
 0.8.4 (2023-07-28)
 ------------------
 * critical bug was fixed in viewer_4D
 
 0.8.5 (2023-08-03)
 ------------------
 * bug fixed in image_by_windows
+
+0.8.6 (2023-08-05)
+------------------
+* viewer_4D handles arrows to move the selected objects.
```

### Comparing `mcemtools-0.8.5/mcemtools.egg-info/SOURCES.txt` & `mcemtools-0.8.6/mcemtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.5/setup.py` & `mcemtools-0.8.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-__version__ = '0.8.5'
+__version__ = '0.8.6'
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
```

### Comparing `mcemtools-0.8.5/tests/test_analysis.py` & `mcemtools-0.8.6/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.5/tests/test_masking.py` & `mcemtools-0.8.6/tests/test_masking.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.5/tests/test_mcemtools.py` & `mcemtools-0.8.6/tests/test_mcemtools.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.5/tests/test_tensor_svd.py` & `mcemtools-0.8.6/tests/test_tensor_svd.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.5/tests/test_transforms.py` & `mcemtools-0.8.6/tests/test_transforms.py`

 * *Files identical despite different names*

