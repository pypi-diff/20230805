# Comparing `tmp/datasette_sqlite_path-0.2.1a1-py3-none-any.whl.zip` & `tmp/datasette_sqlite_path-0.2.1a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2171 bytes, number of entries: 7
--rw-r--r--  2.0 unx      266 b- defN 23-Aug-05 03:01 datasette_sqlite_path/__init__.py
--rw-r--r--  2.0 unx       79 b- defN 23-Aug-05 03:01 datasette_sqlite_path/version.py
--rw-r--r--  2.0 unx      563 b- defN 23-Aug-05 03:01 datasette_sqlite_path-0.2.1a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-05 03:01 datasette_sqlite_path-0.2.1a1.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 23-Aug-05 03:01 datasette_sqlite_path-0.2.1a1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Aug-05 03:01 datasette_sqlite_path-0.2.1a1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      648 b- defN 23-Aug-05 03:01 datasette_sqlite_path-0.2.1a1.dist-info/RECORD
-7 files, 1718 bytes uncompressed, 991 bytes compressed:  42.3%
+Zip file size: 2170 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      266 b- defN 23-Aug-05 03:11 datasette_sqlite_path/__init__.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Aug-05 03:11 datasette_sqlite_path/version.py
+-rw-r--r--  2.0 unx      563 b- defN 23-Aug-05 03:11 datasette_sqlite_path-0.2.1a2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-05 03:11 datasette_sqlite_path-0.2.1a2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 23-Aug-05 03:11 datasette_sqlite_path-0.2.1a2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Aug-05 03:11 datasette_sqlite_path-0.2.1a2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      648 b- defN 23-Aug-05 03:11 datasette_sqlite_path-0.2.1a2.dist-info/RECORD
+7 files, 1718 bytes uncompressed, 990 bytes compressed:  42.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_path/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_path/version.py
 Comment: 
 
-Filename: datasette_sqlite_path-0.2.1a1.dist-info/METADATA
+Filename: datasette_sqlite_path-0.2.1a2.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_path-0.2.1a1.dist-info/WHEEL
+Filename: datasette_sqlite_path-0.2.1a2.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_path-0.2.1a1.dist-info/entry_points.txt
+Filename: datasette_sqlite_path-0.2.1a2.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_path-0.2.1a1.dist-info/top_level.txt
+Filename: datasette_sqlite_path-0.2.1a2.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_path-0.2.1a1.dist-info/RECORD
+Filename: datasette_sqlite_path-0.2.1a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_path/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.2.1-alpha.1"
+__version__ = "0.2.1-alpha.2"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_path-0.2.1a1.dist-info/METADATA` & `datasette_sqlite_path-0.2.1a2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-path
-Version: 0.2.1a1
+Version: 0.2.1a2
 Home-page: https://github.com/asg017/sqlite-path
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-path/issues
 Project-URL: CI, https://github.com/asg017/sqlite-path/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-path/releases
 Requires-Python: >=3.7
```

## Comparing `datasette_sqlite_path-0.2.1a1.dist-info/RECORD` & `datasette_sqlite_path-0.2.1a2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 datasette_sqlite_path/__init__.py,sha256=osdMTJPil1Ppcc-mJ4UMQp-oGKfMOPDyVWLGqPkkq78,266
-datasette_sqlite_path/version.py,sha256=WppcRjRLLKcT4AjiCVj6y2WUrCw5t7pNt9rpyOwDZmE,79
-datasette_sqlite_path-0.2.1a1.dist-info/METADATA,sha256=8sCZxKBqFpMW3UCtkrcrWPRdkpr8Qnm_1fz835PNKlo,563
-datasette_sqlite_path-0.2.1a1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-datasette_sqlite_path-0.2.1a1.dist-info/entry_points.txt,sha256=t24lnlHZ_xRyjyQ6gDYJMK-UBRIjk54QxR3Yi79TWv4,48
-datasette_sqlite_path-0.2.1a1.dist-info/top_level.txt,sha256=EMfolA5zamEfjTvzMVKdVVZIsecWmN4shdy6e5m5QI8,22
-datasette_sqlite_path-0.2.1a1.dist-info/RECORD,,
+datasette_sqlite_path/version.py,sha256=CRIJcMUAZwueE6kdN1m2vVoRLn2LpHt0nta4aK_kq0I,79
+datasette_sqlite_path-0.2.1a2.dist-info/METADATA,sha256=v1I6UDykTta026wQsqNr7O6sCCV9x4qriKSY0pDcuyk,563
+datasette_sqlite_path-0.2.1a2.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+datasette_sqlite_path-0.2.1a2.dist-info/entry_points.txt,sha256=t24lnlHZ_xRyjyQ6gDYJMK-UBRIjk54QxR3Yi79TWv4,48
+datasette_sqlite_path-0.2.1a2.dist-info/top_level.txt,sha256=EMfolA5zamEfjTvzMVKdVVZIsecWmN4shdy6e5m5QI8,22
+datasette_sqlite_path-0.2.1a2.dist-info/RECORD,,
```

