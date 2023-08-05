# Comparing `tmp/txt2voice-0.1.0.tar.gz` & `tmp/txt2voice-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txt2voice-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "txt2voice-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `txt2voice-0.1.0.tar` & `txt2voice-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,16 @@
--rw-r--r--   0        0        0     3084 2023-08-01 15:01:24.365668 txt2voice-0.1.0/.gitignore
--rw-r--r--   0        0        0      141 2023-08-01 14:58:36.076837 txt2voice-0.1.0/.pypirc
--rw-r--r--   0        0        0     1063 2023-08-01 14:43:47.100965 txt2voice-0.1.0/LICENSE
--rw-r--r--   0        0        0       89 2023-08-01 14:43:47.101088 txt2voice-0.1.0/README.md
--rw-r--r--   0        0        0      362 2023-08-01 15:13:18.727536 txt2voice-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      141 2023-08-01 15:02:11.990079 txt2voice-0.1.0/txt2voice/__init__.py
--rw-r--r--   0        0        0      351 1970-01-01 00:00:00.000000 txt2voice-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       49 2023-08-05 07:33:00.398238 txt2voice-0.1.1/.flake8
+-rw-r--r--   0        0        0      894 2023-08-05 07:33:00.398238 txt2voice-0.1.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      661 2023-08-05 07:33:00.398238 txt2voice-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     3094 2023-08-05 07:33:00.398238 txt2voice-0.1.1/.gitignore
+-rw-r--r--   0        0        0      121 2023-08-05 07:33:00.398238 txt2voice-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1063 2023-08-05 07:33:00.398238 txt2voice-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1333 2023-08-05 07:33:00.398238 txt2voice-0.1.1/Makefile
+-rw-r--r--   0        0        0     2929 2023-08-05 07:33:00.398238 txt2voice-0.1.1/README.md
+-rw-r--r--   0        0        0      563 2023-08-05 07:33:00.398238 txt2voice-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-05 07:33:00.398238 txt2voice-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     3467 2023-08-05 07:33:00.398238 txt2voice-0.1.1/tests/test_api.py
+-rw-r--r--   0        0        0      463 2023-08-05 07:33:00.398238 txt2voice-0.1.1/tox.ini
+-rw-r--r--   0        0        0       51 2023-08-05 07:33:00.402238 txt2voice-0.1.1/txt2voice/__init__.py
+-rw-r--r--   0        0        0     2521 2023-08-05 07:33:00.402238 txt2voice-0.1.1/txt2voice/api.py
+-rw-r--r--   0        0        0      874 2023-08-05 07:33:00.402238 txt2voice-0.1.1/txt2voice/models.py
+-rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 txt2voice-0.1.1/PKG-INFO
```

### Comparing `txt2voice-0.1.0/.gitignore` & `txt2voice-0.1.1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.DS_Store
 .idea
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `txt2voice-0.1.0/LICENSE` & `txt2voice-0.1.1/LICENSE`

 * *Files identical despite different names*

