# Comparing `tmp/sqlite_utils_sqlite_path-0.2.0a6-py3-none-any.whl.zip` & `tmp/sqlite_utils_sqlite_path-0.2.1a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2199 bytes, number of entries: 7
--rw-r--r--  2.0 unx      273 b- defN 23-Jul-24 04:22 sqlite_utils_sqlite_path/__init__.py
--rw-r--r--  2.0 unx       79 b- defN 23-Jul-24 04:22 sqlite_utils_sqlite_path/version.py
--rw-r--r--  2.0 unx      516 b- defN 23-Jul-24 04:22 sqlite_utils_sqlite_path-0.2.0a6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 04:22 sqlite_utils_sqlite_path-0.2.0a6.dist-info/WHEEL
--rw-r--r--  2.0 unx       54 b- defN 23-Jul-24 04:22 sqlite_utils_sqlite_path-0.2.0a6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       25 b- defN 23-Jul-24 04:22 sqlite_utils_sqlite_path-0.2.0a6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      669 b- defN 23-Jul-24 04:22 sqlite_utils_sqlite_path-0.2.0a6.dist-info/RECORD
-7 files, 1708 bytes uncompressed, 977 bytes compressed:  42.8%
+Zip file size: 2198 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      273 b- defN 23-Aug-05 03:01 sqlite_utils_sqlite_path/__init__.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Aug-05 03:01 sqlite_utils_sqlite_path/version.py
+-rw-r--r--  2.0 unx      516 b- defN 23-Aug-05 03:01 sqlite_utils_sqlite_path-0.2.1a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-05 03:01 sqlite_utils_sqlite_path-0.2.1a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       54 b- defN 23-Aug-05 03:01 sqlite_utils_sqlite_path-0.2.1a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       25 b- defN 23-Aug-05 03:01 sqlite_utils_sqlite_path-0.2.1a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      669 b- defN 23-Aug-05 03:01 sqlite_utils_sqlite_path-0.2.1a1.dist-info/RECORD
+7 files, 1708 bytes uncompressed, 976 bytes compressed:  42.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: sqlite_utils_sqlite_path/__init__.py
 Comment: 
 
 Filename: sqlite_utils_sqlite_path/version.py
 Comment: 
 
-Filename: sqlite_utils_sqlite_path-0.2.0a6.dist-info/METADATA
+Filename: sqlite_utils_sqlite_path-0.2.1a1.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_utils_sqlite_path-0.2.0a6.dist-info/WHEEL
+Filename: sqlite_utils_sqlite_path-0.2.1a1.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_utils_sqlite_path-0.2.0a6.dist-info/entry_points.txt
+Filename: sqlite_utils_sqlite_path-0.2.1a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: sqlite_utils_sqlite_path-0.2.0a6.dist-info/top_level.txt
+Filename: sqlite_utils_sqlite_path-0.2.1a1.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_utils_sqlite_path-0.2.0a6.dist-info/RECORD
+Filename: sqlite_utils_sqlite_path-0.2.1a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_utils_sqlite_path/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.2.0-alpha.6"
+__version__ = "0.2.1-alpha.1"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_utils_sqlite_path-0.2.0a6.dist-info/METADATA` & `sqlite_utils_sqlite_path-0.2.1a1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-utils-sqlite-path
-Version: 0.2.0a6
+Version: 0.2.1a1
 Summary: TODO
 Author: Alex Garcia
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/asg017/sqlite-path
 Project-URL: Changelog, https://github.com/asg017/sqlite-path/releases
 Project-URL: Issues, https://github.com/asg017/sqlite-path/issues
 Description-Content-Type: text/markdown
```

## Comparing `sqlite_utils_sqlite_path-0.2.0a6.dist-info/RECORD` & `sqlite_utils_sqlite_path-0.2.1a1.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 sqlite_utils_sqlite_path/__init__.py,sha256=Jg7CSD9lnQl9f8RQr-quclP8RMrswmPhSdi3_v8SoZU,273
-sqlite_utils_sqlite_path/version.py,sha256=GPPCcJbIjjy31LREX3juP1vnWG6R2nfVjazgKto0CTY,79
-sqlite_utils_sqlite_path-0.2.0a6.dist-info/METADATA,sha256=2O9fdgP8QPm7MtEijnPoJ1jygjwm3jsrf22yk2QJBaQ,516
-sqlite_utils_sqlite_path-0.2.0a6.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-sqlite_utils_sqlite_path-0.2.0a6.dist-info/entry_points.txt,sha256=ZM_mWXkvs2eISOe0vu2rDrVmZchh6scSDnJ6EnT4bsQ,54
-sqlite_utils_sqlite_path-0.2.0a6.dist-info/top_level.txt,sha256=pM-fKSaZT0qOetpznHBpN-VXp9GvBoFRR1FBOaFQNTo,25
-sqlite_utils_sqlite_path-0.2.0a6.dist-info/RECORD,,
+sqlite_utils_sqlite_path/version.py,sha256=WppcRjRLLKcT4AjiCVj6y2WUrCw5t7pNt9rpyOwDZmE,79
+sqlite_utils_sqlite_path-0.2.1a1.dist-info/METADATA,sha256=AUGcAJGKCnvp1GathejoavthcgNu5vlCSxtmKVW9Ccg,516
+sqlite_utils_sqlite_path-0.2.1a1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+sqlite_utils_sqlite_path-0.2.1a1.dist-info/entry_points.txt,sha256=ZM_mWXkvs2eISOe0vu2rDrVmZchh6scSDnJ6EnT4bsQ,54
+sqlite_utils_sqlite_path-0.2.1a1.dist-info/top_level.txt,sha256=pM-fKSaZT0qOetpznHBpN-VXp9GvBoFRR1FBOaFQNTo,25
+sqlite_utils_sqlite_path-0.2.1a1.dist-info/RECORD,,
```

