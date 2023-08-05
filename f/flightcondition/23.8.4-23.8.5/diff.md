# Comparing `tmp/flightcondition-23.8.4.tar.gz` & `tmp/flightcondition-23.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flightcondition-23.8.4.tar", last modified: Sat Aug  5 01:34:39 2023, max compression
+gzip compressed data, was "flightcondition-23.8.5.tar", last modified: Sat Aug  5 01:43:15 2023, max compression
```

## Comparing `flightcondition-23.8.4.tar` & `flightcondition-23.8.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-08-05 01:34:39.730847 flightcondition-23.8.4/
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     1073 2022-03-31 22:06:28.000000 flightcondition-23.8.4/LICENSE
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    13973 2023-08-05 01:34:39.733734 flightcondition-23.8.4/PKG-INFO
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    13044 2023-08-05 01:00:28.000000 flightcondition-23.8.4/README.md
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     1677 2023-08-05 01:34:39.746246 flightcondition-23.8.4/setup.cfg
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)      132 2022-07-21 02:57:11.000000 flightcondition-23.8.4/setup.py
-drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-08-05 01:34:38.414299 flightcondition-23.8.4/src/
-drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-08-05 01:34:39.173723 flightcondition-23.8.4/src/flightcondition/
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)      587 2022-08-17 22:55:21.000000 flightcondition-23.8.4/src/flightcondition/__init__.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     6820 2023-08-05 01:09:56.000000 flightcondition-23.8.4/src/flightcondition/__main__.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    23414 2023-08-05 00:45:46.000000 flightcondition-23.8.4/src/flightcondition/atmosphere.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     8554 2022-08-21 19:03:21.000000 flightcondition-23.8.4/src/flightcondition/boundarylayer.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     8185 2023-08-05 00:49:22.000000 flightcondition-23.8.4/src/flightcondition/common.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     3529 2022-08-16 02:55:24.000000 flightcondition-23.8.4/src/flightcondition/constants.py
-drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-08-05 01:34:39.667967 flightcondition-23.8.4/src/flightcondition/data/
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     4453 2023-01-20 22:21:17.000000 flightcondition-23.8.4/src/flightcondition/data/constants_en.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    30564 2023-01-20 22:21:17.000000 flightcondition-23.8.4/src/flightcondition/data/fc_units_en.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    51115 2023-08-05 00:40:30.000000 flightcondition-23.8.4/src/flightcondition/flightcondition.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    11868 2023-01-24 00:34:12.000000 flightcondition-23.8.4/src/flightcondition/isentropicflow.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     4127 2022-08-16 02:54:54.000000 flightcondition-23.8.4/src/flightcondition/nondimensional.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     2662 2022-08-16 02:54:58.000000 flightcondition-23.8.4/src/flightcondition/normalshock.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     5378 2023-01-21 02:40:37.000000 flightcondition-23.8.4/src/flightcondition/units.py
-drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-08-05 01:34:39.541783 flightcondition-23.8.4/src/flightcondition.egg-info/
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    13973 2023-08-05 01:34:37.000000 flightcondition-23.8.4/src/flightcondition.egg-info/PKG-INFO
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)      794 2023-08-05 01:34:38.000000 flightcondition-23.8.4/src/flightcondition.egg-info/SOURCES.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        1 2023-08-05 01:34:37.000000 flightcondition-23.8.4/src/flightcondition.egg-info/dependency_links.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)       67 2023-08-05 01:34:37.000000 flightcondition-23.8.4/src/flightcondition.egg-info/entry_points.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)       26 2023-08-05 01:34:37.000000 flightcondition-23.8.4/src/flightcondition.egg-info/requires.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)       16 2023-08-05 01:34:37.000000 flightcondition-23.8.4/src/flightcondition.egg-info/top_level.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        1 2022-04-24 20:23:49.000000 flightcondition-23.8.4/src/flightcondition.egg-info/zip-safe
+drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-08-05 01:43:15.489171 flightcondition-23.8.5/
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     1073 2022-03-31 22:06:28.000000 flightcondition-23.8.5/LICENSE
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    13973 2023-08-05 01:43:15.491748 flightcondition-23.8.5/PKG-INFO
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    13044 2023-08-05 01:00:28.000000 flightcondition-23.8.5/README.md
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     1677 2023-08-05 01:43:15.503704 flightcondition-23.8.5/setup.cfg
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)      132 2022-07-21 02:57:11.000000 flightcondition-23.8.5/setup.py
+drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-08-05 01:43:14.142553 flightcondition-23.8.5/src/
+drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-08-05 01:43:14.917864 flightcondition-23.8.5/src/flightcondition/
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)      587 2022-08-17 22:55:21.000000 flightcondition-23.8.5/src/flightcondition/__init__.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     7086 2023-08-05 01:40:36.000000 flightcondition-23.8.5/src/flightcondition/__main__.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    23414 2023-08-05 00:45:46.000000 flightcondition-23.8.5/src/flightcondition/atmosphere.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     8554 2022-08-21 19:03:21.000000 flightcondition-23.8.5/src/flightcondition/boundarylayer.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     8185 2023-08-05 00:49:22.000000 flightcondition-23.8.5/src/flightcondition/common.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     3529 2022-08-16 02:55:24.000000 flightcondition-23.8.5/src/flightcondition/constants.py
+drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-08-05 01:43:15.424492 flightcondition-23.8.5/src/flightcondition/data/
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     4453 2023-01-20 22:21:17.000000 flightcondition-23.8.5/src/flightcondition/data/constants_en.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    30564 2023-01-20 22:21:17.000000 flightcondition-23.8.5/src/flightcondition/data/fc_units_en.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    51115 2023-08-05 00:40:30.000000 flightcondition-23.8.5/src/flightcondition/flightcondition.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    11868 2023-01-24 00:34:12.000000 flightcondition-23.8.5/src/flightcondition/isentropicflow.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     4127 2022-08-16 02:54:54.000000 flightcondition-23.8.5/src/flightcondition/nondimensional.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     2662 2022-08-16 02:54:58.000000 flightcondition-23.8.5/src/flightcondition/normalshock.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     5378 2023-01-21 02:40:37.000000 flightcondition-23.8.5/src/flightcondition/units.py
+drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-08-05 01:43:15.272502 flightcondition-23.8.5/src/flightcondition.egg-info/
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    13973 2023-08-05 01:43:13.000000 flightcondition-23.8.5/src/flightcondition.egg-info/PKG-INFO
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)      794 2023-08-05 01:43:13.000000 flightcondition-23.8.5/src/flightcondition.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        1 2023-08-05 01:43:13.000000 flightcondition-23.8.5/src/flightcondition.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)       67 2023-08-05 01:43:13.000000 flightcondition-23.8.5/src/flightcondition.egg-info/entry_points.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)       26 2023-08-05 01:43:13.000000 flightcondition-23.8.5/src/flightcondition.egg-info/requires.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)       16 2023-08-05 01:43:13.000000 flightcondition-23.8.5/src/flightcondition.egg-info/top_level.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        1 2022-04-24 20:23:49.000000 flightcondition-23.8.5/src/flightcondition.egg-info/zip-safe
```

### Comparing `flightcondition-23.8.4/LICENSE` & `flightcondition-23.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flightcondition-23.8.4/PKG-INFO` & `flightcondition-23.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flightcondition
-Version: 23.8.4
+Version: 23.8.5
 Summary: Compute airspeed (true/calibrated/equivalent/Mach), atmospheric data, and other flight condition quantities, with easy unit conversion.
 Home-page: https://github.com/MattCJones/flightcondition
 Author: Matthew C. Jones
 Author-email: matt.c.jones.aoe@gmail.com
 License: MIT License
 Keywords: utility,aerospace,engineering,design
 Platform: UNKNOWN
