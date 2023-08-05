# Comparing `tmp/LidamaoToolkit-0.12.tar.gz` & `tmp/LidamaoToolkit-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/LidamaoToolkit-0.12.tar", last modified: Sat Aug  5 09:08:07 2023, max compression
+gzip compressed data, was "dist/LidamaoToolkit-0.13.tar", last modified: Sat Aug  5 09:13:28 2023, max compression
```

## Comparing `LidamaoToolkit-0.12.tar` & `LidamaoToolkit-0.13.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxr-xr-x   0 leeperfect   (501) staff       (20)        0 2023-08-05 09:08:07.000000 LidamaoToolkit-0.12/
-drwxr-xr-x   0 leeperfect   (501) staff       (20)        0 2023-08-05 09:08:07.000000 LidamaoToolkit-0.12/LidamaoToolkit/
--rw-r--r--   0 leeperfect   (501) staff       (20)     2337 2023-08-05 07:53:05.000000 LidamaoToolkit-0.12/LidamaoToolkit/LidamaoToolkit.py
--rw-r--r--   0 leeperfect   (501) staff       (20)        0 2023-08-05 07:24:15.000000 LidamaoToolkit-0.12/LidamaoToolkit/__init__.py
-drwxr-xr-x   0 leeperfect   (501) staff       (20)        0 2023-08-05 09:08:07.000000 LidamaoToolkit-0.12/LidamaoToolkit.egg-info/
--rw-r--r--   0 leeperfect   (501) staff       (20)      219 2023-08-05 09:08:07.000000 LidamaoToolkit-0.12/LidamaoToolkit.egg-info/PKG-INFO
--rw-r--r--   0 leeperfect   (501) staff       (20)      267 2023-08-05 09:08:07.000000 LidamaoToolkit-0.12/LidamaoToolkit.egg-info/SOURCES.txt
--rw-r--r--   0 leeperfect   (501) staff       (20)        1 2023-08-05 09:08:07.000000 LidamaoToolkit-0.12/LidamaoToolkit.egg-info/dependency_links.txt
--rw-r--r--   0 leeperfect   (501) staff       (20)       13 2023-08-05 09:08:07.000000 LidamaoToolkit-0.12/LidamaoToolkit.egg-info/requires.txt
--rw-r--r--   0 leeperfect   (501) staff       (20)       15 2023-08-05 09:08:07.000000 LidamaoToolkit-0.12/LidamaoToolkit.egg-info/top_level.txt
--rw-r--r--   0 leeperfect   (501) staff       (20)      219 2023-08-05 09:08:07.000000 LidamaoToolkit-0.12/PKG-INFO
--rw-r--r--   0 leeperfect   (501) staff       (20)        7 2023-08-05 07:25:59.000000 LidamaoToolkit-0.12/README.md
--rw-r--r--   0 leeperfect   (501) staff       (20)       38 2023-08-05 09:08:07.000000 LidamaoToolkit-0.12/setup.cfg
--rw-r--r--   0 leeperfect   (501) staff       (20)      268 2023-08-05 09:07:35.000000 LidamaoToolkit-0.12/setup.py
+drwxr-xr-x   0 leeperfect   (501) staff       (20)        0 2023-08-05 09:13:28.000000 LidamaoToolkit-0.13/
+drwxr-xr-x   0 leeperfect   (501) staff       (20)        0 2023-08-05 09:13:28.000000 LidamaoToolkit-0.13/LidamaoToolkit.egg-info/
+-rw-r--r--   0 leeperfect   (501) staff       (20)      219 2023-08-05 09:13:28.000000 LidamaoToolkit-0.13/LidamaoToolkit.egg-info/PKG-INFO
+-rw-r--r--   0 leeperfect   (501) staff       (20)      225 2023-08-05 09:13:28.000000 LidamaoToolkit-0.13/LidamaoToolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 leeperfect   (501) staff       (20)        1 2023-08-05 09:13:28.000000 LidamaoToolkit-0.13/LidamaoToolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 leeperfect   (501) staff       (20)       13 2023-08-05 09:13:28.000000 LidamaoToolkit-0.13/LidamaoToolkit.egg-info/requires.txt
+-rw-r--r--   0 leeperfect   (501) staff       (20)       15 2023-08-05 09:13:28.000000 LidamaoToolkit-0.13/LidamaoToolkit.egg-info/top_level.txt
+-rw-r--r--   0 leeperfect   (501) staff       (20)     2337 2023-08-05 07:53:05.000000 LidamaoToolkit-0.13/LidamaoToolkit.py
+-rw-r--r--   0 leeperfect   (501) staff       (20)      219 2023-08-05 09:13:28.000000 LidamaoToolkit-0.13/PKG-INFO
+-rw-r--r--   0 leeperfect   (501) staff       (20)        7 2023-08-05 07:25:59.000000 LidamaoToolkit-0.13/README.md
+-rw-r--r--   0 leeperfect   (501) staff       (20)       38 2023-08-05 09:13:28.000000 LidamaoToolkit-0.13/setup.cfg
+-rw-r--r--   0 leeperfect   (501) staff       (20)      270 2023-08-05 09:13:14.000000 LidamaoToolkit-0.13/setup.py
```

### Comparing `LidamaoToolkit-0.12/LidamaoToolkit/LidamaoToolkit.py` & `LidamaoToolkit-0.13/LidamaoToolkit.py`

 * *Files identical despite different names*

