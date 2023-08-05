# Comparing `tmp/gpt4all-code-review-0.1.tar.gz` & `tmp/gpt4all-code-review-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt4all-code-review-0.1.tar", last modified: Sat Aug  5 15:35:26 2023, max compression
+gzip compressed data, was "gpt4all-code-review-0.11.tar", last modified: Sat Aug  5 15:42:49 2023, max compression
```

## Comparing `gpt4all-code-review-0.1.tar` & `gpt4all-code-review-0.11.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:35:26.211104 gpt4all-code-review-0.1/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      215 2023-08-05 15:35:26.210918 gpt4all-code-review-0.1/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:34:29.000000 gpt4all-code-review-0.1/README.md
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:35:26.206346 gpt4all-code-review-0.1/gpt4all_code_review/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:31:18.000000 gpt4all-code-review-0.1/gpt4all_code_review/__init__.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     6084 2023-08-05 15:35:12.000000 gpt4all-code-review-0.1/gpt4all_code_review/gpt4all_code_review.py
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:35:26.209429 gpt4all-code-review-0.1/gpt4all_code_review.egg-info/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      215 2023-08-05 15:35:26.000000 gpt4all-code-review-0.1/gpt4all_code_review.egg-info/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      307 2023-08-05 15:35:26.000000 gpt4all-code-review-0.1/gpt4all_code_review.egg-info/SOURCES.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2023-08-05 15:35:26.000000 gpt4all-code-review-0.1/gpt4all_code_review.egg-info/dependency_links.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       66 2023-08-05 15:35:26.000000 gpt4all-code-review-0.1/gpt4all_code_review.egg-info/requires.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       20 2023-08-05 15:35:26.000000 gpt4all-code-review-0.1/gpt4all_code_review.egg-info/top_level.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2023-08-05 15:35:26.211147 gpt4all-code-review-0.1/setup.cfg
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      542 2023-08-05 15:34:08.000000 gpt4all-code-review-0.1/setup.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:42:49.503271 gpt4all-code-review-0.11/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      216 2023-08-05 15:42:49.503114 gpt4all-code-review-0.11/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:34:29.000000 gpt4all-code-review-0.11/README.md
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:42:49.501623 gpt4all-code-review-0.11/gpt4all_code_review/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:31:18.000000 gpt4all-code-review-0.11/gpt4all_code_review/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     6084 2023-08-05 15:35:12.000000 gpt4all-code-review-0.11/gpt4all_code_review/gpt4all_code_review.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:42:49.502593 gpt4all-code-review-0.11/gpt4all_code_review.egg-info/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      216 2023-08-05 15:42:49.000000 gpt4all-code-review-0.11/gpt4all_code_review.egg-info/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      307 2023-08-05 15:42:49.000000 gpt4all-code-review-0.11/gpt4all_code_review.egg-info/SOURCES.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2023-08-05 15:42:49.000000 gpt4all-code-review-0.11/gpt4all_code_review.egg-info/dependency_links.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       58 2023-08-05 15:42:49.000000 gpt4all-code-review-0.11/gpt4all_code_review.egg-info/requires.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       20 2023-08-05 15:42:49.000000 gpt4all-code-review-0.11/gpt4all_code_review.egg-info/top_level.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2023-08-05 15:42:49.503312 gpt4all-code-review-0.11/setup.cfg
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      513 2023-08-05 15:42:46.000000 gpt4all-code-review-0.11/setup.py
```

### Comparing `gpt4all-code-review-0.1/gpt4all_code_review/gpt4all_code_review.py` & `gpt4all-code-review-0.11/gpt4all_code_review/gpt4all_code_review.py`

 * *Files identical despite different names*

### Comparing `gpt4all-code-review-0.1/setup.py` & `gpt4all-code-review-0.11/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gpt4all-code-review',
-    version='0.1',
+    version='0.11',
     packages=find_packages(),
     install_requires=[
-        "os",
-        "json",
         "argparse",
         "gpt4all",
         "prettytable",
         "datetime",
         "console_progressbar",
     ],
     author='Evgenii Evstafev',
```

