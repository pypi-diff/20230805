# Comparing `tmp/akrophonobolos-0.0.2.tar.gz` & `tmp/akrophonobolos-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akrophonobolos-0.0.2.tar", last modified: Mon Nov 22 15:10:30 2021, max compression
+gzip compressed data, was "akrophonobolos-1.0.0.tar", last modified: Sat Aug  5 01:06:33 2023, max compression
```

## Comparing `akrophonobolos-0.0.2.tar` & `akrophonobolos-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 seanredmond   (505) staff       (20)        0 2021-11-22 15:10:30.246443 akrophonobolos-0.0.2/
--rw-r--r--   0 seanredmond   (505) staff       (20)    35137 2021-11-18 01:55:06.000000 akrophonobolos-0.0.2/LICENSE
--rw-r--r--   0 seanredmond   (505) staff       (20)    11594 2021-11-22 15:10:30.246528 akrophonobolos-0.0.2/PKG-INFO
--rw-r--r--   0 seanredmond   (505) staff       (20)    10979 2021-11-21 23:11:00.000000 akrophonobolos-0.0.2/README.md
-drwxr-xr-x   0 seanredmond   (505) staff       (20)        0 2021-11-22 15:10:30.245418 akrophonobolos-0.0.2/akrophonobolos/
--rw-r--r--   0 seanredmond   (505) staff       (20)       30 2021-06-15 21:40:23.000000 akrophonobolos-0.0.2/akrophonobolos/__init__.py
--rw-r--r--   0 seanredmond   (505) staff       (20)       63 2021-11-22 15:01:18.000000 akrophonobolos-0.0.2/akrophonobolos/__version__.py
--rw-r--r--   0 seanredmond   (505) staff       (20)    13016 2021-11-22 14:53:22.000000 akrophonobolos-0.0.2/akrophonobolos/akrophonobolos.py
--rw-r--r--   0 seanredmond   (505) staff       (20)     3656 2021-11-21 01:44:50.000000 akrophonobolos-0.0.2/akrophonobolos/logistes.py
--rw-r--r--   0 seanredmond   (505) staff       (20)     1760 2021-11-21 01:43:36.000000 akrophonobolos-0.0.2/akrophonobolos/obol.py
-drwxr-xr-x   0 seanredmond   (505) staff       (20)        0 2021-11-22 15:10:30.245934 akrophonobolos-0.0.2/akrophonobolos.egg-info/
--rw-r--r--   0 seanredmond   (505) staff       (20)    11594 2021-11-22 15:10:30.000000 akrophonobolos-0.0.2/akrophonobolos.egg-info/PKG-INFO
--rw-r--r--   0 seanredmond   (505) staff       (20)      464 2021-11-22 15:10:30.000000 akrophonobolos-0.0.2/akrophonobolos.egg-info/SOURCES.txt
--rw-r--r--   0 seanredmond   (505) staff       (20)        1 2021-11-22 15:10:30.000000 akrophonobolos-0.0.2/akrophonobolos.egg-info/dependency_links.txt
--rw-r--r--   0 seanredmond   (505) staff       (20)       91 2021-11-22 15:10:30.000000 akrophonobolos-0.0.2/akrophonobolos.egg-info/entry_points.txt
--rw-r--r--   0 seanredmond   (505) staff       (20)       21 2021-11-22 15:10:30.000000 akrophonobolos-0.0.2/akrophonobolos.egg-info/top_level.txt
--rw-r--r--   0 seanredmond   (505) staff       (20)      103 2021-06-18 15:06:50.000000 akrophonobolos-0.0.2/pyproject.toml
--rw-r--r--   0 seanredmond   (505) staff       (20)      761 2021-11-22 15:10:30.246811 akrophonobolos-0.0.2/setup.cfg
-drwxr-xr-x   0 seanredmond   (505) staff       (20)        0 2021-11-22 15:10:30.246353 akrophonobolos-0.0.2/tests/
--rw-r--r--   0 seanredmond   (505) staff       (20)        0 2021-06-15 21:41:33.000000 akrophonobolos-0.0.2/tests/__init__.py
--rw-r--r--   0 seanredmond   (505) staff       (20)     4713 2021-11-22 14:19:29.000000 akrophonobolos-0.0.2/tests/test_class.py
--rw-r--r--   0 seanredmond   (505) staff       (20)     8659 2021-11-22 15:01:05.000000 akrophonobolos-0.0.2/tests/test_functions.py
--rw-r--r--   0 seanredmond   (505) staff       (20)     2112 2021-11-21 01:49:22.000000 akrophonobolos-0.0.2/tests/test_inscriptions.py
+drwxr-xr-x   0 seanredmond   (505) staff       (20)        0 2023-08-05 01:06:33.139415 akrophonobolos-1.0.0/
+-rw-r--r--   0 seanredmond   (505) staff       (20)    35137 2021-11-18 01:55:06.000000 akrophonobolos-1.0.0/LICENSE
+-rw-r--r--   0 seanredmond   (505) staff       (20)     3501 2023-08-05 01:06:33.139490 akrophonobolos-1.0.0/PKG-INFO
+-rw-r--r--   0 seanredmond   (505) staff       (20)     2923 2023-08-05 00:21:35.000000 akrophonobolos-1.0.0/README.md
+drwxr-xr-x   0 seanredmond   (505) staff       (20)        0 2023-08-05 01:06:33.138160 akrophonobolos-1.0.0/akrophonobolos/
+-rw-r--r--   0 seanredmond   (505) staff       (20)      168 2023-08-04 23:38:48.000000 akrophonobolos-1.0.0/akrophonobolos/__init__.py
+-rw-r--r--   0 seanredmond   (505) staff       (20)       63 2023-08-05 01:03:30.000000 akrophonobolos-1.0.0/akrophonobolos/__version__.py
+-rw-r--r--   0 seanredmond   (505) staff       (20)    15720 2023-08-04 23:38:48.000000 akrophonobolos-1.0.0/akrophonobolos/akrophonobolos.py
+-rw-r--r--   0 seanredmond   (505) staff       (20)     3656 2021-11-21 01:44:50.000000 akrophonobolos-1.0.0/akrophonobolos/logistes.py
+-rw-r--r--   0 seanredmond   (505) staff       (20)     1760 2021-11-21 01:43:36.000000 akrophonobolos-1.0.0/akrophonobolos/obol.py
+drwxr-xr-x   0 seanredmond   (505) staff       (20)        0 2023-08-05 01:06:33.138845 akrophonobolos-1.0.0/akrophonobolos.egg-info/
+-rw-r--r--   0 seanredmond   (505) staff       (20)     3501 2023-08-05 01:06:33.000000 akrophonobolos-1.0.0/akrophonobolos.egg-info/PKG-INFO
+-rw-r--r--   0 seanredmond   (505) staff       (20)      464 2023-08-05 01:06:33.000000 akrophonobolos-1.0.0/akrophonobolos.egg-info/SOURCES.txt
+-rw-r--r--   0 seanredmond   (505) staff       (20)        1 2023-08-05 01:06:33.000000 akrophonobolos-1.0.0/akrophonobolos.egg-info/dependency_links.txt
+-rw-r--r--   0 seanredmond   (505) staff       (20)       90 2023-08-05 01:06:33.000000 akrophonobolos-1.0.0/akrophonobolos.egg-info/entry_points.txt
+-rw-r--r--   0 seanredmond   (505) staff       (20)       21 2023-08-05 01:06:33.000000 akrophonobolos-1.0.0/akrophonobolos.egg-info/top_level.txt
+-rw-r--r--   0 seanredmond   (505) staff       (20)      103 2021-06-18 15:06:50.000000 akrophonobolos-1.0.0/pyproject.toml
+-rw-r--r--   0 seanredmond   (505) staff       (20)      761 2023-08-05 01:06:33.139765 akrophonobolos-1.0.0/setup.cfg
+drwxr-xr-x   0 seanredmond   (505) staff       (20)        0 2023-08-05 01:06:33.139325 akrophonobolos-1.0.0/tests/
+-rw-r--r--   0 seanredmond   (505) staff       (20)        0 2021-06-15 21:41:33.000000 akrophonobolos-1.0.0/tests/__init__.py
+-rw-r--r--   0 seanredmond   (505) staff       (20)     4713 2021-11-22 14:19:29.000000 akrophonobolos-1.0.0/tests/test_class.py
+-rw-r--r--   0 seanredmond   (505) staff       (20)     8659 2023-08-05 01:04:47.000000 akrophonobolos-1.0.0/tests/test_functions.py
+-rw-r--r--   0 seanredmond   (505) staff       (20)     2112 2021-11-21 01:49:22.000000 akrophonobolos-1.0.0/tests/test_inscriptions.py
```

### Comparing `akrophonobolos-0.0.2/LICENSE` & `akrophonobolos-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `akrophonobolos-0.0.2/akrophonobolos/logistes.py` & `akrophonobolos-1.0.0/akrophonobolos/logistes.py`

 * *Files identical despite different names*

