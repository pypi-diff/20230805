# Comparing `tmp/historydict-1.2.3.tar.gz` & `tmp/historydict-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/historydict-1.2.3.tar", last modified: Thu May 10 12:10:43 2018, max compression
+gzip compressed data, was "historydict-1.2.6.tar", last modified: Sat Aug  5 20:39:16 2023, max compression
```

## Comparing `historydict-1.2.3.tar` & `historydict-1.2.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 dallan     (501) staff       (20)        0 2018-05-10 12:10:43.000000 historydict-1.2.3/
-drwxr-xr-x   0 dallan     (501) staff       (20)        0 2018-05-10 12:10:43.000000 historydict-1.2.3/historydict.egg-info/
--rw-r--r--   0 dallan     (501) staff       (20)        1 2018-05-10 12:10:43.000000 historydict-1.2.3/historydict.egg-info/dependency_links.txt
--rw-r--r--   0 dallan     (501) staff       (20)      333 2018-05-10 12:10:43.000000 historydict-1.2.3/historydict.egg-info/PKG-INFO
--rw-r--r--   0 dallan     (501) staff       (20)      173 2018-05-10 12:10:43.000000 historydict-1.2.3/historydict.egg-info/SOURCES.txt
--rw-r--r--   0 dallan     (501) staff       (20)       12 2018-05-10 12:10:43.000000 historydict-1.2.3/historydict.egg-info/top_level.txt
--rw-r--r--   0 dallan     (501) staff       (20)     6520 2018-05-10 12:09:38.000000 historydict-1.2.3/historydict.py
--rw-r--r--   0 dallan     (501) staff       (20)      333 2018-05-10 12:10:43.000000 historydict-1.2.3/PKG-INFO
--rw-r--r--   0 dallan     (501) staff       (20)     2460 2017-11-28 19:49:16.000000 historydict-1.2.3/README.md
--rw-r--r--   0 dallan     (501) staff       (20)       38 2018-05-10 12:10:43.000000 historydict-1.2.3/setup.cfg
--rw-r--r--   0 dallan     (501) staff       (20)      352 2018-05-10 12:10:17.000000 historydict-1.2.3/setup.py
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2023-08-05 20:39:16.695918 historydict-1.2.6/
+-rw-r--r--   0 mrakitin   (501) staff       (20)      333 2023-08-05 20:39:16.695396 historydict-1.2.6/PKG-INFO
+-rw-r--r--   0 mrakitin   (501) staff       (20)     1955 2023-08-05 20:36:36.000000 historydict-1.2.6/README.md
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2023-08-05 20:39:16.694605 historydict-1.2.6/historydict.egg-info/
+-rw-r--r--   0 mrakitin   (501) staff       (20)      333 2023-08-05 20:39:16.000000 historydict-1.2.6/historydict.egg-info/PKG-INFO
+-rw-r--r--   0 mrakitin   (501) staff       (20)      173 2023-08-05 20:39:16.000000 historydict-1.2.6/historydict.egg-info/SOURCES.txt
+-rw-r--r--   0 mrakitin   (501) staff       (20)        1 2023-08-05 20:39:16.000000 historydict-1.2.6/historydict.egg-info/dependency_links.txt
+-rw-r--r--   0 mrakitin   (501) staff       (20)       12 2023-08-05 20:39:16.000000 historydict-1.2.6/historydict.egg-info/top_level.txt
+-rw-r--r--   0 mrakitin   (501) staff       (20)     6619 2023-08-05 20:36:36.000000 historydict-1.2.6/historydict.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)       38 2023-08-05 20:39:16.696044 historydict-1.2.6/setup.cfg
+-rw-r--r--   0 mrakitin   (501) staff       (20)      387 2023-08-05 20:36:36.000000 historydict-1.2.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `historydict-1.2.3/historydict.py` & `historydict-1.2.6/historydict.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,20 @@
 from __future__ import (absolute_import, division, print_function,
                         unicode_literals)
 import sys
 import logging
 import hashlib
 import sqlite3
 import json
-from collections import MutableMapping
+try:
+    from collections.abc import MutableMapping
+except ImportError:
+    from collections import MutableMapping
+
+__version__ = '1.2.6'
 
 logger = logging.getLogger(__name__)
 
 
 TABLE_NAME = 'HISTORY_1_1'
 CREATION_QUERY = """
 CREATE TABLE {0} (
```

### Comparing `historydict-1.2.3/README.md` & `historydict-1.2.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-[![Build
-Status](https://travis-ci.org/Nikea/historydict.svg?branch=master)](https://travis-ci.org/Nikea/historydict)
-[![codecov.io](http://codecov.io/github/Nikea/historydict/coverage.svg?branch=master)](http://codecov.io/github/Nikea/historydict?branch=master)
-[![Anaconda-Server Badge](https://anaconda.org/lightsource2/historydict/badges/version.svg)](https://anaconda.org/lightsource2/historydict)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/historydict/badges/version.svg)](https://anaconda.org/conda-forge/historydict)
+
 # HistoryDict
 
 HistoryDict is a light weight mapping backed by sqlite which remember the
 history of values.  The intent is for tracking relatively complex
 configurations.
 
 
 ## Conda Recipes
 
-Install the most recent tagged build: `conda install historydict -c lightsource2-tag`
+Install the most recent tagged build: `conda install historydict -c conda-forge`
 
-Install the most recent tagged build: `conda install historydict -c lightsource2-dev`
+conda-forge feedstock: https://github.com/conda-forge/historydict-feedstock
 
-Find the tagged recipe [here](https://github.com/NSLS-II/lightsource2-recipes/tree/master/recipes-tag/historydict) and the dev recipe [here](https://github.com/NSLS-II/lightsource2-recipes/tree/master/recipes-dev/historydict)
 
 
 ## Examples
 
 The interface is very simple and can be accessed either via `[]` like
 a dictionary
```

