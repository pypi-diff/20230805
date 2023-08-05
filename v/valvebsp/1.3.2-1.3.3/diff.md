# Comparing `tmp/valvebsp-1.3.2.tar.gz` & `tmp/valvebsp-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valvebsp-1.3.2.tar", last modified: Thu Jul 20 07:02:00 2023, max compression
+gzip compressed data, was "valvebsp-1.3.3.tar", last modified: Sat Aug  5 00:17:52 2023, max compression
```

## Comparing `valvebsp-1.3.2.tar` & `valvebsp-1.3.3.tar`

### file list

```diff
@@ -1,93 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:02:00.363719 valvebsp-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-20 07:01:57.000000 valvebsp-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-07-20 07:02:00.363719 valvebsp-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-20 07:01:57.000000 valvebsp-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 07:02:00.363719 valvebsp-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-20 07:01:59.000000 valvebsp-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:02:00.343719 valvebsp-1.3.2/valvebsp/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/bsp.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/lumps.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/profiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:02:00.359719 valvebsp-1.3.2/valvebsp/structs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/bsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/bsp_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_10.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_11.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_12.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_13.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_14.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_15.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_16.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_17.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_19.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_20.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_21.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_22.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_23.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_24.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_25.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_26.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_27.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_28.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_29.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_3.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_30.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_31.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_32.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_33.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_34.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_35.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_36.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_37.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_38.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_39.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_4.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_40.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_41.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_42.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_43.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_44.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_45.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_46.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_47.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_48.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_49.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_5.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_50.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_51.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_52.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_53.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_54.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_55.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_56.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_57.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_58.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_59.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_6.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_60.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_61.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_62.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_63.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_7.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_9.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_hlpd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_prpd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_prps.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-20 07:01:57.000000 valvebsp-1.3.2/valvebsp/structs/lump_tlpd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:02:00.343719 valvebsp-1.3.2/valvebsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-07-20 07:02:00.000000 valvebsp-1.3.2/valvebsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-20 07:02:00.000000 valvebsp-1.3.2/valvebsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 07:02:00.000000 valvebsp-1.3.2/valvebsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-20 07:02:00.000000 valvebsp-1.3.2/valvebsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 07:02:00.000000 valvebsp-1.3.2/valvebsp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:17:52.641466 valvebsp-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-05 00:17:43.000000 valvebsp-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-08-05 00:17:52.641466 valvebsp-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-08-05 00:17:43.000000 valvebsp-1.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 00:17:52.641466 valvebsp-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-08-05 00:17:50.000000 valvebsp-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:17:52.641466 valvebsp-1.3.3/valvebsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-05 00:17:43.000000 valvebsp-1.3.3/valvebsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-08-05 00:17:43.000000 valvebsp-1.3.3/valvebsp/bsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-05 00:17:43.000000 valvebsp-1.3.3/valvebsp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-05 00:17:43.000000 valvebsp-1.3.3/valvebsp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-08-05 00:17:43.000000 valvebsp-1.3.3/valvebsp/lumps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-08-05 00:17:43.000000 valvebsp-1.3.3/valvebsp/profiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:17:52.641466 valvebsp-1.3.3/valvebsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-08-05 00:17:52.000000 valvebsp-1.3.3/valvebsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-08-05 00:17:52.000000 valvebsp-1.3.3/valvebsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 00:17:52.000000 valvebsp-1.3.3/valvebsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-05 00:17:52.000000 valvebsp-1.3.3/valvebsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 00:17:52.000000 valvebsp-1.3.3/valvebsp.egg-info/top_level.txt
```

### Comparing `valvebsp-1.3.2/LICENSE` & `valvebsp-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `valvebsp-1.3.2/README.md` & `valvebsp-1.3.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 [![GPLv3 license](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://github.com/pySourceSDK/ValveBSP/blob/master/LICENSE.txt)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/valvebsp.svg)](https://pypi.python.org/pypi/valvebsp/)
+[![Platforms](https://img.shields.io/badge/platform-Linux,_MacOS,_Windows-blue)]()
 [![PyPI version fury.io](https://badge.fury.io/py/valvebsp.svg)](https://pypi.python.org/pypi/valvebsp/)
-[![alt text](https://github.com/pySourceSDK/ValveBSP/blob/master/docs/source/coverage.svg "coverage")]()
+[![GitHub Workflow Status (with event)](https://github.com/pySourceSDK/ValveBSP/actions/workflows/tests.yml/badge.svg)]()
+[![Test coverage](https://github.com/pySourceSDK/ValveBSP/blob/master/docs/source/coverage.svg "coverage")]()
+
 # ValveBSP
 
-ValveBSP is a Python library for parsing .bsp files for the Source Engine. It provides provides access to lump data.
+ValveBSP is a Python library designed to parse and edit .BSP files, which are utilized for game level representation within Valve's Source engine. It provides provides access to lump data in map files.
 
 Full documentation: https://pysourcesdk.github.io/ValveBSP/
+<!--- start pypi omit -->
 
 ### Currently supported lumps
 
 :heavy_check_mark: (52) Supported :x: (6) Unsupported :white_check_mark: (5) Unused :no_good: (1) will not support
 
 | Lump # | Status             | Lump # | Status             | Lump # | Status             | Lump # | Status             |
 | ---    | ---                | ---    | ---                | ---    | ---                | ---    | ---                |
@@ -27,14 +31,15 @@
 | 10     | :heavy_check_mark: | 26     | :heavy_check_mark: | 42     | :heavy_check_mark: | 58     | :heavy_check_mark: |
 | 11     | :heavy_check_mark: | 27     | :heavy_check_mark: | 43     | :heavy_check_mark: | 59     | :heavy_check_mark: |
 | 12     | :heavy_check_mark: | 28     | :heavy_check_mark: | 44     | :heavy_check_mark: | 60     | :heavy_check_mark: |
 | 13     | :heavy_check_mark: | 29     | :x:                | 45     | :heavy_check_mark: | 61     | :x:                |
 | 14     | :heavy_check_mark: | 30     | :heavy_check_mark: | 46     | :heavy_check_mark: | 62     | :x:                |
 | 15     | :heavy_check_mark: | 31     | :heavy_check_mark: | 47     | :heavy_check_mark: | 63     | :x:                |
 
+<!--- end pypi omit -->
 ## Installation
 
 ### PyPI
 
 ValveBSP is available on the Python Package Index. This makes installing it with pip as easy as:
 
 ```bash