```

### Comparing `flightcondition-23.8.4/README.md` & `flightcondition-23.8.5/README.md`

 * *Files identical despite different names*

### Comparing `flightcondition-23.8.4/setup.cfg` & `flightcondition-23.8.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Topic :: Scientific/Engineering
 	Topic :: Utilities
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
-version = 23.08.04
+version = 23.08.05
 
 [options]
 packages = find:
 package_dir = 
 	= src
 zip_safe = True
 python_requires = >=3.8
```

### Comparing `flightcondition-23.8.4/src/flightcondition/__init__.py` & `flightcondition-23.8.5/src/flightcondition/__init__.py`

 * *Files identical despite different names*

### Comparing `flightcondition-23.8.4/src/flightcondition/__main__.py` & `flightcondition-23.8.5/src/flightcondition/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,20 @@
     parser.add_argument(
         '--Length', dest='length_scale', metavar='', nargs=2,
         type=str, default=None, help=argparse.SUPPRESS)
     parser.add_argument(
         '--ell', dest='length_scale', metavar='', nargs=2,
         type=str, default=None, help=argparse.SUPPRESS)
     parser.add_argument(
+        '--ft', dest='ft', metavar='', nargs=None, type=float,
+        default=None, help=argparse.SUPPRESS)
+    parser.add_argument(
+        '--m', dest='m', metavar='', nargs=None, type=float,
+        default=None, help=argparse.SUPPRESS)
+    parser.add_argument(
         '--units', dest='units', metavar='', nargs=None,
         type=str, default="", help=f"Unit system, i.e. {dir(unit.sys)}")
     parser.add_argument(
         '--no-full-output', dest='no_full_output', default=False,
         action='store_true', help="display abbreviated output")
     parser.add_argument(  # hidden option to turn off pretty print
         '--no-pretty-print', dest='no_pretty_print', default=False,
```

### Comparing `flightcondition-23.8.4/src/flightcondition/atmosphere.py` & `flightcondition-23.8.5/src/flightcondition/atmosphere.py`

 * *Files identical despite different names*

### Comparing `flightcondition-23.8.4/src/flightcondition/boundarylayer.py` & `flightcondition-23.8.5/src/flightcondition/boundarylayer.py`

 * *Files identical despite different names*

### Comparing `flightcondition-23.8.4/src/flightcondition/common.py` & `flightcondition-23.8.5/src/flightcondition/common.py`

 * *Files identical despite different names*

### Comparing `flightcondition-23.8.4/src/flightcondition/constants.py` & `flightcondition-23.8.5/src/flightcondition/constants.py`

 * *Files identical despite different names*

### Comparing `flightcondition-23.8.4/src/flightcondition/data/constants_en.txt` & `flightcondition-23.8.5/src/flightcondition/data/constants_en.txt`

 * *Files identical despite different names*

### Comparing `flightcondition-23.8.4/src/flightcondition/data/fc_units_en.txt` & `flightcondition-23.8.5/src/flightcondition/data/fc_units_en.txt`

 * *Files identical despite different names*

### Comparing `flightcondition-23.8.4/src/flightcondition/flightcondition.py` & `flightcondition-23.8.5/src/flightcondition/flightcondition.py`

 * *Files identical despite different names*

### Comparing `flightcondition-23.8.4/src/flightcondition/isentropicflow.py` & `flightcondition-23.8.5/src/flightcondition/isentropicflow.py`

 * *Files identical despite different names*

### Comparing `flightcondition-23.8.4/src/flightcondition/nondimensional.py` & `flightcondition-23.8.5/src/flightcondition/nondimensional.py`

 * *Files identical despite different names*

### Comparing `flightcondition-23.8.4/src/flightcondition/normalshock.py` & `flightcondition-23.8.5/src/flightcondition/normalshock.py`

 * *Files identical despite different names*

### Comparing `flightcondition-23.8.4/src/flightcondition/units.py` & `flightcondition-23.8.5/src/flightcondition/units.py`

 * *Files identical despite different names*

### Comparing `flightcondition-23.8.4/src/flightcondition.egg-info/PKG-INFO` & `flightcondition-23.8.5/src/flightcondition.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flightcondition
-Version: 23.8.4
+Version: 23.8.5
 Summary: Compute airspeed (true/calibrated/equivalent/Mach), atmospheric data, and other flight condition quantities, with easy unit conversion.
 Home-page: https://github.com/MattCJones/flightcondition
 Author: Matthew C. Jones
 Author-email: matt.c.jones.aoe@gmail.com
 License: MIT License
 Keywords: utility,aerospace,engineering,design
 Platform: UNKNOWN
```

### Comparing `flightcondition-23.8.4/src/flightcondition.egg-info/SOURCES.txt` & `flightcondition-23.8.5/src/flightcondition.egg-info/SOURCES.txt`

 * *Files identical despite different names*

