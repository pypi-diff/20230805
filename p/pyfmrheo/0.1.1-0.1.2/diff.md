# Comparing `tmp/pyfmrheo-0.1.1.tar.gz` & `tmp/pyfmrheo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfmrheo-0.1.1.tar", last modified: Thu Jul 27 11:24:44 2023, max compression
+gzip compressed data, was "pyfmrheo-0.1.2.tar", last modified: Sat Aug  5 18:40:33 2023, max compression
```

## Comparing `pyfmrheo-0.1.1.tar` & `pyfmrheo-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 11:24:44.231221 pyfmrheo-0.1.1/
--rw-rw-rw-   0        0        0     1097 2023-07-26 18:07:23.000000 pyfmrheo-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1098 2023-07-27 11:24:44.231221 pyfmrheo-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      478 2023-07-27 11:21:44.000000 pyfmrheo-0.1.1/README.md
--rw-rw-rw-   0        0        0      298 2023-07-27 11:23:13.000000 pyfmrheo-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      830 2023-07-27 11:24:44.239221 pyfmrheo-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-27 11:24:43.926586 pyfmrheo-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-27 11:24:43.966590 pyfmrheo-0.1.1/src/pyfmrheo/
--rw-rw-rw-   0        0        0       68 2023-07-26 18:08:53.000000 pyfmrheo-0.1.1/src/pyfmrheo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:24:44.126607 pyfmrheo-0.1.1/src/pyfmrheo/models/
--rw-rw-rw-   0        0        0      271 2023-07-26 18:36:55.000000 pyfmrheo-0.1.1/src/pyfmrheo/models/__init__.py
--rw-rw-rw-   0        0        0     5535 2023-07-26 18:18:46.000000 pyfmrheo-0.1.1/src/pyfmrheo/models/bec.py
--rw-rw-rw-   0        0        0     9653 2023-07-26 18:18:56.000000 pyfmrheo-0.1.1/src/pyfmrheo/models/calibration.py
--rw-rw-rw-   0        0        0     3335 2023-07-26 18:19:02.000000 pyfmrheo-0.1.1/src/pyfmrheo/models/double_powerlaw.py
--rw-rw-rw-   0        0        0     2759 2023-07-26 18:19:35.000000 pyfmrheo-0.1.1/src/pyfmrheo/models/drag_sphere_model.py
--rw-rw-rw-   0        0        0      817 2023-07-26 18:19:38.000000 pyfmrheo-0.1.1/src/pyfmrheo/models/geom_coeffs.py
--rw-rw-rw-   0        0        0     7596 2023-07-26 18:19:45.000000 pyfmrheo-0.1.1/src/pyfmrheo/models/hertz.py
--rw-rw-rw-   0        0        0     6587 2023-07-26 18:19:49.000000 pyfmrheo-0.1.1/src/pyfmrheo/models/rheology.py
--rw-rw-rw-   0        0        0     3145 2023-07-26 18:20:12.000000 pyfmrheo-0.1.1/src/pyfmrheo/models/sader.py
--rw-rw-rw-   0        0        0     4393 2023-03-10 20:19:23.000000 pyfmrheo-0.1.1/src/pyfmrheo/models/sho.py
--rw-rw-rw-   0        0        0     3358 2023-07-26 18:20:23.000000 pyfmrheo-0.1.1/src/pyfmrheo/models/sine.py
--rw-rw-rw-   0        0        0    12839 2023-03-10 20:19:23.000000 pyfmrheo-0.1.1/src/pyfmrheo/models/ting.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:24:44.207218 pyfmrheo-0.1.1/src/pyfmrheo/routines/
--rw-rw-rw-   0        0        0     3480 2023-03-10 20:19:23.000000 pyfmrheo-0.1.1/src/pyfmrheo/routines/HertzFit.py
--rw-rw-rw-   0        0        0     4673 2023-04-26 10:18:29.000000 pyfmrheo-0.1.1/src/pyfmrheo/routines/MicrorheologyFFT.py
--rw-rw-rw-   0        0        0     6127 2023-04-26 10:18:54.000000 pyfmrheo-0.1.1/src/pyfmrheo/routines/MicrorheologySine.py
--rw-rw-rw-   0        0        0     1157 2023-03-10 20:19:23.000000 pyfmrheo-0.1.1/src/pyfmrheo/routines/NonContactCal.py
--rw-rw-rw-   0        0        0     1186 2023-03-10 20:19:23.000000 pyfmrheo-0.1.1/src/pyfmrheo/routines/PiezoCharacterization.py
--rw-rw-rw-   0        0        0     6517 2023-04-26 10:16:42.000000 pyfmrheo-0.1.1/src/pyfmrheo/routines/TingFit.py
--rw-rw-rw-   0        0        0     3603 2023-07-26 18:21:24.000000 pyfmrheo-0.1.1/src/pyfmrheo/routines/ViscousDragSteps.py
--rw-rw-rw-   0        0        0      215 2023-07-26 18:11:29.000000 pyfmrheo-0.1.1/src/pyfmrheo/routines/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:24:44.231221 pyfmrheo-0.1.1/src/pyfmrheo/utils/
--rw-rw-rw-   0        0        0       61 2023-07-26 18:11:49.000000 pyfmrheo-0.1.1/src/pyfmrheo/utils/__init__.py
--rw-rw-rw-   0        0        0     3382 2023-07-26 18:37:05.000000 pyfmrheo-0.1.1/src/pyfmrheo/utils/force_curves.py
--rw-rw-rw-   0        0        0     3733 2023-03-10 20:19:23.000000 pyfmrheo-0.1.1/src/pyfmrheo/utils/signal_processing.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:24:43.998594 pyfmrheo-0.1.1/src/pyfmrheo.egg-info/
--rw-rw-rw-   0        0        0     1098 2023-07-27 11:24:43.000000 pyfmrheo-0.1.1/src/pyfmrheo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1048 2023-07-27 11:24:43.000000 pyfmrheo-0.1.1/src/pyfmrheo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 11:24:43.000000 pyfmrheo-0.1.1/src/pyfmrheo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-27 11:24:43.000000 pyfmrheo-0.1.1/src/pyfmrheo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-27 11:24:43.000000 pyfmrheo-0.1.1/src/pyfmrheo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 18:40:33.943650 pyfmrheo-0.1.2/
+-rw-rw-rw-   0        0        0     1097 2023-07-26 18:07:23.000000 pyfmrheo-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1098 2023-08-05 18:40:33.943650 pyfmrheo-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      478 2023-07-27 11:21:44.000000 pyfmrheo-0.1.2/README.md
+-rw-rw-rw-   0        0        0      298 2023-08-05 18:38:27.000000 pyfmrheo-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      830 2023-08-05 18:40:33.950652 pyfmrheo-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-05 18:40:33.733411 pyfmrheo-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-08-05 18:40:33.760609 pyfmrheo-0.1.2/src/pyfmrheo/
+-rw-rw-rw-   0        0        0       68 2023-07-26 18:08:53.000000 pyfmrheo-0.1.2/src/pyfmrheo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:40:33.863633 pyfmrheo-0.1.2/src/pyfmrheo/models/
+-rw-rw-rw-   0        0        0      271 2023-07-26 18:36:55.000000 pyfmrheo-0.1.2/src/pyfmrheo/models/__init__.py
+-rw-rw-rw-   0        0        0     5535 2023-07-26 18:18:46.000000 pyfmrheo-0.1.2/src/pyfmrheo/models/bec.py
+-rw-rw-rw-   0        0        0     9653 2023-07-26 18:18:56.000000 pyfmrheo-0.1.2/src/pyfmrheo/models/calibration.py
+-rw-rw-rw-   0        0        0     3335 2023-07-26 18:19:02.000000 pyfmrheo-0.1.2/src/pyfmrheo/models/double_powerlaw.py
+-rw-rw-rw-   0        0        0     2759 2023-07-26 18:19:35.000000 pyfmrheo-0.1.2/src/pyfmrheo/models/drag_sphere_model.py
+-rw-rw-rw-   0        0        0      817 2023-07-26 18:19:38.000000 pyfmrheo-0.1.2/src/pyfmrheo/models/geom_coeffs.py
+-rw-rw-rw-   0        0        0     7596 2023-07-26 18:19:45.000000 pyfmrheo-0.1.2/src/pyfmrheo/models/hertz.py
+-rw-rw-rw-   0        0        0     6587 2023-07-26 18:19:49.000000 pyfmrheo-0.1.2/src/pyfmrheo/models/rheology.py
+-rw-rw-rw-   0        0        0     3145 2023-07-26 18:20:12.000000 pyfmrheo-0.1.2/src/pyfmrheo/models/sader.py
+-rw-rw-rw-   0        0        0     4393 2023-03-10 20:19:23.000000 pyfmrheo-0.1.2/src/pyfmrheo/models/sho.py
+-rw-rw-rw-   0        0        0     3358 2023-07-26 18:20:23.000000 pyfmrheo-0.1.2/src/pyfmrheo/models/sine.py
+-rw-rw-rw-   0        0        0    13041 2023-08-05 18:02:51.000000 pyfmrheo-0.1.2/src/pyfmrheo/models/ting.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:40:33.922645 pyfmrheo-0.1.2/src/pyfmrheo/routines/
+-rw-rw-rw-   0        0        0     3480 2023-03-10 20:19:23.000000 pyfmrheo-0.1.2/src/pyfmrheo/routines/HertzFit.py
+-rw-rw-rw-   0        0        0     4673 2023-04-26 10:18:29.000000 pyfmrheo-0.1.2/src/pyfmrheo/routines/MicrorheologyFFT.py
+-rw-rw-rw-   0        0        0     6127 2023-04-26 10:18:54.000000 pyfmrheo-0.1.2/src/pyfmrheo/routines/MicrorheologySine.py
+-rw-rw-rw-   0        0        0     1157 2023-03-10 20:19:23.000000 pyfmrheo-0.1.2/src/pyfmrheo/routines/NonContactCal.py
+-rw-rw-rw-   0        0        0     1186 2023-03-10 20:19:23.000000 pyfmrheo-0.1.2/src/pyfmrheo/routines/PiezoCharacterization.py
+-rw-rw-rw-   0        0        0     6591 2023-08-05 18:29:58.000000 pyfmrheo-0.1.2/src/pyfmrheo/routines/TingFit.py
+-rw-rw-rw-   0        0        0     3603 2023-07-26 18:21:24.000000 pyfmrheo-0.1.2/src/pyfmrheo/routines/ViscousDragSteps.py
+-rw-rw-rw-   0        0        0      215 2023-07-26 18:11:29.000000 pyfmrheo-0.1.2/src/pyfmrheo/routines/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:40:33.938649 pyfmrheo-0.1.2/src/pyfmrheo/utils/
+-rw-rw-rw-   0        0        0       61 2023-07-26 18:11:49.000000 pyfmrheo-0.1.2/src/pyfmrheo/utils/__init__.py
+-rw-rw-rw-   0        0        0     3382 2023-07-26 18:37:05.000000 pyfmrheo-0.1.2/src/pyfmrheo/utils/force_curves.py
+-rw-rw-rw-   0        0        0     3733 2023-03-10 20:19:23.000000 pyfmrheo-0.1.2/src/pyfmrheo/utils/signal_processing.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:40:33.782614 pyfmrheo-0.1.2/src/pyfmrheo.egg-info/
+-rw-rw-rw-   0        0        0     1098 2023-08-05 18:40:33.000000 pyfmrheo-0.1.2/src/pyfmrheo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1048 2023-08-05 18:40:33.000000 pyfmrheo-0.1.2/src/pyfmrheo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 18:40:33.000000 pyfmrheo-0.1.2/src/pyfmrheo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-08-05 18:40:33.000000 pyfmrheo-0.1.2/src/pyfmrheo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-05 18:40:33.000000 pyfmrheo-0.1.2/src/pyfmrheo.egg-info/top_level.txt
```

### Comparing `pyfmrheo-0.1.1/LICENSE` & `pyfmrheo-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.1/PKG-INFO` & `pyfmrheo-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfmrheo
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python package to perform analysis of Force Microscopy data.
 Home-page: https://github.com/jlopezalo/PyFMRheo
 Author: Javier Lopez Alonso
 Author-email: jla.lopez.18@gmail.com
 Project-URL: Bug Tracker, https://github.com/jlopezalo/PyFMRheo/issues
 Project-URL: repository, https://github.com/jlopezalo/PyFMRheo
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyfmrheo-0.1.1/setup.cfg` & `pyfmrheo-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7966 6d72 6865 6f0d 0a76 6572   = pyfmrheo..ver
-00000020: 7369 6f6e 203d 2030 2e31 2e31 0d0a 6175  sion = 0.1.1..au
+00000020: 7369 6f6e 203d 2030 2e31 2e32 0d0a 6175  sion = 0.1.2..au
 00000030: 7468 6f72 203d 204a 6176 6965 7220 4c6f  thor = Javier Lo
 00000040: 7065 7a20 416c 6f6e 736f 0d0a 6175 7468  pez Alonso..auth
 00000050: 6f72 5f65 6d61 696c 203d 206a 6c61 2e6c  or_email = jla.l
 00000060: 6f70 657a 2e31 3840 676d 6169 6c2e 636f  opez.18@gmail.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2041 2070 7974 686f 6e20 7061 636b 6167   A python packag
 00000090: 6520 746f 2070 6572 666f 726d 2061 6e61  e to perform ana
