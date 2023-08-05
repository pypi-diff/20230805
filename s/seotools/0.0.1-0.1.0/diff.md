# Comparing `tmp/seotools-0.0.1.tar.gz` & `tmp/seotools-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seotools-0.0.1.tar", last modified: Thu Aug  3 19:28:51 2023, max compression
+gzip compressed data, was "seotools-0.1.0.tar", last modified: Sat Aug  5 09:33:44 2023, max compression
```

## Comparing `seotools-0.0.1.tar` & `seotools-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-03 19:28:51.086884 seotools-0.0.1/
--rw-r--r--   0 james      (501) staff       (20)     1063 2023-08-03 19:09:09.000000 seotools-0.0.1/LICENSE
--rw-r--r--   0 james      (501) staff       (20)      759 2023-08-03 19:28:51.086676 seotools-0.0.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      270 2023-08-03 19:27:40.000000 seotools-0.0.1/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-03 19:28:51.085627 seotools-0.0.1/seotools.egg-info/
--rw-r--r--   0 james      (501) staff       (20)      759 2023-08-03 19:28:51.000000 seotools-0.0.1/seotools.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      224 2023-08-03 19:28:51.000000 seotools-0.0.1/seotools.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-08-03 19:28:51.000000 seotools-0.0.1/seotools.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)      141 2023-08-03 19:28:51.000000 seotools-0.0.1/seotools.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)        4 2023-08-03 19:28:51.000000 seotools-0.0.1/seotools.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-08-03 19:28:51.086949 seotools-0.0.1/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1242 2023-08-03 19:28:41.000000 seotools-0.0.1/setup.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-03 19:28:51.086307 seotools-0.0.1/src/
--rw-r--r--   0 james      (501) staff       (20)       22 2023-08-03 09:43:56.000000 seotools-0.0.1/src/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     1499 2023-08-03 19:25:07.000000 seotools-0.0.1/src/links.py
--rw-r--r--   0 james      (501) staff       (20)     8048 2023-08-03 19:28:33.000000 seotools-0.0.1/src/nx.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-05 09:33:44.070274 seotools-0.1.0/
+-rw-r--r--   0 james      (501) staff       (20)     1063 2023-08-03 19:09:09.000000 seotools-0.1.0/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)      865 2023-08-03 09:42:54.000000 seotools-0.1.0/Makefile
+-rw-r--r--   0 james      (501) staff       (20)     3478 2023-08-05 09:33:44.069895 seotools-0.1.0/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     2989 2023-08-03 23:46:43.000000 seotools-0.1.0/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-05 09:33:44.066930 seotools-0.1.0/docs/
+-rw-r--r--   0 james      (501) staff       (20)     2591 2023-08-03 22:41:36.000000 seotools-0.1.0/docs/index.md
+-rw-r--r--   0 james      (501) staff       (20)     1000 2023-08-03 22:15:29.000000 seotools-0.1.0/mkdocs.yml
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-05 09:33:44.068177 seotools-0.1.0/seotools/
+-rw-r--r--   0 james      (501) staff       (20)       22 2023-08-05 09:32:38.000000 seotools-0.1.0/seotools/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    14350 2023-08-04 11:00:44.000000 seotools-0.1.0/seotools/app.py
+-rw-r--r--   0 james      (501) staff       (20)      522 2023-08-03 19:45:20.000000 seotools-0.1.0/seotools/crawl_bot_validation.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-05 09:33:44.069595 seotools-0.1.0/seotools.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     3478 2023-08-05 09:33:44.000000 seotools-0.1.0/seotools.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      289 2023-08-05 09:33:44.000000 seotools-0.1.0/seotools.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-08-05 09:33:44.000000 seotools-0.1.0/seotools.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      141 2023-08-05 09:33:44.000000 seotools-0.1.0/seotools.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)        9 2023-08-05 09:33:44.000000 seotools-0.1.0/seotools.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-08-05 09:33:44.070347 seotools-0.1.0/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1247 2023-08-05 09:33:36.000000 seotools-0.1.0/setup.py
```

### Comparing `seotools-0.0.1/LICENSE` & `seotools-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seotools-0.0.1/setup.py` & `seotools-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 from setuptools import find_packages
 import re
 
-with open("./src/__init__.py", 'r') as f:
+with open("./seotools/__init__.py", 'r') as f:
     content = f.read()
     # from https://www.py4u.net/discuss/139845
     version = re.search(r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]', content).group(1)
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
```

