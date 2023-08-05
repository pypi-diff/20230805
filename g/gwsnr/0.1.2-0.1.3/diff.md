# Comparing `tmp/gwsnr-0.1.2.tar.gz` & `tmp/gwsnr-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwsnr-0.1.2.tar", last modified: Fri Aug  4 10:39:10 2023, max compression
+gzip compressed data, was "gwsnr-0.1.3.tar", last modified: Sat Aug  5 18:47:11 2023, max compression
```

## Comparing `gwsnr-0.1.2.tar` & `gwsnr-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 phurailatpamhemantakumar   (502) staff       (20)        0 2023-08-04 10:39:10.239718 gwsnr-0.1.2/
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)      210 2023-08-04 10:39:10.239577 gwsnr-0.1.2/PKG-INFO
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)      437 2023-05-29 15:15:36.000000 gwsnr-0.1.2/README.md
-drwxr-xr-x   0 phurailatpamhemantakumar   (502) staff       (20)        0 2023-08-04 10:39:10.238525 gwsnr-0.1.2/gwsnr/
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)       26 2023-05-29 15:15:36.000000 gwsnr-0.1.2/gwsnr/__init__.py
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)    61048 2023-07-17 20:13:57.000000 gwsnr-0.1.2/gwsnr/gwsnr.py
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)        0 2023-05-29 15:15:36.000000 gwsnr-0.1.2/gwsnr/pdet.py
-drwxr-xr-x   0 phurailatpamhemantakumar   (502) staff       (20)        0 2023-08-04 10:39:10.239309 gwsnr-0.1.2/gwsnr.egg-info/
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)      210 2023-08-04 10:39:10.000000 gwsnr-0.1.2/gwsnr.egg-info/PKG-INFO
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)      209 2023-08-04 10:39:10.000000 gwsnr-0.1.2/gwsnr.egg-info/SOURCES.txt
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)        1 2023-08-04 10:39:10.000000 gwsnr-0.1.2/gwsnr.egg-info/dependency_links.txt
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)       83 2023-08-04 10:39:10.000000 gwsnr-0.1.2/gwsnr.egg-info/requires.txt
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)        6 2023-08-04 10:39:10.000000 gwsnr-0.1.2/gwsnr.egg-info/top_level.txt
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)       38 2023-08-04 10:39:10.239795 gwsnr-0.1.2/setup.cfg
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)      529 2023-08-04 10:38:51.000000 gwsnr-0.1.2/setup.py
+drwxr-xr-x   0 phurailatpamhemantakumar   (502) staff       (20)        0 2023-08-05 18:47:11.626374 gwsnr-0.1.3/
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)      217 2023-08-05 18:47:11.626163 gwsnr-0.1.3/PKG-INFO
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)      437 2023-05-29 15:15:36.000000 gwsnr-0.1.3/README.md
+drwxr-xr-x   0 phurailatpamhemantakumar   (502) staff       (20)        0 2023-08-05 18:47:11.625382 gwsnr-0.1.3/gwsnr/
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)       26 2023-05-29 15:15:36.000000 gwsnr-0.1.3/gwsnr/__init__.py
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)    61048 2023-07-17 20:13:57.000000 gwsnr-0.1.3/gwsnr/gwsnr.py
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)        0 2023-05-29 15:15:36.000000 gwsnr-0.1.3/gwsnr/pdet.py
+drwxr-xr-x   0 phurailatpamhemantakumar   (502) staff       (20)        0 2023-08-05 18:47:11.626005 gwsnr-0.1.3/gwsnr.egg-info/
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)      217 2023-08-05 18:47:11.000000 gwsnr-0.1.3/gwsnr.egg-info/PKG-INFO
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)      209 2023-08-05 18:47:11.000000 gwsnr-0.1.3/gwsnr.egg-info/SOURCES.txt
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)        1 2023-08-05 18:47:11.000000 gwsnr-0.1.3/gwsnr.egg-info/dependency_links.txt
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)       83 2023-08-05 18:47:11.000000 gwsnr-0.1.3/gwsnr.egg-info/requires.txt
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)        6 2023-08-05 18:47:11.000000 gwsnr-0.1.3/gwsnr.egg-info/top_level.txt
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)       38 2023-08-05 18:47:11.626410 gwsnr-0.1.3/setup.cfg
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)      536 2023-08-05 18:45:37.000000 gwsnr-0.1.3/setup.py
```

### Comparing `gwsnr-0.1.2/gwsnr/gwsnr.py` & `gwsnr-0.1.3/gwsnr/gwsnr.py`

 * *Files identical despite different names*

### Comparing `gwsnr-0.1.2/setup.py` & `gwsnr-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 setup(name='gwsnr',
-      version='0.1.2',
+      version='0.1.3',
       description='Fast SNR interpolator',
-      author='Hemantakumar, Otto',
+      author='Hemantakumar Phurailatpam',
       license="MIT",
       author_email='hemantaphurailatpam@gmail.com',
       url='https://github.com/hemantaph/gwsnr',
       packages=find_packages(),
       install_requires=[
         "setuptools>=61.1.0",
         "bilby>=1.0.2",
```

