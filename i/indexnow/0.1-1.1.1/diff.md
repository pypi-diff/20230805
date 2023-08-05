# Comparing `tmp/IndexNow-0.1.tar.gz` & `tmp/indexnow-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IndexNow-0.1.tar", last modified: Mon Nov 15 15:08:01 2021, max compression
+gzip compressed data, was "indexnow-1.1.1.tar", last modified: Sat Aug  5 16:03:49 2023, max compression
```

## Comparing `IndexNow-0.1.tar` & `indexnow-1.1.1.tar`

### file list

```diff
@@ -1,7 +1,14 @@
-drwxrwxr-x   0 ajitjasrotia  (1000) ajitjasrotia  (1000)        0 2021-11-15 15:08:01.420758 IndexNow-0.1/
-drwxrwxr-x   0 ajitjasrotia  (1000) ajitjasrotia  (1000)        0 2021-11-15 15:08:01.420758 IndexNow-0.1/IndexNow/
--rw-rw-r--   0 ajitjasrotia  (1000) ajitjasrotia  (1000)        0 2021-11-15 15:07:57.360479 IndexNow-0.1/IndexNow/__init__.py
--rw-rw-r--   0 ajitjasrotia  (1000) ajitjasrotia  (1000)      746 2021-11-15 15:08:01.420758 IndexNow-0.1/PKG-INFO
--rw-rw-r--   0 ajitjasrotia  (1000) ajitjasrotia  (1000)        0 2021-11-15 14:46:05.484017 IndexNow-0.1/README.rst
--rw-rw-r--   0 ajitjasrotia  (1000) ajitjasrotia  (1000)       62 2021-11-15 14:58:36.305216 IndexNow-0.1/setup.cfg
--rw-rw-r--   0 ajitjasrotia  (1000) ajitjasrotia  (1000)     1396 2021-11-15 15:07:05.612702 IndexNow-0.1/setup.py
+drwxr-xr-x   0 ajitjasrotia   (501) staff       (20)        0 2023-08-05 16:03:49.033386 indexnow-1.1.1/
+-rw-rw-r--   0 ajitjasrotia   (501) staff       (20)     1070 2021-11-15 15:04:46.000000 indexnow-1.1.1/LICENSE.txt
+-rw-rw-r--   0 ajitjasrotia   (501) staff       (20)        0 2021-11-15 15:07:20.000000 indexnow-1.1.1/MANIFEST.in
+-rw-r--r--   0 ajitjasrotia   (501) staff       (20)     2620 2023-08-05 16:03:49.033778 indexnow-1.1.1/PKG-INFO
+-rw-rw-r--   0 ajitjasrotia   (501) staff       (20)     1768 2023-08-05 15:47:21.000000 indexnow-1.1.1/README.rst
+drwxr-xr-x   0 ajitjasrotia   (501) staff       (20)        0 2023-08-05 16:03:49.031400 indexnow-1.1.1/indexnow/
+-rw-rw-r--   0 ajitjasrotia   (501) staff       (20)     1103 2023-08-05 15:53:59.000000 indexnow-1.1.1/indexnow/__init__.py
+drwxr-xr-x   0 ajitjasrotia   (501) staff       (20)        0 2023-08-05 16:03:49.032766 indexnow-1.1.1/indexnow.egg-info/
+-rw-r--r--   0 ajitjasrotia   (501) staff       (20)     2620 2023-08-05 16:03:48.000000 indexnow-1.1.1/indexnow.egg-info/PKG-INFO
+-rw-r--r--   0 ajitjasrotia   (501) staff       (20)      202 2023-08-05 16:03:48.000000 indexnow-1.1.1/indexnow.egg-info/SOURCES.txt
+-rw-r--r--   0 ajitjasrotia   (501) staff       (20)        1 2023-08-05 16:03:48.000000 indexnow-1.1.1/indexnow.egg-info/dependency_links.txt
+-rw-r--r--   0 ajitjasrotia   (501) staff       (20)        9 2023-08-05 16:03:48.000000 indexnow-1.1.1/indexnow.egg-info/top_level.txt
+-rw-rw-r--   0 ajitjasrotia   (501) staff       (20)       80 2023-08-05 16:03:49.034627 indexnow-1.1.1/setup.cfg
+-rw-rw-r--   0 ajitjasrotia   (501) staff       (20)     1079 2023-08-05 15:44:01.000000 indexnow-1.1.1/setup.py
```

