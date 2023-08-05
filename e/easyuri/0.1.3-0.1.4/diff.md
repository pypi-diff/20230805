# Comparing `tmp/easyuri-0.1.3.tar.gz` & `tmp/easyuri-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyuri-0.1.3.tar", max compression
+gzip compressed data, was "easyuri-0.1.4.tar", max compression
```

## Comparing `easyuri-0.1.3.tar` & `easyuri-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      612 2023-02-13 03:51:06.361115 easyuri-0.1.3/README.md
--rw-r--r--   0        0        0    21030 2023-02-13 23:42:00.841468 easyuri-0.1.3/easyuri/__init__.py
--rw-r--r--   0        0        0      779 2023-08-05 03:12:04.530474 easyuri-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1342 1970-01-01 00:00:00.000000 easyuri-0.1.3/setup.py
--rw-r--r--   0        0        0     1405 1970-01-01 00:00:00.000000 easyuri-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      612 2023-02-13 03:51:06.361115 easyuri-0.1.4/README.md
+-rw-r--r--   0        0        0    21040 2023-08-05 03:14:19.308572 easyuri-0.1.4/easyuri/__init__.py
+-rw-r--r--   0        0        0      779 2023-08-05 03:14:21.940613 easyuri-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1342 1970-01-01 00:00:00.000000 easyuri-0.1.4/setup.py
+-rw-r--r--   0        0        0     1405 1970-01-01 00:00:00.000000 easyuri-0.1.4/PKG-INFO
```

### Comparing `easyuri-0.1.3/README.md` & `easyuri-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `easyuri-0.1.3/easyuri/__init__.py` & `easyuri-0.1.4/easyuri/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import mimetypes
 import unicodedata
 import urllib.parse
 from dataclasses import dataclass
 
 import hstspreload
 import pkg_resources
+import requests
 
 __all__ = ["parse", "supported_schemes"]
 
 
 class DifficultURLError(Exception):
     """"""
 
@@ -708,23 +709,23 @@
 class PublicSuffixList:
     """Reads and parses the public suffix list."""
 
     def __init__(self):
         input_path = pkg_resources.resource_filename(
             "easyuri", "public_suffix_list.dat"
         )
-        # try:
-        with codecs.open(input_path, "r", "utf8") as fp:
-            self._build_structure(fp)
-        # except FileNotFoundError:
-        #     res = requests.get("https://publicsuffix.org/list/public_suffix_list.dat")
-        #     with codecs.open(input_path, "w", "utf8") as fp:
-        #         fp.write(res.text)
-        #     with codecs.open(input_path, "r", "utf8") as fp:
-        #         self._build_structure(fp)
+        try:
+            with codecs.open(input_path, "r", "utf8") as fp:
+                self._build_structure(fp)
+        except FileNotFoundError:
+            res = requests.get("https://publicsuffix.org/list/public_suffix_list.dat")
+            with codecs.open(input_path, "w", "utf8") as fp:
+                fp.write(res.text)
+            with codecs.open(input_path, "r", "utf8") as fp:
+                self._build_structure(fp)
 
     def lookup(self, matches, depth, parts, parent=None):
         if parent is None:
             parent = self.root
         if parent in (0, 1):
             negate = parent
             children = None
```

### Comparing `easyuri-0.1.3/pyproject.toml` & `easyuri-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easyuri"
-version = "0.1.3"
+version = "0.1.4"
 description = "a dumb URL parser with a smart interface"
 keywords = ["web", "www"]
 readme = "README.md"
 homepage = "https://ragt.ag/code/projects/easyuri"
 repository = "https://ragt.ag/code/projects/easyuri.git"
 documentation = "https://ragt.ag/code/projects/easyuri/api"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
```

### Comparing `easyuri-0.1.3/setup.py` & `easyuri-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['hstspreload>=2023.1.1,<2024.0.0', 'requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'easyuri',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'a dumb URL parser with a smart interface',
     'long_description': '`easyuri` is a dumb URL parser with a smart interface.\n\n    >>> import easyuri\n    >>> uri = easyuri.parse("en.wikipedia.org/wiki/Jabberwocky")\n    >>> uri.is_secure, uri.in_hsts\n    (True, True)\n    >>> uri.scheme, uri.host, uri.port\n    (\'https\', \'en.wikipedia.org\', 443)\n    >>> uri.subdomain, uri.domain, uri.suffix, uri.path\n    (\'en\', \'wikipedia\', \'org\', \'wiki/Jabberwocky\')\n    >>> str(uri)\n    \'https://en.wikipedia.org/wiki/Jabberwocky\'\n\n    >>> uri = easyuri.parse("http://evil.com\\\\@good.com/")  # doctest: +IGNORE_EXCEPTION_DETAIL\n    Traceback (most recent call last):\n    ...\n    DifficultURLError\n',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://ragt.ag/code/projects/easyuri',
```

### Comparing `easyuri-0.1.3/PKG-INFO` & `easyuri-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyuri
-Version: 0.1.3
+Version: 0.1.4
 Summary: a dumb URL parser with a smart interface
 Home-page: https://ragt.ag/code/projects/easyuri
 License: BSD-2-Clause
 Keywords: web,www
 Author: Angelo Gladding
 Author-email: angelo@ragt.ag
 Requires-Python: >=3.8,<3.11
```

