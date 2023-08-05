# Comparing `tmp/calfcv-0.0.7.tar.gz` & `tmp/calfcv-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calfcv-0.0.7.tar", last modified: Sat Jul 29 23:00:05 2023, max compression
+gzip compressed data, was "calfcv-0.0.8.tar", last modified: Sun Jul 30 00:04:43 2023, max compression
```

## Comparing `calfcv-0.0.7.tar` & `calfcv-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 23:00:05.796597 calfcv-0.0.7/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1495 2023-07-29 01:55:36.000000 calfcv-0.0.7/LICENSE
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-24 23:20:23.000000 calfcv-0.0.7/MANIFEST.in
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     4834 2023-07-29 23:00:05.796597 calfcv-0.0.7/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     4206 2023-07-29 22:54:27.000000 calfcv-0.0.7/README.rst
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 23:00:05.796597 calfcv-0.0.7/calfcv/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       98 2023-07-28 23:01:34.000000 calfcv-0.0.7/calfcv/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-07-29 01:59:39.000000 calfcv-0.0.7/calfcv/_version.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     8479 2023-07-29 02:15:49.000000 calfcv-0.0.7/calfcv/calfcv.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 23:00:05.796597 calfcv-0.0.7/calfcv/tests/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-07-24 23:20:23.000000 calfcv-0.0.7/calfcv/tests/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1563 2023-07-28 13:25:35.000000 calfcv-0.0.7/calfcv/tests/test_calfcv.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      257 2023-07-28 12:52:06.000000 calfcv-0.0.7/calfcv/tests/test_common.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 23:00:05.796597 calfcv-0.0.7/calfcv.egg-info/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     4834 2023-07-29 23:00:05.000000 calfcv-0.0.7/calfcv.egg-info/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      380 2023-07-29 23:00:05.000000 calfcv-0.0.7/calfcv.egg-info/SOURCES.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-07-29 23:00:05.000000 calfcv-0.0.7/calfcv.egg-info/dependency_links.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-07-28 23:40:52.000000 calfcv-0.0.7/calfcv.egg-info/not-zip-safe
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-29 23:00:05.000000 calfcv-0.0.7/calfcv.egg-info/requires.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        7 2023-07-29 23:00:05.000000 calfcv-0.0.7/calfcv.egg-info/top_level.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       24 2023-07-24 23:20:23.000000 calfcv-0.0.7/requirements.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-07-29 23:00:05.796597 calfcv-0.0.7/setup.cfg
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1929 2023-07-29 22:59:10.000000 calfcv-0.0.7/setup.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-30 00:04:43.893520 calfcv-0.0.8/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1495 2023-07-29 01:55:36.000000 calfcv-0.0.8/LICENSE
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-24 23:20:23.000000 calfcv-0.0.8/MANIFEST.in
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     4855 2023-07-30 00:04:43.893520 calfcv-0.0.8/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     4227 2023-07-30 00:04:25.000000 calfcv-0.0.8/README.rst
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-30 00:04:43.893520 calfcv-0.0.8/calfcv/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       98 2023-07-28 23:01:34.000000 calfcv-0.0.8/calfcv/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-07-29 01:59:39.000000 calfcv-0.0.8/calfcv/_version.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     8479 2023-07-29 02:15:49.000000 calfcv-0.0.8/calfcv/calfcv.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-30 00:04:43.893520 calfcv-0.0.8/calfcv/tests/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-07-24 23:20:23.000000 calfcv-0.0.8/calfcv/tests/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1563 2023-07-28 13:25:35.000000 calfcv-0.0.8/calfcv/tests/test_calfcv.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      257 2023-07-28 12:52:06.000000 calfcv-0.0.8/calfcv/tests/test_common.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-30 00:04:43.893520 calfcv-0.0.8/calfcv.egg-info/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     4855 2023-07-30 00:04:43.000000 calfcv-0.0.8/calfcv.egg-info/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      380 2023-07-30 00:04:43.000000 calfcv-0.0.8/calfcv.egg-info/SOURCES.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-07-30 00:04:43.000000 calfcv-0.0.8/calfcv.egg-info/dependency_links.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-07-28 23:40:52.000000 calfcv-0.0.8/calfcv.egg-info/not-zip-safe
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-30 00:04:43.000000 calfcv-0.0.8/calfcv.egg-info/requires.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        7 2023-07-30 00:04:43.000000 calfcv-0.0.8/calfcv.egg-info/top_level.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       24 2023-07-24 23:20:23.000000 calfcv-0.0.8/requirements.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-07-30 00:04:43.893520 calfcv-0.0.8/setup.cfg
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1929 2023-07-29 23:07:22.000000 calfcv-0.0.8/setup.py
```

### Comparing `calfcv-0.0.7/LICENSE` & `calfcv-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `calfcv-0.0.7/PKG-INFO` & `calfcv-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calfcv
-Version: 0.0.7
+Version: 0.0.8
 Summary: Coarse approximation linear function with cross validation
 Home-page: 
 Download-URL: https://github.com/scikit-learn-contrib/project-template
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
@@ -12,20 +12,17 @@
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
-.. -*- mode: rst -*-
-
-
-===============
+#####################################
 CalfCV
-===============
+#####################################
 
 A binomial classifier that implements the Coarse Approximation Linear Function (CALF).
 
 Contact
 ------------------
 Rolf Carlson hrolfrc@gmail.com
```

