# Comparing `tmp/pyNekobin-2.8.tar.gz` & `tmp/pyNekobin-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyNekobin-2.8.tar", last modified: Sat Aug  5 15:40:46 2023, max compression
+gzip compressed data, was "pyNekobin-2.9.tar", last modified: Sat Aug  5 16:38:19 2023, max compression
```

## Comparing `pyNekobin-2.8.tar` & `pyNekobin-2.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 15:40:46.293666 pyNekobin-2.8/
--rw-rw-rw-   0        0        0     1052 2023-07-26 08:20:42.000000 pyNekobin-2.8/LICENSE
--rw-rw-rw-   0        0        0     4473 2023-08-05 15:40:46.292669 pyNekobin-2.8/PKG-INFO
--rw-rw-rw-   0        0        0     3589 2023-08-05 15:39:16.000000 pyNekobin-2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-08-05 15:40:46.245826 pyNekobin-2.8/nekobin/
--rw-rw-rw-   0        0        0       52 2023-08-05 15:38:34.000000 pyNekobin-2.8/nekobin/__init__.py
--rw-rw-rw-   0        0        0     4431 2023-08-05 15:38:09.000000 pyNekobin-2.8/nekobin/main.py
-drwxrwxrwx   0        0        0        0 2023-08-05 15:40:46.291673 pyNekobin-2.8/pyNekobin.egg-info/
--rw-rw-rw-   0        0        0     4473 2023-08-05 15:40:45.000000 pyNekobin-2.8/pyNekobin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-08-05 15:40:46.000000 pyNekobin-2.8/pyNekobin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 15:40:45.000000 pyNekobin-2.8/pyNekobin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-08-05 15:40:45.000000 pyNekobin-2.8/pyNekobin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-05 15:40:45.000000 pyNekobin-2.8/pyNekobin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-05 15:40:46.293666 pyNekobin-2.8/setup.cfg
--rw-rw-rw-   0        0        0     1639 2023-07-26 08:20:42.000000 pyNekobin-2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 16:38:19.880433 pyNekobin-2.9/
+-rw-rw-rw-   0        0        0     1052 2023-07-26 08:20:42.000000 pyNekobin-2.9/LICENSE
+-rw-rw-rw-   0        0        0     4473 2023-08-05 16:38:19.878205 pyNekobin-2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3589 2023-08-05 15:39:16.000000 pyNekobin-2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 16:38:19.805920 pyNekobin-2.9/nekobin/
+-rw-rw-rw-   0        0        0       50 2023-08-05 16:35:53.000000 pyNekobin-2.9/nekobin/__init__.py
+-rw-rw-rw-   0        0        0     4431 2023-08-05 15:38:09.000000 pyNekobin-2.9/nekobin/main.py
+drwxrwxrwx   0        0        0        0 2023-08-05 16:38:19.876213 pyNekobin-2.9/pyNekobin.egg-info/
+-rw-rw-rw-   0        0        0     4473 2023-08-05 16:38:19.000000 pyNekobin-2.9/pyNekobin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-08-05 16:38:19.000000 pyNekobin-2.9/pyNekobin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 16:38:19.000000 pyNekobin-2.9/pyNekobin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-08-05 16:38:19.000000 pyNekobin-2.9/pyNekobin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-05 16:38:19.000000 pyNekobin-2.9/pyNekobin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 16:38:19.880433 pyNekobin-2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1639 2023-07-26 08:20:42.000000 pyNekobin-2.9/setup.py
```

### Comparing `pyNekobin-2.8/LICENSE` & `pyNekobin-2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyNekobin-2.8/PKG-INFO` & `pyNekobin-2.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyNekobin
-Version: 2.8
+Version: 2.9
 Summary: Paste codes to Nekobin.com with python
 Home-page: https://github.com/Nusab19/pyNekobin
-Download-URL: https://github.com/Nusab19/pyNekobin/releases/tag/pyNekobin-2.8
+Download-URL: https://github.com/Nusab19/pyNekobin/releases/tag/pyNekobin-2.9
 Author: Nusab Taha
 Author-email: nusabtaha33@gmail.com
 License: MIT
 Keywords: Nekobin,pyNekobin,Paste Code,Paste Bin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Education
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pyNekobin Version: 2.8 Summary: Paste codes to
+Metadata-Version: 2.1 Name: pyNekobin Version: 2.9 Summary: Paste codes to
 Nekobin.com with python Home-page: https://github.com/Nusab19/pyNekobin
-Download-URL: https://github.com/Nusab19/pyNekobin/releases/tag/pyNekobin-2.8
+Download-URL: https://github.com/Nusab19/pyNekobin/releases/tag/pyNekobin-2.9
 Author: Nusab Taha Author-email: nusabtaha33@gmail.com License: MIT Keywords:
 Nekobin,pyNekobin,Paste Code,Paste Bin Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Education Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `pyNekobin-2.8/README.md` & `pyNekobin-2.9/README.md`

 * *Files identical despite different names*

### Comparing `pyNekobin-2.8/nekobin/main.py` & `pyNekobin-2.9/nekobin/main.py`

 * *Files identical despite different names*

### Comparing `pyNekobin-2.8/pyNekobin.egg-info/PKG-INFO` & `pyNekobin-2.9/pyNekobin.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyNekobin
-Version: 2.8
+Version: 2.9
 Summary: Paste codes to Nekobin.com with python
 Home-page: https://github.com/Nusab19/pyNekobin
-Download-URL: https://github.com/Nusab19/pyNekobin/releases/tag/pyNekobin-2.8
+Download-URL: https://github.com/Nusab19/pyNekobin/releases/tag/pyNekobin-2.9
 Author: Nusab Taha
 Author-email: nusabtaha33@gmail.com
 License: MIT
 Keywords: Nekobin,pyNekobin,Paste Code,Paste Bin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Education
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pyNekobin Version: 2.8 Summary: Paste codes to
+Metadata-Version: 2.1 Name: pyNekobin Version: 2.9 Summary: Paste codes to
 Nekobin.com with python Home-page: https://github.com/Nusab19/pyNekobin
-Download-URL: https://github.com/Nusab19/pyNekobin/releases/tag/pyNekobin-2.8
+Download-URL: https://github.com/Nusab19/pyNekobin/releases/tag/pyNekobin-2.9
 Author: Nusab Taha Author-email: nusabtaha33@gmail.com License: MIT Keywords:
 Nekobin,pyNekobin,Paste Code,Paste Bin Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Education Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `pyNekobin-2.8/setup.py` & `pyNekobin-2.9/setup.py`

 * *Files identical despite different names*

