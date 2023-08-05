# Comparing `tmp/pysensibo-1.0.8.tar.gz` & `tmp/pysensibo-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysensibo-1.0.8.tar", last modified: Wed Mar  2 21:17:59 2022, max compression
+gzip compressed data, was "pysensibo-1.0.9.tar", last modified: Sun Mar 20 13:02:02 2022, max compression
```

## Comparing `pysensibo-1.0.8.tar` & `pysensibo-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-03-02 21:17:58.993766 pysensibo-1.0.8/
--rw-rw-rw-   0        0        0     1084 2022-02-13 19:48:00.000000 pysensibo-1.0.8/LICENSE
--rw-rw-rw-   0        0        0      654 2022-03-02 21:17:58.995757 pysensibo-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       99 2022-02-13 19:48:00.000000 pysensibo-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-03-02 21:17:58.949360 pysensibo-1.0.8/pysensibo/
--rw-rw-rw-   0        0        0    10721 2022-03-02 21:14:08.000000 pysensibo-1.0.8/pysensibo/__init__.py
--rw-rw-rw-   0        0        0      479 2022-02-20 09:34:02.000000 pysensibo-1.0.8/pysensibo/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-03-02 21:17:58.990942 pysensibo-1.0.8/pysensibo.egg-info/
--rw-rw-rw-   0        0        0      654 2022-03-02 21:17:58.000000 pysensibo-1.0.8/pysensibo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2022-03-02 21:17:58.000000 pysensibo-1.0.8/pysensibo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-02 21:17:58.000000 pysensibo-1.0.8/pysensibo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-03-02 21:17:58.000000 pysensibo-1.0.8/pysensibo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-03-02 21:17:58.000000 pysensibo-1.0.8/pysensibo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-02-19 14:37:53.000000 pysensibo-1.0.8/pysensibo.egg-info/zip-safe
--rw-rw-rw-   0        0        0       86 2022-03-02 21:17:59.000982 pysensibo-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      911 2022-03-02 21:12:50.000000 pysensibo-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-03-20 13:02:02.414723 pysensibo-1.0.9/
+-rw-rw-rw-   0        0        0     1084 2022-02-13 19:48:00.000000 pysensibo-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0      654 2022-03-20 13:02:02.415717 pysensibo-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       99 2022-02-13 19:48:00.000000 pysensibo-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-03-20 13:02:02.184606 pysensibo-1.0.9/pysensibo/
+-rw-rw-rw-   0        0        0    16273 2022-03-20 10:39:46.000000 pysensibo-1.0.9/pysensibo/__init__.py
+-rw-rw-rw-   0        0        0      479 2022-03-20 09:23:24.000000 pysensibo-1.0.9/pysensibo/exceptions.py
+-rw-rw-rw-   0        0        0     1841 2022-03-20 10:57:31.000000 pysensibo-1.0.9/pysensibo/model.py
+drwxrwxrwx   0        0        0        0 2022-03-20 13:02:02.411752 pysensibo-1.0.9/pysensibo.egg-info/
+-rw-rw-rw-   0        0        0      654 2022-03-20 13:02:00.000000 pysensibo-1.0.9/pysensibo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2022-03-20 13:02:00.000000 pysensibo-1.0.9/pysensibo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-03-20 13:02:00.000000 pysensibo-1.0.9/pysensibo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2022-03-20 13:02:00.000000 pysensibo-1.0.9/pysensibo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2022-03-20 13:02:00.000000 pysensibo-1.0.9/pysensibo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-02-19 14:37:53.000000 pysensibo-1.0.9/pysensibo.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       86 2022-03-20 13:02:02.418761 pysensibo-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      911 2022-03-20 10:57:31.000000 pysensibo-1.0.9/setup.py
```

### Comparing `pysensibo-1.0.8/LICENSE` & `pysensibo-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pysensibo-1.0.8/PKG-INFO` & `pysensibo-1.0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysensibo
-Version: 1.0.8
+Version: 1.0.9
 Summary: asyncio-friendly python API for Sensibo
 Home-page: https://github.com/andrey-git/pysensibo
 Author: andrey-git
 Author-email: andrey-git@users.noreply.github.com
 License: MIT
 Keywords: Sensibo
 Platform: UNKNOWN
```

### Comparing `pysensibo-1.0.8/pysensibo.egg-info/PKG-INFO` & `pysensibo-1.0.9/pysensibo.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysensibo
-Version: 1.0.8
+Version: 1.0.9
 Summary: asyncio-friendly python API for Sensibo
 Home-page: https://github.com/andrey-git/pysensibo
 Author: andrey-git
 Author-email: andrey-git@users.noreply.github.com
 License: MIT
 Keywords: Sensibo
 Platform: UNKNOWN
```

### Comparing `pysensibo-1.0.8/setup.py` & `pysensibo-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """A setuptools based setup module."""
 
 from setuptools import setup, find_packages
 
 print(find_packages())
 setup(
     name='pysensibo',
-    version='1.0.8',
+    version='1.0.9',
     description='asyncio-friendly python API for Sensibo',
     long_description='asyncio-friendly python API for Sensibo'
                      '(https://sensibo.com). Requires Python 3.4+',
     url='https://github.com/andrey-git/pysensibo',
     license='MIT',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

