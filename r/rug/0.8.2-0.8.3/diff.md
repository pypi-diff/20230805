# Comparing `tmp/rug-0.8.2.tar.gz` & `tmp/rug-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rug-0.8.2.tar", max compression
+gzip compressed data, was "rug-0.8.3.tar", max compression
```

## Comparing `rug-0.8.2.tar` & `rug-0.8.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      762 2023-06-16 06:42:16.417052 rug-0.8.2/README.md
--rw-r--r--   0        0        0      853 2023-08-04 15:39:36.862174 rug-0.8.2/pyproject.toml
--rw-r--r--   0        0        0      288 2022-12-15 16:02:47.957044 rug-0.8.2/rug/__init__.py
--rw-r--r--   0        0        0     4266 2022-10-10 19:45:59.707606 rug-0.8.2/rug/alphaquery.py
--rw-r--r--   0        0        0     2688 2022-08-11 07:37:52.820634 rug-0.8.2/rug/barchart.py
--rw-r--r--   0        0        0     4997 2023-06-16 06:35:11.344249 rug-0.8.2/rug/base.py
--rw-r--r--   0        0        0     4150 2022-12-23 18:09:17.774153 rug-0.8.2/rug/etfdb.py
--rw-r--r--   0        0        0      683 2022-07-27 20:03:36.438856 rug-0.8.2/rug/exceptions.py
--rw-r--r--   0        0        0     3038 2023-06-16 06:33:17.358960 rug-0.8.2/rug/finviz.py
--rw-r--r--   0        0        0     5272 2023-08-04 15:27:05.100546 rug-0.8.2/rug/stockanalysis.py
--rw-r--r--   0        0        0     1947 2022-08-11 08:42:20.047418 rug-0.8.2/rug/stocktwits.py
--rw-r--r--   0        0        0     6910 2023-05-05 06:58:34.815386 rug-0.8.2/rug/tipranks.py
--rw-r--r--   0        0        0     1764 1970-01-01 00:00:00.000000 rug-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0      762 2023-06-16 06:42:16.417052 rug-0.8.3/README.md
+-rw-r--r--   0        0        0      853 2023-08-04 16:21:48.574465 rug-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0      263 2023-08-04 16:20:35.385529 rug-0.8.3/rug/__init__.py
+-rw-r--r--   0        0        0     4266 2022-10-10 19:45:59.707606 rug-0.8.3/rug/alphaquery.py
+-rw-r--r--   0        0        0     2688 2022-08-11 07:37:52.820634 rug-0.8.3/rug/barchart.py
+-rw-r--r--   0        0        0     4997 2023-06-16 06:35:11.344249 rug-0.8.3/rug/base.py
+-rw-r--r--   0        0        0     4150 2022-12-23 18:09:17.774153 rug-0.8.3/rug/etfdb.py
+-rw-r--r--   0        0        0      683 2022-07-27 20:03:36.438856 rug-0.8.3/rug/exceptions.py
+-rw-r--r--   0        0        0     3038 2023-06-16 06:33:17.358960 rug-0.8.3/rug/finviz.py
+-rw-r--r--   0        0        0     5272 2023-08-04 15:27:05.100546 rug-0.8.3/rug/stockanalysis.py
+-rw-r--r--   0        0        0     1947 2022-08-11 08:42:20.047418 rug-0.8.3/rug/stocktwits.py
+-rw-r--r--   0        0        0     6910 2023-05-05 06:58:34.815386 rug-0.8.3/rug/tipranks.py
+-rw-r--r--   0        0        0     1764 1970-01-01 00:00:00.000000 rug-0.8.3/PKG-INFO
```

### Comparing `rug-0.8.2/README.md` & `rug-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `rug-0.8.2/pyproject.toml` & `rug-0.8.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rug"
-version = "0.8.2"
+version = "0.8.3"
 description = "Library for fetching various stock data from the internet (official and unofficial APIs)."
 authors = ["Pavel Hrdina"]
 classifiers = [
     "Programming Language :: Python :: 3.6",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
     "Intended Audience :: Developers",
```

### Comparing `rug-0.8.2/rug/alphaquery.py` & `rug-0.8.3/rug/alphaquery.py`

 * *Files identical despite different names*

### Comparing `rug-0.8.2/rug/barchart.py` & `rug-0.8.3/rug/barchart.py`

 * *Files identical despite different names*

### Comparing `rug-0.8.2/rug/base.py` & `rug-0.8.3/rug/base.py`

 * *Files identical despite different names*

### Comparing `rug-0.8.2/rug/etfdb.py` & `rug-0.8.3/rug/etfdb.py`

 * *Files identical despite different names*

### Comparing `rug-0.8.2/rug/exceptions.py` & `rug-0.8.3/rug/exceptions.py`

 * *Files identical despite different names*

### Comparing `rug-0.8.2/rug/finviz.py` & `rug-0.8.3/rug/finviz.py`

 * *Files identical despite different names*

### Comparing `rug-0.8.2/rug/stockanalysis.py` & `rug-0.8.3/rug/stockanalysis.py`

 * *Files identical despite different names*

### Comparing `rug-0.8.2/rug/stocktwits.py` & `rug-0.8.3/rug/stocktwits.py`

 * *Files identical despite different names*

### Comparing `rug-0.8.2/rug/tipranks.py` & `rug-0.8.3/rug/tipranks.py`

 * *Files identical despite different names*

### Comparing `rug-0.8.2/PKG-INFO` & `rug-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rug
-Version: 0.8.2
+Version: 0.8.3
 Summary: Library for fetching various stock data from the internet (official and unofficial APIs).
 Home-page: https://github.com/im-n1/rug
 License: MIT
 Author: Pavel Hrdina
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

