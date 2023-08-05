# Comparing `tmp/dpivsoft-0.2.6.tar.gz` & `tmp/dpivsoft-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpivsoft-0.2.6.tar", last modified: Sat Jun  3 13:41:54 2023, max compression
+gzip compressed data, was "dpivsoft-0.3.0.tar", last modified: Sat Aug  5 19:19:02 2023, max compression
```

## Comparing `dpivsoft-0.2.6.tar` & `dpivsoft-0.3.0.tar`

### file list

```diff
@@ -1,52 +1,55 @@
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2023-06-03 13:41:54.150883 dpivsoft-0.2.6/
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    35150 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/LICENSE.txt
--rw-rw-r--   0 jorge     (1000) jorge     (1000)       79 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/MANIFEST.in
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     3247 2023-06-03 13:41:54.150883 dpivsoft-0.2.6/PKG-INFO
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     2577 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/README.md
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2023-06-03 13:41:54.146882 dpivsoft-0.2.6/dpivsoft/
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    27256 2023-01-14 17:00:20.000000 dpivsoft-0.2.6/dpivsoft/Cl_DPIV.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    11533 2023-01-14 17:00:20.000000 dpivsoft-0.2.6/dpivsoft/Classes.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    40654 2023-06-03 13:34:49.000000 dpivsoft-0.2.6/dpivsoft/DPIV.py
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2023-06-03 13:41:54.146882 dpivsoft-0.2.6/dpivsoft/Examples/
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2023-06-03 13:41:54.146882 dpivsoft-0.2.6/dpivsoft/Examples/CFD/
--rw-rw-r--   0 jorge     (1000) jorge     (1000)  2160128 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/Examples/CFD/Mixing_Flow.npy
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     5235 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/Examples/Performance.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      338 2023-01-14 17:00:20.000000 dpivsoft-0.2.6/dpivsoft/Examples/Performance_parameters.yaml
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     5292 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/Examples/Tutorial_1.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      338 2023-01-14 17:00:20.000000 dpivsoft-0.2.6/dpivsoft/Examples/Tutorial_1_parameters.yaml
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2023-06-03 13:41:54.150883 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)    12288 2021-10-24 10:54:01.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.Jacobian.cl.swp
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)    12288 2021-12-06 11:16:20.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.deform_image.cl.swp
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)    12288 2022-11-26 11:46:07.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.directCorrelation.cl.swn
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)    12288 2022-11-26 11:05:39.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.directCorrelation.cl.swo
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)    12288 2022-11-26 10:54:56.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.directCorrelation.cl.swp
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)    16384 2022-11-26 15:22:43.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.find_peak.cl.swn
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)    16384 2021-10-15 18:39:27.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.find_peak.cl.swo
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)    20480 2021-10-14 10:16:50.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.find_peak.cl.swp
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)    12288 2021-12-10 16:30:18.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.gaussian_filter.cl.swp
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     1004 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/Jacobian.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      497 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/Normalize_Img.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      573 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/Slice.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      686 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/SubMean.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      689 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/Weighting.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      496 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/box_blur.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     2567 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/deform_image.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     2090 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/directCorrelation.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     6179 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/find_peak.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4341 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/find_peak_direct.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      976 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/gaussian_filter.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      271 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/ini_index.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      707 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/interpolation.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4001 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/median_filter.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      214 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/GPU_Kernels/multiply_them.cl
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    12471 2023-01-14 17:00:20.000000 dpivsoft-0.2.6/dpivsoft/SyIm.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)        0 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/__init__.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     8617 2022-12-03 15:03:54.000000 dpivsoft-0.2.6/dpivsoft/meshTools.py
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2023-06-03 13:41:54.146882 dpivsoft-0.2.6/dpivsoft.egg-info/
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)     3247 2023-06-03 13:41:53.000000 dpivsoft-0.2.6/dpivsoft.egg-info/PKG-INFO
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)     1437 2023-06-03 13:41:53.000000 dpivsoft-0.2.6/dpivsoft.egg-info/SOURCES.txt
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)        1 2023-06-03 13:41:53.000000 dpivsoft-0.2.6/dpivsoft.egg-info/dependency_links.txt
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)      159 2023-06-03 13:41:53.000000 dpivsoft-0.2.6/dpivsoft.egg-info/requires.txt
--rwxrwxrwx   0 jorge     (1000) jorge     (1000)        9 2023-06-03 13:41:53.000000 dpivsoft-0.2.6/dpivsoft.egg-info/top_level.txt
--rw-rw-r--   0 jorge     (1000) jorge     (1000)       38 2023-06-03 13:41:54.150883 dpivsoft-0.2.6/setup.cfg
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     1326 2023-06-03 13:34:49.000000 dpivsoft-0.2.6/setup.py
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2023-08-05 19:19:02.096069 dpivsoft-0.3.0/
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    35150 2022-12-03 15:03:54.000000 dpivsoft-0.3.0/LICENSE.txt
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)       79 2022-12-03 15:03:54.000000 dpivsoft-0.3.0/MANIFEST.in
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     3247 2023-08-05 19:19:02.096069 dpivsoft-0.3.0/PKG-INFO
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     2577 2023-08-05 18:53:47.000000 dpivsoft-0.3.0/README.md
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2023-08-05 19:19:02.092069 dpivsoft-0.3.0/dpivsoft/
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    27256 2023-08-05 17:39:16.000000 dpivsoft-0.3.0/dpivsoft/Cl_DPIV.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    12315 2023-08-05 19:15:58.000000 dpivsoft-0.3.0/dpivsoft/Classes.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    40654 2023-08-05 17:41:37.000000 dpivsoft-0.3.0/dpivsoft/DPIV.py
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2023-08-05 19:19:02.092069 dpivsoft-0.3.0/dpivsoft/Examples/
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2023-08-05 19:19:02.092069 dpivsoft-0.3.0/dpivsoft/Examples/CFD/
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)  2160128 2022-12-03 15:03:54.000000 dpivsoft-0.3.0/dpivsoft/Examples/CFD/Mixing_Flow.npy
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     5235 2022-12-03 15:03:54.000000 dpivsoft-0.3.0/dpivsoft/Examples/Performance.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      338 2023-01-14 17:00:20.000000 dpivsoft-0.3.0/dpivsoft/Examples/Performance_parameters.yaml
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     5317 2023-08-05 19:15:58.000000 dpivsoft-0.3.0/dpivsoft/Examples/simple_tutorial.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      338 2023-08-05 19:15:58.000000 dpivsoft-0.3.0/dpivsoft/Examples/simple_tutorial_parameters.yaml
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     6782 2023-08-05 19:15:58.000000 dpivsoft-0.3.0/dpivsoft/Examples/stereo_tutorial.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      391 2023-08-05 19:15:58.000000 dpivsoft-0.3.0/dpivsoft/Examples/stereo_tutorial_parameters.yaml
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2023-08-05 19:19:02.096069 dpivsoft-0.3.0/dpivsoft/GPU_Kernels/
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)    12288 2021-10-24 10:54:01.000000 dpivsoft-0.3.0/dpivsoft/GPU_Kernels/.Jacobian.cl.swp
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)    12288 2021-12-06 11:16:20.000000 dpivsoft-0.3.0/dpivsoft/GPU_Kernels/.deform_image.cl.swp
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)    12288 2022-11-26 11:46:07.000000 dpivsoft-0.3.0/dpivsoft/GPU_Kernels/.directCorrelation.cl.swn
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)    12288 2022-11-26 11:05:39.000000 dpivsoft-0.3.0/dpivsoft/GPU_Kernels/.directCorrelation.cl.swo
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)    12288 2022-11-26 10:54:56.000000 dpivsoft-0.3.0/dpivsoft/GPU_Kernels/.directCorrelation.cl.swp
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)    16384 2022-11-26 15:22:43.000000 dpivsoft-0.3.0/dpivsoft/GPU_Kernels/.find_peak.cl.swn
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)    16384 2021-10-15 18:39:27.000000 dpivsoft-0.3.0/dpivsoft/GPU_Kernels/.find_peak.cl.swo
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)    20480 2021-10-14 10:16:50.000000 dpivsoft-0.3.0/dpivsoft/GPU_Kernels/.find_peak.cl.swp
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)    12288 2021-12-10 16:30:18.000000 dpivsoft-0.3.0/dpivsoft/GPU_Kernels/.gaussian_filter.cl.swp
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     1004 2022-12-03 15:03:54.000000 dpivsoft-0.3.0/dpivsoft/GPU_Kernels/Jacobian.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      497 2022-12-03 15:03:54.000000 dpivsoft-0.3.0/dpivsoft/GPU_Kernels/Normalize_Img.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      573 2022-12-03 15:03:54.000000 dpivsoft-0.3.0/dpivsoft/GPU_Kernels/Slice.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      686 2022-12-03 15:03:54.000000 dpivsoft-0.3.0/dpivsoft/GPU_Kernels/SubMean.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      689 2022-12-03 15:03:54.000000 dpivsoft-0.3.0/dpivsoft/GPU_Kernels/Weighting.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      496 2022-12-03 15:03:54.000000 dpivsoft-0.3.0/dpivsoft/GPU_Kernels/box_blur.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     2567 2022-12-03 15:03:54.000000 dpivsoft-0.3.0/dpivsoft/GPU_Kernels/deform_image.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     2090 2022-12-03 15:03:54.000000 dpivsoft-0.3.0/dpivsoft/GPU_Kernels/directCorrelation.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     6179 2022-12-03 15:03:54.000000 dpivsoft-0.3.0/dpivsoft/GPU_Kernels/find_peak.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4341 2022-12-03 15:03:54.000000 dpivsoft-0.3.0/dpivsoft/GPU_Kernels/find_peak_direct.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      976 2022-12-03 15:03:54.000000 dpivsoft-0.3.0/dpivsoft/GPU_Kernels/gaussian_filter.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      271 2022-12-03 15:03:54.000000 dpivsoft-0.3.0/dpivsoft/GPU_Kernels/ini_index.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      707 2022-12-03 15:03:54.000000 dpivsoft-0.3.0/dpivsoft/GPU_Kernels/interpolation.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4001 2022-12-03 15:03:54.000000 dpivsoft-0.3.0/dpivsoft/GPU_Kernels/median_filter.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      214 2022-12-03 15:03:54.000000 dpivsoft-0.3.0/dpivsoft/GPU_Kernels/multiply_them.cl
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    12471 2023-01-14 17:00:20.000000 dpivsoft-0.3.0/dpivsoft/SyIm.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)        0 2022-12-03 15:03:54.000000 dpivsoft-0.3.0/dpivsoft/__init__.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     8617 2022-12-03 15:03:54.000000 dpivsoft-0.3.0/dpivsoft/meshTools.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    53072 2023-08-05 19:15:58.000000 dpivsoft-0.3.0/dpivsoft/stereo_DPIV.py
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2023-08-05 19:19:02.092069 dpivsoft-0.3.0/dpivsoft.egg-info/
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)     3247 2023-08-05 19:19:01.000000 dpivsoft-0.3.0/dpivsoft.egg-info/PKG-INFO
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)     1558 2023-08-05 19:19:01.000000 dpivsoft-0.3.0/dpivsoft.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)        1 2023-08-05 19:19:01.000000 dpivsoft-0.3.0/dpivsoft.egg-info/dependency_links.txt
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)      188 2023-08-05 19:19:01.000000 dpivsoft-0.3.0/dpivsoft.egg-info/requires.txt
+-rwxrwxrwx   0 jorge     (1000) jorge     (1000)        9 2023-08-05 19:19:01.000000 dpivsoft-0.3.0/dpivsoft.egg-info/top_level.txt
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)       38 2023-08-05 19:19:02.096069 dpivsoft-0.3.0/setup.cfg
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     1377 2023-08-05 19:15:58.000000 dpivsoft-0.3.0/setup.py
```

### Comparing `dpivsoft-0.2.6/LICENSE.txt` & `dpivsoft-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/PKG-INFO` & `dpivsoft-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpivsoft
-Version: 0.2.6
+Version: 0.3.0
 Summary: UNKNOWN
 Home-page: https://gitlab.com/jacabello/dpivsoft_python
 Author: Jorge Aguilar-Cabello
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dpivsoft-0.2.6/README.md` & `dpivsoft-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/Cl_DPIV.py` & `dpivsoft-0.3.0/dpivsoft/Cl_DPIV.py`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/Classes.py` & `dpivsoft-0.3.0/dpivsoft/Classes.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,88 +42,120 @@
     no_iter_2 = 2
 
     #Direct calculation or FFT
     direct_calc = 0  #1=direct; 0=FFT
 
     #default general parameters
     mask = 0
+    stereo = 0
     peak_ratio = 1
     weighting = 0
     gaussian_size = 0
     median_limit = 0.5
     calibration = 1
     delta_t = 1
 
     #Extra data needed in some cases
     class Data:
         #path of mask images
         path_mask = "none"
+        path_stereo = "none"
+
+    class Stereo_Calibration:
+        def __init__(self, npz_file):
+            self.load_variables(npz_file)
+
+        def load_variables(self, npz_file):
+            temp = np.load(npz_file)
+            self.a_l = temp['a_l']
+            self.b_l = temp['b_l']
+            self.a_r = temp['a_r']
+            self.b_r = temp['b_r']
+            self.theta_l = temp['theta_l']
+            self.theta_r = temp['theta_r']
+            self.beta_l = temp['beta_l']
+            self.beta_r = temp['beta_r']
 
     @classmethod
     def readParameters(self,fileName):
         """
         Read parameters from a yaml file
         """
         with open(fileName) as f:
             data = yaml.load(f, Loader=yaml.FullLoader)
+            print("starting")
 
-            try:
-                #Default first step parameters
-                self.box_size_1_x = data['box_size_1_x']
-                self.box_size_1_y = data['box_size_1_y']
-                self.no_boxes_1_x = data['no_boxes_1_x']
-                self.no_boxes_1_y = data['no_boxes_1_y']
-                self.window_1_x =   data['window_1_x']
-                self.window_1_y =   data['window_1_y']
-
-                #Number of pass of first step
-                self.no_iter_1 = data['no_iter_1']
-                self.no_iter_2 = data['no_iter_2']
-
-                #Direct calculation or FFT
-                self.direct_calc = data['direct_calc']
-
-                #Default first step parameters
-                self.box_size_2_x = data['box_size_2_x']
-                self.box_size_2_y = data['box_size_2_y']
-                self.no_boxes_2_x = data['no_boxes_2_x']
-                self.no_boxes_2_y = data['no_boxes_2_y']
-                self.window_2_x =   data['window_2_x']
-                self.window_2_y =   data['window_2_y']
+            #try:
+            #Default first step parameters
+            self.box_size_1_x = data['box_size_1_x']
+            self.box_size_1_y = data['box_size_1_y']
+            self.no_boxes_1_x = data['no_boxes_1_x']
+            self.no_boxes_1_y = data['no_boxes_1_y']
+            self.window_1_x =   data['window_1_x']
+            self.window_1_y =   data['window_1_y']
+
+            #Number of pass of first step
+            self.no_iter_1 = data['no_iter_1']
+            self.no_iter_2 = data['no_iter_2']
+
+            #Direct calculation or FFT
+            self.direct_calc = data['direct_calc']
+
+            #Default first step parameters
+            self.box_size_2_x = data['box_size_2_x']
+            self.box_size_2_y = data['box_size_2_y']
+            self.no_boxes_2_x = data['no_boxes_2_x']
+            self.no_boxes_2_y = data['no_boxes_2_y']
+            self.window_2_x =   data['window_2_x']
+            self.window_2_y =   data['window_2_y']
 
-                #default general parameters
-                self.mask = data['mask']
-                self.peak_ratio = data['peak_ratio']
-                self.weighting = data['weighting']
-                self.gaussian_size = data['gaussian_size']
-                self.median_limit = data['median_limit']
-                self.calibration = data['calibration']
-                self.delta_t = data['delta_t']
-
-                #Extra data
-                if self.mask:
-                    if data['path_mask'].endswith('.np'):
-                        self.Data.mask = bool(np.load(data['path_mask']))
-                    else:
-                        self.Data.mask = np.asarray(cv2.cvtColor(cv2.imread(
-                            data['path_mask']), cv2.COLOR_BGR2GRAY)).astype(bool)
+            #default general parameters
 
+            try:
+                self.mask = data['mask']
             except:
-                print('Error: Wrong parameters definition. Some Parameters'
-                      ' have been renamed in order to make them'
-                      ' more consistent with the matlab DPIVSoft version.'
-                      ' Please rename the following parameters as indicated:')
-                print(" - Window_axis_number --> window_number_axis")
-                print(" - gaussian_filter --> gaussian_size")
-                print(" - factor --> calibration")
-                print(" - dt --> delta_t")
-                print("You can also check the new parameters definition in "
-                        "Classes.py file or copy them from the examples. "
-                        "Sorry for the inconvenience.")
-                exit()
+                self.mask = 0
+            try:
+                self.stereo = data['stereo']
+            except:
+                self.stereo = 0
+
+            self.peak_ratio = data['peak_ratio']
+            self.weighting = data['weighting']
+            self.gaussian_size = data['gaussian_size']
+            self.median_limit = data['median_limit']
+            self.calibration = data['calibration']
+            self.delta_t = data['delta_t']
+
+            #Extra data
+            if self.mask:
+                if data['path_mask'].endswith('.np'):
+                    self.Data.mask = bool(np.load(data['path_mask']))
+                else:
+                    self.Data.mask = np.asarray(cv2.cvtColor(cv2.imread(
+                        data['path_mask']), cv2.COLOR_BGR2GRAY)).astype(bool)
+
+            if self.stereo:
+                self.stereo_calibration = self.Stereo_Calibration(
+                        data['path_stereo'])
+
+            #except:
+            #    print('Error: Wrong parameters definition. Some Parameters'
+            #          ' have been renamed in order to make them'
+            #          ' more consistent with the matlab DPIVSoft version.'
+            #          ' Please rename the following parameters as indicated:')
+            #    print(" - Window_axis_number --> window_number_axis")
+            #    print(" - gaussian_filter --> gaussian_size")
+            #    print(" - factor --> calibration")
+            #    print(" - dt --> delta_t")
+            #    print("You can also check the new parameters definition in "
+            #            "Classes.py file or copy them from the examples. "
+            #            "Sorry for the inconvenience.")
+            #    exit()
+
     def introParameters():
         """
         Introduce a parameter manually, not implemented yet (probably
         needed for a GUI)
         """
         pass
```

