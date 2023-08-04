# Comparing `tmp/instacrawl-0.1.3.tar.gz` & `tmp/instacrawl-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instacrawl-0.1.3.tar", max compression
+gzip compressed data, was "instacrawl-0.1.4.tar", max compression
```

## Comparing `instacrawl-0.1.3.tar` & `instacrawl-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-08-03 00:31:26.417628 instacrawl-0.1.3/README.md
--rw-r--r--   0        0        0      123 2023-08-03 22:29:44.075564 instacrawl-0.1.3/instacrawl/__init__.py
--rw-r--r--   0        0        0     1549 2023-08-03 18:21:10.090362 instacrawl-0.1.3/instacrawl/__main__.py
--rw-r--r--   0        0        0    19796 2023-08-03 15:00:36.161900 instacrawl-0.1.3/instacrawl/analysis.py
--rw-r--r--   0        0        0    11537 2023-08-03 14:57:04.543184 instacrawl-0.1.3/instacrawl/cli_utils.py
--rw-r--r--   0        0        0       86 2023-08-03 15:01:47.156347 instacrawl-0.1.3/instacrawl/console.py
--rw-r--r--   0        0        0    47521 2023-08-03 22:21:48.024639 instacrawl-0.1.3/instacrawl/insta.py
--rw-r--r--   0        0        0    17346 2023-08-03 15:57:25.477020 instacrawl-0.1.3/instacrawl/prompts.py
--rw-r--r--   0        0        0     7856 2023-08-03 15:03:09.852583 instacrawl-0.1.3/instacrawl/steps.py
--rw-r--r--   0        0        0      570 2023-08-03 15:03:33.274542 instacrawl-0.1.3/instacrawl/verbose.py
--rw-r--r--   0        0        0      954 2023-08-03 22:29:52.450080 instacrawl-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1520 1970-01-01 00:00:00.000000 instacrawl-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-03 00:31:26.417628 instacrawl-0.1.4/README.md
+-rw-r--r--   0        0        0      123 2023-08-03 23:03:56.980333 instacrawl-0.1.4/instacrawl/__init__.py
+-rw-r--r--   0        0        0     1549 2023-08-03 18:21:10.090362 instacrawl-0.1.4/instacrawl/__main__.py
+-rw-r--r--   0        0        0    19796 2023-08-03 15:00:36.161900 instacrawl-0.1.4/instacrawl/analysis.py
+-rw-r--r--   0        0        0    11537 2023-08-03 14:57:04.543184 instacrawl-0.1.4/instacrawl/cli_utils.py
+-rw-r--r--   0        0        0       86 2023-08-03 15:01:47.156347 instacrawl-0.1.4/instacrawl/console.py
+-rw-r--r--   0        0        0    47521 2023-08-03 22:21:48.024639 instacrawl-0.1.4/instacrawl/insta.py
+-rw-r--r--   0        0        0    17346 2023-08-03 15:57:25.477020 instacrawl-0.1.4/instacrawl/prompts.py
+-rw-r--r--   0        0        0     7856 2023-08-03 15:03:09.852583 instacrawl-0.1.4/instacrawl/steps.py
+-rw-r--r--   0        0        0      570 2023-08-03 15:03:33.274542 instacrawl-0.1.4/instacrawl/verbose.py
+-rw-r--r--   0        0        0     1006 2023-08-03 23:04:30.218187 instacrawl-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1614 1970-01-01 00:00:00.000000 instacrawl-0.1.4/PKG-INFO
```

### Comparing `instacrawl-0.1.3/instacrawl/__main__.py` & `instacrawl-0.1.4/instacrawl/__main__.py`

 * *Files identical despite different names*

### Comparing `instacrawl-0.1.3/instacrawl/analysis.py` & `instacrawl-0.1.4/instacrawl/analysis.py`

 * *Files identical despite different names*

### Comparing `instacrawl-0.1.3/instacrawl/cli_utils.py` & `instacrawl-0.1.4/instacrawl/cli_utils.py`

 * *Files identical despite different names*

### Comparing `instacrawl-0.1.3/instacrawl/insta.py` & `instacrawl-0.1.4/instacrawl/insta.py`

 * *Files identical despite different names*

### Comparing `instacrawl-0.1.3/instacrawl/prompts.py` & `instacrawl-0.1.4/instacrawl/prompts.py`

 * *Files identical despite different names*

### Comparing `instacrawl-0.1.3/instacrawl/steps.py` & `instacrawl-0.1.4/instacrawl/steps.py`

 * *Files identical despite different names*

### Comparing `instacrawl-0.1.3/instacrawl/verbose.py` & `instacrawl-0.1.4/instacrawl/verbose.py`

 * *Files identical despite different names*

### Comparing `instacrawl-0.1.3/pyproject.toml` & `instacrawl-0.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "instacrawl"
-version = "0.1.3"
+version = "0.1.4"
 description = "A simple CLI Instagram crawler with a focus on algorithm analytics."
 authors = [
   "Analetta Ehler <annie.ehler.4@gmail.com>"
 ]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/annie444/instacrawl"
@@ -32,12 +32,14 @@
 typing-extensions = "^4.7.1"
 transformers = "^4.31.0"
 scikit-learn = "^1.3.0"
 requests = "^2.31.0"
 python-dotenv = "^1.0.0"
 html5lib = "^1.1"
 timm = "^0.9.2"
+face-recognition-models = "^0.3.0"
+tqdm = "^4.65.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `instacrawl-0.1.3/PKG-INFO` & `instacrawl-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: instacrawl
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple CLI Instagram crawler with a focus on algorithm analytics.
 Home-page: https://github.com/annie444/instacrawl
 License: MIT
 Author: Analetta Ehler
 Author-email: annie.ehler.4@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: dtale (>=3.3.0,<4.0.0)
 Requires-Dist: eva-decord (>=0.6.1,<0.7.0)
 Requires-Dist: face-recognition (>=1.3.0,<2.0.0)
+Requires-Dist: face-recognition-models (>=0.3.0,<0.4.0)
 Requires-Dist: html5lib (>=1.1,<2.0)
 Requires-Dist: kaleido (==0.2.1)
 Requires-Dist: numpy (>=1.25.2,<2.0.0)
 Requires-Dist: opencv-python (>=4.8.0.74,<5.0.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: pillow (>=10.0.0,<11.0.0)
 Requires-Dist: pynput (>=1.7.6,<2.0.0)
@@ -26,14 +27,15 @@
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.5.2,<14.0.0)
 Requires-Dist: scikit-learn (>=1.3.0,<2.0.0)
 Requires-Dist: selenium (>=4.11.2,<5.0.0)
 Requires-Dist: selenium-wire (>=5.1.0,<6.0.0)
 Requires-Dist: timm (>=0.9.2,<0.10.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: transformers (>=4.31.0,<5.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: typing-extensions (>=4.7.1,<5.0.0)
 Project-URL: Repository, https://github.com/annie444/instacrawl
 Description-Content-Type: text/markdown
```

