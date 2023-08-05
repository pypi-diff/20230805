# Comparing `tmp/nullspace_optimizer-1.1.2.tar.gz` & `tmp/nullspace_optimizer-1.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nullspace_optimizer-1.1.2.tar", last modified: Tue Feb 15 09:12:31 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

