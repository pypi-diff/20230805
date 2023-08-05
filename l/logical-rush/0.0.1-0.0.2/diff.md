# Comparing `tmp/logical_rush-0.0.1-py3-none-any.whl.zip` & `tmp/logical_rush-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,9 @@
-Zip file size: 2522 bytes, number of entries: 5
+Zip file size: 776819 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat      131 b- defN 23-Jun-16 01:14 logical_rush/__init__.py
--rw-rw-rw-  2.0 fat     3502 b- defN 23-Aug-05 15:19 logical_rush-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-05 15:19 logical_rush-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Aug-05 15:19 logical_rush-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      398 b- defN 23-Aug-05 15:19 logical_rush-0.0.1.dist-info/RECORD
-5 files, 4136 bytes uncompressed, 1776 bytes compressed:  57.1%
+-rw-rw-rw-  2.0 fat  1508352 b- defN 23-Jun-16 01:14 logical_rush/logical_rush.cp310-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   793088 b- defN 23-May-02 17:20 logical_rush/logical_rush.so
+-rw-rw-rw-  2.0 fat     3502 b- defN 23-Aug-05 15:49 logical_rush-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-05 15:49 logical_rush-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Aug-05 15:49 logical_rush-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      590 b- defN 23-Aug-05 15:49 logical_rush-0.0.2.dist-info/RECORD
+7 files, 2305768 bytes uncompressed, 775775 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -1,16 +1,22 @@
 Filename: logical_rush/__init__.py
 Comment: 
 
-Filename: logical_rush-0.0.1.dist-info/METADATA
+Filename: logical_rush/logical_rush.cp310-win_amd64.pyd
 Comment: 
 
-Filename: logical_rush-0.0.1.dist-info/WHEEL
+Filename: logical_rush/logical_rush.so
 Comment: 
 
-Filename: logical_rush-0.0.1.dist-info/top_level.txt
+Filename: logical_rush-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: logical_rush-0.0.1.dist-info/RECORD
+Filename: logical_rush-0.0.2.dist-info/WHEEL
+Comment: 
+
+Filename: logical_rush-0.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: logical_rush-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `logical_rush-0.0.1.dist-info/METADATA` & `logical_rush-0.0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logical-rush
-Version: 0.0.1
+Version: 0.0.2
 Summary: Batch-computing solution for cashflow calculations.
 Author: Blasser Analytica (Rodolfo Blasser)
 Author-email: <rodolfoblasser@gmail.com>
 Keywords: python,panama,finance,stocks,fixed income,data,api,market data,latinex
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

