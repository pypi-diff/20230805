# Comparing `tmp/indexnow-0.0.2.tar.gz` & `tmp/indexnow-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indexnow-0.0.2.tar", last modified: Mon Nov 15 18:49:53 2021, max compression
+gzip compressed data, was "indexnow-1.0.0.tar", last modified: Sat Aug  5 17:57:08 2023, max compression
```

## Comparing `indexnow-0.0.2.tar` & `indexnow-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,14 @@
-drwxrwxr-x   0 ajitjasrotia  (1000) ajitjasrotia  (1000)        0 2021-11-15 18:49:53.950495 indexnow-0.0.2/
--rw-rw-r--   0 ajitjasrotia  (1000) ajitjasrotia  (1000)      712 2021-11-15 18:49:53.950495 indexnow-0.0.2/PKG-INFO
--rw-rw-r--   0 ajitjasrotia  (1000) ajitjasrotia  (1000)        0 2021-11-15 14:46:05.484017 indexnow-0.0.2/README.rst
-drwxrwxr-x   0 ajitjasrotia  (1000) ajitjasrotia  (1000)        0 2021-11-15 18:49:53.950495 indexnow-0.0.2/indexnow/
--rw-rw-r--   0 ajitjasrotia  (1000) ajitjasrotia  (1000)       70 2021-11-15 15:16:29.436784 indexnow-0.0.2/indexnow/__init__.py
--rw-rw-r--   0 ajitjasrotia  (1000) ajitjasrotia  (1000)       62 2021-11-15 14:58:36.305216 indexnow-0.0.2/setup.cfg
--rw-rw-r--   0 ajitjasrotia  (1000) ajitjasrotia  (1000)      814 2021-11-15 18:49:48.482426 indexnow-0.0.2/setup.py
+drwxr-xr-x   0 ajitjasrotia   (501) staff       (20)        0 2023-08-05 17:57:08.072873 indexnow-1.0.0/
+-rw-rw-r--   0 ajitjasrotia   (501) staff       (20)     1070 2023-08-05 16:55:27.000000 indexnow-1.0.0/LICENSE.txt
+-rw-rw-r--   0 ajitjasrotia   (501) staff       (20)        0 2021-11-15 15:07:20.000000 indexnow-1.0.0/MANIFEST.in
+-rw-r--r--   0 ajitjasrotia   (501) staff       (20)     2716 2023-08-05 17:57:08.073015 indexnow-1.0.0/PKG-INFO
+-rw-rw-r--   0 ajitjasrotia   (501) staff       (20)     1864 2023-08-05 17:31:12.000000 indexnow-1.0.0/README.rst
+drwxr-xr-x   0 ajitjasrotia   (501) staff       (20)        0 2023-08-05 17:57:08.071626 indexnow-1.0.0/indexnow/
+-rw-rw-r--   0 ajitjasrotia   (501) staff       (20)     1114 2023-08-05 17:43:16.000000 indexnow-1.0.0/indexnow/__init__.py
+drwxr-xr-x   0 ajitjasrotia   (501) staff       (20)        0 2023-08-05 17:57:08.072661 indexnow-1.0.0/indexnow.egg-info/
+-rw-r--r--   0 ajitjasrotia   (501) staff       (20)     2716 2023-08-05 17:57:08.000000 indexnow-1.0.0/indexnow.egg-info/PKG-INFO
+-rw-r--r--   0 ajitjasrotia   (501) staff       (20)      202 2023-08-05 17:57:08.000000 indexnow-1.0.0/indexnow.egg-info/SOURCES.txt
+-rw-r--r--   0 ajitjasrotia   (501) staff       (20)        1 2023-08-05 17:57:08.000000 indexnow-1.0.0/indexnow.egg-info/dependency_links.txt
+-rw-r--r--   0 ajitjasrotia   (501) staff       (20)        9 2023-08-05 17:57:08.000000 indexnow-1.0.0/indexnow.egg-info/top_level.txt
+-rw-rw-r--   0 ajitjasrotia   (501) staff       (20)       80 2023-08-05 17:57:08.073359 indexnow-1.0.0/setup.cfg
+-rw-rw-r--   0 ajitjasrotia   (501) staff       (20)     1079 2023-08-05 17:56:56.000000 indexnow-1.0.0/setup.py
```

### Comparing `indexnow-0.0.2/setup.py` & `indexnow-1.0.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,35 @@
-from distutils.core import setup
+import os
+
+from setuptools import setup
+
+long_description = ""
+
+if os.path.isfile("README.rst"):
+    with open("README.rst") as f:
+        long_description = f.read()
 
 setup(
-    name = 'indexnow',
-    packages = ['indexnow'],
-    version = '0.0.2',
+    name='indexnow',
+    packages=['indexnow'],
+    version='1.0.0',
     license='MIT',
-    description = 'TYPE YOUR DESCRIPTION HERE',
-    author = 'Ajit Jasrotia',
-    author_email = 'ajitjasrotia012@gmail.com',
-    url = 'https://github.com/ajitjasrotia/indexnow',
-    download_url = 'https://github.com/ajitjasrotia/indexnow/archive/v_01.tar.gz',
-    keywords = ['index', 'indexnow'],
+    description='An IndexNow URL submitter for Python.',
+    long_description=long_description,
+    author='Ajit Jasrotia',
+    author_email='ajitjasrotia012@gmail.com',
+    url='https://github.com/ajitjasrotia/indexnow',
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Build Tools',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Topic :: Utilities",
     ],
 )
```

