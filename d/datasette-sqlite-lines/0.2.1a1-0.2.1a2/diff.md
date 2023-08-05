# Comparing `tmp/datasette_sqlite_lines-0.2.1a1-py3-none-any.whl.zip` & `tmp/datasette_sqlite_lines-0.2.1a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 2294 bytes, number of entries: 7
--rw-r--r--  2.0 unx      515 b- defN 23-Aug-05 03:54 datasette_sqlite_lines/__init__.py
--rw-r--r--  2.0 unx       79 b- defN 23-Aug-05 03:54 datasette_sqlite_lines/version.py
--rw-r--r--  2.0 unx      569 b- defN 23-Aug-05 03:54 datasette_sqlite_lines-0.2.1a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-05 03:54 datasette_sqlite_lines-0.2.1a1.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 23-Aug-05 03:54 datasette_sqlite_lines-0.2.1a1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 23-Aug-05 03:54 datasette_sqlite_lines-0.2.1a1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      655 b- defN 23-Aug-05 03:54 datasette_sqlite_lines-0.2.1a1.dist-info/RECORD
+-rw-r--r--  2.0 unx      515 b- defN 23-Aug-05 03:57 datasette_sqlite_lines/__init__.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Aug-05 03:57 datasette_sqlite_lines/version.py
+-rw-r--r--  2.0 unx      569 b- defN 23-Aug-05 03:57 datasette_sqlite_lines-0.2.1a2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-05 03:57 datasette_sqlite_lines-0.2.1a2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 23-Aug-05 03:57 datasette_sqlite_lines-0.2.1a2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-Aug-05 03:57 datasette_sqlite_lines-0.2.1a2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      655 b- defN 23-Aug-05 03:57 datasette_sqlite_lines-0.2.1a2.dist-info/RECORD
 7 files, 1983 bytes uncompressed, 1100 bytes compressed:  44.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_lines/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_lines/version.py
 Comment: 
 
-Filename: datasette_sqlite_lines-0.2.1a1.dist-info/METADATA
+Filename: datasette_sqlite_lines-0.2.1a2.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_lines-0.2.1a1.dist-info/WHEEL
+Filename: datasette_sqlite_lines-0.2.1a2.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_lines-0.2.1a1.dist-info/entry_points.txt
+Filename: datasette_sqlite_lines-0.2.1a2.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_lines-0.2.1a1.dist-info/top_level.txt
+Filename: datasette_sqlite_lines-0.2.1a2.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_lines-0.2.1a1.dist-info/RECORD
+Filename: datasette_sqlite_lines-0.2.1a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_lines/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.2.1-alpha.1"
+__version__ = "0.2.1-alpha.2"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_lines-0.2.1a1.dist-info/METADATA` & `datasette_sqlite_lines-0.2.1a2.dist-info/METADATA`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-lines
-Version: 0.2.1a1
+Version: 0.2.1a2
 Home-page: https://github.com/asg017/sqlite-lines
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-lines/issues
 Project-URL: CI, https://github.com/asg017/sqlite-lines/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-lines/releases
 Requires-Python: >=3.7
```

## Comparing `datasette_sqlite_lines-0.2.1a1.dist-info/RECORD` & `datasette_sqlite_lines-0.2.1a2.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 datasette_sqlite_lines/__init__.py,sha256=IVoGo6FxLmgeAYuy8my_SVqau7RS9lnkAZu9JJ2u8_4,515
-datasette_sqlite_lines/version.py,sha256=WppcRjRLLKcT4AjiCVj6y2WUrCw5t7pNt9rpyOwDZmE,79
-datasette_sqlite_lines-0.2.1a1.dist-info/METADATA,sha256=miDDRjyFPktY_bN4J0Y8xhMv7XeuDWqYvDy2hFJN09g,569
-datasette_sqlite_lines-0.2.1a1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-datasette_sqlite_lines-0.2.1a1.dist-info/entry_points.txt,sha256=Z2nWqfeSXw3d4dsEsZy2O2e2J1uSU472UOJqHKxJ1Zk,50
-datasette_sqlite_lines-0.2.1a1.dist-info/top_level.txt,sha256=jjwGSIqlzC1NIT-yOeknY_wyjRTMY1UhUFKAMmb1U9E,23
-datasette_sqlite_lines-0.2.1a1.dist-info/RECORD,,
+datasette_sqlite_lines/version.py,sha256=CRIJcMUAZwueE6kdN1m2vVoRLn2LpHt0nta4aK_kq0I,79
+datasette_sqlite_lines-0.2.1a2.dist-info/METADATA,sha256=dCPwDABEpNg8w_4aI3qittZEwsiyUl3V17zjXl01sSU,569
+datasette_sqlite_lines-0.2.1a2.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+datasette_sqlite_lines-0.2.1a2.dist-info/entry_points.txt,sha256=Z2nWqfeSXw3d4dsEsZy2O2e2J1uSU472UOJqHKxJ1Zk,50
+datasette_sqlite_lines-0.2.1a2.dist-info/top_level.txt,sha256=jjwGSIqlzC1NIT-yOeknY_wyjRTMY1UhUFKAMmb1U9E,23
+datasette_sqlite_lines-0.2.1a2.dist-info/RECORD,,
```

