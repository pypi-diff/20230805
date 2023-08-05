# Comparing `tmp/up2b-0.7.1a4.tar.gz` & `tmp/up2b-0.7.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up2b-0.7.1a4.tar", last modified: Sun Jul 16 02:05:46 2023, max compression
+gzip compressed data, was "up2b-0.7.1a5.tar", last modified: Sat Aug  5 06:47:10 2023, max compression
```

## Comparing `up2b-0.7.1a4.tar` & `up2b-0.7.1a5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:05:46.941675 up2b-0.7.1a4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:05:46.925675 up2b-0.7.1a4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:05:46.933675 up2b-0.7.1a4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-16 02:05:34.000000 up2b-0.7.1a4/.github/workflows/check.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-16 02:05:34.000000 up2b-0.7.1a4/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-16 02:05:34.000000 up2b-0.7.1a4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-16 02:05:34.000000 up2b-0.7.1a4/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-16 02:05:34.000000 up2b-0.7.1a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-07-16 02:05:46.941675 up2b-0.7.1a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-07-16 02:05:34.000000 up2b-0.7.1a4/README.en_US.md
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-16 02:05:34.000000 up2b-0.7.1a4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-16 02:05:34.000000 up2b-0.7.1a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-16 02:05:34.000000 up2b-0.7.1a4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 02:05:46.941675 up2b-0.7.1a4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:05:46.933675 up2b-0.7.1a4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-16 02:05:34.000000 up2b-0.7.1a4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:05:46.933675 up2b-0.7.1a4/tests/images/
--rw-r--r--   0 runner    (1001) docker     (123)    28768 2023-07-16 02:05:34.000000 up2b-0.7.1a4/tests/images/1.png
--rw-r--r--   0 runner    (1001) docker     (123)   142746 2023-07-16 02:05:34.000000 up2b-0.7.1a4/tests/images/2.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    36038 2023-07-16 02:05:34.000000 up2b-0.7.1a4/tests/images/3.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-16 02:05:34.000000 up2b-0.7.1a4/tests/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-16 02:05:34.000000 up2b-0.7.1a4/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-16 02:05:34.000000 up2b-0.7.1a4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-16 02:05:34.000000 up2b-0.7.1a4/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:05:46.933675 up2b-0.7.1a4/up2b/
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:05:46.941675 up2b-0.7.1a4/up2b/up2b_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/log.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:05:46.941675 up2b-0.7.1a4/up2b/up2b_lib/up2b_api/
--rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/up2b_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/up2b_api/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/up2b_api/github.py
--rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/up2b_api/imgtg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/up2b_api/imgtu.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/up2b_api/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/up2b_api/sm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/watermark.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-16 02:05:46.000000 up2b-0.7.1a4/up2b/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:05:46.937675 up2b-0.7.1a4/up2b.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-07-16 02:05:46.000000 up2b-0.7.1a4/up2b.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-16 02:05:46.000000 up2b-0.7.1a4/up2b.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 02:05:46.000000 up2b-0.7.1a4/up2b.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-16 02:05:46.000000 up2b-0.7.1a4/up2b.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-16 02:05:46.000000 up2b-0.7.1a4/up2b.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-16 02:05:46.000000 up2b-0.7.1a4/up2b.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:47:10.484478 up2b-0.7.1a5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:47:10.468478 up2b-0.7.1a5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:47:10.472478 up2b-0.7.1a5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-08-05 06:47:00.000000 up2b-0.7.1a5/.github/workflows/check.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-05 06:47:00.000000 up2b-0.7.1a5/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-05 06:47:00.000000 up2b-0.7.1a5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-05 06:47:00.000000 up2b-0.7.1a5/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-05 06:47:00.000000 up2b-0.7.1a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-08-05 06:47:10.484478 up2b-0.7.1a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-08-05 06:47:00.000000 up2b-0.7.1a5/README.en_US.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-08-05 06:47:00.000000 up2b-0.7.1a5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-05 06:47:00.000000 up2b-0.7.1a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-05 06:47:00.000000 up2b-0.7.1a5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 06:47:10.484478 up2b-0.7.1a5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:47:10.472478 up2b-0.7.1a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-05 06:47:00.000000 up2b-0.7.1a5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:47:10.472478 up2b-0.7.1a5/tests/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    28768 2023-08-05 06:47:00.000000 up2b-0.7.1a5/tests/images/1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   142746 2023-08-05 06:47:00.000000 up2b-0.7.1a5/tests/images/2.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    36038 2023-08-05 06:47:00.000000 up2b-0.7.1a5/tests/images/3.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-08-05 06:47:00.000000 up2b-0.7.1a5/tests/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-08-05 06:47:00.000000 up2b-0.7.1a5/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-08-05 06:47:00.000000 up2b-0.7.1a5/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-05 06:47:00.000000 up2b-0.7.1a5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:47:10.476478 up2b-0.7.1a5/up2b/
+-rw-r--r--   0 runner    (1001) docker     (123)     9331 2023-08-05 06:47:00.000000 up2b-0.7.1a5/up2b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-05 06:47:00.000000 up2b-0.7.1a5/up2b/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-05 06:47:00.000000 up2b-0.7.1a5/up2b/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:47:10.480478 up2b-0.7.1a5/up2b/up2b_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-05 06:47:00.000000 up2b-0.7.1a5/up2b/up2b_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-08-05 06:47:00.000000 up2b-0.7.1a5/up2b/up2b_lib/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-08-05 06:47:00.000000 up2b-0.7.1a5/up2b/up2b_lib/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-05 06:47:00.000000 up2b-0.7.1a5/up2b/up2b_lib/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-05 06:47:00.000000 up2b-0.7.1a5/up2b/up2b_lib/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-08-05 06:47:00.000000 up2b-0.7.1a5/up2b/up2b_lib/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-05 06:47:00.000000 up2b-0.7.1a5/up2b/up2b_lib/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-05 06:47:00.000000 up2b-0.7.1a5/up2b/up2b_lib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:47:10.484478 up2b-0.7.1a5/up2b/up2b_lib/up2b_api/
+-rw-r--r--   0 runner    (1001) docker     (123)    16403 2023-08-05 06:47:00.000000 up2b-0.7.1a5/up2b/up2b_lib/up2b_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-08-05 06:47:00.000000 up2b-0.7.1a5/up2b/up2b_lib/up2b_api/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-08-05 06:47:00.000000 up2b-0.7.1a5/up2b/up2b_lib/up2b_api/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-08-05 06:47:00.000000 up2b-0.7.1a5/up2b/up2b_lib/up2b_api/imgtg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-08-05 06:47:00.000000 up2b-0.7.1a5/up2b/up2b_lib/up2b_api/imgtu.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-05 06:47:00.000000 up2b-0.7.1a5/up2b/up2b_lib/up2b_api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-08-05 06:47:00.000000 up2b-0.7.1a5/up2b/up2b_lib/up2b_api/sm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-08-05 06:47:00.000000 up2b-0.7.1a5/up2b/up2b_lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-08-05 06:47:00.000000 up2b-0.7.1a5/up2b/up2b_lib/watermark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-05 06:47:10.000000 up2b-0.7.1a5/up2b/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:47:10.476478 up2b-0.7.1a5/up2b.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-08-05 06:47:10.000000 up2b-0.7.1a5/up2b.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-05 06:47:10.000000 up2b-0.7.1a5/up2b.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 06:47:10.000000 up2b-0.7.1a5/up2b.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-05 06:47:10.000000 up2b-0.7.1a5/up2b.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-05 06:47:10.000000 up2b-0.7.1a5/up2b.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-05 06:47:10.000000 up2b-0.7.1a5/up2b.egg-info/top_level.txt
```

### Comparing `up2b-0.7.1a4/.github/workflows/check.yaml` & `up2b-0.7.1a5/.github/workflows/check.yaml`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a4/.github/workflows/publish.yaml` & `up2b-0.7.1a5/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a4/LICENSE` & `up2b-0.7.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a4/PKG-INFO` & `up2b-0.7.1a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: up2b
-Version: 0.7.1a4
+Version: 0.7.1a5
 Summary: 上传图片到图床
 Author-email: thep0y <thepoy@163.com>
 License: MIT License
         
         Copyright (c) 2021 thep0y
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: up2b Version: 0.7.1a4 Summary:
+Metadata-Version: 2.1 Name: up2b Version: 0.7.1a5 Summary:
 ä¸ä¼ å¾çå°å¾åº Author-email: thep0y
 163.com> License: MIT License Copyright (c) 2021 thep0y Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `up2b-0.7.1a4/README.en_US.md` & `up2b-0.7.1a5/README.en_US.md`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a4/README.md` & `up2b-0.7.1a5/README.md`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a4/pyproject.toml` & `up2b-0.7.1a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 requires-python = ">=3"
 license = { file = "LICENSE" }
 classifiers = ["Programming Language :: Python :: 3"]
 keywords = ["typora", "image bed", "upload"]
 dependencies = [
     "requests",
     "click",
-    "colorful-logger>=0.2.0b1",
+    "colorful-logger>=0.2.0b2",
     "typing_extensions; python_version<'3.8'",
 ]
 dynamic = ["version"]
 
 [project.urls]
 homepage = "https://github.com/thep0y/up2b"
 repository = "https://github.com/thep0y/up2b"