### Comparing `dpivsoft-0.2.6/dpivsoft/DPIV.py` & `dpivsoft-0.3.0/dpivsoft/DPIV.py`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/Examples/CFD/Mixing_Flow.npy` & `dpivsoft-0.3.0/dpivsoft/Examples/CFD/Mixing_Flow.npy`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/Examples/Performance.py` & `dpivsoft-0.3.0/dpivsoft/Examples/Performance.py`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/Examples/Tutorial_1.py` & `dpivsoft-0.3.0/dpivsoft/Examples/simple_tutorial.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 from dpivsoft.Classes  import GPU
 from dpivsoft.Classes  import Synt_Img
 
 #=============================================================================
 # WORKING FOLDERS
 #=============================================================================
 dirCode = os.getcwd()   #Current path
-dirImg = dirCode + "/Images/Tutorial_1"   #Images folder
-dirRes = dirCode + "/Results/Tutorial_1"  #Results folder
+dirImg = dirCode + "/Images/simple_tutorial"   #Images folder
+dirRes = dirCode + "/Results/simple_tutorial"  #Results folder
 
 if not os.path.exists(dirImg):
     os.makedirs(dirImg)
 if not os.path.exists(dirRes):
     os.makedirs(dirRes)
 
 #=============================================================================
@@ -56,15 +56,15 @@
 #=============================================================================
 # SET PIV PARAMETERS
 #=============================================================================
 # 1: Set parameters manually (see Classes.py for more details):
 Parameters.box_size_2_x = 32
 
 # 2: Arternateively parameters can be load from a file using readParamters():