```

### Comparing `pyfmrheo-0.1.1/src/pyfmrheo/models/bec.py` & `pyfmrheo-0.1.2/src/pyfmrheo/models/bec.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.1/src/pyfmrheo/models/calibration.py` & `pyfmrheo-0.1.2/src/pyfmrheo/models/calibration.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.1/src/pyfmrheo/models/double_powerlaw.py` & `pyfmrheo-0.1.2/src/pyfmrheo/models/double_powerlaw.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.1/src/pyfmrheo/models/drag_sphere_model.py` & `pyfmrheo-0.1.2/src/pyfmrheo/models/drag_sphere_model.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.1/src/pyfmrheo/models/geom_coeffs.py` & `pyfmrheo-0.1.2/src/pyfmrheo/models/geom_coeffs.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.1/src/pyfmrheo/models/hertz.py` & `pyfmrheo-0.1.2/src/pyfmrheo/models/hertz.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.1/src/pyfmrheo/models/rheology.py` & `pyfmrheo-0.1.2/src/pyfmrheo/models/rheology.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.1/src/pyfmrheo/models/sader.py` & `pyfmrheo-0.1.2/src/pyfmrheo/models/sader.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.1/src/pyfmrheo/models/sho.py` & `pyfmrheo-0.1.2/src/pyfmrheo/models/sho.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.1/src/pyfmrheo/models/sine.py` & `pyfmrheo-0.1.2/src/pyfmrheo/models/sine.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.1/src/pyfmrheo/models/ting.py` & `pyfmrheo-0.1.2/src/pyfmrheo/models/ting.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,30 +138,34 @@
         # Determine contact trace region
         idxCt=np.where(time>=0)[0]
         # Get indices corresponding to contact trace region.
         # Including t max.
         idxCt = np.arange(idxCt[0], idx_tm + 1)
         # Determine contact time trace.
         ttc=time[idxCt]
