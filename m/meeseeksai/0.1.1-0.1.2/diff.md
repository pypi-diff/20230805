# Comparing `tmp/meeseeksai-0.1.1.tar.gz` & `tmp/meeseeksai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meeseeksai-0.1.1.tar", max compression
+gzip compressed data, was "meeseeksai-0.1.2.tar", max compression
```

## Comparing `meeseeksai-0.1.1.tar` & `meeseeksai-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0        0 2023-08-04 18:37:05.638104 meeseeksai-0.1.1/README.md
--rw-r--r--   0        0        0      122 2023-08-04 22:17:11.485207 meeseeksai-0.1.1/meeseeksai/.env
--rw-r--r--   0        0        0        4 2023-08-04 22:23:44.825126 meeseeksai-0.1.1/meeseeksai/.gitignore
--rw-r--r--   0        0        0        0 2023-08-04 18:37:05.638104 meeseeksai-0.1.1/meeseeksai/__init__.py
--rw-r--r--   0        0        0     1782 2023-08-04 22:19:53.125171 meeseeksai-0.1.1/meeseeksai/meeseeksai.py
--rw-r--r--   0        0        0      356 2023-08-04 22:27:22.495074 meeseeksai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 meeseeksai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-04 18:37:05.638104 meeseeksai-0.1.2/README.md
+-rw-r--r--   0        0        0      122 2023-08-04 22:17:11.485207 meeseeksai-0.1.2/meeseeksai/.env
+-rw-r--r--   0        0        0        0 2023-08-04 18:37:05.638104 meeseeksai-0.1.2/meeseeksai/__init__.py
+-rw-r--r--   0        0        0     1782 2023-08-04 22:19:53.125171 meeseeksai-0.1.2/meeseeksai/meeseeksai.py
+-rw-r--r--   0        0        0      356 2023-08-04 22:28:45.955057 meeseeksai-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 meeseeksai-0.1.2/PKG-INFO
```

### Comparing `meeseeksai-0.1.1/meeseeksai/meeseeksai.py` & `meeseeksai-0.1.2/meeseeksai/meeseeksai.py`

 * *Files identical despite different names*

