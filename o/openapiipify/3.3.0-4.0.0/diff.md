# Comparing `tmp/openapiipify-3.3.0.tar.gz` & `tmp/openapiipify-4.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapiipify-3.3.0.tar", last modified: Sat Nov 19 12:44:53 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

