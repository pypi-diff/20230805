# Comparing `tmp/docsig-0.7.0.tar.gz` & `tmp/docsig-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docsig-0.7.0.tar", max compression
+gzip compressed data, was "docsig-0.9.0.tar", max compression
```

## Comparing `docsig-0.7.0.tar` & `docsig-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1073 2022-06-18 03:35:03.133689 docsig-0.7.0/LICENSE
--rw-r--r--   0        0        0     1560 2022-06-24 03:59:20.210809 docsig-0.7.0/README.rst
--rw-r--r--   0        0        0      148 2022-06-18 04:29:27.142681 docsig-0.7.0/docsig/__init__.py
--rw-r--r--   0        0        0      155 2022-06-18 03:35:03.136689 docsig-0.7.0/docsig/__main__.py
--rw-r--r--   0        0        0     1178 2022-06-24 03:57:12.683223 docsig-0.7.0/docsig/_cli.py
--rw-r--r--   0        0        0     4306 2022-06-24 03:52:20.929833 docsig-0.7.0/docsig/_core.py
--rw-r--r--   0        0        0     4381 2022-06-24 03:52:20.930832 docsig-0.7.0/docsig/_function.py
--rw-r--r--   0        0        0     1205 2022-06-24 03:57:12.683223 docsig-0.7.0/docsig/_main.py
--rw-r--r--   0        0        0     1881 2022-06-22 09:17:04.551849 docsig-0.7.0/docsig/_module.py
--rw-r--r--   0        0        0      609 2022-06-24 03:52:20.930832 docsig-0.7.0/docsig/_objects.py
--rw-r--r--   0        0        0     2753 2022-06-24 03:52:20.931832 docsig-0.7.0/docsig/_report.py
--rw-r--r--   0        0        0     2739 2022-06-24 03:52:20.931832 docsig-0.7.0/docsig/_repr.py
--rw-r--r--   0        0        0      515 2022-06-24 03:52:20.931832 docsig-0.7.0/docsig/_utils.py
--rw-r--r--   0        0        0      210 2022-06-24 03:57:12.684223 docsig-0.7.0/docsig/_version.py
--rw-r--r--   0        0        0      445 2022-06-23 07:03:33.054047 docsig-0.7.0/docsig/messages.py
--rw-r--r--   0        0        0     2391 2022-06-24 03:57:12.685223 docsig-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2411 2022-06-24 04:01:50.193193 docsig-0.7.0/setup.py
--rw-r--r--   0        0        0     2392 2022-06-24 04:01:50.194352 docsig-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-06-18 03:35:03.133689 docsig-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1576 2022-06-26 08:16:25.640358 docsig-0.9.0/README.rst
+-rw-r--r--   0        0        0      148 2022-06-18 04:29:27.142681 docsig-0.9.0/docsig/__init__.py
+-rw-r--r--   0        0        0      155 2022-06-18 03:35:03.136689 docsig-0.9.0/docsig/__main__.py
+-rw-r--r--   0        0        0     1146 2022-06-25 09:34:40.978657 docsig-0.9.0/docsig/_cli.py
+-rw-r--r--   0        0        0     4324 2022-06-26 01:33:35.655441 docsig-0.9.0/docsig/_core.py
+-rw-r--r--   0        0        0     5208 2022-06-26 08:16:49.123329 docsig-0.9.0/docsig/_function.py
+-rw-r--r--   0        0        0     1205 2022-06-24 07:11:47.172948 docsig-0.9.0/docsig/_main.py
+-rw-r--r--   0        0        0     1881 2022-06-22 09:17:04.551849 docsig-0.9.0/docsig/_module.py
+-rw-r--r--   0        0        0      602 2022-06-25 09:34:40.979657 docsig-0.9.0/docsig/_objects.py
+-rw-r--r--   0        0        0     3181 2022-06-26 08:16:49.123329 docsig-0.9.0/docsig/_report.py
+-rw-r--r--   0        0        0     2762 2022-06-25 11:05:38.872628 docsig-0.9.0/docsig/_repr.py
+-rw-r--r--   0        0        0      553 2022-06-25 09:40:23.800011 docsig-0.9.0/docsig/_utils.py
+-rw-r--r--   0        0        0      210 2022-06-26 08:18:35.381197 docsig-0.9.0/docsig/_version.py
+-rw-r--r--   0        0        0      633 2022-06-26 08:16:49.123329 docsig-0.9.0/docsig/messages.py
+-rw-r--r--   0        0        0     2391 2022-06-26 08:18:35.383197 docsig-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2427 2022-06-26 08:21:21.029754 docsig-0.9.0/setup.py
+-rw-r--r--   0        0        0     2408 2022-06-26 08:21:21.030710 docsig-0.9.0/PKG-INFO
```

### Comparing `docsig-0.7.0/LICENSE` & `docsig-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `docsig-0.7.0/README.rst` & `docsig-0.9.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -38,17 +38,17 @@
 -----
 
 Commandline
 ***********
 
 .. code-block:: console
 
-    usage: docsig [-h] [-v] path
+    usage: docsig [-h] [-v] [path [path ...]]
 
     Check docstring matches signature
 
     positional arguments:
-      path           directory or file to check
+      path           directories or files to check
 
     optional arguments:
       -h, --help     show this help message and exit
       -v, --version  show version and exit
```

