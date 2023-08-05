# Comparing `tmp/PySiglent_SSA3000x-0.3.tar.gz` & `tmp/PySiglent_SSA3000x-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySiglent_SSA3000x-0.3.tar", last modified: Sat Aug  5 12:59:51 2023, max compression
+gzip compressed data, was "PySiglent_SSA3000x-0.4.tar", last modified: Sat Aug  5 14:50:35 2023, max compression
```

## Comparing `PySiglent_SSA3000x-0.3.tar` & `PySiglent_SSA3000x-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 12:59:51.276339 PySiglent_SSA3000x-0.3/
--rw-rw-rw-   0        0        0     1091 2023-06-25 20:17:12.000000 PySiglent_SSA3000x-0.3/LICENSE
--rw-rw-rw-   0        0        0      413 2023-08-05 12:59:51.276339 PySiglent_SSA3000x-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-05 12:59:51.266784 PySiglent_SSA3000x-0.3/PySiglent_SSA3000x/
--rw-rw-rw-   0        0        0    26295 2023-08-05 12:59:14.000000 PySiglent_SSA3000x-0.3/PySiglent_SSA3000x/PySiglent_SSA3000x.py
--rw-rw-rw-   0        0        0       54 2023-06-25 20:17:12.000000 PySiglent_SSA3000x-0.3/PySiglent_SSA3000x/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-05 12:59:51.274307 PySiglent_SSA3000x-0.3/PySiglent_SSA3000x.egg-info/
--rw-rw-rw-   0        0        0      413 2023-08-05 12:59:51.000000 PySiglent_SSA3000x-0.3/PySiglent_SSA3000x.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-08-05 12:59:51.000000 PySiglent_SSA3000x-0.3/PySiglent_SSA3000x.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 12:59:51.000000 PySiglent_SSA3000x-0.3/PySiglent_SSA3000x.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-08-05 12:59:51.000000 PySiglent_SSA3000x-0.3/PySiglent_SSA3000x.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-08-05 12:59:51.000000 PySiglent_SSA3000x-0.3/PySiglent_SSA3000x.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-05 12:59:51.277346 PySiglent_SSA3000x-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1076 2023-06-25 20:19:33.000000 PySiglent_SSA3000x-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 14:50:35.464750 PySiglent_SSA3000x-0.4/
+-rw-rw-rw-   0        0        0     1091 2023-06-25 20:17:12.000000 PySiglent_SSA3000x-0.4/LICENSE
+-rw-rw-rw-   0        0        0      413 2023-08-05 14:50:35.463751 PySiglent_SSA3000x-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-05 14:50:35.436751 PySiglent_SSA3000x-0.4/PySiglent_SSA3000x/
+-rw-rw-rw-   0        0        0    26391 2023-08-05 14:50:14.000000 PySiglent_SSA3000x-0.4/PySiglent_SSA3000x/PySiglent_SSA3000x.py
+-rw-rw-rw-   0        0        0       54 2023-06-25 20:17:12.000000 PySiglent_SSA3000x-0.4/PySiglent_SSA3000x/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 14:50:35.459752 PySiglent_SSA3000x-0.4/PySiglent_SSA3000x.egg-info/
+-rw-rw-rw-   0        0        0      413 2023-08-05 14:50:35.000000 PySiglent_SSA3000x-0.4/PySiglent_SSA3000x.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-08-05 14:50:35.000000 PySiglent_SSA3000x-0.4/PySiglent_SSA3000x.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 14:50:35.000000 PySiglent_SSA3000x-0.4/PySiglent_SSA3000x.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-08-05 14:50:35.000000 PySiglent_SSA3000x-0.4/PySiglent_SSA3000x.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-08-05 14:50:35.000000 PySiglent_SSA3000x-0.4/PySiglent_SSA3000x.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 14:50:35.465754 PySiglent_SSA3000x-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1076 2023-06-25 20:19:33.000000 PySiglent_SSA3000x-0.4/setup.py
```

### Comparing `PySiglent_SSA3000x-0.3/LICENSE` & `PySiglent_SSA3000x-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PySiglent_SSA3000x-0.3/PySiglent_SSA3000x/PySiglent_SSA3000x.py` & `PySiglent_SSA3000x-0.4/PySiglent_SSA3000x/PySiglent_SSA3000x.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,15 +363,17 @@
     # LEVEL
     def reference_level(self, level: float = None):
         """This command sets the reference level for the Y-axis. [dBm]
         Gets reference level."""
         if level is not None and not self.ref_level_min <= level <= self.ref_level_max:
             raise self.Exceptions.ReferenceLevelOutOfRange(level)
         # todo : test resolution
-        return float(self._set_get(':DISPlay:WINDow:TRACe:Y:RLEVel', level + ' dBm'))
+        if level is not None: # build string if level has to be set
+            level = f'{level} dBm'
+        return float(self._set_get(':DISPlay:WINDow:TRACe:Y:RLEVel', level))
 
     def input_attenuator(self, att: int = None):
         """Sets the input attenuator of the spectrum analyzer. [dB]
         Gets the input attenuator"""
         if att is not None and not self.input_att_min <= att <= self.input_att_max:
             raise self.Exceptions.InputAttenuatorOutOfRange(att)
         # todo : test resolution
```

### Comparing `PySiglent_SSA3000x-0.3/setup.py` & `PySiglent_SSA3000x-0.4/setup.py`

 * *Files identical despite different names*

