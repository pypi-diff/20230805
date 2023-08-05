# Comparing `tmp/pssepath-0.2.2.tar.gz` & `tmp/pssepath-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pssepath-0.2.2.tar", last modified: Wed Aug  2 03:43:34 2023, max compression
+gzip compressed data, was "pssepath-0.2.3.tar", last modified: Sat Aug  5 02:56:23 2023, max compression
```

## Comparing `pssepath-0.2.2.tar` & `pssepath-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 danielhillier   (501) staff       (20)        0 2023-08-02 03:43:34.280082 pssepath-0.2.2/
--rw-r--r--   0 danielhillier   (501) staff       (20)     1072 2023-08-02 03:12:39.000000 pssepath-0.2.2/LICENSE
--rw-r--r--   0 danielhillier   (501) staff       (20)       27 2023-08-02 03:12:39.000000 pssepath-0.2.2/MANIFEST.in
--rw-r--r--   0 danielhillier   (501) staff       (20)     6339 2023-08-02 03:43:34.279946 pssepath-0.2.2/PKG-INFO
--rw-r--r--   0 danielhillier   (501) staff       (20)     5312 2023-08-02 03:12:39.000000 pssepath-0.2.2/README.md
-drwxr-xr-x   0 danielhillier   (501) staff       (20)        0 2023-08-02 03:43:34.279009 pssepath-0.2.2/pssepath/
--rw-r--r--   0 danielhillier   (501) staff       (20)      150 2023-08-02 03:12:39.000000 pssepath-0.2.2/pssepath/__init__.py
--rw-r--r--   0 danielhillier   (501) staff       (20)       63 2023-08-02 03:12:39.000000 pssepath-0.2.2/pssepath/__version__.py
-drwxr-xr-x   0 danielhillier   (501) staff       (20)        0 2023-08-02 03:43:34.279776 pssepath-0.2.2/pssepath/compat/
--rw-r--r--   0 danielhillier   (501) staff       (20)      614 2023-08-02 03:12:39.000000 pssepath-0.2.2/pssepath/compat/__init__.py
--rw-r--r--   0 danielhillier   (501) staff       (20)       88 2023-08-02 03:12:39.000000 pssepath-0.2.2/pssepath/compat/_compat2.py
--rw-r--r--   0 danielhillier   (501) staff       (20)       85 2023-08-02 03:12:39.000000 pssepath-0.2.2/pssepath/compat/_compat3.py
--rw-r--r--   0 danielhillier   (501) staff       (20)    22791 2023-08-02 03:12:39.000000 pssepath-0.2.2/pssepath/core.py
--rw-r--r--   0 danielhillier   (501) staff       (20)     3954 2023-08-02 03:12:39.000000 pssepath-0.2.2/pssepath/helpers.py
--rw-r--r--   0 danielhillier   (501) staff       (20)      602 2023-08-02 03:12:39.000000 pssepath-0.2.2/pssepath/pssepathinfo.py
-drwxr-xr-x   0 danielhillier   (501) staff       (20)        0 2023-08-02 03:43:34.279414 pssepath-0.2.2/pssepath.egg-info/
--rw-r--r--   0 danielhillier   (501) staff       (20)     6339 2023-08-02 03:43:34.000000 pssepath-0.2.2/pssepath.egg-info/PKG-INFO
--rw-r--r--   0 danielhillier   (501) staff       (20)      357 2023-08-02 03:43:34.000000 pssepath-0.2.2/pssepath.egg-info/SOURCES.txt
--rw-r--r--   0 danielhillier   (501) staff       (20)        1 2023-08-02 03:43:34.000000 pssepath-0.2.2/pssepath.egg-info/dependency_links.txt
--rw-r--r--   0 danielhillier   (501) staff       (20)        9 2023-08-02 03:43:34.000000 pssepath-0.2.2/pssepath.egg-info/top_level.txt
--rw-r--r--   0 danielhillier   (501) staff       (20)       38 2023-08-02 03:43:34.280115 pssepath-0.2.2/setup.cfg
--rw-r--r--   0 danielhillier   (501) staff       (20)     3525 2023-08-02 03:12:39.000000 pssepath-0.2.2/setup.py
+drwxr-xr-x   0 danielhillier   (501) staff       (20)        0 2023-08-05 02:56:23.660636 pssepath-0.2.3/
+-rw-r--r--   0 danielhillier   (501) staff       (20)     1072 2023-08-02 03:12:39.000000 pssepath-0.2.3/LICENSE
+-rw-r--r--   0 danielhillier   (501) staff       (20)       27 2023-08-02 03:12:39.000000 pssepath-0.2.3/MANIFEST.in
+-rw-r--r--   0 danielhillier   (501) staff       (20)     6339 2023-08-05 02:56:23.660488 pssepath-0.2.3/PKG-INFO
+-rw-r--r--   0 danielhillier   (501) staff       (20)     5312 2023-08-02 03:12:39.000000 pssepath-0.2.3/README.md
+drwxr-xr-x   0 danielhillier   (501) staff       (20)        0 2023-08-05 02:56:23.659168 pssepath-0.2.3/pssepath/
+-rw-r--r--   0 danielhillier   (501) staff       (20)      150 2023-08-02 03:12:39.000000 pssepath-0.2.3/pssepath/__init__.py
+-rw-r--r--   0 danielhillier   (501) staff       (20)       63 2023-08-05 02:52:52.000000 pssepath-0.2.3/pssepath/__version__.py
+drwxr-xr-x   0 danielhillier   (501) staff       (20)        0 2023-08-05 02:56:23.660268 pssepath-0.2.3/pssepath/compat/
+-rw-r--r--   0 danielhillier   (501) staff       (20)      614 2023-08-02 03:12:39.000000 pssepath-0.2.3/pssepath/compat/__init__.py
+-rw-r--r--   0 danielhillier   (501) staff       (20)       88 2023-08-02 03:12:39.000000 pssepath-0.2.3/pssepath/compat/_compat2.py
+-rw-r--r--   0 danielhillier   (501) staff       (20)       85 2023-08-02 03:12:39.000000 pssepath-0.2.3/pssepath/compat/_compat3.py
+-rw-r--r--   0 danielhillier   (501) staff       (20)    22713 2023-08-05 02:49:50.000000 pssepath-0.2.3/pssepath/core.py
+-rw-r--r--   0 danielhillier   (501) staff       (20)     5309 2023-08-05 02:50:38.000000 pssepath-0.2.3/pssepath/helpers.py
+-rw-r--r--   0 danielhillier   (501) staff       (20)      602 2023-08-02 03:12:39.000000 pssepath-0.2.3/pssepath/pssepathinfo.py
+drwxr-xr-x   0 danielhillier   (501) staff       (20)        0 2023-08-05 02:56:23.659705 pssepath-0.2.3/pssepath.egg-info/
+-rw-r--r--   0 danielhillier   (501) staff       (20)     6339 2023-08-05 02:56:23.000000 pssepath-0.2.3/pssepath.egg-info/PKG-INFO
+-rw-r--r--   0 danielhillier   (501) staff       (20)      357 2023-08-05 02:56:23.000000 pssepath-0.2.3/pssepath.egg-info/SOURCES.txt
+-rw-r--r--   0 danielhillier   (501) staff       (20)        1 2023-08-05 02:56:23.000000 pssepath-0.2.3/pssepath.egg-info/dependency_links.txt
+-rw-r--r--   0 danielhillier   (501) staff       (20)        9 2023-08-05 02:56:23.000000 pssepath-0.2.3/pssepath.egg-info/top_level.txt
+-rw-r--r--   0 danielhillier   (501) staff       (20)       38 2023-08-05 02:56:23.660678 pssepath-0.2.3/setup.cfg
+-rw-r--r--   0 danielhillier   (501) staff       (20)     3525 2023-08-02 03:12:39.000000 pssepath-0.2.3/setup.py
```

### Comparing `pssepath-0.2.2/LICENSE` & `pssepath-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pssepath-0.2.2/PKG-INFO` & `pssepath-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pssepath
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simplified PSSe python importing
 Home-page: https://github.com/danifus/pssepath
 Author: Daniel Hillier
 Author-email: daniel.hillier@gmail.com
 License: MIT
 Keywords: psse extension utility pssepath
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pssepath-0.2.2/README.md` & `pssepath-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pssepath-0.2.2/pssepath/compat/__init__.py` & `pssepath-0.2.3/pssepath/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `pssepath-0.2.2/pssepath/core.py` & `pssepath-0.2.3/pssepath/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -501,16 +501,14 @@
         eg. ("2.7", "32bit")
     """
     probable_pyc = os.path.join(psspy_dir, "psspy.pyc")
     if not os.path.isfile(probable_pyc):
         return None
 
     py_ver = helpers.read_magic_number(probable_pyc)
-    # only the first 3 digits are important (2.x etc)
-    py_ver = py_ver[:3]
     if psse_ver is None:
         return py_ver, None
     else:
         return py_ver, get_psse_arch(psse_ver)
 
 
 def get_required_python_ver_psse_33_and_older(pssbin, psse_ver):
```

### Comparing `pssepath-0.2.2/pssepath/pssepathinfo.py` & `pssepath-0.2.3/pssepath/pssepathinfo.py`

 * *Files identical despite different names*

### Comparing `pssepath-0.2.2/pssepath.egg-info/PKG-INFO` & `pssepath-0.2.3/pssepath.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pssepath
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simplified PSSe python importing
 Home-page: https://github.com/danifus/pssepath
 Author: Daniel Hillier
 Author-email: daniel.hillier@gmail.com
 License: MIT
 Keywords: psse extension utility pssepath
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pssepath-0.2.2/setup.py` & `pssepath-0.2.3/setup.py`

 * *Files identical despite different names*