-Parameters.readParameters(dirCode+'/Tutorial_1_parameters.yaml')
+Parameters.readParameters(dirCode+'/simple_tutorial_parameters.yaml')
 
 
 #=============================================================================
 # PYTHON PROCESSING
 #=============================================================================
 start = time.time()
 # Loop for load all images (only one in the example)
@@ -89,15 +89,15 @@
 
 #=============================================================================
 # OPENCL PROCESSING (The same but much faster)
 #=============================================================================
 
 # Select platform (only needed once). If more than one platform is installed
 # use "selection"
-thr = Cl_DPIV.select_Platform(0)
+thr = Cl_DPIV.select_Platform("selection")
 os.environ['PYOPENCL_COMPILER_OUTPUT'] = '1'
 
 # Load first pair of images to start the computation and set arrays sizes
 name_img_1 = dirImg+'/'+files[0]
 name_img_2 = dirImg+'/'+files[1]
 Img1, Img2 = DPIV.load_images(name_img_1, name_img_2)
 [height, width] = Img1.shape
```

### Comparing `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.Jacobian.cl.swp` & `dpivsoft-0.3.0/dpivsoft/GPU_Kernels/.Jacobian.cl.swp`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.deform_image.cl.swp` & `dpivsoft-0.3.0/dpivsoft/GPU_Kernels/.deform_image.cl.swp`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.directCorrelation.cl.swn` & `dpivsoft-0.3.0/dpivsoft/GPU_Kernels/.directCorrelation.cl.swn`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.directCorrelation.cl.swo` & `dpivsoft-0.3.0/dpivsoft/GPU_Kernels/.directCorrelation.cl.swo`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.directCorrelation.cl.swp` & `dpivsoft-0.3.0/dpivsoft/GPU_Kernels/.directCorrelation.cl.swp`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.find_peak.cl.swn` & `dpivsoft-0.3.0/dpivsoft/GPU_Kernels/.find_peak.cl.swn`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.find_peak.cl.swo` & `dpivsoft-0.3.0/dpivsoft/GPU_Kernels/.find_peak.cl.swo`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.find_peak.cl.swp` & `dpivsoft-0.3.0/dpivsoft/GPU_Kernels/.find_peak.cl.swp`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/.gaussian_filter.cl.swp` & `dpivsoft-0.3.0/dpivsoft/GPU_Kernels/.gaussian_filter.cl.swp`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/Jacobian.cl` & `dpivsoft-0.3.0/dpivsoft/GPU_Kernels/Jacobian.cl`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/Slice.cl` & `dpivsoft-0.3.0/dpivsoft/GPU_Kernels/Slice.cl`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/SubMean.cl` & `dpivsoft-0.3.0/dpivsoft/GPU_Kernels/SubMean.cl`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/Weighting.cl` & `dpivsoft-0.3.0/dpivsoft/GPU_Kernels/Weighting.cl`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/deform_image.cl` & `dpivsoft-0.3.0/dpivsoft/GPU_Kernels/deform_image.cl`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/directCorrelation.cl` & `dpivsoft-0.3.0/dpivsoft/GPU_Kernels/directCorrelation.cl`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/find_peak.cl` & `dpivsoft-0.3.0/dpivsoft/GPU_Kernels/find_peak.cl`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/find_peak_direct.cl` & `dpivsoft-0.3.0/dpivsoft/GPU_Kernels/find_peak_direct.cl`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/gaussian_filter.cl` & `dpivsoft-0.3.0/dpivsoft/GPU_Kernels/gaussian_filter.cl`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/interpolation.cl` & `dpivsoft-0.3.0/dpivsoft/GPU_Kernels/interpolation.cl`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/GPU_Kernels/median_filter.cl` & `dpivsoft-0.3.0/dpivsoft/GPU_Kernels/median_filter.cl`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/SyIm.py` & `dpivsoft-0.3.0/dpivsoft/SyIm.py`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft/meshTools.py` & `dpivsoft-0.3.0/dpivsoft/meshTools.py`

 * *Files identical despite different names*

