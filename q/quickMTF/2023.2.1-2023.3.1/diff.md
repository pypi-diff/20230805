# Comparing `tmp/quickMTF-2023.2.1.tar.gz` & `tmp/quickMTF-2023.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\quickMTF-2023.2.1.tar", last modified: Sat Aug  5 03:46:21 2023, max compression
+gzip compressed data, was "dist\quickMTF-2023.3.1.tar", last modified: Sat Aug  5 04:43:28 2023, max compression
```

## Comparing `quickMTF-2023.2.1.tar` & `quickMTF-2023.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 03:46:21.000000 quickMTF-2023.2.1/
--rw-rw-rw-   0        0        0     3555 2023-08-05 03:46:21.000000 quickMTF-2023.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-05 03:46:21.000000 quickMTF-2023.2.1/quickMTF.egg-info/
--rw-rw-rw-   0        0        0        1 2023-08-05 03:46:20.000000 quickMTF-2023.2.1/quickMTF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     3555 2023-08-05 03:46:20.000000 quickMTF-2023.2.1/quickMTF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      147 2023-08-05 03:46:20.000000 quickMTF-2023.2.1/quickMTF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 03:46:20.000000 quickMTF-2023.2.1/quickMTF.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2402 2023-08-05 03:41:49.000000 quickMTF-2023.2.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-08-05 03:46:21.000000 quickMTF-2023.2.1/setup.cfg
--rw-rw-rw-   0        0        0      762 2023-08-05 03:46:17.000000 quickMTF-2023.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 04:43:28.000000 quickMTF-2023.3.1/
+-rw-rw-rw-   0        0        0     3682 2023-08-05 04:43:28.000000 quickMTF-2023.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-05 04:43:27.000000 quickMTF-2023.3.1/quickMTF.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-08-05 04:43:26.000000 quickMTF-2023.3.1/quickMTF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     3682 2023-08-05 04:43:26.000000 quickMTF-2023.3.1/quickMTF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2023-08-05 04:43:26.000000 quickMTF-2023.3.1/quickMTF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 04:43:26.000000 quickMTF-2023.3.1/quickMTF.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2521 2023-08-05 03:51:23.000000 quickMTF-2023.3.1/README.rst
+-rw-rw-rw-   0        0        0       42 2023-08-05 04:43:28.000000 quickMTF-2023.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      762 2023-08-05 04:43:09.000000 quickMTF-2023.3.1/setup.py
```

### Comparing `quickMTF-2023.2.1/PKG-INFO` & `quickMTF-2023.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickMTF
-Version: 2023.2.1
+Version: 2023.3.1
 Summary: quick MTF for Line_pair and SFR
 Home-page: https://github.com/Lorrytoolcenter/quickMTF
 Author: lorry_rui
 Author-email: lorryruizhihua@gmail.com
 License: UNKNOWN
 Description: Copyright (c) 2022 lorry_rui , Fremont ,USA  
         
@@ -19,15 +19,16 @@
          
         *for image quaility test purpose like lens focus test   @  Lorry RUi  
         
         
         =======================
         Homepage: quickMTF
         =======================
-        
+        - [PyPI Package Page](https://pypi.org/project/quickMTF/)
+        - [Source Code](https://github.com/Lorrytoolcenter/quickMTF)
         .. image:: https://github.com/Lorrytoolcenter/quickMTF/doc/linepair2.png
            :align: center
         .. image:: doc/linepair2.png
            :width: 600
         
         :github_url: https://github.com/Lorrytoolcenter/quickMTF
```

### Comparing `quickMTF-2023.2.1/quickMTF.egg-info/PKG-INFO` & `quickMTF-2023.3.1/quickMTF.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickMTF
-Version: 2023.2.1
+Version: 2023.3.1
 Summary: quick MTF for Line_pair and SFR
 Home-page: https://github.com/Lorrytoolcenter/quickMTF
 Author: lorry_rui
 Author-email: lorryruizhihua@gmail.com
 License: UNKNOWN
 Description: Copyright (c) 2022 lorry_rui , Fremont ,USA  
         
@@ -19,15 +19,16 @@
          
         *for image quaility test purpose like lens focus test   @  Lorry RUi  
         
         
         =======================
         Homepage: quickMTF
         =======================
-        
+        - [PyPI Package Page](https://pypi.org/project/quickMTF/)
+        - [Source Code](https://github.com/Lorrytoolcenter/quickMTF)
         .. image:: https://github.com/Lorrytoolcenter/quickMTF/doc/linepair2.png
            :align: center
         .. image:: doc/linepair2.png
            :width: 600
         
         :github_url: https://github.com/Lorrytoolcenter/quickMTF
```

### Comparing `quickMTF-2023.2.1/README.rst` & `quickMTF-2023.3.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,16 @@
  
 *for image quaility test purpose like lens focus test   @  Lorry RUi  
 
 
 =======================
 Homepage: quickMTF
 =======================
-
+- [PyPI Package Page](https://pypi.org/project/quickMTF/)
+- [Source Code](https://github.com/Lorrytoolcenter/quickMTF)
 .. image:: https://github.com/Lorrytoolcenter/quickMTF/doc/linepair2.png
    :align: center
 .. image:: doc/linepair2.png
    :width: 600
 
 :github_url: https://github.com/Lorrytoolcenter/quickMTF
```

### Comparing `quickMTF-2023.2.1/setup.py` & `quickMTF-2023.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quickMTF", # Replace with your own username
-    version="2023.2.1",
+    version="2023.3.1",
     author="lorry_rui",
     author_email="lorryruizhihua@gmail.com",
     description="quick MTF for Line_pair and SFR",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Lorrytoolcenter/quickMTF",
     packages=setuptools.find_packages(),
```