-        if v0t is None:
+        if v0t is None and self.v0t is None:
             # Define range to compute trace speed.
             # Including t max.
             range_v0t=np.arange((idx_tm-int(len(ttc)*3/4)), idx_tm)
             # Fit 1 degree polynomial (x0 + m) to trace and retrace for determining
             # the corresponding speeds (x0)
             v0t = np.polyfit(time[range_v0t], delta[range_v0t], 1)[0]
             self.v0t = v0t
-        if v0r is None:
+        elif v0t is None and self.v0t is not None:
+            v0t = self.v0t
+        if v0r is None and self.v0r is None:
             # Define range to compute retrace speed.
             # Excluding t max.
             range_v0r=np.arange(idx_tm+2, (idx_tm+1+int(len(ttc)*3/4)))
             # Fit 1 degree polynomial (x0 + m) to trace and retrace for determining
             # the corresponding speeds (x0) 
             v0r = -1 * np.polyfit(time[range_v0r], delta[range_v0r], 1)[0]
-            self.v0t = v0r
+            self.v0r = v0r
+        elif v0r is None and self.v0r is not None:
+            v0r = self.v0r
         # Compute mean speed.
         v0=(v0r+v0t)/2
         # Compute retrace contact time.
         # TO DO: ADD REFERENCE TO ARTICLE!!!!
         tcr=(1+v0r/v0t)**(1/(1-betaE))/((1+v0r/v0t)**(1/(1-betaE))-1)*tm
         # If the retrace contact time is smaller than t max,
         # define the end of the contact retrace region as 3 times t max.
