# Comparing `tmp/datahammer-1.0.2.tar.gz` & `tmp/datahammer-1.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datahammer-1.0.2.tar", last modified: Thu Aug 16 15:00:55 2018, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

