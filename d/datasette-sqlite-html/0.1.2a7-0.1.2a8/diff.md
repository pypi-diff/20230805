# Comparing `tmp/datasette_sqlite_html-0.1.2a7-py3-none-any.whl.zip` & `tmp/datasette_sqlite_html-0.1.2a8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 2173 bytes, number of entries: 7
--rw-r--r--  2.0 unx      266 b- defN 23-Jun-10 22:16 datasette_sqlite_html/__init__.py
--rw-r--r--  2.0 unx       79 b- defN 23-Jun-10 22:16 datasette_sqlite_html/version.py
--rw-r--r--  2.0 unx      563 b- defN 23-Jun-10 22:17 datasette_sqlite_html-0.1.2a7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-10 22:17 datasette_sqlite_html-0.1.2a7.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 23-Jun-10 22:17 datasette_sqlite_html-0.1.2a7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-10 22:17 datasette_sqlite_html-0.1.2a7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      648 b- defN 23-Jun-10 22:17 datasette_sqlite_html-0.1.2a7.dist-info/RECORD
+-rw-r--r--  2.0 unx      266 b- defN 23-Aug-05 03:34 datasette_sqlite_html/__init__.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Aug-05 03:34 datasette_sqlite_html/version.py
+-rw-r--r--  2.0 unx      563 b- defN 23-Aug-05 03:34 datasette_sqlite_html-0.1.2a8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-05 03:34 datasette_sqlite_html-0.1.2a8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 23-Aug-05 03:34 datasette_sqlite_html-0.1.2a8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Aug-05 03:34 datasette_sqlite_html-0.1.2a8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      648 b- defN 23-Aug-05 03:34 datasette_sqlite_html-0.1.2a8.dist-info/RECORD
 7 files, 1718 bytes uncompressed, 993 bytes compressed:  42.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_html/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_html/version.py
 Comment: 
 
-Filename: datasette_sqlite_html-0.1.2a7.dist-info/METADATA
+Filename: datasette_sqlite_html-0.1.2a8.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_html-0.1.2a7.dist-info/WHEEL
+Filename: datasette_sqlite_html-0.1.2a8.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_html-0.1.2a7.dist-info/entry_points.txt
+Filename: datasette_sqlite_html-0.1.2a8.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_html-0.1.2a7.dist-info/top_level.txt
+Filename: datasette_sqlite_html-0.1.2a8.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_html-0.1.2a7.dist-info/RECORD
+Filename: datasette_sqlite_html-0.1.2a8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_html/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.2-alpha.7"
+__version__ = "0.1.2-alpha.8"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_html-0.1.2a7.dist-info/METADATA` & `datasette_sqlite_html-0.1.2a8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-html
-Version: 0.1.2a7
+Version: 0.1.2a8
 Home-page: https://github.com/asg017/sqlite-html
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-html/issues
 Project-URL: CI, https://github.com/asg017/sqlite-html/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-html/releases
 Requires-Python: >=3.7
```

## Comparing `datasette_sqlite_html-0.1.2a7.dist-info/RECORD` & `datasette_sqlite_html-0.1.2a8.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 datasette_sqlite_html/__init__.py,sha256=ziq-rB8yRAubkqikIZWqeA0LneQKWCSDJnOW7xBsbCk,266
-datasette_sqlite_html/version.py,sha256=sewLkTuz4MzoIX27O70vwieFrURFWOTwyl_IP50Hp5g,79
-datasette_sqlite_html-0.1.2a7.dist-info/METADATA,sha256=uW4cn3SgjgOHa5exRfQ3K2srprcDUFoaGR6dc5dEO2w,563
-datasette_sqlite_html-0.1.2a7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-datasette_sqlite_html-0.1.2a7.dist-info/entry_points.txt,sha256=Ty_dShJsQ23N4JA2PDKNMxbZ5bPiqj27zovbiCDI39I,48
-datasette_sqlite_html-0.1.2a7.dist-info/top_level.txt,sha256=bWwftX05h2WWmdOY-2uemMvvSCnkABrOTsdkOEgVOEg,22
-datasette_sqlite_html-0.1.2a7.dist-info/RECORD,,
+datasette_sqlite_html/version.py,sha256=a6ilR6CjxR9StqOMKXCV6EhiUw099cJdEQ9WT0X2X4o,79
+datasette_sqlite_html-0.1.2a8.dist-info/METADATA,sha256=i74VcLHY2IqGVxG-ABbsbloOjCOT7TcYtXHn1sCM5nk,563
+datasette_sqlite_html-0.1.2a8.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+datasette_sqlite_html-0.1.2a8.dist-info/entry_points.txt,sha256=Ty_dShJsQ23N4JA2PDKNMxbZ5bPiqj27zovbiCDI39I,48
+datasette_sqlite_html-0.1.2a8.dist-info/top_level.txt,sha256=bWwftX05h2WWmdOY-2uemMvvSCnkABrOTsdkOEgVOEg,22
+datasette_sqlite_html-0.1.2a8.dist-info/RECORD,,
```