### Comparing `akrophonobolos-0.0.2/akrophonobolos/obol.py` & `akrophonobolos-1.0.0/akrophonobolos/obol.py`

 * *Files identical despite different names*

### Comparing `akrophonobolos-0.0.2/setup.cfg` & `akrophonobolos-1.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = akrophonobolos
-version = 0.0.2
+version = 1.0.0
 author = Sean Redmond
 author_email = github-smr@sneakemail.com
 description = Ancient Athenian acrophonic numeral converter
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/seanredmond/Akrophonobolos
 project_urls =
```

### Comparing `akrophonobolos-0.0.2/tests/test_class.py` & `akrophonobolos-1.0.0/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `akrophonobolos-0.0.2/tests/test_functions.py` & `akrophonobolos-1.0.0/tests/test_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import akrophonobolos as obol
 from fractions import Fraction
 
 
 def test_version():
-    assert obol.version() == "0.0.2"
+    assert obol.version() == "1.0.0"
 
 
 def test_parse_amt():
     assert obol.parse_amount("1T") == 36_000
     assert obol.parse_amount("1t") == 36_000
     assert obol.parse_amount("813D") == 4_878
     assert obol.parse_amount("813d") == 4_878
```

### Comparing `akrophonobolos-0.0.2/tests/test_inscriptions.py` & `akrophonobolos-1.0.0/tests/test_inscriptions.py`

 * *Files identical despite different names*

