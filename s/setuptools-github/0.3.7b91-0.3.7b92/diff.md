# Comparing `tmp/setuptools-github-0.3.7b91.tar.gz` & `tmp/setuptools-github-0.3.7b92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-github-0.3.7b91.tar", last modified: Fri Aug  4 19:54:42 2023, max compression
+gzip compressed data, was "setuptools-github-0.3.7b92.tar", last modified: Fri Aug  4 22:21:41 2023, max compression
```

## Comparing `setuptools-github-0.3.7b91.tar` & `setuptools-github-0.3.7b92.tar`

### file list

```diff
@@ -1,32 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:54:42.211853 setuptools-github-0.3.7b91/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-08-04 19:54:42.211853 setuptools-github-0.3.7b91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-08-04 19:54:42.000000 setuptools-github-0.3.7b91/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 19:54:42.211853 setuptools-github-0.3.7b91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:54:42.207853 setuptools-github-0.3.7b91/setuptools_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-08-04 19:54:42.000000 setuptools-github-0.3.7b91/setuptools_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-04 19:54:42.000000 setuptools-github-0.3.7b91/setuptools_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 19:54:42.000000 setuptools-github-0.3.7b91/setuptools_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-04 19:54:42.000000 setuptools-github-0.3.7b91/setuptools_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 19:54:42.000000 setuptools-github-0.3.7b91/setuptools_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-04 19:54:42.000000 setuptools-github-0.3.7b91/setuptools_github.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:54:42.207853 setuptools-github-0.3.7b91/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:54:42.211853 setuptools-github-0.3.7b91/src/setuptools_github/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-04 19:54:42.000000 setuptools-github-0.3.7b91/src/setuptools_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/src/setuptools_github/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/src/setuptools_github/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/src/setuptools_github/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/src/setuptools_github/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/src/setuptools_github/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:54:42.211853 setuptools-github-0.3.7b91/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/tests/test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    11085 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:21:41.628932 setuptools-github-0.3.7b92/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-08-04 22:21:41.628932 setuptools-github-0.3.7b92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-08-04 22:21:41.000000 setuptools-github-0.3.7b92/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 22:21:41.628932 setuptools-github-0.3.7b92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:21:41.628932 setuptools-github-0.3.7b92/setuptools_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-08-04 22:21:41.000000 setuptools-github-0.3.7b92/setuptools_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-04 22:21:41.000000 setuptools-github-0.3.7b92/setuptools_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 22:21:41.000000 setuptools-github-0.3.7b92/setuptools_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-04 22:21:41.000000 setuptools-github-0.3.7b92/setuptools_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 22:21:41.000000 setuptools-github-0.3.7b92/setuptools_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-04 22:21:41.000000 setuptools-github-0.3.7b92/setuptools_github.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:21:41.624932 setuptools-github-0.3.7b92/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:21:41.628932 setuptools-github-0.3.7b92/src/setuptools_github/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-04 22:21:41.000000 setuptools-github-0.3.7b92/src/setuptools_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/src/setuptools_github/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/src/setuptools_github/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/src/setuptools_github/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/src/setuptools_github/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:21:41.628932 setuptools-github-0.3.7b92/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11085 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/tests/test_tools.py
```

### Comparing `setuptools-github-0.3.7b91/LICENSE` & `setuptools-github-0.3.7b92/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.7b91/PKG-INFO` & `setuptools-github-0.3.7b92/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.7b91
+Version: 0.3.7b92
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `setuptools-github-0.3.7b91/README.md` & `setuptools-github-0.3.7b92/README.md`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.7b91/pyproject.toml` & `setuptools-github-0.3.7b92/pyproject.toml`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.7b91/setup.py` & `setuptools-github-0.3.7b92/setup.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.7b91/setuptools_github.egg-info/PKG-INFO` & `setuptools-github-0.3.7b92/setuptools_github.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.7b91
+Version: 0.3.7b92
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `setuptools-github-0.3.7b91/setuptools_github.egg-info/SOURCES.txt` & `setuptools-github-0.3.7b92/setuptools_github.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,20 +6,18 @@
 setuptools_github.egg-info/PKG-INFO
 setuptools_github.egg-info/SOURCES.txt
 setuptools_github.egg-info/dependency_links.txt
 setuptools_github.egg-info/entry_points.txt
 setuptools_github.egg-info/requires.txt
 setuptools_github.egg-info/top_level.txt
 src/setuptools_github/__init__.py
-src/setuptools_github/checks.py
 src/setuptools_github/cli.py
 src/setuptools_github/scm.py
 src/setuptools_github/script.py
 src/setuptools_github/tools.py
 tests/conftest.py
 tests/requirements.txt
-tests/test_checks.py
 tests/test_cli.py
 tests/test_conftest.py
 tests/test_scm.py
 tests/test_script.py
 tests/test_tools.py
```

### Comparing `setuptools-github-0.3.7b91/src/setuptools_github/cli.py` & `setuptools-github-0.3.7b92/src/setuptools_github/cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.7b91/src/setuptools_github/scm.py` & `setuptools-github-0.3.7b92/src/setuptools_github/scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.7b91/src/setuptools_github/script.py` & `setuptools-github-0.3.7b92/src/setuptools_github/script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.7b91/src/setuptools_github/tools.py` & `setuptools-github-0.3.7b92/src/setuptools_github/tools.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.7b91/tests/conftest.py` & `setuptools-github-0.3.7b92/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.7b91/tests/test_conftest.py` & `setuptools-github-0.3.7b92/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.7b91/tests/test_scm.py` & `setuptools-github-0.3.7b92/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.7b91/tests/test_script.py` & `setuptools-github-0.3.7b92/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.7b91/tests/test_tools.py` & `setuptools-github-0.3.7b92/tests/test_tools.py`

 * *Files identical despite different names*

