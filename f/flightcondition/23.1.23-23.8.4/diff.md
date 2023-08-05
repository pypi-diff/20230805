# Comparing `tmp/flightcondition-23.1.23.tar.gz` & `tmp/flightcondition-23.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flightcondition-23.1.23.tar", last modified: Tue Jan 24 00:36:10 2023, max compression
+gzip compressed data, was "flightcondition-23.8.4.tar", last modified: Sat Aug  5 01:34:39 2023, max compression
```

## Comparing `flightcondition-23.1.23.tar` & `flightcondition-23.8.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-01-24 00:36:10.887394 flightcondition-23.1.23/
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     1073 2022-03-31 22:06:28.000000 flightcondition-23.1.23/LICENSE
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    13879 2023-01-24 00:36:10.888398 flightcondition-23.1.23/PKG-INFO
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    13041 2022-09-10 02:00:09.000000 flightcondition-23.1.23/README.md
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     1677 2023-01-24 00:36:10.892392 flightcondition-23.1.23/setup.cfg
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)      132 2022-07-21 02:57:11.000000 flightcondition-23.1.23/setup.py
-drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-01-24 00:36:10.556397 flightcondition-23.1.23/src/
-drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-01-24 00:36:10.741394 flightcondition-23.1.23/src/flightcondition/
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)      587 2022-08-17 22:55:21.000000 flightcondition-23.1.23/src/flightcondition/__init__.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     5891 2022-10-01 20:37:25.000000 flightcondition-23.1.23/src/flightcondition/__main__.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    23464 2022-09-10 00:12:33.000000 flightcondition-23.1.23/src/flightcondition/atmosphere.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     8554 2022-08-21 19:03:21.000000 flightcondition-23.1.23/src/flightcondition/boundarylayer.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     8360 2022-09-10 00:12:52.000000 flightcondition-23.1.23/src/flightcondition/common.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     3529 2022-08-16 02:55:24.000000 flightcondition-23.1.23/src/flightcondition/constants.py
-drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-01-24 00:36:10.872396 flightcondition-23.1.23/src/flightcondition/data/
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     4453 2023-01-20 22:21:17.000000 flightcondition-23.1.23/src/flightcondition/data/constants_en.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    30564 2023-01-20 22:21:17.000000 flightcondition-23.1.23/src/flightcondition/data/fc_units_en.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    51445 2022-09-10 00:11:32.000000 flightcondition-23.1.23/src/flightcondition/flightcondition.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    11868 2023-01-24 00:34:12.000000 flightcondition-23.1.23/src/flightcondition/isentropicflow.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     4127 2022-08-16 02:54:54.000000 flightcondition-23.1.23/src/flightcondition/nondimensional.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     2662 2022-08-16 02:54:58.000000 flightcondition-23.1.23/src/flightcondition/normalshock.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     5378 2023-01-21 02:40:37.000000 flightcondition-23.1.23/src/flightcondition/units.py
-drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-01-24 00:36:10.839392 flightcondition-23.1.23/src/flightcondition.egg-info/
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    13879 2023-01-24 00:36:10.000000 flightcondition-23.1.23/src/flightcondition.egg-info/PKG-INFO
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)      794 2023-01-24 00:36:10.000000 flightcondition-23.1.23/src/flightcondition.egg-info/SOURCES.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        1 2023-01-24 00:36:10.000000 flightcondition-23.1.23/src/flightcondition.egg-info/dependency_links.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)       66 2023-01-24 00:36:10.000000 flightcondition-23.1.23/src/flightcondition.egg-info/entry_points.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)       26 2023-01-24 00:36:10.000000 flightcondition-23.1.23/src/flightcondition.egg-info/requires.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)       16 2023-01-24 00:36:10.000000 flightcondition-23.1.23/src/flightcondition.egg-info/top_level.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        1 2022-04-24 20:23:49.000000 flightcondition-23.1.23/src/flightcondition.egg-info/zip-safe
+drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-08-05 01:34:39.730847 flightcondition-23.8.4/
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     1073 2022-03-31 22:06:28.000000 flightcondition-23.8.4/LICENSE
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    13973 2023-08-05 01:34:39.733734 flightcondition-23.8.4/PKG-INFO
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    13044 2023-08-05 01:00:28.000000 flightcondition-23.8.4/README.md
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     1677 2023-08-05 01:34:39.746246 flightcondition-23.8.4/setup.cfg
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)      132 2022-07-21 02:57:11.000000 flightcondition-23.8.4/setup.py
+drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-08-05 01:34:38.414299 flightcondition-23.8.4/src/
+drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-08-05 01:34:39.173723 flightcondition-23.8.4/src/flightcondition/
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)      587 2022-08-17 22:55:21.000000 flightcondition-23.8.4/src/flightcondition/__init__.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     6820 2023-08-05 01:09:56.000000 flightcondition-23.8.4/src/flightcondition/__main__.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    23414 2023-08-05 00:45:46.000000 flightcondition-23.8.4/src/flightcondition/atmosphere.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     8554 2022-08-21 19:03:21.000000 flightcondition-23.8.4/src/flightcondition/boundarylayer.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     8185 2023-08-05 00:49:22.000000 flightcondition-23.8.4/src/flightcondition/common.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     3529 2022-08-16 02:55:24.000000 flightcondition-23.8.4/src/flightcondition/constants.py
+drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-08-05 01:34:39.667967 flightcondition-23.8.4/src/flightcondition/data/
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     4453 2023-01-20 22:21:17.000000 flightcondition-23.8.4/src/flightcondition/data/constants_en.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    30564 2023-01-20 22:21:17.000000 flightcondition-23.8.4/src/flightcondition/data/fc_units_en.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    51115 2023-08-05 00:40:30.000000 flightcondition-23.8.4/src/flightcondition/flightcondition.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    11868 2023-01-24 00:34:12.000000 flightcondition-23.8.4/src/flightcondition/isentropicflow.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     4127 2022-08-16 02:54:54.000000 flightcondition-23.8.4/src/flightcondition/nondimensional.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     2662 2022-08-16 02:54:58.000000 flightcondition-23.8.4/src/flightcondition/normalshock.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     5378 2023-01-21 02:40:37.000000 flightcondition-23.8.4/src/flightcondition/units.py
+drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-08-05 01:34:39.541783 flightcondition-23.8.4/src/flightcondition.egg-info/
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    13973 2023-08-05 01:34:37.000000 flightcondition-23.8.4/src/flightcondition.egg-info/PKG-INFO
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)      794 2023-08-05 01:34:38.000000 flightcondition-23.8.4/src/flightcondition.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        1 2023-08-05 01:34:37.000000 flightcondition-23.8.4/src/flightcondition.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)       67 2023-08-05 01:34:37.000000 flightcondition-23.8.4/src/flightcondition.egg-info/entry_points.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)       26 2023-08-05 01:34:37.000000 flightcondition-23.8.4/src/flightcondition.egg-info/requires.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)       16 2023-08-05 01:34:37.000000 flightcondition-23.8.4/src/flightcondition.egg-info/top_level.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        1 2022-04-24 20:23:49.000000 flightcondition-23.8.4/src/flightcondition.egg-info/zip-safe
```

### Comparing `flightcondition-23.1.23/LICENSE` & `flightcondition-23.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flightcondition-23.1.23/PKG-INFO` & `flightcondition-23.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: flightcondition
-Version: 23.1.23
-Summary: Compute airspeed (true/calibrated/equivalent/Mach), atmospheric
+Version: 23.8.4
+Summary: Compute airspeed (true/calibrated/equivalent/Mach), atmospheric data, and other flight condition quantities, with easy unit conversion.
 Home-page: https://github.com/MattCJones/flightcondition
 Author: Matthew C. Jones
 Author-email: matt.c.jones.aoe@gmail.com
 License: MIT License
 Keywords: utility,aerospace,engineering,design
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
@@ -105,32 +106,32 @@
 Input quantities must be dimensionalized - see the usage below.  Alternatively
 use `KTAS`, `KCAS`, or `KEAS` for convenience.  For example, `KCAS=233`
 is equivalent to `CAS=233*unit('knots')`.
 
 #### Output Quantities
 
 The following tables list the quantities and the variables used to access them.