```

### Comparing `up2b-0.7.1a4/tests/images/1.png` & `up2b-0.7.1a5/tests/images/1.png`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a4/tests/images/2.jpeg` & `up2b-0.7.1a5/tests/images/2.jpeg`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a4/tests/images/3.jpeg` & `up2b-0.7.1a5/tests/images/3.jpeg`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a4/tests/server.py` & `up2b-0.7.1a5/tests/server.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a4/tests/test_upload.py` & `up2b-0.7.1a5/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a4/tests/test_utils.py` & `up2b-0.7.1a5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a4/up2b/__init__.py` & `up2b-0.7.1a5/up2b/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # @Author:      thepoy
 # @Email:       thepoy@163.com
 # @File Name:   __init__.py
 # @Created At:  2021-02-08 15:43:32
 # @Modified At: 2023-04-19 14:45:15
 # @Modified By: thepoy
 
+from pathlib import Path
 import sys
 import json
 import click
 
 from typing import Any, Dict, Tuple, Type, Union
 from colort import display_style as ds
 from up2b.up2b_lib.up2b_api import choose_image_bed
@@ -18,14 +19,15 @@
 from up2b.up2b_lib.up2b_api.imgtu import Imgtu
 from up2b.up2b_lib.up2b_api.github import Github
 from up2b.up2b_lib.up2b_api.imgtg import Imgtg
 from up2b.up2b_lib.constants import (
     CACHE_PATH,
     CONF_FILE,
     IMAGE_BEDS_HELP_MESSAGE,
+    IMAGE_BEDS_NAME,
     ImageBedCode,
 )
 from up2b.up2b_lib.utils import check_paths, read_conf
 from up2b.up2b_lib.log import logger
 from up2b.version import __version__  # Automatically create version.py after building
 
 IMAGE_BEDS: Dict[
@@ -195,14 +197,27 @@
 
     paths = check_paths(image_paths)
 
     ib.upload_images(*paths)
 
 
 @cli.command(
+    short_help="手动添加缓存", help="某些图床禁止上传重复图片，但在上传时又不返回旧图片地址，此时需要你手动获取原图片地址并执行此命令添加到缓存中。"
+)
+@click.argument(
+    "image_path",
+    type=click.Path(exists=True, file_okay=True, dir_okay=False, path_type=Path),
+)
+@click.argument("url", type=str)
+def add_cache(image_path: Path, url: str):
+    ib = _read_image_bed()
+    ib.cache.add(image_path, url, IMAGE_BEDS_NAME[ib.image_bed_code])
+
+
+@cli.command(
     short_help="配置文字水印",
     help="""
     参数解释：
 
         - x 整数，横坐标
     
         - y 整数，纵坐标
```