@@ -51,8 +56,8 @@
 git clone git@github.com:pySourceSDK/ValveBSP.git
 ```
 
 and install it with:
 
 ```bash
 python3 setup.py install
-```
+```
```

### Comparing `valvebsp-1.3.2/setup.py` & `valvebsp-1.3.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 from setuptools import setup, find_packages
+import re
 
 with open('README.md') as f:
-    long_description = f.read()
+    re_omit = r'<!--- start pypi omit -->.*<!--- end pypi omit -->'
+    long_description = re.sub(re_omit, '', f.read(), flags=re.S)
 
-VERSION = '1.3.2'
+VERSION = 'v1.3.3'
 if 'VERSION_PLACEHOLDER' in VERSION:
     VERSION = '0.0.0'
 
 setup(
     name='valvebsp',
-    packages=find_packages(exclude=["tests", "tests.*", '*docs*']),
+    packages=['valvebsp'],
     version=VERSION,
-    description='A library to parse .bsp files (level files for the Source engine).',
+    description='A library to parse .BSP files (level files for the Source engine).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='gpl-3.0',
     author='Maxime Dupuis',
     author_email='mdupuis@hotmail.ca',
-    url='https://github.com/pySourceSDK/ValveBSP',
+    url='https://pysourcesdk.github.io/ValveBSP/',
+    project_urls={
+        'Documentation': 'https://pysourcesdk.github.io/ValveBSP/',
+        'Github': 'https://github.com/pySourceSDK/ValveBSP',
+    },
     keywords=['bsp', 'source', 'sourcesdk', 'hammer', 'valve'],
     install_requires=['construct', 'pyparsing', 'future'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
```

### Comparing `valvebsp-1.3.2/valvebsp/bsp.py` & `valvebsp-1.3.3/valvebsp/bsp.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from builtins import open
 from builtins import range
 from builtins import str
 from future import standard_library
 standard_library.install_aliases()
 
-import collections
+import collections  # NOQA: #402
 from shutil import copyfile  # NOQA: #402
 
 from construct import *  # NOQA: #402
 import valvebsp.structs.bsp as BSP  # NOQA: #402
 
 try:
     collectionsAbc = collections.abc
```

### Comparing `valvebsp-1.3.2/valvebsp/constants.py` & `valvebsp-1.3.3/valvebsp/constants.py`

 * *Files identical despite different names*

### Comparing `valvebsp-1.3.2/valvebsp/lumps.py` & `valvebsp-1.3.3/valvebsp/lumps.py`

 * *Files identical despite different names*

### Comparing `valvebsp-1.3.2/valvebsp/profiles.py` & `valvebsp-1.3.3/valvebsp/profiles.py`

 * *Files identical despite different names*

