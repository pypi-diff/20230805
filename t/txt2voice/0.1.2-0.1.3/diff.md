# Comparing `tmp/txt2voice-0.1.2.tar.gz` & `tmp/txt2voice-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txt2voice-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "txt2voice-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `txt2voice-0.1.2.tar` & `txt2voice-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       49 2023-08-05 07:48:47.839487 txt2voice-0.1.2/.flake8
--rw-r--r--   0        0        0      894 2023-08-05 07:48:47.839487 txt2voice-0.1.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      661 2023-08-05 07:48:47.839487 txt2voice-0.1.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0     3094 2023-08-05 07:48:47.839487 txt2voice-0.1.2/.gitignore
--rw-r--r--   0        0        0      121 2023-08-05 07:48:47.839487 txt2voice-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0     1063 2023-08-05 07:48:47.839487 txt2voice-0.1.2/LICENSE
--rw-r--r--   0        0        0     1333 2023-08-05 07:48:47.839487 txt2voice-0.1.2/Makefile
--rw-r--r--   0        0        0     2922 2023-08-05 07:48:47.839487 txt2voice-0.1.2/README.md
--rw-r--r--   0        0        0      563 2023-08-05 07:48:47.839487 txt2voice-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-05 07:48:47.839487 txt2voice-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     3467 2023-08-05 07:48:47.839487 txt2voice-0.1.2/tests/test_api.py
--rw-r--r--   0        0        0      463 2023-08-05 07:48:47.839487 txt2voice-0.1.2/tox.ini
--rw-r--r--   0        0        0       51 2023-08-05 07:48:47.839487 txt2voice-0.1.2/txt2voice/__init__.py
--rw-r--r--   0        0        0     2521 2023-08-05 07:48:47.843487 txt2voice-0.1.2/txt2voice/api.py
--rw-r--r--   0        0        0      874 2023-08-05 07:48:47.843487 txt2voice-0.1.2/txt2voice/models.py
--rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 txt2voice-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       49 2023-08-05 08:00:42.714875 txt2voice-0.1.3/.flake8
+-rw-r--r--   0        0        0      894 2023-08-05 08:00:42.714875 txt2voice-0.1.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      661 2023-08-05 08:00:42.714875 txt2voice-0.1.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     3094 2023-08-05 08:00:42.714875 txt2voice-0.1.3/.gitignore
+-rw-r--r--   0        0        0      121 2023-08-05 08:00:42.714875 txt2voice-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1063 2023-08-05 08:00:42.714875 txt2voice-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1333 2023-08-05 08:00:42.714875 txt2voice-0.1.3/Makefile
+-rw-r--r--   0        0        0     2922 2023-08-05 08:00:42.714875 txt2voice-0.1.3/README.md
+-rw-r--r--   0        0        0      563 2023-08-05 08:00:42.714875 txt2voice-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-05 08:00:42.714875 txt2voice-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     3467 2023-08-05 08:00:42.714875 txt2voice-0.1.3/tests/test_api.py
+-rw-r--r--   0        0        0      463 2023-08-05 08:00:42.714875 txt2voice-0.1.3/tox.ini
+-rw-r--r--   0        0        0       97 2023-08-05 08:00:42.714875 txt2voice-0.1.3/txt2voice/__init__.py
+-rw-r--r--   0        0        0     2521 2023-08-05 08:00:42.714875 txt2voice-0.1.3/txt2voice/api.py
+-rw-r--r--   0        0        0      874 2023-08-05 08:00:42.714875 txt2voice-0.1.3/txt2voice/models.py
+-rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 txt2voice-0.1.3/PKG-INFO
```

### Comparing `txt2voice-0.1.2/.github/workflows/build.yml` & `txt2voice-0.1.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `txt2voice-0.1.2/.github/workflows/publish.yml` & `txt2voice-0.1.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `txt2voice-0.1.2/.gitignore` & `txt2voice-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `txt2voice-0.1.2/LICENSE` & `txt2voice-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `txt2voice-0.1.2/Makefile` & `txt2voice-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `txt2voice-0.1.2/README.md` & `txt2voice-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `txt2voice-0.1.2/pyproject.toml` & `txt2voice-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `txt2voice-0.1.2/tests/test_api.py` & `txt2voice-0.1.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `txt2voice-0.1.2/txt2voice/api.py` & `txt2voice-0.1.3/txt2voice/api.py`

 * *Files identical despite different names*

### Comparing `txt2voice-0.1.2/txt2voice/models.py` & `txt2voice-0.1.3/txt2voice/models.py`

 * *Files identical despite different names*

### Comparing `txt2voice-0.1.2/PKG-INFO` & `txt2voice-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txt2voice
-Version: 0.1.2
+Version: 0.1.3
 Summary: Convert text to voice
 Author: zemags
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: pydub>=0.25.1
```

