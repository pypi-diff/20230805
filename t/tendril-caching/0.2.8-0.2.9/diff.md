# Comparing `tmp/tendril-caching-0.2.8.tar.gz` & `tmp/tendril-caching-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-caching-0.2.8.tar", last modified: Fri Jun 30 18:10:02 2023, max compression
+gzip compressed data, was "tendril-caching-0.2.9.tar", last modified: Sat Aug  5 20:52:41 2023, max compression
```

## Comparing `tendril-caching-0.2.8.tar` & `tendril-caching-0.2.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 18:10:02.639705 tendril-caching-0.2.8/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-11-29 08:29:31.000000 tendril-caching-0.2.8/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-11-29 08:29:31.000000 tendril-caching-0.2.8/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-11-29 08:29:31.000000 tendril-caching-0.2.8/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-11-29 08:29:31.000000 tendril-caching-0.2.8/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-11-29 08:29:31.000000 tendril-caching-0.2.8/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-11-29 08:29:31.000000 tendril-caching-0.2.8/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3481 2023-06-30 18:10:02.639705 tendril-caching-0.2.8/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2192 2022-11-29 08:29:31.000000 tendril-caching-0.2.8/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 18:10:02.635705 tendril-caching-0.2.8/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-11-29 08:29:31.000000 tendril-caching-0.2.8/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 18:10:02.635705 tendril-caching-0.2.8/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-11-29 08:29:31.000000 tendril-caching-0.2.8/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-11-29 08:29:31.000000 tendril-caching-0.2.8/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-11-29 08:29:31.000000 tendril-caching-0.2.8/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-11-29 08:29:31.000000 tendril-caching-0.2.8/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 18:10:02.635705 tendril-caching-0.2.8/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-caching-0.2.8/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 18:10:02.635705 tendril-caching-0.2.8/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-11-29 08:29:31.000000 tendril-caching-0.2.8/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13460 2022-11-29 08:29:31.000000 tendril-caching-0.2.8/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      903 2022-11-29 08:29:31.000000 tendril-caching-0.2.8/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1536 2022-11-29 08:29:31.000000 tendril-caching-0.2.8/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 18:10:02.639705 tendril-caching-0.2.8/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-11-29 08:29:31.000000 tendril-caching-0.2.8/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-11-29 08:29:31.000000 tendril-caching-0.2.8/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-06-30 18:10:02.643705 tendril-caching-0.2.8/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3133 2022-11-29 09:11:32.000000 tendril-caching-0.2.8/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 18:10:02.631705 tendril-caching-0.2.8/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 18:10:02.639705 tendril-caching-0.2.8/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2022-11-29 08:29:31.000000 tendril-caching-0.2.8/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 18:10:02.639705 tendril-caching-0.2.8/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 10:22:20.000000 tendril-caching-0.2.8/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 18:10:02.639705 tendril-caching-0.2.8/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 10:22:45.000000 tendril-caching-0.2.8/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      863 2023-06-26 13:20:44.000000 tendril-caching-0.2.8/src/tendril/apiserver/routers/tokens.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 18:10:02.639705 tendril-caching-0.2.8/src/tendril/caching/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      449 2022-11-29 14:28:12.000000 tendril-caching-0.2.8/src/tendril/caching/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 18:10:02.639705 tendril-caching-0.2.8/src/tendril/caching/providers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-11-29 08:53:59.000000 tendril-caching-0.2.8/src/tendril/caching/providers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      272 2022-11-29 13:57:11.000000 tendril-caching-0.2.8/src/tendril/caching/providers/dummy.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1910 2022-11-29 14:11:44.000000 tendril-caching-0.2.8/src/tendril/caching/providers/redis.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4594 2023-06-30 18:07:40.000000 tendril-caching-0.2.8/src/tendril/caching/tokens.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2349 2023-06-25 19:47:22.000000 tendril-caching-0.2.8/src/tendril/caching/transit.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 18:10:02.639705 tendril-caching-0.2.8/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:07.000000 tendril-caching-0.2.8/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1689 2023-06-26 10:43:35.000000 tendril-caching-0.2.8/src/tendril/config/caching.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 18:10:02.639705 tendril-caching-0.2.8/src/tendril_caching.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3481 2023-06-30 18:10:02.000000 tendril-caching-0.2.8/src/tendril_caching.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1035 2023-06-30 18:10:02.000000 tendril-caching-0.2.8/src/tendril_caching.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-06-30 18:10:02.000000 tendril-caching-0.2.8/src/tendril_caching.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      503 2023-06-30 18:10:02.000000 tendril-caching-0.2.8/src/tendril_caching.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-06-30 18:10:02.000000 tendril-caching-0.2.8/src/tendril_caching.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 18:10:02.639705 tendril-caching-0.2.8/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-11-29 08:29:31.000000 tendril-caching-0.2.8/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-11-29 08:29:31.000000 tendril-caching-0.2.8/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-11-29 08:29:31.000000 tendril-caching-0.2.8/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:52:41.440129 tendril-caching-0.2.9/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-11-29 08:29:31.000000 tendril-caching-0.2.9/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-11-29 08:29:31.000000 tendril-caching-0.2.9/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-11-29 08:29:31.000000 tendril-caching-0.2.9/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-11-29 08:29:31.000000 tendril-caching-0.2.9/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-11-29 08:29:31.000000 tendril-caching-0.2.9/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-11-29 08:29:31.000000 tendril-caching-0.2.9/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3481 2023-08-05 20:52:41.440129 tendril-caching-0.2.9/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2192 2022-11-29 08:29:31.000000 tendril-caching-0.2.9/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:52:41.432129 tendril-caching-0.2.9/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-11-29 08:29:31.000000 tendril-caching-0.2.9/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:52:41.436129 tendril-caching-0.2.9/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-11-29 08:29:31.000000 tendril-caching-0.2.9/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-11-29 08:29:31.000000 tendril-caching-0.2.9/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-11-29 08:29:31.000000 tendril-caching-0.2.9/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-11-29 08:29:31.000000 tendril-caching-0.2.9/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:52:41.436129 tendril-caching-0.2.9/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-caching-0.2.9/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:52:41.436129 tendril-caching-0.2.9/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-11-29 08:29:31.000000 tendril-caching-0.2.9/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13460 2022-11-29 08:29:31.000000 tendril-caching-0.2.9/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      903 2022-11-29 08:29:31.000000 tendril-caching-0.2.9/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1536 2022-11-29 08:29:31.000000 tendril-caching-0.2.9/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:52:41.436129 tendril-caching-0.2.9/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-11-29 08:29:31.000000 tendril-caching-0.2.9/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-11-29 08:29:31.000000 tendril-caching-0.2.9/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-08-05 20:52:41.440129 tendril-caching-0.2.9/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3133 2022-11-29 09:11:32.000000 tendril-caching-0.2.9/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:52:41.432129 tendril-caching-0.2.9/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:52:41.436129 tendril-caching-0.2.9/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2022-11-29 08:29:31.000000 tendril-caching-0.2.9/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:52:41.436129 tendril-caching-0.2.9/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 10:22:20.000000 tendril-caching-0.2.9/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:52:41.436129 tendril-caching-0.2.9/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 10:22:45.000000 tendril-caching-0.2.9/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      863 2023-06-26 13:20:44.000000 tendril-caching-0.2.9/src/tendril/apiserver/routers/tokens.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:52:41.440129 tendril-caching-0.2.9/src/tendril/caching/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      449 2022-11-29 14:28:12.000000 tendril-caching-0.2.9/src/tendril/caching/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:52:41.440129 tendril-caching-0.2.9/src/tendril/caching/providers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-11-29 08:53:59.000000 tendril-caching-0.2.9/src/tendril/caching/providers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      272 2022-11-29 13:57:11.000000 tendril-caching-0.2.9/src/tendril/caching/providers/dummy.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1910 2022-11-29 14:11:44.000000 tendril-caching-0.2.9/src/tendril/caching/providers/redis.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4594 2023-06-30 18:07:40.000000 tendril-caching-0.2.9/src/tendril/caching/tokens.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2376 2023-08-05 17:32:30.000000 tendril-caching-0.2.9/src/tendril/caching/transit.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:52:41.440129 tendril-caching-0.2.9/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:07.000000 tendril-caching-0.2.9/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1689 2023-07-29 11:11:08.000000 tendril-caching-0.2.9/src/tendril/config/caching.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:52:41.440129 tendril-caching-0.2.9/src/tendril_caching.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3481 2023-08-05 20:52:41.000000 tendril-caching-0.2.9/src/tendril_caching.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1035 2023-08-05 20:52:41.000000 tendril-caching-0.2.9/src/tendril_caching.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-08-05 20:52:41.000000 tendril-caching-0.2.9/src/tendril_caching.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      503 2023-08-05 20:52:41.000000 tendril-caching-0.2.9/src/tendril_caching.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-08-05 20:52:41.000000 tendril-caching-0.2.9/src/tendril_caching.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:52:41.440129 tendril-caching-0.2.9/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-11-29 08:29:31.000000 tendril-caching-0.2.9/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-11-29 08:29:31.000000 tendril-caching-0.2.9/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-11-29 08:29:31.000000 tendril-caching-0.2.9/tox.ini
```

### Comparing `tendril-caching-0.2.8/.gitignore` & `tendril-caching-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.8/.readthedocs.yml` & `tendril-caching-0.2.9/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.8/.travis.yml` & `tendril-caching-0.2.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.8/LICENSE` & `tendril-caching-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.8/PKG-INFO` & `tendril-caching-0.2.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-caching
-Version: 0.2.8
+Version: 0.2.9
 Summary: Caching Infrastructure for Tendril
 Home-page: https://github.com/tendril-framework/tendril-caching
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-caching.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-caching/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-caching
```

### Comparing `tendril-caching-0.2.8/README.rst` & `tendril-caching-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.8/docs/Makefile` & `tendril-caching-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.8/docs/_static/custom.css` & `tendril-caching-0.2.9/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.8/docs/_static/favicon.ico` & `tendril-caching-0.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.8/docs/_static/logo.png` & `tendril-caching-0.2.9/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.8/docs/_static/logo_packed.png` & `tendril-caching-0.2.9/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.8/docs/_templates/about.html` & `tendril-caching-0.2.9/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.8/docs/conf.py` & `tendril-caching-0.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.8/docs/index.rst` & `tendril-caching-0.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.8/docs/installation.rst` & `tendril-caching-0.2.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.8/setup.py` & `tendril-caching-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.8/src/tendril/apiserver/routers/tokens.py` & `tendril-caching-0.2.9/src/tendril/apiserver/routers/tokens.py`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.8/src/tendril/caching/providers/redis.py` & `tendril-caching-0.2.9/src/tendril/caching/providers/redis.py`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.8/src/tendril/caching/tokens.py` & `tendril-caching-0.2.9/src/tendril/caching/tokens.py`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.8/src/tendril/caching/transit.py` & `tendril-caching-0.2.9/src/tendril/caching/transit.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,18 +52,18 @@
                     f"key {key}. Using 'transit' instead.")
         namespace = 'transit'
 
     cache_key = "{}:{}".format(namespace, key)
     return cache_key
 
 
-def write(value=None, namespace=None, ttl=None, key=None, ser=json.dumps):
+def write(value=None, namespace=None, ttl=None, key=None, ser=json.dumps, get=False):
     cache_key = _common(namespace=namespace, key=key)
     logger.debug(f"Writing {value} to {cache_key}")
-    redis_connection.set(cache_key, ser(value), ex=ttl)
+    return redis_connection.set(cache_key, ser(value), ex=ttl, get=get)
 
 
 def read(namespace=None, key=None, deser=json.loads):
     cache_key = _common(namespace=namespace, key=key)
     cached_value = redis_connection.get(cache_key)
     logger.debug(f"Read {cached_value} from {cache_key}")
     if cached_value:
```

### Comparing `tendril-caching-0.2.8/src/tendril/config/__init__.py` & `tendril-caching-0.2.9/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.8/src/tendril/config/caching.py` & `tendril-caching-0.2.9/src/tendril/config/caching.py`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.8/src/tendril_caching.egg-info/PKG-INFO` & `tendril-caching-0.2.9/src/tendril_caching.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-caching
-Version: 0.2.8
+Version: 0.2.9
 Summary: Caching Infrastructure for Tendril
 Home-page: https://github.com/tendril-framework/tendril-caching
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-caching.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-caching/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-caching
```

### Comparing `tendril-caching-0.2.8/src/tendril_caching.egg-info/SOURCES.txt` & `tendril-caching-0.2.9/src/tendril_caching.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.8/tests/coveralls.py` & `tendril-caching-0.2.9/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.8/tox.ini` & `tendril-caching-0.2.9/tox.ini`

 * *Files identical despite different names*