-Quantities may be accessed by either (a) their shorter variable names, e.g.
-`.TAS`, or (b) by their longer, full names, e.g.  `byname.true_airspeed`. They
+Quantities may be accessed by either (a) their abbreviated variable, e.g.
+`.TAS`, or (b) by their full names, e.g.  `byname.true_airspeed`. They
 may also be accessed through their particular sub-category: `byalt`, `byvel`,
 or `bylen`, e.g.  `.byvel.TAS` or `.byvel.byname.true_airspeed`.
 
-| Altitude Quantity     | Name    | Full Name (via `.byname.`) |
-|-----------------------|---------|----------------------------|
-| Geometric altitude    | `h`     | `geometric_altitude`       |
-| Geopotential altitude | `H`     | `geopotential_altitude`    |
-| Pressure              | `p`     | `pressure`                 |
-| Temperature           | `T`     | `temperature`              |
-| Density               | `rho`   | `density`                  |
-| Sound speed           | `a`     | `sounds_speed`             |
-| Dynamic viscosity     | `mu`    | `dynamic_viscosity`        |
-| Kinematic viscosity   | `nu`    | `kinematic_viscosity`      |
-| Thermal conductivity  | `k`     | `thermal_conductivity`     |
-| Gravity               | `g`     | `gravity`                  |
-| Mean free path        | `MFP`   | `mean_free_path`           |
+| Altitude Quantity     | Variable | Full Name (via `.byname.`) |
+|-----------------------|----------|----------------------------|
+| Geometric altitude    | `h`      | `geometric_altitude`       |
+| Geopotential altitude | `H`      | `geopotential_altitude`    |
+| Pressure              | `p`      | `pressure`                 |
+| Temperature           | `T`      | `temperature`              |
+| Density               | `rho`    | `density`                  |
+| Sound speed           | `a`      | `sounds_speed`             |
+| Dynamic viscosity     | `mu`     | `dynamic_viscosity`        |
+| Kinematic viscosity   | `nu`     | `kinematic_viscosity`      |
+| Thermal conductivity  | `k`      | `thermal_conductivity`     |
+| Gravity               | `g`      | `gravity`                  |
+| Mean free path        | `MFP`    | `mean_free_path`           |
 
 | Velocity Quantity                | Name      | Full Name (via `.byname.`)       |
 |----------------------------------|-----------|----------------------------------|
 | True airspeed (TAS)              | `TAS`     | `true_airspeed`                  |
 | Calibrated airspeed (CAS)        | `CAS`     | `calibrated_airspeed`            |
 | Equivalent airspeed (EAS)        | `EAS`     | `equivalent_airspeed`            |
 | Mach number                      | `M`       | `mach_number`                    |
@@ -350,7 +351,9 @@
 The software is provided "as is", without warranty of any kind, express or
 implied, including but not limited to the warranties of merchantability,
 fitness for a particular purpose and noninfringement. In no event shall the
 authors or copyright holders be liable for any claim, damages or other
 liability, whether in an action of contract, tort or otherwise, arising from,
 out of or in connection with the software or the use or other dealings in the
 software.
+
+
```

### Comparing `flightcondition-23.1.23/README.md` & `flightcondition-23.8.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -82,32 +82,32 @@
 Input quantities must be dimensionalized - see the usage below.  Alternatively
 use `KTAS`, `KCAS`, or `KEAS` for convenience.  For example, `KCAS=233`
 is equivalent to `CAS=233*unit('knots')`.
 
 #### Output Quantities
 
 The following tables list the quantities and the variables used to access them.
-Quantities may be accessed by either (a) their shorter variable names, e.g.
-`.TAS`, or (b) by their longer, full names, e.g.  `byname.true_airspeed`. They
+Quantities may be accessed by either (a) their abbreviated variable, e.g.
+`.TAS`, or (b) by their full names, e.g.  `byname.true_airspeed`. They
 may also be accessed through their particular sub-category: `byalt`, `byvel`,
 or `bylen`, e.g.  `.byvel.TAS` or `.byvel.byname.true_airspeed`.
 
