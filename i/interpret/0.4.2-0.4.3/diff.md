# Comparing `tmp/interpret-0.4.2.tar.gz` & `tmp/interpret-0.4.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interpret-0.4.2.tar", last modified: Thu Jun  1 03:28:16 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