```

### Comparing `pyfmrheo-0.1.1/src/pyfmrheo/routines/HertzFit.py` & `pyfmrheo-0.1.2/src/pyfmrheo/routines/HertzFit.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.1/src/pyfmrheo/routines/MicrorheologyFFT.py` & `pyfmrheo-0.1.2/src/pyfmrheo/routines/MicrorheologyFFT.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.1/src/pyfmrheo/routines/MicrorheologySine.py` & `pyfmrheo-0.1.2/src/pyfmrheo/routines/MicrorheologySine.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.1/src/pyfmrheo/routines/NonContactCal.py` & `pyfmrheo-0.1.2/src/pyfmrheo/routines/NonContactCal.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.1/src/pyfmrheo/routines/PiezoCharacterization.py` & `pyfmrheo-0.1.2/src/pyfmrheo/routines/PiezoCharacterization.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.1/src/pyfmrheo/routines/TingFit.py` & `pyfmrheo-0.1.2/src/pyfmrheo/routines/TingFit.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,18 @@
     # Compute downfactor
     downfactor= len(time_fit) // param_dict['pts_downsample']
     # Get indices to downsample signal
     idxDown = list(range(0, len(time_fit), downfactor))
     # Compute tm and F0 using the downsampled signal
     idx_tm = np.argmax(force_fit[idxDown])
     f0idx = np.where(time_fit==0)[0]