-| Altitude Quantity     | Name    | Full Name (via `.byname.`) |
-|-----------------------|---------|----------------------------|
-| Geometric altitude    | `h`     | `geometric_altitude`       |
-| Geopotential altitude | `H`     | `geopotential_altitude`    |
-| Pressure              | `p`     | `pressure`                 |
-| Temperature           | `T`     | `temperature`              |
-| Density               | `rho`   | `density`                  |
-| Sound speed           | `a`     | `sounds_speed`             |
-| Dynamic viscosity     | `mu`    | `dynamic_viscosity`        |
-| Kinematic viscosity   | `nu`    | `kinematic_viscosity`      |
-| Thermal conductivity  | `k`     | `thermal_conductivity`     |
-| Gravity               | `g`     | `gravity`                  |
-| Mean free path        | `MFP`   | `mean_free_path`           |
+| Altitude Quantity     | Variable | Full Name (via `.byname.`) |
+|-----------------------|----------|----------------------------|
+| Geometric altitude    | `h`      | `geometric_altitude`       |
+| Geopotential altitude | `H`      | `geopotential_altitude`    |
+| Pressure              | `p`      | `pressure`                 |
+| Temperature           | `T`      | `temperature`              |
+| Density               | `rho`    | `density`                  |
+| Sound speed           | `a`      | `sounds_speed`             |
+| Dynamic viscosity     | `mu`     | `dynamic_viscosity`        |
+| Kinematic viscosity   | `nu`     | `kinematic_viscosity`      |
+| Thermal conductivity  | `k`      | `thermal_conductivity`     |
+| Gravity               | `g`      | `gravity`                  |
+| Mean free path        | `MFP`    | `mean_free_path`           |
 
 | Velocity Quantity                | Name      | Full Name (via `.byname.`)       |
 |----------------------------------|-----------|----------------------------------|
 | True airspeed (TAS)              | `TAS`     | `true_airspeed`                  |
 | Calibrated airspeed (CAS)        | `CAS`     | `calibrated_airspeed`            |
 | Equivalent airspeed (EAS)        | `EAS`     | `equivalent_airspeed`            |
 | Mach number                      | `M`       | `mach_number`                    |
```

### Comparing `flightcondition-23.1.23/setup.cfg` & `flightcondition-23.8.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Topic :: Scientific/Engineering
 	Topic :: Utilities
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
-version = 23.01.23
+version = 23.08.04
 
 [options]
 packages = find:
 package_dir = 
 	= src
 zip_safe = True
 python_requires = >=3.8
