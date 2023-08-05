# Comparing `tmp/stream_unzip-0.0.88.tar.gz` & `tmp/stream-unzip-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "/Users/dituser/dev/stream-unzip/dist/tmp74d7pg01/stream-unzip-0.0.9.tar", last modified: Tue May 18 03:10:27 2021, max compression
```

## Comparing `stream_unzip-0.0.88.tar` & `stream-unzip-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,12 @@
--rw-r--r--   0        0        0    20342 2020-02-02 00:00:00.000000 stream_unzip-0.0.88/stream_unzip.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 stream_unzip-0.0.88/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 stream_unzip-0.0.88/LICENSE
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 stream_unzip-0.0.88/README.md
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 stream_unzip-0.0.88/pyproject.toml
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 stream_unzip-0.0.88/PKG-INFO
+drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-05-18 03:10:27.987233 stream-unzip-0.0.9/
+-rw-r--r--   0 dituser    (501) staff       (20)     1091 2021-05-16 14:23:12.000000 stream-unzip-0.0.9/LICENSE
+-rw-r--r--   0 dituser    (501) staff       (20)     2521 2021-05-18 03:10:27.986728 stream-unzip-0.0.9/PKG-INFO
+-rw-r--r--   0 dituser    (501) staff       (20)     1701 2021-05-17 09:27:01.000000 stream-unzip-0.0.9/README.md
+-rw-r--r--   0 dituser    (501) staff       (20)       38 2021-05-18 03:10:27.987368 stream-unzip-0.0.9/setup.cfg
+-rw-r--r--   0 dituser    (501) staff       (20)      782 2021-05-18 03:09:44.000000 stream-unzip-0.0.9/setup.py
+drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-05-18 03:10:27.986064 stream-unzip-0.0.9/stream_unzip.egg-info/
+-rw-r--r--   0 dituser    (501) staff       (20)     2521 2021-05-18 03:10:27.000000 stream-unzip-0.0.9/stream_unzip.egg-info/PKG-INFO
+-rw-r--r--   0 dituser    (501) staff       (20)      186 2021-05-18 03:10:27.000000 stream-unzip-0.0.9/stream_unzip.egg-info/SOURCES.txt
+-rw-r--r--   0 dituser    (501) staff       (20)        1 2021-05-18 03:10:27.000000 stream-unzip-0.0.9/stream_unzip.egg-info/dependency_links.txt
+-rw-r--r--   0 dituser    (501) staff       (20)       13 2021-05-18 03:10:27.000000 stream-unzip-0.0.9/stream_unzip.egg-info/top_level.txt
+-rw-r--r--   0 dituser    (501) staff       (20)     5497 2021-05-18 03:09:34.000000 stream-unzip-0.0.9/stream_unzip.py
```

### Comparing `stream_unzip-0.0.88/LICENSE` & `stream-unzip-0.0.9/LICENSE`

 * *Files identical despite different names*

