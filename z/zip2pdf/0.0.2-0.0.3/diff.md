# Comparing `tmp/zip2pdf-0.0.2.tar.gz` & `tmp/zip2pdf-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zip2pdf-0.0.2.tar", last modified: Sat Aug  5 09:45:41 2023, max compression
+gzip compressed data, was "zip2pdf-0.0.3.tar", last modified: Sat Aug  5 09:52:44 2023, max compression
```

## Comparing `zip2pdf-0.0.2.tar` & `zip2pdf-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 09:45:41.794614 zip2pdf-0.0.2/
--rw-rw-rw-   0        0        0       54 2023-08-05 09:45:41.794614 zip2pdf-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-05-20 22:22:52.000000 zip2pdf-0.0.2/README.md
--rw-rw-rw-   0        0        0      325 2023-08-05 09:45:41.798974 zip2pdf-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-05-20 22:22:52.000000 zip2pdf-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-05 09:45:41.768087 zip2pdf-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-08-05 09:45:41.773666 zip2pdf-0.0.2/src/zip2pdf/
--rw-rw-rw-   0        0        0       34 2023-05-20 22:22:52.000000 zip2pdf-0.0.2/src/zip2pdf/__init__.py
--rw-rw-rw-   0        0        0     1903 2023-05-20 22:22:52.000000 zip2pdf-0.0.2/src/zip2pdf/main.py
-drwxrwxrwx   0        0        0        0 2023-08-05 09:45:41.793111 zip2pdf-0.0.2/src/zip2pdf.egg-info/
--rw-rw-rw-   0        0        0       54 2023-08-05 09:45:41.000000 zip2pdf-0.0.2/src/zip2pdf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-08-05 09:45:41.000000 zip2pdf-0.0.2/src/zip2pdf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 09:45:41.000000 zip2pdf-0.0.2/src/zip2pdf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-08-05 09:45:41.000000 zip2pdf-0.0.2/src/zip2pdf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-08-05 09:45:41.000000 zip2pdf-0.0.2/src/zip2pdf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-05 09:45:41.000000 zip2pdf-0.0.2/src/zip2pdf.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 09:52:44.867093 zip2pdf-0.0.3/
+-rw-rw-rw-   0        0        0      311 2023-08-05 09:52:44.867093 zip2pdf-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-05-20 22:22:52.000000 zip2pdf-0.0.3/README.md
+-rw-rw-rw-   0        0        0      214 2023-08-05 09:47:06.000000 zip2pdf-0.0.3/README_PYPI.md
+-rw-rw-rw-   0        0        0      378 2023-08-05 09:52:44.872634 zip2pdf-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-05-20 22:22:52.000000 zip2pdf-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:52:44.842552 zip2pdf-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-08-05 09:52:44.849059 zip2pdf-0.0.3/src/zip2pdf/
+-rw-rw-rw-   0        0        0       34 2023-05-20 22:22:52.000000 zip2pdf-0.0.3/src/zip2pdf/__init__.py
+-rw-rw-rw-   0        0        0     1903 2023-05-20 22:22:52.000000 zip2pdf-0.0.3/src/zip2pdf/main.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:52:44.866092 zip2pdf-0.0.3/src/zip2pdf.egg-info/
+-rw-rw-rw-   0        0        0      311 2023-08-05 09:52:44.000000 zip2pdf-0.0.3/src/zip2pdf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-08-05 09:52:44.000000 zip2pdf-0.0.3/src/zip2pdf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 09:52:44.000000 zip2pdf-0.0.3/src/zip2pdf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-08-05 09:52:44.000000 zip2pdf-0.0.3/src/zip2pdf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-08-05 09:52:44.000000 zip2pdf-0.0.3/src/zip2pdf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-05 09:52:44.000000 zip2pdf-0.0.3/src/zip2pdf.egg-info/top_level.txt
```

### Comparing `zip2pdf-0.0.2/src/zip2pdf/main.py` & `zip2pdf-0.0.3/src/zip2pdf/main.py`

 * *Files identical despite different names*

