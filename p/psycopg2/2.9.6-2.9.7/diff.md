# Comparing `tmp/psycopg2-2.9.6.tar.gz` & `tmp/psycopg2-2.9.7-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psycopg2-2.9.6.tar", last modified: Sun Apr  2 15:59:20 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

