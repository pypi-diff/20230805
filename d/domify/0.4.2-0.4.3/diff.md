# Comparing `tmp/domify-0.4.2.tar.gz` & `tmp/domify-0.4.3.tar.gz`

## Comparing `domify-0.4.2.tar` & `domify-0.4.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 domify-0.4.2/domify/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domify-0.4.2/domify/__init__.py
--rw-r--r--   0        0        0    11908 2020-02-02 00:00:00.000000 domify-0.4.2/domify/base_element.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 domify-0.4.2/domify/exc.py
--rw-r--r--   0        0        0    25411 2020-02-02 00:00:00.000000 domify-0.4.2/domify/html_elements.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domify-0.4.2/domify/py.typed
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 domify-0.4.2/domify/validators.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 domify-0.4.2/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 domify-0.4.2/LICENSE
--rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 domify-0.4.2/README.md
--rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 domify-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 domify-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 domify-0.4.3/domify/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domify-0.4.3/domify/__init__.py
+-rw-r--r--   0        0        0    11942 2020-02-02 00:00:00.000000 domify-0.4.3/domify/base_element.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 domify-0.4.3/domify/exc.py
+-rw-r--r--   0        0        0    25266 2020-02-02 00:00:00.000000 domify-0.4.3/domify/html_elements.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domify-0.4.3/domify/py.typed
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 domify-0.4.3/domify/validators.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 domify-0.4.3/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 domify-0.4.3/LICENSE
+-rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 domify-0.4.3/README.md
+-rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 domify-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 domify-0.4.3/PKG-INFO
```

### Comparing `domify-0.4.2/domify/base_element.py` & `domify-0.4.3/domify/base_element.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import sys
 import warnings
 from contextvars import ContextVar
 from html import escape
 from types import TracebackType
 from typing import (
     Callable,
+    ClassVar,
     Dict,
     Iterable,
     Iterator,
     Set,
     TypeVar,
     Union,
     cast,
@@ -32,16 +33,16 @@
 _T_attributes_dict = Dict[str, Union[Set[str], Callable[[_T_attribute], bool]]]
 
 
 class BaseElement:
     """Base class representing an element"""
 
     is_empty = False
-    global_attributes: _T_attributes_dict = {}
-    element_attributes: _T_attributes_dict = {}
+    global_attributes: ClassVar[_T_attributes_dict] = {}
+    element_attributes: ClassVar[_T_attributes_dict] = {}
     any_attribute = False
 
     _default_prepend_doctype = False
 
     _stack_var: ContextVar[list[list[BaseElement]] | None] = ContextVar(
         "stack", default=None
     )
```

### Comparing `domify-0.4.2/domify/exc.py` & `domify-0.4.3/domify/exc.py`

 * *Files identical despite different names*

### Comparing `domify-0.4.2/domify/html_elements.py` & `domify-0.4.3/domify/html_elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ruff: noqa: E742
+# ruff: noqa: E742, RUF012
 
 from __future__ import annotations
 
 from domify import validators as v
 from domify.base_element import BaseElement
 from domify.base_element import RawTextNode as RawTextNode
 from domify.base_element import TextNode as TextNode
@@ -890,20 +890,14 @@
 
 
 class Picture(HtmlElement):
     """
     Image
     """
 
-    element_attributes = {
-        "height": v.attribute_int_ge_zero,
-        "media": v.attribute_str,
-        "width": v.attribute_int_ge_zero,
-    }
-
 
 class Pre(HtmlElement):
     """
     Block of preformatted text
     """
```

### Comparing `domify-0.4.2/domify/validators.py` & `domify-0.4.3/domify/validators.py`

 * *Files identical despite different names*

### Comparing `domify-0.4.2/LICENSE` & `domify-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `domify-0.4.2/README.md` & `domify-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `domify-0.4.2/pyproject.toml` & `domify-0.4.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -11,26 +11,36 @@
 license = "MIT"
 authors = [
     {name="Parnassius", email="Parnassius@users.noreply.github.com"},
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Code Generators",
     "Topic :: Text Processing :: Markup :: HTML",
     "Typing :: Typed",
 ]
 dependencies = [
     "typing-extensions>=3.7; python_version<'3.8'",
 ]
 dynamic = ["version"]
 
 [project.urls]
-homepage = "https://github.com/Parnassius/domify"
+Homepage = "https://github.com/Parnassius/domify"
 
 
 [tool.hatch.build]
 packages = ["domify"]
 
 [tool.hatch.envs.default]
 skip-install = true
@@ -65,31 +75,42 @@
     "_create_tag",
     "_create_dev_commit",
 ]
 
 [tool.hatch.envs.lint]
 template = "lint"
 dependencies = [
-    "black==23.3.0",
+    "black==23.7.0",
     "darglint==1.8.1",
-    "mypy==1.3.0",
-    "pytest==7.3.1",
-    "ruff==0.0.270",
+    "mypy==1.4.1",
+    "pytest==7.4.0",
+    "ruff==0.0.282",
 ]
 
 [tool.hatch.envs.test]
 template = "test"
 dependencies = [
-    "pytest==7.3.1",
+    "pytest==7.4.0",
     "pytest-cov==4.1.0",
     "typing-extensions==3.7.2; python_version<'3.8'",
 ]
 
 [[tool.hatch.envs.test.matrix]]
-python = ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12", "pypy3.7", "pypy3.8", "pypy3.9"]
+python = [
+    "3.7",
+    "3.8",
+    "3.9",
+    "3.10",
+    "3.11",
+    "3.12",
+    "pypy3.7",
+    "pypy3.8",
+    "pypy3.9",
+    "pypy3.10",
+]
 
 [tool.hatch.version]
 path = "domify/__about__.py"
 
 
 [tool.coverage.report]
 exclude_lines = [
```

### Comparing `domify-0.4.2/PKG-INFO` & `domify-0.4.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 Metadata-Version: 2.1
 Name: domify
-Version: 0.4.2
+Version: 0.4.3
 Summary: HTML generator using pure Python
-Project-URL: homepage, https://github.com/Parnassius/domify
+Project-URL: Homepage, https://github.com/Parnassius/domify
 Author-email: Parnassius <Parnassius@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: typing-extensions>=3.7; python_version < '3.8'
 Description-Content-Type: text/markdown
```