### Comparing `up2b-0.7.1a4/up2b/up2b_lib/cache.py` & `up2b-0.7.1a5/up2b/up2b_lib/cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,9 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
-# @Author:      thepoy
-# @Email:       thepoy@163.com
-# @File Name:   cache.py
-# @Created At:  2023-02-28 22:16:22
-# @Modified At: 2023-03-06 20:34:24
-# @Modified By: thepoy
 
 import sqlite3
 import hashlib
 
 from up2b.up2b_lib.constants import CACHE_DATABASE, PYTHON_VERSION
 
 if PYTHON_VERSION >= (3, 9):
@@ -148,14 +142,28 @@
         else:
             sql = """
                 INSERT INTO cache (url, hash, image_bed) VALUES (?, ?, ?);
             """
 
             return self.execute(sql, url, md5, image_bed)
 
+    def add(self, image_path: Path, url: str, image_bed: str):
+        md5 = file_md5(image_path)
+        exists = self.is_exists(md5, image_bed)
+        if exists:
+            logger.warning("缓存中已有此图片，无需重复添加")
+            return
+
+        sql = """
+            INSERT INTO cache (url, hash, image_bed) VALUES (?, ?, ?);
+        """
+        self.execute(sql, url, md5, image_bed)
+
+        logger.info("已手动添加缓存", image=image_path, url=url, image_bed=image_bed)
+
     def execute(self, sql: str, *params: Any):
         c = self.conn.cursor()
         return c.execute(sql, params)
 
     def commit(self):
         self.conn.commit()
