# Comparing `tmp/moderne_visualizations_misc-0.1.8.tar.gz` & `tmp/moderne_visualizations_misc-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moderne_visualizations_misc-0.1.8.tar", last modified: Wed Aug  2 22:24:34 2023, max compression
+gzip compressed data, was "moderne_visualizations_misc-0.1.9.tar", last modified: Thu Aug  3 04:51:36 2023, max compression
```

## Comparing `moderne_visualizations_misc-0.1.8.tar` & `moderne_visualizations_misc-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:24:34.891662 moderne_visualizations_misc-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-02 22:24:34.891662 moderne_visualizations_misc-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:24:34.887662 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/cobol_find_copy_book.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/dependency_vulnerabilities.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/find_methods.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    25481 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/find_source_files.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:24:34.891662 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/images/
--rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/images/cobol_find_copy_book.300.png
--rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/images/dependency_vulnerabilities.300.png
--rw-r--r--   0 runner    (1001) docker     (123)    31410 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/images/language_composition.300.png
--rw-r--r--   0 runner    (1001) docker     (123)    23912 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/images/parse_failure_analysis.300.png
--rw-r--r--   0 runner    (1001) docker     (123)    24871 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/images/sql_crud.300.png
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/language_composition.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/parse_failure_analysis.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:24:34.891662 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/specs/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/specs/cobol_find_copy_book.yml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/specs/dependency_vulnerabilities.yml
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/specs/find_methods.yml
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/specs/find_source_files.yml
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/specs/language_composition.yml
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/specs/parse_failure_analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/specs/sql_crud.yml
--rw-r--r--   0 runner    (1001) docker     (123)   152398 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/sql_crud.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:24:34.891662 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-02 22:24:34.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-02 22:24:34.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 22:24:34.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-02 22:24:34.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 22:24:34.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 22:24:34.891662 moderne_visualizations_misc-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 04:51:36.334367 moderne_visualizations_misc-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-03 04:51:18.000000 moderne_visualizations_misc-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-03 04:51:36.334367 moderne_visualizations_misc-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-03 04:51:18.000000 moderne_visualizations_misc-0.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 04:51:36.330367 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 04:51:18.000000 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-03 04:51:18.000000 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/cobol_find_copy_book.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-08-03 04:51:18.000000 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/dependency_vulnerabilities.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-08-03 04:51:18.000000 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/find_methods.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    25481 2023-08-03 04:51:18.000000 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/find_source_files.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 04:51:36.334367 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-08-03 04:51:18.000000 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/images/cobol_find_copy_book.300.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-08-03 04:51:18.000000 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/images/dependency_vulnerabilities.300.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31410 2023-08-03 04:51:18.000000 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/images/language_composition.300.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23912 2023-08-03 04:51:18.000000 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/images/parse_failure_analysis.300.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24871 2023-08-03 04:51:18.000000 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/images/sql_crud.300.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-08-03 04:51:18.000000 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/language_composition.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-08-03 04:51:18.000000 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/parse_failure_analysis.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 04:51:36.334367 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-03 04:51:18.000000 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/specs/cobol_find_copy_book.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-03 04:51:18.000000 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/specs/dependency_vulnerabilities.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-03 04:51:18.000000 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/specs/find_methods.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-03 04:51:18.000000 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/specs/find_source_files.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-03 04:51:18.000000 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/specs/language_composition.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-03 04:51:18.000000 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/specs/parse_failure_analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-03 04:51:18.000000 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/specs/sql_crud.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   152398 2023-08-03 04:51:18.000000 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/sql_crud.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 04:51:36.334367 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-03 04:51:36.000000 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-03 04:51:36.000000 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 04:51:36.000000 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-03 04:51:36.000000 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-03 04:51:36.000000 moderne_visualizations_misc-0.1.9/moderne_visualizations_misc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-08-03 04:51:18.000000 moderne_visualizations_misc-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 04:51:36.334367 moderne_visualizations_misc-0.1.9/setup.cfg
```

### Comparing `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/cobol_find_copy_book.ipynb` & `moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/cobol_find_copy_book.ipynb`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/dependency_vulnerabilities.ipynb` & `moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/dependency_vulnerabilities.ipynb`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/find_methods.ipynb` & `moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/find_methods.ipynb`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/find_source_files.ipynb` & `moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/find_source_files.ipynb`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/images/cobol_find_copy_book.300.png` & `moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/images/cobol_find_copy_book.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/images/dependency_vulnerabilities.300.png` & `moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/images/dependency_vulnerabilities.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/images/language_composition.300.png` & `moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/images/language_composition.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/images/parse_failure_analysis.300.png` & `moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/images/parse_failure_analysis.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/images/sql_crud.300.png` & `moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/images/sql_crud.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/language_composition.ipynb` & `moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/language_composition.ipynb`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/parse_failure_analysis.ipynb` & `moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/parse_failure_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/specs/dependency_vulnerabilities.yml` & `moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/specs/dependency_vulnerabilities.yml`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/specs/parse_failure_analysis.yml` & `moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/specs/parse_failure_analysis.yml`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/sql_crud.ipynb` & `moderne_visualizations_misc-0.1.9/moderne_visualizations_misc/sql_crud.ipynb`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc.egg-info/SOURCES.txt` & `moderne_visualizations_misc-0.1.9/moderne_visualizations_misc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.8/pyproject.toml` & `moderne_visualizations_misc-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # @see https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 
 [project]
 name = "moderne_visualizations_misc"
-version = "0.1.8"
+version = "0.1.9"
 description = "Miscellaneous visualizations for the Moderne platform"
 authors = [
     { name = "Jonathan Schneider", email = "jonathan@moderne.io" },
     { name = "Kyle Scully", email = "kyle@moderne.io" }
 ]
 license = { text = "Apache-2.0" }
 dependencies = [
```

