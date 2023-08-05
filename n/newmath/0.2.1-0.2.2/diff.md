# Comparing `tmp/newmath-0.2.1.tar.gz` & `tmp/newmath-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newmath-0.2.1.tar", max compression
+gzip compressed data, was "newmath-0.2.2.tar", max compression
```

## Comparing `newmath-0.2.1.tar` & `newmath-0.2.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     7142 2023-01-27 00:43:43.548122 newmath-0.2.1/newmath.py
--rw-r--r--   0        0        0      490 2023-01-27 05:06:34.527889 newmath-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      562 1970-01-01 00:00:00.000000 newmath-0.2.1/setup.py
--rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 newmath-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     7142 2023-01-27 00:43:43.548122 newmath-0.2.2/newmath.py
+-rw-r--r--   0        0        0      490 2023-08-05 04:11:19.036917 newmath-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      562 1970-01-01 00:00:00.000000 newmath-0.2.2/setup.py
+-rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 newmath-0.2.2/PKG-INFO
```

### Comparing `newmath-0.2.1/newmath.py` & `newmath-0.2.2/newmath.py`

 * *Files identical despite different names*

### Comparing `newmath-0.2.1/setup.py` & `newmath-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 modules = \
 ['newmath']
 install_requires = \
 ['pycryptodome>=3.16.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'newmath',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'utilities for using NewBase60',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