```

### Comparing `up2b-0.7.1a4/up2b/up2b_lib/constants.py` & `up2b-0.7.1a5/up2b/up2b_lib/constants.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a4/up2b/up2b_lib/custom_types.py` & `up2b-0.7.1a5/up2b/up2b_lib/custom_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,8 @@
 #!/usr/bin/env python3
-# -*- coding:utf-8 -*-
-# @Author:      thepoy
-# @Email:       thepoy@163.com
-# @File Name:   custom_types.py
-# @Created At:  2021-02-09 11:27:21
-# @Modified At: 2023-02-21 12:41:21
-# @Modified By: thepoy
 
 from enum import IntEnum
 from typing import Any, Dict, List, Optional, Union
 from dataclasses import dataclass, asdict
 from pathlib import Path
 
 from up2b.up2b_lib.constants import ImageBedCode
```

### Comparing `up2b-0.7.1a4/up2b/up2b_lib/i18n.py` & `up2b-0.7.1a5/up2b/up2b_lib/i18n.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a4/up2b/up2b_lib/log.py` & `up2b-0.7.1a5/up2b/up2b_lib/log.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # @Email:       thepoy@163.com
 # @File Name:   log.py
 # @Created At:  2023-02-07 12:13:41
 # @Modified At: 2023-04-03 20:55:06
 # @Modified By: thepoy
 
 from colorful_logger import get_logger, child_logger as cl
-from colorful_logger.logger import is_debug
+from colorful_logger.logger import is_debug, get_level_from_env
 from up2b.up2b_lib.constants import CONFIG_FOLDER_PATH
 
 log_file_path = None
 show = True
 
 if is_debug():
     log_file_path = CONFIG_FOLDER_PATH / "up2b.log"
@@ -22,12 +22,13 @@
 def child_logger(name: str):
     return cl(name, logger)
 
 
 logger = get_logger(
     "up2b",
     show=show,
+    level=get_level_from_env(),
     file_path=log_file_path,
     add_file_path=False,
     disable_line_number_filter=True,
     asynchronous=False,
 )
```

### Comparing `up2b-0.7.1a4/up2b/up2b_lib/up2b_api/__init__.py` & `up2b-0.7.1a5/up2b/up2b_lib/up2b_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,30 +287,30 @@
         )
 
     def _clear_cache(self):
         if os.path.exists(CACHE_PATH):
             shutil.rmtree(CACHE_PATH)
             os.mkdir(CACHE_PATH)
 
-            logger.info("cache folder has been cleared", cache_path=CACHE_PATH)
+            logger.debug("cache folder has been cleared", cache_path=CACHE_PATH)
 
     def _check_cache(self, image: Path) -> Tuple[str, str, bool]:
         url, md5, ok = self.cache.check_cache_of_image_bed(
             image, IMAGE_BEDS_NAME[self.image_bed_code]
         )
 
         if ok:
             if self.ignore_cache:
                 logger.info("缓存中找到此图片链接，但用户选择忽略缓存强制上传")
             else:
                 logger.info("缓存中找到此图片链接", url=url)
 
             return (url, md5, ok)
 
-        logger.debug("缓存中未找到此图片链接")
+        logger.info("缓存中未找到此图片链接，开始上传")
         return (url, md5, ok)
 
     def upload_images(
         self, *images: Union[ImageType, DownloadErrorResponse], to_console: bool = True
     ) -> List[Union[str, DownloadErrorResponse, UploadErrorResponse]]:
         self.check_login()
 
@@ -327,15 +327,18 @@
             else:
                 result = self.upload_image_stream(img)
 
             image_urls.append(result)
 
         if to_console:
             for iu in image_urls:
-                print(iu)
+                if isinstance(iu, UploadErrorResponse):
+                    logger.error("上传出错", status_code=iu.status_code, error=iu.error)
+                else:
+                    print(iu)
 
         self._clear_cache()
         return image_urls
 
 
 class GitBase(Base):
     headers: Dict[str, str]