### Comparing `calfcv-0.0.7/README.rst` & `calfcv-0.0.8/calfcv.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,28 @@
-.. -*- mode: rst -*-
+Metadata-Version: 2.1
+Name: calfcv
+Version: 0.0.8
+Summary: Coarse approximation linear function with cross validation
+Home-page: 
+Download-URL: https://github.com/scikit-learn-contrib/project-template
+Maintainer: Carlson Research, LLC
+Maintainer-email: hrolfrc@gmail.com
+License: new BSD
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: License :: OSI Approved
+Classifier: Topic :: Scientific/Engineering
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
 
-
-===============
+#####################################
 CalfCV
-===============
+#####################################
 
 A binomial classifier that implements the Coarse Approximation Linear Function (CALF).
 
 Contact
 ------------------
 Rolf Carlson hrolfrc@gmail.com
```

### Comparing `calfcv-0.0.7/calfcv/calfcv.py` & `calfcv-0.0.8/calfcv/calfcv.py`

 * *Files identical despite different names*

### Comparing `calfcv-0.0.7/calfcv/tests/test_calfcv.py` & `calfcv-0.0.8/calfcv/tests/test_calfcv.py`

 * *Files identical despite different names*

### Comparing `calfcv-0.0.7/calfcv.egg-info/PKG-INFO` & `calfcv-0.0.8/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,10 @@
-Metadata-Version: 2.1
-Name: calfcv
-Version: 0.0.7
-Summary: Coarse approximation linear function with cross validation
-Home-page: 
-Download-URL: https://github.com/scikit-learn-contrib/project-template
-Maintainer: Carlson Research, LLC
-Maintainer-email: hrolfrc@gmail.com
-License: new BSD
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: License :: OSI Approved
-Classifier: Topic :: Scientific/Engineering
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-License-File: LICENSE
-
-.. -*- mode: rst -*-
-
-
-===============
+#####################################
 CalfCV
-===============
+#####################################
 
 A binomial classifier that implements the Coarse Approximation Linear Function (CALF).
 
 Contact
 ------------------
 Rolf Carlson hrolfrc@gmail.com
```

### Comparing `calfcv-0.0.7/setup.py` & `calfcv-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 with codecs.open('README.rst', encoding='utf-8-sig') as f:
     LONG_DESCRIPTION = f.read()
 MAINTAINER = 'Carlson Research, LLC'
 MAINTAINER_EMAIL = 'hrolfrc@gmail.com'
 URL = ''
 LICENSE = 'new BSD'
 DOWNLOAD_URL = 'https://github.com/scikit-learn-contrib/project-template'
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 INSTALL_REQUIRES = ['numpy', 'scipy', 'scikit-learn']
 CLASSIFIERS = ['Intended Audience :: Science/Research',
                'Intended Audience :: Developers',
                'Development Status :: 2 - Pre-Alpha',
                'License :: OSI Approved',
                'Topic :: Scientific/Engineering',
                'Operating System :: OS Independent',
```