```

### Comparing `flightcondition-23.1.23/src/flightcondition/__init__.py` & `flightcondition-23.8.4/src/flightcondition/__init__.py`

 * *Files identical despite different names*

### Comparing `flightcondition-23.1.23/src/flightcondition/__main__.py` & `flightcondition-23.8.4/src/flightcondition/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -61,27 +61,45 @@
     parser.add_argument(
         '--Mach', dest='M', metavar='', nargs=None, type=float,
         default=None, help=argparse.SUPPRESS)
     parser.add_argument(
         '--TAS', dest='TAS', metavar='', nargs=2, type=str, default=None,
         help="true airspeed and speed unit, e.g. '150 knots'")
     parser.add_argument(
+        '--tas', dest='TAS', metavar='', nargs=None, type=float,
+        default=None, help=argparse.SUPPRESS)
+    parser.add_argument(
+        '--KTAS', dest='KTAS', metavar='', nargs=None, type=float,
+        default=None, help=argparse.SUPPRESS)
+    parser.add_argument(
+        '--ktas', dest='KTAS', metavar='', nargs=None, type=float,
+        default=None, help=argparse.SUPPRESS)
+    parser.add_argument(
         '--CAS', dest='CAS', metavar='', nargs=2, type=str, default=None,
         help="calibrated airspeed and speed unit, e.g. '150 knots'")
     parser.add_argument(
+        '--cas', dest='CAS', metavar='', nargs=None, type=float,
+        default=None, help=argparse.SUPPRESS)
+    parser.add_argument(
+        '--KCAS', dest='KCAS', metavar='', nargs=None, type=float,
+        default=None, help=argparse.SUPPRESS)
+    parser.add_argument(
+        '--kcas', dest='KCAS', metavar='', nargs=None, type=float,
+        default=None, help=argparse.SUPPRESS)
+    parser.add_argument(
         '--EAS', dest='EAS', metavar='', nargs=2, type=str, default=None,
         help="equivalent airspeed and speed unit, e.g. '150 knots'")
     parser.add_argument(
-        '--KTAS', dest='KTAS', metavar='', nargs=None, type=float,
+        '--eas', dest='EAS', metavar='', nargs=None, type=float,
         default=None, help=argparse.SUPPRESS)
     parser.add_argument(
-        '--KCAS', dest='KCAS', metavar='', nargs=None, type=float,
+        '--KEAS', dest='KEAS', metavar='', nargs=None, type=float,
         default=None, help=argparse.SUPPRESS)
     parser.add_argument(
-        '--KEAS', dest='KEAS', metavar='', nargs=None, type=float,
+        '--keas', dest='KEAS', metavar='', nargs=None, type=float,
         default=None, help=argparse.SUPPRESS)
     parser.add_argument(
         '--L', dest='length_scale', metavar='', nargs=2,
         type=str, default=None,
         help=("length scale, e.g. '10 ft'; aliases include: "
               "--length-scale --Length --ell"))
     parser.add_argument(
@@ -132,14 +150,16 @@
     TAS_ = None if args.TAS is None else _dimension(args.TAS)
     CAS_ = None if args.CAS is None else _dimension(args.CAS)
     EAS_ = None if args.EAS is None else _dimension(args.EAS)
     TAS_ = TAS_ if args.KTAS is None else args.KTAS*unit('knots')
     CAS_ = CAS_ if args.KCAS is None else args.KCAS*unit('knots')
     EAS_ = EAS_ if args.KEAS is None else args.KEAS*unit('knots')
     L_ = None if args.length_scale is None else _dimension(args.length_scale)
+    L_ = L_ if args.ft is None else args.ft*unit('ft')
+    L_ = L_ if args.m is None else args.m*unit('m')
     fc = FlightCondition(h=h_, M=M_, TAS=TAS_, CAS=CAS_, EAS=EAS_, L=L_,
                          units=args.units)
 
     # Print output but catch common unicode exception
     full_output = not args.no_full_output
     try:
         print(fc.tostring(full_output=full_output,
```

### Comparing `flightcondition-23.1.23/src/flightcondition/atmosphere.py` & `flightcondition-23.8.4/src/flightcondition/atmosphere.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from flightcondition.units import unit, check_dimensioned,\
     check_length_dimensioned, check_US_length_units
 
 
 class Layer(DimensionalData):
     """Class to compute and store layer data. """
 
-    full_names = {
+    names = {
         'name': 'layer_name',
         'H_base': 'base_geopotential_height',
         'T_base': 'base_geopotential_temperature',
         'T_grad': 'temperature_gradient',
         'p_base': 'base_static_pressure',
     }
 
@@ -57,15 +57,15 @@
             self._H_base[idx] = Atmo.H_base[jdx]
             self._T_base[idx] = Atmo.T_base[jdx]
             self._T_grad[idx] = Atmo.T_grad[jdx]
             self._p_base[idx] = Atmo.p_base[jdx]
 
         # Initialize access by full quantity name through .byname.<name>
         self.byname = AliasAttributes(
-            varsobj_arr=[self, ], full_names_dict_arr=[__class__.full_names, ])
+            varsobj_arr=[self, ], names_dict_arr=[__class__.names, ])
 
     @staticmethod
     def _layer_idx(H):
         """Find index for layer data.
 
         Args:
             H_arr (length): Geopotential altitude
@@ -114,17 +114,17 @@
             H_base_units   = 'km'
             T_base_units   = 'degK'
             T_grad_units   = 'degK/km'
             p_base_units   = 'Pa'
 
         # Insert longer variable name into output
         if max_sym_chars is None:
-            max_sym_chars = max([len(v) for v in self.full_names.keys()])
+            max_sym_chars = max([len(v) for v in self.names.keys()])
         if max_name_chars is None:
-            max_name_chars = max([len(v) for v in self.full_names.values()])
+            max_name_chars = max([len(v) for v in self.names.values()])
 
         H_base_str = self._vartostr(var=self.H_base, var_str='H_base',
                                     to_units=H_base_units,
                                     max_sym_chars=max_sym_chars,
                                     max_name_chars=max_name_chars,
                                     fmt_val="10.5g", pretty_print=pretty_print)
         T_base_str = self._vartostr(var=self.T_base, var_str='T_base',
@@ -218,15 +218,15 @@
 
         # Compute additional properties such as mean free path
         # Explore the class data structure for all options
         print( f"\nThe mean free path = {atm.MFP:.3g}")
         # >>> The mean free path = [7.25e-08 4.04e-05 0.00564] yd
     """
 
-    full_names = {
+    names = {
         'h': 'geometric_altitude',
         'H': 'geopotential_altitude',
         'p': 'pressure',
         'T': 'temperature',
         'rho': 'density',
         'a': 'sound_speed',
         'mu': 'dynamic_viscosity',
@@ -292,15 +292,15 @@
             if check_US_length_units(h):
                 self.units = 'US'
             else:
                 self.units = 'SI'
 
         # Initialize access by full quantity name through .byname.<name>
         self.byname = AliasAttributes(
-            varsobj_arr=[self, ], full_names_dict_arr=[__class__.full_names, ])
+            varsobj_arr=[self, ], names_dict_arr=[__class__.names, ])
 
     def tostring(self, full_output=None, units=None, max_sym_chars=None,
                  max_name_chars=None, pretty_print=True):
         """String representation of data structure.
 
         Args:
             full_output (bool): Set to True for full output
@@ -338,17 +338,17 @@
             nu_units  = 'm^2/s'
             k_units   = 'W/m/K'
             g_units   = 'm/s^2'
             MFP_units = 'm'
 
         # Insert longer variable name into output
         if max_sym_chars is None:
-            max_sym_chars = max([len(v) for v in self.full_names.keys()])
+            max_sym_chars = max([len(v) for v in self.names.keys()])
         if max_name_chars is None:
-            max_name_chars = max([len(v) for v in self.full_names.values()])
+            max_name_chars = max([len(v) for v in self.names.values()])
 
         h_str = self._vartostr(var=self.h, var_str='h', to_units=h_units,
                                max_sym_chars=max_sym_chars,
                                max_name_chars=max_name_chars,
                                fmt_val="10.5g", pretty_print=pretty_print)
         H_str = self._vartostr(var=self.H, var_str='H', to_units=H_units,
                                max_sym_chars=max_sym_chars,
```

### Comparing `flightcondition-23.1.23/src/flightcondition/boundarylayer.py` & `flightcondition-23.8.4/src/flightcondition/boundarylayer.py`

 * *Files identical despite different names*

### Comparing `flightcondition-23.1.23/src/flightcondition/common.py` & `flightcondition-23.8.4/src/flightcondition/common.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,61 +16,61 @@
 
 from flightcondition.units import to_base_units_wrapper
 
 
 class AliasAttributes():
     """Nested alias class to reference quantities by prescribed aliases. """
 
-    def __init__(self, varsobj_arr, full_names_dict_arr):
+    def __init__(self, varsobj_arr, names_dict_arr):
         """Populate full names and link to variable
         Args:
             varsobj (list): List of objects that holds all of the variables
-            full_names_dict (list): List of dictionaries that maps variables to
+            names_dict (list): List of dictionaries that maps variables to
                 their alias names
         """
         # Avoid infinite loop when setting properties
         super().__setattr__("varsobj_arr", varsobj_arr)
-        super().__setattr__("full_names_dict_arr", full_names_dict_arr)
+        super().__setattr__("names_dict_arr", names_dict_arr)
 
     def __dir__(self):
         """Add tab completion for alias names. """
-        # Avoid infinite loop when loading varsobj and full_names_dict
-        full_names_dict_arr = super().__getattribute__("full_names_dict_arr")
-        full_names_arr = []
-        for full_names_dict in full_names_dict_arr:
-            for varname in full_names_dict.values():
-                full_names_arr.append(varname)
-        return full_names_arr
+        # Avoid infinite loop when loading varsobj and names_dict
+        names_dict_arr = super().__getattribute__("names_dict_arr")
+        names_arr = []
+        for names_dict in names_dict_arr:
+            for varname in names_dict.values():
+                names_arr.append(varname)
+        return names_arr
 
     def __getattribute__(self, attr):
         """Get referenced quantity
 
         Args:
             attr (str): attribute name
         """
-        # Avoid infinite loop when loading varsobj and full_names_dict
+        # Avoid infinite loop when loading varsobj and names_dict
         varsobj_arr = super().__getattribute__("varsobj_arr")
-        full_names_dict_arr = super().__getattribute__("full_names_dict_arr")
-        for varsobj, full_names_dict in zip(varsobj_arr, full_names_dict_arr):
-            for var, varname in full_names_dict.items():
+        names_dict_arr = super().__getattribute__("names_dict_arr")
+        for varsobj, names_dict in zip(varsobj_arr, names_dict_arr):
+            for var, varname in names_dict.items():
                 if attr == varname:
                     return getattr(varsobj, var)
 
     def __setattr__(self, attr, attrval):
         """Set referenced quantity
 
         Args:
             attr (str): attribute name
             attrval (quantity): attribute value
         """
-        # Avoid infinite loop when loading varsobj and full_names_dict
+        # Avoid infinite loop when loading varsobj and names_dict
         varsobj_arr = super().__getattribute__("varsobj_arr")
-        full_names_dict_arr = super().__getattribute__("full_names_dict_arr")
-        for varsobj, full_names_dict in zip(varsobj_arr, full_names_dict_arr):
-            for var, varname in full_names_dict.items():
+        names_dict_arr = super().__getattribute__("names_dict_arr")
+        for varsobj, names_dict in zip(varsobj_arr, names_dict_arr):
+            for var, varname in names_dict.items():
                 if attr == varname:
                     return setattr(varsobj, var, attrval)
 
     def __repr__(self):
         """Output string representation of class object.
 
         Returns:
@@ -88,25 +88,25 @@
         except TypeError:
             return ""
 
 
 class DimensionalData:
     """Parent class to hold dimensional data"""
 
-    full_names = {}
+    names = {}
 
     def __eq__(self, other):
         """Check equality.
         Returns:
             dict: Dictionary representation of object
         """
         if other.__class__ is not self.__class__:
             return NotImplemented
 
-        for var in self.full_names.keys():
+        for var in self.names.keys():
             a = self.asdict[var]
             b = other.asdict[var]
             if not (np.shape(a) == np.shape(b)):
                 return False
             else:
                 if not ((a == b) | (np.isnan(a) & np.isnan(b))).all():
                     return False
@@ -137,39 +137,39 @@
         if self.full_output is None:
             full_output = False
         else:
             full_output = self.full_output
 
         return self.tostring(full_output=full_output)
 
-    def _asdict_template(self, full_names_dict=None):
+    def _asdict_template(self, names_dict=None):
         """Return class data as dictionary.
 
         Args:
-            full_names_dict (dict): Optionally specified variable names
+            names_dict (dict): Optionally specified variable names
                 dicitonary
 
         Returns:
             dict: Class data
         """
-        if full_names_dict is None:
-            full_names_dict = self.full_names
+        if names_dict is None:
+            names_dict = self.names
         obj_dict = {}
-        for var, varname in full_names_dict.items():
+        for var, varname in names_dict.items():
             obj_dict[var] = getattr(self, var)
         return obj_dict
 
     @property
     def asdict(self):
         """Return class data as dictionary.
 
         Returns:
             dict: Class data
         """
-        return self._asdict_template(self.full_names)
+        return self._asdict_template(self.names)
 
     def print(self, *args, **kwargs):
         """Print tostring() function to stdout. """
         print(self.tostring(*args, **kwargs))
 
     def tostring(self, full_output=True):
         """Override this function to output string representation of class
@@ -197,15 +197,15 @@
             fmt_val (str): String for formatting value
             pretty_print (bool): Pretty print format
 
         Returns:
             str: formatted string
         """
         pp_ = "~P" if pretty_print else ""
-        var_name = self.full_names[var_str]
+        var_name = self.names[var_str]
         if to_units is None:
             var_units_str = ""
         else:
             var.ito(to_units)
             var_units_str = f"{var.units:{pp_}}"
 
         if np.size(var) > 6:
```

### Comparing `flightcondition-23.1.23/src/flightcondition/constants.py` & `flightcondition-23.8.4/src/flightcondition/constants.py`

 * *Files identical despite different names*

### Comparing `flightcondition-23.1.23/src/flightcondition/data/constants_en.txt` & `flightcondition-23.8.4/src/flightcondition/data/constants_en.txt`

 * *Files identical despite different names*

### Comparing `flightcondition-23.1.23/src/flightcondition/data/fc_units_en.txt` & `flightcondition-23.8.4/src/flightcondition/data/fc_units_en.txt`

 * *Files identical despite different names*

### Comparing `flightcondition-23.1.23/src/flightcondition/flightcondition.py` & `flightcondition-23.8.4/src/flightcondition/flightcondition.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,16 +86,16 @@
         # >>> [ True  True  True]
 
         # Or by their sub-categories: `byalt`, `byvel`, or `bylen`
         print(fc.byvel.TAS == fc.byvel.byname.true_airspeed)
         # >>> [ True  True  True]
     """
     # Define dictionaries mapping variables to their full names
-    _byalt_full_names = Atmosphere.full_names
-    _byvel_full_names = {
+    _byalt_names = Atmosphere.names
+    _byvel_names = {
         'TAS': 'true_airspeed',
         'CAS': 'calibrated_airspeed',
         'EAS': 'equivalent_airspeed',
         'KTAS': 'knots_true_airspeed',
         'KCAS': 'knots_calibrated_airspeed',
         'KEAS': 'knots_equivalent_airspeed',
         'M': 'mach_number',
@@ -105,27 +105,27 @@
         'p0': 'stagnation_pressure',
         'T0': 'stagnation_temperature',
         'Tr_lamr': 'recovery_temperature_laminar',
         'Tr_turb': 'recovery_temperature_turbulent',
         'Re_by_L': 'reynolds_per_length',
     }
 
-    _bylen_full_names = {
+    _bylen_names = {
         'L': 'length_scale',
         'Re': 'reynolds_number',
         'h_BL_lamr': 'boundary_thickness_laminar',
         'h_BL_turb': 'boundary_thickness_turbulent',
         'Cf_lamr': 'friction_coefficient_laminar',
         'Cf_turb': 'friction_coefficient_turbulent',
         'h_yplus1': 'wall_distance_yplus1',
     }
-    full_names = {}
-    full_names.update(_byalt_full_names)
-    full_names.update(_byvel_full_names)
-    full_names.update(_bylen_full_names)
+    names = {}
+    names.update(_byalt_names)
+    names.update(_byvel_names)
+    names.update(_bylen_names)
 
 # =========================================================================== #
 #                       GENERAL FUNCTIONS & PROPERTIES                        #
 # =========================================================================== #
     def __init__(
         self, h=None, M=None, TAS=None, CAS=None, EAS=None, L=None, Re=None,
         units=None, full_output=None, **kwargs,
@@ -271,95 +271,95 @@
                 msg = "Overriding velocity based on Reynolds number."
                 warnings.warn(msg)
             self.Re = Re  # velocity is set based on Re and L
 
         # Set up behind-the scenes quantity access features
         # Set up sub-categories asdict functions
         self._byalt_asdict = self._asdict_template(
-            full_names_dict=self._byalt_full_names)
+            names_dict=self._byalt_names)
         self._byvel_asdict = self._asdict_template(
-            full_names_dict=self._byvel_full_names)
+            names_dict=self._byvel_names)
         self._bylen_asdict = self._asdict_template(
-            full_names_dict=self._bylen_full_names)
+            names_dict=self._bylen_names)
 
         # Set alias references by name _byalt_byname.<name>
         self._byalt_byname = AliasAttributes(
             varsobj_arr=[self, ],
-            full_names_dict_arr=[self._byalt_full_names, ]
+            names_dict_arr=[self._byalt_names, ]
         )
 
         # Set alias references by name _byvel_byname.<name>
         self._byvel_byname = AliasAttributes(
             varsobj_arr=[self, ],
-            full_names_dict_arr=[self._byvel_full_names, ]
+            names_dict_arr=[self._byvel_names, ]
         )
 
         # Set alias references by name _bylen_byname.<name>
         self._bylen_byname = AliasAttributes(
             varsobj_arr=[self, ],
-            full_names_dict_arr=[self._bylen_full_names, ]
+            names_dict_arr=[self._bylen_names, ]
         )
 
         # Set alias references by name generally .byname.<name>
         self.byname = AliasAttributes(
             varsobj_arr=[self, self, self],
-            full_names_dict_arr=[
-                self._byalt_full_names,
-                self._byvel_full_names,
-                self._bylen_full_names,
+            names_dict_arr=[
+                self._byalt_names,
+                self._byvel_names,
+                self._bylen_names,
             ]
         )
 
         # Set variable aliases by altitude properties to .byalt.<var>
-        byalt_vars = {key: key for key in self._byalt_full_names.keys()}
+        byalt_vars = {key: key for key in self._byalt_names.keys()}
         self.byalt = AliasAttributes(
             varsobj_arr=[self, self, self, self, self, self, ],
-            full_names_dict_arr=[
+            names_dict_arr=[
                 byalt_vars,
-                {"_byalt_full_names": "full_names"},
+                {"_byalt_names": "names"},
                 {"_byalt_tostring": "tostring"},
                 {"full_output": "full_output"},
                 {"_byalt_byname": "byname"},
                 {"_byalt_asdict": "asdict"},
             ]
         )
 
         # Set variable aliases by velocity properties to .byvel.<var>
-        byvel_vars = {key: key for key in self._byvel_full_names.keys()}
+        byvel_vars = {key: key for key in self._byvel_names.keys()}
         self.byvel = AliasAttributes(
             varsobj_arr=[self, self, self, self, self, self, ],
-            full_names_dict_arr=[
+            names_dict_arr=[
                 byvel_vars,
-                {"_byvel_full_names": "full_names"},
+                {"_byvel_names": "names"},
                 {"_byvel_tostring": "tostring"},
                 {"full_output": "full_output"},
                 {"_byvel_byname": "byname"},
                 {"_byvel_asdict": "asdict"},
             ]
         )
 
         # Set variable aliases by length properties to .bylen.<var>
-        bylen_vars = {key: key for key in self._bylen_full_names.keys()}
+        bylen_vars = {key: key for key in self._bylen_names.keys()}
         self.bylen = AliasAttributes(
             varsobj_arr=[self, self, self, self, self, self, self, ],
-            full_names_dict_arr=[
+            names_dict_arr=[
                 bylen_vars,
-                {"_bylen_full_names": "full_names"},
+                {"_bylen_names": "names"},
                 {"_bylen_tostring": "tostring"},
                 {"full_output": "full_output"},
                 {"_bylen_byname": "byname"},
                 {"_bylen_asdict": "asdict"},
                 {"wall_distance_from_yplus": "wall_distance_from_yplus"},
             ]
         )
 
         # Set all property variable references to .byvar.<var>
         self.byvar = AliasAttributes(
             varsobj_arr=[self.byalt, self.byvel, self.bylen, ],
-            full_names_dict_arr=[byalt_vars, byvel_vars, bylen_vars, ]
+            names_dict_arr=[byalt_vars, byvel_vars, bylen_vars, ]
         )
 
     def tostring(self, full_output=True, units=None, pretty_print=True):
         """String representation of data structure.
 
         Args:
             full_output (bool): Set to True for full output
@@ -383,22 +383,22 @@
         # Check that quantity array sizes are consistent, otherwise raise error
         self._check_compatible_array_sizes(raise_warning=True,
                                            raise_error=True)
 
         # Determine maximum characters to add spaces for and assemble string
         if full_output:
             max_sym_chars = max([  # length of variables
-                max([len(v) for v in self._byalt_full_names.keys()]),
-                max([len(v) for v in self._byvel_full_names.keys()]),
-                max([len(v) for v in self._bylen_full_names.keys()]),
+                max([len(v) for v in self._byalt_names.keys()]),
+                max([len(v) for v in self._byvel_names.keys()]),
+                max([len(v) for v in self._bylen_names.keys()]),
             ])
             max_name_chars = max([  # length of variable names
-                max([len(v) for v in self._byalt_full_names.values()]),
-                max([len(v) for v in self._byvel_full_names.values()]),
-                max([len(v) for v in self._bylen_full_names.values()]),
+                max([len(v) for v in self._byalt_names.values()]),
+                max([len(v) for v in self._byvel_names.values()]),
+                max([len(v) for v in self._bylen_names.values()]),
             ])
         else:
             max_sym_chars = 7  # length of variables
             max_name_chars = 19  # length of variable names
 
         # Build output strings from sub-categories
         alti_str = self._byalt_tostring(full_output, self.units,
@@ -618,16 +618,16 @@
         super(FlightCondition, self.__class__).h.fset(self, h)
 
         # Set airspeed and length array sizes if they are singular and altitude
         # is non-singular
         if hasattr(self, '_M'):
             if __class__._check_compatible_array_size(
                     arr1=h, arr2=self._M,
-                    arr_name1=self.full_names['h'],
-                    arr_name2=self.full_names['M'],
+                    arr_name1=self.names['h'],
+                    arr_name2=self.names['M'],
                     raise_warning=True):
                 if self._holdconst_vel_var == 'M':
                     self.M = __class__._reshape_arr1_like_arr2(self._M, h)
                 elif self._holdconst_vel_var == 'TAS':
                     self.TAS = __class__._reshape_arr1_like_arr2(self._TAS, h)
                 elif self._holdconst_vel_var == 'CAS':
                     self.CAS = __class__._reshape_arr1_like_arr2(self._CAS, h)
@@ -635,16 +635,16 @@
                     self.EAS = __class__._reshape_arr1_like_arr2(self._EAS, h)
                 else:  # default to holding EAS constant
                     self.EAS = __class__._reshape_arr1_like_arr2(self._EAS, h)
 
         if hasattr(self, '_L'):
             if __class__._check_compatible_array_size(
                     arr1=h, arr2=self._L,
-                    arr_name1=self.full_names['h'],
-                    arr_name2=self.full_names['L'],
+                    arr_name1=self.names['h'],
+                    arr_name2=self.names['L'],
                     raise_warning=True):
                 self._L = __class__._reshape_arr1_like_arr2(self._L, h)
 
 # =========================================================================== #
 #                       VELOCITY FUNCTIONS & PROPERTIES                       #
 # =========================================================================== #
     def _process_input_velocity(self, vel_arr, vel_name="Velocity"):
@@ -656,21 +656,21 @@
 
         Returns:
             bool: True if compatible else False
         """
         if hasattr(self, '_h'):
             if __class__._check_compatible_array_size(
                     arr1=vel_arr, arr2=self._h,
-                    arr_name1=vel_name, arr_name2=self.full_names["h"],
+                    arr_name1=vel_name, arr_name2=self.names["h"],
                     raise_warning=True, raise_error=True):
                 self._h = __class__._reshape_arr1_like_arr2(self._h, vel_arr)
         if hasattr(self, '_L'):
             if __class__._check_compatible_array_size(
                     arr1=vel_arr, arr2=self._L,
-                    arr_name1=vel_name, arr_name2=self.full_names["L"],
+                    arr_name1=vel_name, arr_name2=self.names["L"],
                     raise_warning=True):
                 self._L = __class__._reshape_arr1_like_arr2(self._L, vel_arr)
 
     def _byvel_tostring(self, full_output=None, units=None, max_sym_chars=None,
                         max_name_chars=None, pretty_print=True):
         """String representation of data structure.
 
@@ -716,17 +716,17 @@
             T0_units    = 'degK'
             Tr_lamr_units = 'degK'
             Tr_turb_units = 'degK'
             Re_by_L_units = '1/mm'
 
         # Insert longer variable name into output
         if max_sym_chars is None:
-            max_sym_chars = max([len(v) for v in self.full_names.keys()])
+            max_sym_chars = max([len(v) for v in self.names.keys()])
         if max_name_chars is None:
-            max_name_chars = max([len(v) for v in self.full_names.values()])
+            max_name_chars = max([len(v) for v in self.names.values()])
 
         M_str = self._vartostr(
             var=self.M, var_str='M', to_units='',
             max_sym_chars=max_sym_chars, max_name_chars=max_name_chars,
             fmt_val="10.5g", pretty_print=pretty_print) + "\n"
         TAS_str = self._vartostr(
             var=self.TAS, var_str='TAS', to_units=TAS_units,
@@ -1000,15 +1000,15 @@
         return self._M
 
     @M.setter
     def M(self, M):
         """Mach number :math:`M` """
         M *= dimless  # add dimless for raw float input
         self._M = __class__._preprocess_arr(M, input_alt=self.h)
-        self._process_input_velocity(self._M, vel_name=self.full_names['M'])
+        self._process_input_velocity(self._M, vel_name=self.names['M'])
 
         self._TAS = self._TAS_from_M(self.M)
         self._EAS = self._EAS_from_TAS(self.TAS, self.M)
         self._q_c = self._q_c_from_M(self.M)
         self._CAS = self._CAS_from_q_c(self.q_c)
 
         # Out of all velocity quantities, hold this one constant over altitude
@@ -1020,15 +1020,15 @@
         return self._TAS
 
     @TAS.setter
     def TAS(self, TAS):
         """Set true airspeed. """
         self._TAS = __class__._preprocess_arr(TAS, input_alt=self.h)
         self._process_input_velocity(
-            self._TAS, vel_name=self.full_names['TAS'])
+            self._TAS, vel_name=self.names['TAS'])
 
         self._M = self._M_from_TAS(TAS)
         self._EAS = self._EAS_from_TAS(self.TAS, self.M)
         self._q_c = self._q_c_from_M(self.M)
         self._CAS = self._CAS_from_q_c(self.q_c)
 
         # Out of all velocity quantities, hold this one constant over altitude
@@ -1040,15 +1040,15 @@
         return self._CAS
 
     @CAS.setter
     def CAS(self, CAS):
         """Calibrated airspeed. """
         self._CAS = __class__._preprocess_arr(CAS, input_alt=self.h)
         self._process_input_velocity(
-            self._CAS, vel_name=self.full_names['CAS'])
+            self._CAS, vel_name=self.names['CAS'])
 
         self._q_c = self._q_c_from_CAS(self.CAS)
         self._M = self._M_from_q_c(self.q_c)
         self._TAS = self._TAS_from_M(self.M)
         self._EAS = self._EAS_from_TAS(self.TAS, self.M)
 
         # Out of all velocity quantities, hold this one constant over altitude
@@ -1060,15 +1060,15 @@
         return self._EAS
 
     @EAS.setter
     def EAS(self, EAS):
         """Set equivalent airspeed. """
         self._EAS = __class__._preprocess_arr(EAS, input_alt=self.h)
         self._process_input_velocity(
-            self._EAS, vel_name=self.full_names['EAS'])
+            self._EAS, vel_name=self.names['EAS'])
 
         self._M = self._M_from_EAS(self.EAS)
         self._TAS = self._TAS_from_M(self.M)
         self._q_c = self._q_c_from_M(self.M)
         self._CAS = self._CAS_from_q_c(self.q_c)
 
         # Out of all velocity quantities, hold this one constant over altitude
@@ -1203,17 +1203,17 @@
             h_BL_units = 'in'
         else:  # default to SI units
             L_units = 'm'
             h_BL_units = 'mm'
 
         # Insert longer variable name into output
         if max_sym_chars is None:
-            max_sym_chars = max([len(v) for v in self.full_names.keys()])
+            max_sym_chars = max([len(v) for v in self.names.keys()])
         if max_name_chars is None:
-            max_name_chars = max([len(v) for v in self.full_names.values()])
+            max_name_chars = max([len(v) for v in self.names.values()])
 
         L_str = self._vartostr(
             var=self.L, var_str='L', to_units=L_units,
             max_sym_chars=max_sym_chars, max_name_chars=max_name_chars,
             fmt_val="10.5g", pretty_print=pretty_print)
         Re_str = self._vartostr(
             var=self.Re, var_str='Re', to_units='',
@@ -1296,24 +1296,24 @@
         self._L = L
 
         # Set altitude and airspeed array sizes if they are singular and length
         # is non-singular
         if hasattr(self, '_h'):
             if __class__._check_compatible_array_size(
                     arr1=self._h, arr2=L,
-                    arr_name1=self.full_names['h'],
-                    arr_name2=self.full_names['L'],
+                    arr_name1=self.names['h'],
+                    arr_name2=self.names['L'],
                     raise_warning=True):
                 pass
                 # self._h = __class__._reshape_arr1_like_arr2(self._h, L)
         if hasattr(self, '_M'):
             if __class__._check_compatible_array_size(
                     arr1=self.M, arr2=L,
-                    arr_name1=self.full_names['M'],
-                    arr_name2=self.full_names['L'],
+                    arr_name1=self.names['M'],
+                    arr_name2=self.names['L'],
                     raise_warning=True):
                 pass
                 # self.M = __class__._reshape_arr1_like_arr2(self._M, L)
 
     @_property_decorators
     def Re(self):
         """Get Reynolds number :math:`Re`"""
@@ -1325,16 +1325,16 @@
     def Re(self, Re):
         """Set Reynolds number :math:`Re`
         Set the true airspeed based on Reynolds number and length scale. """
         Re *= dimless  # add dimless for raw float input
         Re = self._preprocess_arr(
             Re, input_alt=self.h, input_vel=self.M)
         __class__._check_compatible_array_size(
-            arr1=self.M, arr2=Re, arr_name1=self.full_names['M'],
-            arr_name2=self.full_names['L'], raise_warning=True,
+            arr1=self.M, arr2=Re, arr_name1=self.names['M'],
+            arr_name2=self.names['L'], raise_warning=True,
             raise_error=True)
         self.TAS = NonDimensional.reynolds_number_velocity(
             Re_L=Re, L=self.L, nu=self.nu)
 
     @_property_decorators
     def h_BL_lamr(self):
         """Get laminar Boundary Layer Thickness :math:`\\h_BL_{lamr}` """
```

### Comparing `flightcondition-23.1.23/src/flightcondition/isentropicflow.py` & `flightcondition-23.8.4/src/flightcondition/isentropicflow.py`

 * *Files identical despite different names*

### Comparing `flightcondition-23.1.23/src/flightcondition/nondimensional.py` & `flightcondition-23.8.4/src/flightcondition/nondimensional.py`

 * *Files identical despite different names*

### Comparing `flightcondition-23.1.23/src/flightcondition/normalshock.py` & `flightcondition-23.8.4/src/flightcondition/normalshock.py`

 * *Files identical despite different names*

### Comparing `flightcondition-23.1.23/src/flightcondition/units.py` & `flightcondition-23.8.4/src/flightcondition/units.py`

 * *Files identical despite different names*

### Comparing `flightcondition-23.1.23/src/flightcondition.egg-info/PKG-INFO` & `flightcondition-23.8.4/src/flightcondition.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: flightcondition
-Version: 23.1.23
-Summary: Compute airspeed (true/calibrated/equivalent/Mach), atmospheric
+Version: 23.8.4
+Summary: Compute airspeed (true/calibrated/equivalent/Mach), atmospheric data, and other flight condition quantities, with easy unit conversion.
 Home-page: https://github.com/MattCJones/flightcondition
 Author: Matthew C. Jones
 Author-email: matt.c.jones.aoe@gmail.com
 License: MIT License
 Keywords: utility,aerospace,engineering,design
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
@@ -105,32 +106,32 @@
 Input quantities must be dimensionalized - see the usage below.  Alternatively
 use `KTAS`, `KCAS`, or `KEAS` for convenience.  For example, `KCAS=233`
 is equivalent to `CAS=233*unit('knots')`.
 
 #### Output Quantities
 
 The following tables list the quantities and the variables used to access them.
-Quantities may be accessed by either (a) their shorter variable names, e.g.
-`.TAS`, or (b) by their longer, full names, e.g.  `byname.true_airspeed`. They
+Quantities may be accessed by either (a) their abbreviated variable, e.g.
+`.TAS`, or (b) by their full names, e.g.  `byname.true_airspeed`. They
 may also be accessed through their particular sub-category: `byalt`, `byvel`,
 or `bylen`, e.g.  `.byvel.TAS` or `.byvel.byname.true_airspeed`.
 
-| Altitude Quantity     | Name    | Full Name (via `.byname.`) |
-|-----------------------|---------|----------------------------|
-| Geometric altitude    | `h`     | `geometric_altitude`       |
-| Geopotential altitude | `H`     | `geopotential_altitude`    |
-| Pressure              | `p`     | `pressure`                 |
-| Temperature           | `T`     | `temperature`              |
-| Density               | `rho`   | `density`                  |
-| Sound speed           | `a`     | `sounds_speed`             |
-| Dynamic viscosity     | `mu`    | `dynamic_viscosity`        |
-| Kinematic viscosity   | `nu`    | `kinematic_viscosity`      |
-| Thermal conductivity  | `k`     | `thermal_conductivity`     |
-| Gravity               | `g`     | `gravity`                  |
-| Mean free path        | `MFP`   | `mean_free_path`           |
+| Altitude Quantity     | Variable | Full Name (via `.byname.`) |
+|-----------------------|----------|----------------------------|
+| Geometric altitude    | `h`      | `geometric_altitude`       |
+| Geopotential altitude | `H`      | `geopotential_altitude`    |
+| Pressure              | `p`      | `pressure`                 |
+| Temperature           | `T`      | `temperature`              |
+| Density               | `rho`    | `density`                  |
+| Sound speed           | `a`      | `sounds_speed`             |
+| Dynamic viscosity     | `mu`     | `dynamic_viscosity`        |
+| Kinematic viscosity   | `nu`     | `kinematic_viscosity`      |
+| Thermal conductivity  | `k`      | `thermal_conductivity`     |
+| Gravity               | `g`      | `gravity`                  |
+| Mean free path        | `MFP`    | `mean_free_path`           |
 
 | Velocity Quantity                | Name      | Full Name (via `.byname.`)       |
 |----------------------------------|-----------|----------------------------------|
 | True airspeed (TAS)              | `TAS`     | `true_airspeed`                  |
 | Calibrated airspeed (CAS)        | `CAS`     | `calibrated_airspeed`            |
 | Equivalent airspeed (EAS)        | `EAS`     | `equivalent_airspeed`            |
 | Mach number                      | `M`       | `mach_number`                    |
@@ -350,7 +351,9 @@
 The software is provided "as is", without warranty of any kind, express or
 implied, including but not limited to the warranties of merchantability,
 fitness for a particular purpose and noninfringement. In no event shall the
 authors or copyright holders be liable for any claim, damages or other
 liability, whether in an action of contract, tort or otherwise, arising from,
 out of or in connection with the software or the use or other dealings in the
 software.
+
+
```

### Comparing `flightcondition-23.1.23/src/flightcondition.egg-info/SOURCES.txt` & `flightcondition-23.8.4/src/flightcondition.egg-info/SOURCES.txt`

 * *Files identical despite different names*