-    F0_init=force_fit[f0idx]-param_dict['vdrag']*v0t
+    if v0t is not None:
+        F0_init=force_fit[f0idx]-param_dict['vdrag']*v0t
+    else:
+        F0_init=force_fit[f0idx]
     # Compute bounds for tc and F0
     tc_max = tc_fit+downfactor/(1/(time_fit[1]-time_fit[0]))*10
     tc_min = tc_fit-downfactor/(1/(time_fit[1]-time_fit[0]))*10
     f0_max = F0_init+100e-12
     f0_min = F0_init-100e-12
     # Set params for betaE
     if param_dict['auto_init_betaE']:
```

### Comparing `pyfmrheo-0.1.1/src/pyfmrheo/routines/ViscousDragSteps.py` & `pyfmrheo-0.1.2/src/pyfmrheo/routines/ViscousDragSteps.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.1/src/pyfmrheo/utils/force_curves.py` & `pyfmrheo-0.1.2/src/pyfmrheo/utils/force_curves.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.1/src/pyfmrheo/utils/signal_processing.py` & `pyfmrheo-0.1.2/src/pyfmrheo/utils/signal_processing.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.1/src/pyfmrheo.egg-info/PKG-INFO` & `pyfmrheo-0.1.2/src/pyfmrheo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfmrheo
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python package to perform analysis of Force Microscopy data.
 Home-page: https://github.com/jlopezalo/PyFMRheo
 Author: Javier Lopez Alonso
 Author-email: jla.lopez.18@gmail.com
 Project-URL: Bug Tracker, https://github.com/jlopezalo/PyFMRheo/issues
 Project-URL: repository, https://github.com/jlopezalo/PyFMRheo
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyfmrheo-0.1.1/src/pyfmrheo.egg-info/SOURCES.txt` & `pyfmrheo-0.1.2/src/pyfmrheo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

