# Comparing `tmp/plot2vid-1.0.0.tar.gz` & `tmp/plot2vid-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plot2vid-1.0.0.tar", last modified: Sat Aug  5 10:01:21 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `plot2vid-1.0.0.tar` & `plot2vid-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,7 @@
-drwxr-xr-x   0 franciszekszewczyk   (501) staff       (20)        0 2023-08-05 10:01:21.570894 plot2vid-1.0.0/
--rw-r--r--   0 franciszekszewczyk   (501) staff       (20)        0 2023-08-05 08:48:22.000000 plot2vid-1.0.0/LICENSE
--rw-r--r--   0 franciszekszewczyk   (501) staff       (20)     1247 2023-08-05 10:01:21.570505 plot2vid-1.0.0/PKG-INFO
--rw-r--r--   0 franciszekszewczyk   (501) staff       (20)      799 2023-08-05 09:33:36.000000 plot2vid-1.0.0/README.md
--rw-r--r--   0 franciszekszewczyk   (501) staff       (20)      705 2023-08-05 10:01:08.000000 plot2vid-1.0.0/pyproject.toml
--rw-r--r--   0 franciszekszewczyk   (501) staff       (20)       38 2023-08-05 10:01:21.571048 plot2vid-1.0.0/setup.cfg
--rw-r--r--   0 franciszekszewczyk   (501) staff       (20)       50 2023-08-05 09:47:46.000000 plot2vid-1.0.0/setup.py
-drwxr-xr-x   0 franciszekszewczyk   (501) staff       (20)        0 2023-08-05 10:01:21.566897 plot2vid-1.0.0/src/
--rw-r--r--   0 franciszekszewczyk   (501) staff       (20)       22 2023-08-05 09:38:05.000000 plot2vid-1.0.0/src/__init__.py
--rw-r--r--   0 franciszekszewczyk   (501) staff       (20)        0 2023-08-05 09:36:39.000000 plot2vid-1.0.0/src/__main__.py
--rw-r--r--   0 franciszekszewczyk   (501) staff       (20)        0 2023-08-05 09:43:46.000000 plot2vid-1.0.0/src/config.toml
-drwxr-xr-x   0 franciszekszewczyk   (501) staff       (20)        0 2023-08-05 10:01:21.570003 plot2vid-1.0.0/src/plot2vid.egg-info/
--rw-r--r--   0 franciszekszewczyk   (501) staff       (20)     1247 2023-08-05 10:01:21.000000 plot2vid-1.0.0/src/plot2vid.egg-info/PKG-INFO
--rw-r--r--   0 franciszekszewczyk   (501) staff       (20)      284 2023-08-05 10:01:21.000000 plot2vid-1.0.0/src/plot2vid.egg-info/SOURCES.txt
--rw-r--r--   0 franciszekszewczyk   (501) staff       (20)        1 2023-08-05 10:01:21.000000 plot2vid-1.0.0/src/plot2vid.egg-info/dependency_links.txt
--rw-r--r--   0 franciszekszewczyk   (501) staff       (20)       56 2023-08-05 10:01:21.000000 plot2vid-1.0.0/src/plot2vid.egg-info/requires.txt
--rw-r--r--   0 franciszekszewczyk   (501) staff       (20)       27 2023-08-05 10:01:21.000000 plot2vid-1.0.0/src/plot2vid.egg-info/top_level.txt
--rw-r--r--   0 franciszekszewczyk   (501) staff       (20)     1396 2023-08-05 09:52:05.000000 plot2vid-1.0.0/src/recorder.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 plot2vid-1.0.1/src/plot2vid/__init__.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 plot2vid-1.0.1/src/plot2vid/recorder.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 plot2vid-1.0.1/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plot2vid-1.0.1/LICENSE
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 plot2vid-1.0.1/README.md
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 plot2vid-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 plot2vid-1.0.1/PKG-INFO
```

### Comparing `plot2vid-1.0.0/PKG-INFO` & `plot2vid-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: plot2vid
-Version: 1.0.0
+Version: 1.0.1
 Summary: The easiest way to create animations using plots.
-Author-email: Franciszek Szewczyk <szewczyk.franciszek02@gmail.com>
 Project-URL: Homepage, https://github.com/fszewczyk/plot2vid
-Keywords: plot,animation,video
+Author-email: Franciszek Szewczyk <szewczyk.franciszek02@gmail.com>
+License-File: LICENSE
+Keywords: animation,plot,video
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
+Requires-Dist: matplotlib>=3.6.0
+Requires-Dist: numpy>=1.24.3
+Requires-Dist: opencv-python>=4.6.0.66
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # plot2vid
 
 _The easiest way to create animations using plots._
 
 This small Python package lets you store seperate matplotlib plots to create a video.
```

### Comparing `plot2vid-1.0.0/README.md` & `plot2vid-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `plot2vid-1.0.0/src/recorder.py` & `plot2vid-1.0.1/src/plot2vid/recorder.py`

 * *Files identical despite different names*

