# Comparing `tmp/sourmash_mixers-0.2.1.tar.gz` & `tmp/sourmash_mixers-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourmash_mixers-0.2.1.tar", last modified: Thu Aug  3 14:10:22 2023, max compression
+gzip compressed data, was "sourmash_mixers-0.2.2.tar", last modified: Sat Aug  5 12:06:29 2023, max compression
```

## Comparing `sourmash_mixers-0.2.1.tar` & `sourmash_mixers-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-03 14:10:22.127921 sourmash_mixers-0.2.1/
--rw-r--r--   0 t          (502) staff       (20)     1501 2023-07-27 23:30:51.000000 sourmash_mixers-0.2.1/LICENSE
--rw-r--r--   0 t          (502) staff       (20)      289 2023-08-03 14:10:22.127779 sourmash_mixers-0.2.1/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)       74 2023-07-27 23:30:51.000000 sourmash_mixers-0.2.1/README.md
--rw-r--r--   0 t          (502) staff       (20)      622 2023-08-03 14:08:51.000000 sourmash_mixers-0.2.1/pyproject.toml
--rw-r--r--   0 t          (502) staff       (20)       38 2023-08-03 14:10:22.127960 sourmash_mixers-0.2.1/setup.cfg
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-03 14:10:22.127635 sourmash_mixers-0.2.1/sourmash_mixers.egg-info/
--rw-r--r--   0 t          (502) staff       (20)      289 2023-08-03 14:10:22.000000 sourmash_mixers-0.2.1/sourmash_mixers.egg-info/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)      226 2023-08-03 14:10:22.000000 sourmash_mixers-0.2.1/sourmash_mixers.egg-info/SOURCES.txt
--rw-r--r--   0 t          (502) staff       (20)        1 2023-08-03 14:10:22.000000 sourmash_mixers-0.2.1/sourmash_mixers.egg-info/dependency_links.txt
--rw-r--r--   0 t          (502) staff       (20)      166 2023-08-03 14:10:22.000000 sourmash_mixers-0.2.1/sourmash_mixers.egg-info/requires.txt
--rw-r--r--   0 t          (502) staff       (20)        1 2023-08-03 14:10:22.000000 sourmash_mixers-0.2.1/sourmash_mixers.egg-info/top_level.txt
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-05 12:06:29.317790 sourmash_mixers-0.2.2/
+-rw-r--r--   0 t          (502) staff       (20)     1501 2023-07-27 23:30:51.000000 sourmash_mixers-0.2.2/LICENSE
+-rw-r--r--   0 t          (502) staff       (20)     3221 2023-08-05 12:06:29.317664 sourmash_mixers-0.2.2/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)     3006 2023-08-05 12:05:23.000000 sourmash_mixers-0.2.2/README.md
+-rw-r--r--   0 t          (502) staff       (20)      622 2023-08-05 12:05:29.000000 sourmash_mixers-0.2.2/pyproject.toml
+-rw-r--r--   0 t          (502) staff       (20)       38 2023-08-05 12:06:29.317822 sourmash_mixers-0.2.2/setup.cfg
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-05 12:06:29.317516 sourmash_mixers-0.2.2/sourmash_mixers.egg-info/
+-rw-r--r--   0 t          (502) staff       (20)     3221 2023-08-05 12:06:29.000000 sourmash_mixers-0.2.2/sourmash_mixers.egg-info/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)      226 2023-08-05 12:06:29.000000 sourmash_mixers-0.2.2/sourmash_mixers.egg-info/SOURCES.txt
+-rw-r--r--   0 t          (502) staff       (20)        1 2023-08-05 12:06:29.000000 sourmash_mixers-0.2.2/sourmash_mixers.egg-info/dependency_links.txt
+-rw-r--r--   0 t          (502) staff       (20)      166 2023-08-05 12:06:29.000000 sourmash_mixers-0.2.2/sourmash_mixers.egg-info/requires.txt
+-rw-r--r--   0 t          (502) staff       (20)        1 2023-08-05 12:06:29.000000 sourmash_mixers-0.2.2/sourmash_mixers.egg-info/top_level.txt
```

### Comparing `sourmash_mixers-0.2.1/LICENSE` & `sourmash_mixers-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sourmash_mixers-0.2.1/pyproject.toml` & `sourmash_mixers-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "sourmash_mixers"
 description = "this meta-package installs a collection of sourmash plugins!"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.2.1"
+version = "0.2.2"
 
 dependencies = ["sourmash>=4.8.0,<5",
                 "sourmash_plugin_venn>=0.4",
                 "get-some-ncbi-genomes>=0.2",
                 "sourmash_plugin_commonhash>=0.3",
                 "sourmash_plugin_abundhist>=0.3",
                 "sourmash_plugin_sketchall>=0.2",
```

