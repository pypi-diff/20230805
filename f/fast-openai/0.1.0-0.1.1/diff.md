# Comparing `tmp/fast_openai-0.1.0.tar.gz` & `tmp/fast_openai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_openai-0.1.0.tar", max compression
+gzip compressed data, was "fast_openai-0.1.1.tar", max compression
```

## Comparing `fast_openai-0.1.0.tar` & `fast_openai-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,19 @@
--rw-r--r--   0        0        0        0 2023-08-04 23:36:33.206542 fast_openai-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-08-04 23:36:33.206542 fast_openai-0.1.0/fast_openai/__init__.py
--rw-r--r--   0        0        0      303 2023-08-04 23:36:33.210542 fast_openai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      334 1970-01-01 00:00:00.000000 fast_openai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-04 23:36:33.206542 fast_openai-0.1.1/README.md
+-rw-r--r--   0        0        0       84 2023-08-05 01:00:30.931425 fast_openai-0.1.1/fast_openai/__init__.py
+-rw-r--r--   0        0        0     2110 2023-08-05 02:03:38.737275 fast_openai-0.1.1/fast_openai/application.py
+-rw-r--r--   0        0        0    11120 2023-08-05 01:10:51.203081 fast_openai-0.1.1/fast_openai/client.py
+-rw-r--r--   0        0        0        0 2023-08-04 23:45:49.334138 fast_openai-0.1.1/fast_openai/db/__init__.py
+-rw-r--r--   0        0        0     7771 2023-08-04 23:57:15.297656 fast_openai-0.1.1/fast_openai/db/errors.py
+-rw-r--r--   0        0        0     5659 2023-08-04 23:57:23.389650 fast_openai-0.1.1/fast_openai/db/objects.py
+-rw-r--r--   0        0        0     1637 2023-08-04 23:57:19.373653 fast_openai-0.1.1/fast_openai/db/page.py
+-rw-r--r--   0        0        0    17374 2023-08-04 23:57:19.269653 fast_openai-0.1.1/fast_openai/db/query.py
+-rw-r--r--   0        0        0      231 2023-08-05 00:18:28.264808 fast_openai-0.1.1/fast_openai/fields.py
+-rw-r--r--   0        0        0     6436 2023-08-04 23:57:30.649645 fast_openai-0.1.1/fast_openai/json.py
+-rw-r--r--   0        0        0       55 2023-08-05 00:18:28.264808 fast_openai-0.1.1/fast_openai/llm/__init__.py
+-rw-r--r--   0        0        0    10343 2023-08-05 00:18:28.464808 fast_openai-0.1.1/fast_openai/llm/llm.py
+-rw-r--r--   0        0        0     2381 2023-08-05 00:18:28.332808 fast_openai-0.1.1/fast_openai/llm/schemas.py
+-rw-r--r--   0        0        0     9745 2023-08-05 01:03:16.859335 fast_openai-0.1.1/fast_openai/odm.py
+-rw-r--r--   0        0        0     1941 2023-08-05 00:18:28.364808 fast_openai-0.1.1/fast_openai/typedefs.py
+-rw-r--r--   0        0        0     2914 2023-08-05 02:09:22.633053 fast_openai-0.1.1/fast_openai/utils.py
+-rw-r--r--   0        0        0      519 2023-08-05 02:05:12.629216 fast_openai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 fast_openai-0.1.1/PKG-INFO
```