### Comparing `docsig-0.7.0/docsig/_cli.py` & `docsig-0.9.0/docsig/_cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,14 @@
         super().__init__(
             prog=_color.cyan.get(NAME),
             description="Check docstring matches signature",
         )
         self._add_arguments()
         self._version_request()
         self.args = self.parse_args()
-        self._version_request()
 
     def _add_arguments(self) -> None:
         self.add_argument(
             "path",
             nargs="*",
             action="store",
             type=_Path,
```

### Comparing `docsig-0.7.0/docsig/_core.py` & `docsig-0.9.0/docsig/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 docsig._core
 ============
 """
+from __future__ import annotations
+
 import typing as _t
 from itertools import zip_longest as _zip_longest
 from pathlib import Path as _Path
 
 from ._function import Function as _Function
 from ._module import Module as _Module
 from ._module import Parent as _Parent
@@ -36,17 +38,15 @@
         paths.append(root)
 
     if root.is_dir():
         for path in root.iterdir():
             get_files(path, paths)
 
 
-def _compare_args(
-    arg: _t.Optional[str], doc: _t.Optional[str], kind: str
-) -> bool:
+def _compare_args(arg: str | None, doc: str | None, kind: str) -> bool:
     if kind in ("key", "keyword") and arg is not None:
         return arg[:2] == "**"
 
     if isinstance(arg, str):
         arg = arg.replace("*", "")
 
     return arg == doc and arg is not None and doc is not None
```

### Comparing `docsig-0.7.0/docsig/_main.py` & `docsig-0.9.0/docsig/_main.py`

 * *Files identical despite different names*

### Comparing `docsig-0.7.0/docsig/_module.py` & `docsig-0.9.0/docsig/_module.py`

 * *Files identical despite different names*

### Comparing `docsig-0.7.0/docsig/_objects.py` & `docsig-0.9.0/docsig/_objects.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """
 docsig._objects
 ===============
 """
 import typing as _t
 
-_T = _t.TypeVar("_T")
+T = _t.TypeVar("T")
 
 
-class MutableSet(_t.MutableSet[_T]):
+class MutableSet(_t.MutableSet[T]):
     """Set objet to inherit from."""
 
     def __init__(self) -> None:
-        self._set: _t.Set[_T] = set()
+        self._set: _t.Set[T] = set()
 
-    def add(self, value: _T) -> None:
+    def add(self, value: T) -> None:
         self._set.add(value)
 
-    def discard(self, value: _T) -> None:
+    def discard(self, value: T) -> None:
         self._set.discard(value)
 
     def __contains__(self, x: object) -> bool:
         return self._set.__contains__(x)
 
     def __len__(self) -> int:
         return self._set.__len__()
 
-    def __iter__(self) -> _t.Iterator[_T]:
+    def __iter__(self) -> _t.Iterator[T]:
         return self._set.__iter__()
```

### Comparing `docsig-0.7.0/docsig/_report.py` & `docsig-0.9.0/docsig/_report.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,44 @@
 """
 docsig._report
 ==============
 """
+from __future__ import annotations
+
 import typing as _t
 import warnings as _warnings
 from collections import Counter as _Counter
 
 from ._function import Function as _Function
 from ._objects import MutableSet as _MutableSet
-from .messages import E101, E102, E103, E104, E105, E106, E107, W101
+from .messages import (
+    E101,
+    E102,
+    E103,
+    E104,
+    E105,
+    E106,
+    E107,
+    H101,
+    H102,
+    W101,
+)
 
 
 class Report(_MutableSet):
     """Compile and produce report.
 
     :param func: Function object.
     """
 
     def __init__(self, func: _Function) -> None:
         super().__init__()
         self._func = func
 
-    def order(self, arg: _t.Optional[str], doc: _t.Optional[str]) -> None:
+    def order(self, arg: str | None, doc: str | None) -> None:
         """Test for documented parameters and their order.
 
         :param arg: Signature argument.
         :param doc: Docstring argument.
         """
         if (
             arg in self._func.docstring.args
@@ -37,35 +50,45 @@
         """Test that non-existing parameter is not documented."""
         if len(self._func.docstring.args) > len(self._func.signature.args):
             self.add(E102)
 
     def missing(self) -> None:
         """Test that parameter is not missing from documentation."""
         if len(self._func.signature.args) > len(self._func.docstring.args):
-            self.add(E103)
+            message = E103
+            docstring = self._func.docstring.docstring
+            if docstring is not None and all(
+                f"param {i}" in docstring for i in self._func.signature.args
+            ):
+                message += f"\n{H101}"
+
+            self.add(message)
 
     def duplicates(self) -> None:
         """Test that there are no duplicate parameters in docstring."""
         if any(
             k for k, v in _Counter(self._func.docstring.args).items() if v > 1
         ):
             self.add(E106)
 
     def extra_return(self) -> None:
         """Check that return is not documented when there is none."""
         if self._func.docstring.returns and not self._func.signature.returns:
-            self.add(E104)
+            message = E104
+            if self._func.isproperty:
+                message += f"\n{H102}"
+
+            self.add(message)
 
     def missing_return(self) -> None:
-        """Check that return is documented when function returns
-        value."""
+        """Check that return is documented when func returns value."""
         if self._func.signature.returns and not self._func.docstring.returns:
             self.add(E105)
 
-    def incorrect(self, arg: _t.Optional[str], doc: _t.Optional[str]) -> None:
+    def incorrect(self, arg: str | None, doc: str | None) -> None:
         """Test that proper syntax is used when documenting parameters.
 
         :param arg: Signature argument.
         :param doc: Docstring argument.
         """
         if arg is None and doc is None:
             self.add(E107)
```

### Comparing `docsig-0.7.0/docsig/_repr.py` & `docsig-0.9.0/docsig/_repr.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 docsig._repr
 ============
 """
-import typing as _t
+from __future__ import annotations
+
 from collections import UserString as _UserString
 
 from pygments import highlight as _highlight
 from pygments.formatters.terminal256 import (
     Terminal256Formatter as _Terminal256Formatter,
 )
 
@@ -44,39 +45,36 @@
         """Set mark to a cross or a check.
 
         :param failed: Boolean to test that check failed.
         """
         self._mark = self.CROSS if failed else self.CHECK
 
     def add_param(
-        self,
-        arg: _t.Optional[str],
-        doc: _t.Optional[str],
-        kind: str,
-        failed: bool = False,
+        self, arg: str | None, doc: str | None, kind: str, failed: bool = False
     ) -> None:
         """Add parameters to docstring.
 
         :param arg: Signature argument.
         :param doc: Docstring argument.
+        :param kind: Type of docstring parameter.
         :param failed: Boolean to test that check failed.
         """
         self.set_mark(failed)
         self.data += f"{self._mark}{arg}"
         self._docstring += f"\n{self.TAB}:{kind} {doc}: {self._mark}"
 
     def add_return(self, failed: bool = False) -> None:
         """Add return statement to docstring.
 
         :param failed: Boolean to test that check failed.
         """
         self.set_mark(failed)
         self._docstring += f"\n{self.TAB}:return: {self._mark}"
 
-    def close_sig(self, arg: _t.Optional[str]):
+    def close_sig(self, arg: str | None) -> None:
         """Close function signature.
 
         :param arg: Signature argument.
         """
         self.data += "{}{}{}{}".format(
             self._lexer(") -> "), self._mark, arg, self._lexer(":")
         )
```

### Comparing `docsig-0.7.0/pyproject.toml` & `docsig-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 license = "MIT"
 maintainers = [
     "jshwi <stephen@jshwisolutions.com>",
 ]
 name = "docsig"
 readme = "README.rst"
 repository = "https://github.com/jshwi/docsig"
-version = "0.7.0"
+version = "0.9.0"
 
 [tool.poetry.dependencies]
 object-colors = "^2.1.0"
 python = "^3.8"
 
 [tool.poetry.dev-dependencies]
 bump2version = "^1.0.1"
```

### Comparing `docsig-0.7.0/setup.py` & `docsig-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['object-colors>=2.1.0,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['docsig = docsig.__main__:main']}
 
 setup_kwargs = {
     'name': 'docsig',
-    'version': '0.7.0',
+    'version': '0.9.0',
     'description': 'Check signature params for proper documentation',
-    'long_description': 'docsig\n======\n.. image:: https://img.shields.io/badge/License-MIT-yellow.svg\n    :target: https://opensource.org/licenses/MIT\n    :alt: License\n.. image:: https://img.shields.io/pypi/v/docsig\n    :target: https://img.shields.io/pypi/v/docsig\n    :alt: pypi\n.. image:: https://github.com/jshwi/docsig/actions/workflows/ci.yml/badge.svg\n    :target: https://github.com/jshwi/docsig/actions/workflows/ci.yml\n    :alt: CI\n.. image:: https://codecov.io/gh/jshwi/docsig/branch/master/graph/badge.svg\n    :target: https://codecov.io/gh/jshwi/docsig\n    :alt: codecov.io\n.. image:: https://readthedocs.org/projects/docsig/badge/?version=latest\n    :target: https://docsig.readthedocs.io/en/latest/?badge=latest\n    :alt: readthedocs.org\n.. image:: https://img.shields.io/badge/python-3.8-blue.svg\n    :target: https://www.python.org/downloads/release/python-380\n    :alt: python3.8\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n    :target: https://github.com/psf/black\n    :alt: black\n\nCheck signature params for proper documentation\n-----------------------------------------------\n\nCurrently only supports reStructuredText (Sphinx)\n\nInstallation\n------------\n\n.. code-block:: console\n\n    $ pip install docsig\n\nUsage\n-----\n\nCommandline\n***********\n\n.. code-block:: console\n\n    usage: docsig [-h] [-v] path\n\n    Check docstring matches signature\n\n    positional arguments:\n      path           directory or file to check\n\n    optional arguments:\n      -h, --help     show this help message and exit\n      -v, --version  show version and exit\n',
+    'long_description': 'docsig\n======\n.. image:: https://img.shields.io/badge/License-MIT-yellow.svg\n    :target: https://opensource.org/licenses/MIT\n    :alt: License\n.. image:: https://img.shields.io/pypi/v/docsig\n    :target: https://img.shields.io/pypi/v/docsig\n    :alt: pypi\n.. image:: https://github.com/jshwi/docsig/actions/workflows/ci.yml/badge.svg\n    :target: https://github.com/jshwi/docsig/actions/workflows/ci.yml\n    :alt: CI\n.. image:: https://codecov.io/gh/jshwi/docsig/branch/master/graph/badge.svg\n    :target: https://codecov.io/gh/jshwi/docsig\n    :alt: codecov.io\n.. image:: https://readthedocs.org/projects/docsig/badge/?version=latest\n    :target: https://docsig.readthedocs.io/en/latest/?badge=latest\n    :alt: readthedocs.org\n.. image:: https://img.shields.io/badge/python-3.8-blue.svg\n    :target: https://www.python.org/downloads/release/python-380\n    :alt: python3.8\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n    :target: https://github.com/psf/black\n    :alt: black\n\nCheck signature params for proper documentation\n-----------------------------------------------\n\nCurrently only supports reStructuredText (Sphinx)\n\nInstallation\n------------\n\n.. code-block:: console\n\n    $ pip install docsig\n\nUsage\n-----\n\nCommandline\n***********\n\n.. code-block:: console\n\n    usage: docsig [-h] [-v] [path [path ...]]\n\n    Check docstring matches signature\n\n    positional arguments:\n      path           directories or files to check\n\n    optional arguments:\n      -h, --help     show this help message and exit\n      -v, --version  show version and exit\n',
     'author': 'jshwi',
     'author_email': 'stephen@jshwisolutions.com',
     'maintainer': 'jshwi',
     'maintainer_email': 'stephen@jshwisolutions.com',
     'url': 'https://pypi.org/project/docsig/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `docsig-0.7.0/PKG-INFO` & `docsig-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docsig
-Version: 0.7.0
+Version: 0.9.0
 Summary: Check signature params for proper documentation
 Home-page: https://pypi.org/project/docsig/
 License: MIT
 Keywords: docstring,signature,params,check,docs
 Author: jshwi
 Author-email: stephen@jshwisolutions.com
 Maintainer: jshwi
@@ -60,18 +60,18 @@
 -----
 
 Commandline
 ***********
 
 .. code-block:: console
 
-    usage: docsig [-h] [-v] path
+    usage: docsig [-h] [-v] [path [path ...]]
 
     Check docstring matches signature
 
     positional arguments:
-      path           directory or file to check
+      path           directories or files to check
 
     optional arguments:
       -h, --help     show this help message and exit
       -v, --version  show version and exit
```