```

### Comparing `up2b-0.7.1a4/up2b/up2b_lib/up2b_api/__init__.pyi` & `up2b-0.7.1a5/up2b/up2b_lib/up2b_api/__init__.pyi`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a4/up2b/up2b_lib/up2b_api/github.py` & `up2b-0.7.1a5/up2b/up2b_lib/up2b_api/github.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a4/up2b/up2b_lib/up2b_api/imgtg.py` & `up2b-0.7.1a5/up2b/up2b_lib/up2b_api/imgtg.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,14 +133,21 @@
         auth_token = auth_token.group(1)
         if not self.auth_info:
             self.auth_info = {}
 
         self.auth_info["token"] = self.token = auth_token
         self._save_auth_info(self.auth_info)
 
+    @staticmethod
+    def _is_in_maintenance(status_code: int, text: str, image: ImageType):
+        if "<h1>网站正在维护中</h1>" in text:
+            return UploadErrorResponse(500, "网站正在维护", str(image))
+
+        return UploadErrorResponse(status_code, text, str(image))
+
     def __upload(
         self, image: ImageType, retries: int = 0
     ) -> Union[str, UploadErrorResponse]:
         self.check_login()
 
         url, md5, ok = self._check_cache(image)  # type: ignore
 
@@ -186,23 +193,28 @@
             "nsfw": "0",
         }
 
         files = {
             "source": (filename, img_buffer, mime_type),
         }
 
+        logger.debug("请求头", header=self.headers)
+
         resp = requests.post(
             url, headers=self.headers, data=data, files=files, timeout=self.timeout  # type: ignore
         )
         resp.encoding = "utf-8"
 
+        logger.debug("实际请求头", header=resp.request.headers)
+        logger.trace("请求体", body=resp.request.body)
+
         try:
             json_resp = resp.json()
         except json.decoder.JSONDecodeError:
-            return UploadErrorResponse(resp.status_code, resp.text, str(image))
+            return self._is_in_maintenance(resp.status_code, resp.text, image)
 
         try:
             uploaded_url: str = json_resp["image"]["image"]["url"]
             logger.info(
                 "uploaded",
                 target=image,
                 url=uploaded_url,
@@ -227,14 +239,16 @@
                     "`auth_token` has expired, the program will try to update `auth_token` automatically, number of retries: %d",
                     retries + 1,
                 )
                 self._update_auth_token()
 
                 return self.__upload(image, retries + 1)
             else:
+                logger.debug("上传出错", error=resp.json())
+                logger.error("imgtg 禁止上传重复图片，请检查你之前是否已上传过此图片", image=image)
                 return UploadErrorResponse(
                     resp.status_code, resp.json()["error"]["message"], str(image)
                 )
 
     def upload_image(self, image_path: ImagePath) -> Union[str, UploadErrorResponse]:
         image_path = self._add_watermark(image_path)
```

### Comparing `up2b-0.7.1a4/up2b/up2b_lib/up2b_api/imgtu.py` & `up2b-0.7.1a5/up2b/up2b_lib/up2b_api/imgtu.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a4/up2b/up2b_lib/up2b_api/sm.py` & `up2b-0.7.1a5/up2b/up2b_lib/up2b_api/sm.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a4/up2b/up2b_lib/utils.py` & `up2b-0.7.1a5/up2b/up2b_lib/utils.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a4/up2b/up2b_lib/watermark.py` & `up2b-0.7.1a5/up2b/up2b_lib/watermark.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a4/up2b.egg-info/PKG-INFO` & `up2b-0.7.1a5/up2b.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: up2b
-Version: 0.7.1a4
+Version: 0.7.1a5
 Summary: 上传图片到图床
 Author-email: thep0y <thepoy@163.com>
 License: MIT License
         
         Copyright (c) 2021 thep0y
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: up2b Version: 0.7.1a4 Summary:
+Metadata-Version: 2.1 Name: up2b Version: 0.7.1a5 Summary:
 ä¸ä¼ å¾çå°å¾åº Author-email: thep0y
 163.com> License: MIT License Copyright (c) 2021 thep0y Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `up2b-0.7.1a4/up2b.egg-info/SOURCES.txt` & `up2b-0.7.1a5/up2b.egg-info/SOURCES.txt`

 * *Files identical despite different names*

