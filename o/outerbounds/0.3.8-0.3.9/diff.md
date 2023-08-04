# Comparing `tmp/outerbounds-0.3.8-py3-none-any.whl.zip` & `tmp/outerbounds-0.3.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 5334 bytes, number of entries: 5
+Zip file size: 5335 bytes, number of entries: 5
 -rw-r--r--  2.0 unx    13611 b- defN 80-Jan-01 00:00 outerbounds/__init__.py
-?rw-r--r--  2.0 unx       47 b- defN 16-Jan-01 00:00 outerbounds-0.3.8.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 outerbounds-0.3.8.dist-info/WHEEL
-?rw-r--r--  2.0 unx      872 b- defN 16-Jan-01 00:00 outerbounds-0.3.8.dist-info/METADATA
-?rw-r--r--  2.0 unx      397 b- defN 16-Jan-01 00:00 outerbounds-0.3.8.dist-info/RECORD
-5 files, 15015 bytes uncompressed, 4592 bytes compressed:  69.4%
+?rw-r--r--  2.0 unx       47 b- defN 16-Jan-01 00:00 outerbounds-0.3.9.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 outerbounds-0.3.9.dist-info/WHEEL
+?rw-r--r--  2.0 unx      872 b- defN 16-Jan-01 00:00 outerbounds-0.3.9.dist-info/METADATA
+?rw-r--r--  2.0 unx      397 b- defN 16-Jan-01 00:00 outerbounds-0.3.9.dist-info/RECORD
+5 files, 15015 bytes uncompressed, 4593 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: outerbounds/__init__.py
 Comment: 
 
-Filename: outerbounds-0.3.8.dist-info/entry_points.txt
+Filename: outerbounds-0.3.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: outerbounds-0.3.8.dist-info/WHEEL
+Filename: outerbounds-0.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: outerbounds-0.3.8.dist-info/METADATA
+Filename: outerbounds-0.3.9.dist-info/METADATA
 Comment: 
 
-Filename: outerbounds-0.3.8.dist-info/RECORD
+Filename: outerbounds-0.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `outerbounds-0.3.8.dist-info/METADATA` & `outerbounds-0.3.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: outerbounds
-Version: 0.3.8
+Version: 0.3.9
 Summary: More Data Science, Less Administration
 License: Proprietary
 Keywords: data science,machine learning,MLOps
 Author: Outerbounds, Inc.
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: ob-metaflow (==2.7.19.7)
-Requires-Dist: ob-metaflow-extensions (==1.1.7)
+Requires-Dist: ob-metaflow-extensions (==1.1.8)
 Requires-Dist: opentelemetry-distro (==0.35b0)
 Requires-Dist: opentelemetry-exporter-otlp-proto-http (==1.15.0)
 Requires-Dist: opentelemetry-instrumentation-requests (==0.35b0)
 Project-URL: Documentation, https://docs.metaflow.org
```