### Comparing `dpivsoft-0.2.6/dpivsoft.egg-info/PKG-INFO` & `dpivsoft-0.3.0/dpivsoft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpivsoft
-Version: 0.2.6
+Version: 0.3.0
 Summary: UNKNOWN
 Home-page: https://gitlab.com/jacabello/dpivsoft_python
 Author: Jorge Aguilar-Cabello
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dpivsoft-0.2.6/dpivsoft.egg-info/SOURCES.txt` & `dpivsoft-0.3.0/dpivsoft.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 setup.py
 dpivsoft/Cl_DPIV.py
 dpivsoft/Classes.py
 dpivsoft/DPIV.py
 dpivsoft/SyIm.py
 dpivsoft/__init__.py
 dpivsoft/meshTools.py
+dpivsoft/stereo_DPIV.py
 dpivsoft.egg-info/PKG-INFO
 dpivsoft.egg-info/SOURCES.txt
 dpivsoft.egg-info/dependency_links.txt
 dpivsoft.egg-info/requires.txt
 dpivsoft.egg-info/top_level.txt
 dpivsoft/Examples/Performance.py
 dpivsoft/Examples/Performance_parameters.yaml
-dpivsoft/Examples/Tutorial_1.py
-dpivsoft/Examples/Tutorial_1_parameters.yaml
+dpivsoft/Examples/simple_tutorial.py
+dpivsoft/Examples/simple_tutorial_parameters.yaml
+dpivsoft/Examples/stereo_tutorial.py
+dpivsoft/Examples/stereo_tutorial_parameters.yaml
 dpivsoft/Examples/CFD/Mixing_Flow.npy
 dpivsoft/GPU_Kernels/.Jacobian.cl.swp
 dpivsoft/GPU_Kernels/.deform_image.cl.swp
 dpivsoft/GPU_Kernels/.directCorrelation.cl.swn
 dpivsoft/GPU_Kernels/.directCorrelation.cl.swo
 dpivsoft/GPU_Kernels/.directCorrelation.cl.swp
 dpivsoft/GPU_Kernels/.find_peak.cl.swn
```

### Comparing `dpivsoft-0.2.6/setup.py` & `dpivsoft-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = "dpivsoft",
-    version="0.2.6",
+    version="0.3.0",
     url="https://gitlab.com/jacabello/dpivsoft_python",
     author = "Jorge Aguilar-Cabello",
     python_requires=">=3.7",
     packages = find_packages(),
     include_package_data = True,
     long_description = long_description,
     long_description_content_type = "text/markdown",
     setup_requires=[
         'setuptools',
     ],
     install_requires = [
         'numpy>=1.3,<1.24.0',
         'reikna>=0.7.6',
         'scipy>=1.5',
+        'scikit-image>=0.20',
         'opencv-python>=4.5',
+        'Pillow>=9',
         'matplotlib>=3',
         'PyYAML>=5.4',
         'pyopencl>=2021',
         'Shapely>=1.7',
         'importlib_resources>=5',
     ],
     extras_require = {
```

