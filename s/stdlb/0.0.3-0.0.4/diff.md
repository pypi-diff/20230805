# Comparing `tmp/stdlb-0.0.3.tar.gz` & `tmp/stdlb-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdlb-0.0.3.tar", last modified: Fri Aug  4 14:58:34 2023, max compression
+gzip compressed data, was "stdlb-0.0.4.tar", last modified: Sat Aug  5 15:35:39 2023, max compression
```

## Comparing `stdlb-0.0.3.tar` & `stdlb-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:58:34.391280 stdlb-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-08-04 14:58:34.391280 stdlb-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-08-04 14:58:06.000000 stdlb-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 14:58:34.391280 stdlb-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-04 14:58:06.000000 stdlb-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:58:34.391280 stdlb-0.0.3/stdlb/
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-04 14:58:06.000000 stdlb-0.0.3/stdlb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-08-04 14:58:06.000000 stdlb-0.0.3/stdlb/cached_property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:58:34.391280 stdlb-0.0.3/stdlb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-08-04 14:58:34.000000 stdlb-0.0.3/stdlb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-04 14:58:34.000000 stdlb-0.0.3/stdlb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 14:58:34.000000 stdlb-0.0.3/stdlb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-04 14:58:34.000000 stdlb-0.0.3/stdlb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:35:39.577962 stdlb-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-08-05 15:35:39.577962 stdlb-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-08-05 15:35:27.000000 stdlb-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 15:35:39.577962 stdlb-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-05 15:35:27.000000 stdlb-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:35:39.577962 stdlb-0.0.4/stdlb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-08-05 15:35:27.000000 stdlb-0.0.4/stdlb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-08-05 15:35:27.000000 stdlb-0.0.4/stdlb/cached_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:35:39.577962 stdlb-0.0.4/stdlb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-08-05 15:35:39.000000 stdlb-0.0.4/stdlb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-05 15:35:39.000000 stdlb-0.0.4/stdlb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 15:35:39.000000 stdlb-0.0.4/stdlb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-05 15:35:39.000000 stdlb-0.0.4/stdlb.egg-info/top_level.txt
```

### Comparing `stdlb-0.0.3/PKG-INFO` & `stdlb-0.0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,58 @@
-Metadata-Version: 2.1
-Name: stdlb
-Version: 0.0.3
-Summary: Wildcard-import the Python standard library
-Home-page: UNKNOWN
-Author: Ryan Williams
-Author-email: ryan@runsascoded.com
-License: MIT
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 # `stdlb`
 
 Wildcard-import the Python standard library
 
+[![PyPI badge: "stdlb" library](https://img.shields.io/pypi/v/stdlb.svg)](https://pypi.python.org/pypi/stdlb)
+
 ```python
 from stdlb import *
 
 # Most of the standard library is now available:
 print(f"Current directory: {getcwd()}")
 stderr.write("Python version: {version}\n")
 ```
 
-## Install
+- [Install](#install)
+- [Notes](#notes)
+    - [Collision Resolution](#collisions)
+        - [`__builtins` vs. module members](#builtins)
+        - [Module/Members](#module-members)
+    - [Aliases](#aliases)
+    - [Custom `cached_property`](#cached-property)
+
+## Install <a id="install"></a>
 ```bash
 pip install stdlb
 ```
 
-## Notes
+## Notes <a id="notes"></a>
 I've found this especially useful in Jupyter notebooks, where I don't have an easy "add `import` statements as I add code" setup.
 
 Importing seems to take a few milliseconds (on my Macbook Air):
 ```ipython
 %%time
 from stdlb import *
 # CPU times: user 914 µs, sys: 397 µs, total: 1.31 ms
 # Wall time: 1.6 ms
 ```
 
-### Collisions / Aliases
+### Collision Resolution <a id="collisions"></a>
+
+#### `__builtins` vs. module members <a id="builtins"></a>
+`stdlb` avoids overwriting `__builtins__` with conflicting module members, e.g.:
+- `open` vs. `os.open`
+- `compile` vs. `re.compile`
+- `pow` vs. `math.pow`
+- `copyright` vs. `sys.copyright`
+- `BlockingIOError` vs. `io.BlockingIOError`
+
+[`test.ipynb`](test.ipynb) is executed as part of [`ci.yml`](.github/workflows/ci.yml) to verify there are no `__builtins__` are unexpectedly shadowed.
+
+#### Module/Members <a id="module-members"></a>
 In a few cases, a top-level standard library module also contains a member with the same name (e.g. `datetime`, `shlex`, `time`). `stdlb` makes an effort to ensure the module "wins" in this case:
 
 ```python
 from stdlb import *
 
 datetime  # <module 'datetime' from '$PYTHON_HOME/lib/python3.9/datetime.py'>
 shlex     # <module 'shlex' from '$PYTHON_HOME/lib/python3.9/shlex.py'>
@@ -50,18 +61,18 @@
 
 A few names are disambiguated with the most sensible-seeming defaults:
 ```python
 path  # resolves to os.path, not sys.path
 join  # os.path.join, not shlex.join
 ```
 
+### Aliases <a id="aliases"></a>
+
 For convenience, `datetime.datetime` is also exposed as `dt`, and a few of its members are exported directly:
 ```python
 dt.now()       # datetime.datetime(2023, 8, 3, 10, 9, 43, 981458)
 fromtimestamp  # datetime.datetime.fromtimestamp
 fromisoformat  # datetime.datetime.fromisoformat
 ```
 
-### Custom `cached_property`
+### Custom `cached_property` <a id="cached-property"></a>
 One additional bit of functionality is [this custom `cached_property` decorator](stdlb/cached_property.py), which omits an unnecessary/unserializable lock found in `functools.cached_property`. [cpython#87634](https://github.com/python/cpython/issues/87634) has more info, seems like [a fix is coming in Python 3.12](https://github.com/python/cpython/issues/87634#issuecomment-1467140709).
-
-
```

### Comparing `stdlb-0.0.3/README.md` & `stdlb-0.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,69 @@
+Metadata-Version: 2.1
+Name: stdlb
+Version: 0.0.4
+Summary: Wildcard-import the Python standard library
+Home-page: https://github.com/runsascoded/stdlb
+Author: Ryan Williams
+Author-email: ryan@runsascoded.com
+License: MIT
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
 # `stdlb`
 
 Wildcard-import the Python standard library
 
+[![PyPI badge: "stdlb" library](https://img.shields.io/pypi/v/stdlb.svg)](https://pypi.python.org/pypi/stdlb)
+
 ```python
 from stdlb import *
 
 # Most of the standard library is now available:
 print(f"Current directory: {getcwd()}")
 stderr.write("Python version: {version}\n")
 ```
 
-## Install
+- [Install](#install)
+- [Notes](#notes)
+    - [Collision Resolution](#collisions)
+        - [`__builtins` vs. module members](#builtins)
+        - [Module/Members](#module-members)
+    - [Aliases](#aliases)
+    - [Custom `cached_property`](#cached-property)
+
+## Install <a id="install"></a>
 ```bash
 pip install stdlb
 ```
 
-## Notes
+## Notes <a id="notes"></a>
 I've found this especially useful in Jupyter notebooks, where I don't have an easy "add `import` statements as I add code" setup.
 
 Importing seems to take a few milliseconds (on my Macbook Air):
 ```ipython
 %%time
 from stdlb import *
 # CPU times: user 914 µs, sys: 397 µs, total: 1.31 ms
 # Wall time: 1.6 ms
 ```
 
-### Collisions / Aliases
+### Collision Resolution <a id="collisions"></a>
+
+#### `__builtins` vs. module members <a id="builtins"></a>
+`stdlb` avoids overwriting `__builtins__` with conflicting module members, e.g.:
+- `open` vs. `os.open`
+- `compile` vs. `re.compile`
+- `pow` vs. `math.pow`
+- `copyright` vs. `sys.copyright`
+- `BlockingIOError` vs. `io.BlockingIOError`
+
+[`test.ipynb`](test.ipynb) is executed as part of [`ci.yml`](.github/workflows/ci.yml) to verify there are no `__builtins__` are unexpectedly shadowed.
+
+#### Module/Members <a id="module-members"></a>
 In a few cases, a top-level standard library module also contains a member with the same name (e.g. `datetime`, `shlex`, `time`). `stdlb` makes an effort to ensure the module "wins" in this case:
 
 ```python
 from stdlb import *
 
 datetime  # <module 'datetime' from '$PYTHON_HOME/lib/python3.9/datetime.py'>
 shlex     # <module 'shlex' from '$PYTHON_HOME/lib/python3.9/shlex.py'>
@@ -39,16 +72,20 @@
 
 A few names are disambiguated with the most sensible-seeming defaults:
 ```python
 path  # resolves to os.path, not sys.path
 join  # os.path.join, not shlex.join
 ```
 
+### Aliases <a id="aliases"></a>
+
 For convenience, `datetime.datetime` is also exposed as `dt`, and a few of its members are exported directly:
 ```python
 dt.now()       # datetime.datetime(2023, 8, 3, 10, 9, 43, 981458)
 fromtimestamp  # datetime.datetime.fromtimestamp
 fromisoformat  # datetime.datetime.fromisoformat
 ```
 
-### Custom `cached_property`
+### Custom `cached_property` <a id="cached-property"></a>
 One additional bit of functionality is [this custom `cached_property` decorator](stdlb/cached_property.py), which omits an unnecessary/unserializable lock found in `functools.cached_property`. [cpython#87634](https://github.com/python/cpython/issues/87634) has more info, seems like [a fix is coming in Python 3.12](https://github.com/python/cpython/issues/87634#issuecomment-1467140709).
+
+
```

### Comparing `stdlb-0.0.3/stdlb/__init__.py` & `stdlb-0.0.4/stdlb/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,47 +24,51 @@
 import glob
 
 import hashlib
 from hashlib import *
 
 import io
 from io import *
+BlockingIOError = __builtins__['BlockingIOError']
 
 import itertools
 from itertools import *
 
 import json
 
 import math
 from math import *
+pow = __builtins__['pow']
 
 import os
 from os import *
 open = __builtins__['open']
 from os.path import *
 
 import pathlib
 from pathlib import *
 
 import re
 from re import *
+compile = __builtins__['compile']
 
 from shlex import *
 import shlex
 
 import shutil
 from shutil import *
 join = os.path.join  # seems like a better default than shlex.join
 
 import subprocess
 from subprocess import *
 
 import sys
 from sys import *
 path = os.path
+copyright = __builtins__['copyright']
 
 import tempfile
 from tempfile import *
 
 from time import *
 import time
```

### Comparing `stdlb-0.0.3/stdlb/cached_property.py` & `stdlb-0.0.4/stdlb/cached_property.py`

 * *Files identical despite different names*

### Comparing `stdlb-0.0.3/stdlb.egg-info/PKG-INFO` & `stdlb-0.0.4/stdlb.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,69 @@
 Metadata-Version: 2.1
 Name: stdlb
-Version: 0.0.3
+Version: 0.0.4
 Summary: Wildcard-import the Python standard library
-Home-page: UNKNOWN
+Home-page: https://github.com/runsascoded/stdlb
 Author: Ryan Williams
 Author-email: ryan@runsascoded.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # `stdlb`
 
 Wildcard-import the Python standard library
 
+[![PyPI badge: "stdlb" library](https://img.shields.io/pypi/v/stdlb.svg)](https://pypi.python.org/pypi/stdlb)
+
 ```python
 from stdlb import *
 
 # Most of the standard library is now available:
 print(f"Current directory: {getcwd()}")
 stderr.write("Python version: {version}\n")
 ```
 
-## Install
+- [Install](#install)
+- [Notes](#notes)
+    - [Collision Resolution](#collisions)
+        - [`__builtins` vs. module members](#builtins)
+        - [Module/Members](#module-members)
+    - [Aliases](#aliases)
+    - [Custom `cached_property`](#cached-property)
+
+## Install <a id="install"></a>
 ```bash
 pip install stdlb
 ```
 
-## Notes
+## Notes <a id="notes"></a>
 I've found this especially useful in Jupyter notebooks, where I don't have an easy "add `import` statements as I add code" setup.
 
 Importing seems to take a few milliseconds (on my Macbook Air):
 ```ipython
 %%time
 from stdlb import *
 # CPU times: user 914 µs, sys: 397 µs, total: 1.31 ms
 # Wall time: 1.6 ms
 ```
 
-### Collisions / Aliases
+### Collision Resolution <a id="collisions"></a>
+
+#### `__builtins` vs. module members <a id="builtins"></a>
+`stdlb` avoids overwriting `__builtins__` with conflicting module members, e.g.:
+- `open` vs. `os.open`
+- `compile` vs. `re.compile`
+- `pow` vs. `math.pow`
+- `copyright` vs. `sys.copyright`
+- `BlockingIOError` vs. `io.BlockingIOError`
+
+[`test.ipynb`](test.ipynb) is executed as part of [`ci.yml`](.github/workflows/ci.yml) to verify there are no `__builtins__` are unexpectedly shadowed.
+
+#### Module/Members <a id="module-members"></a>
 In a few cases, a top-level standard library module also contains a member with the same name (e.g. `datetime`, `shlex`, `time`). `stdlb` makes an effort to ensure the module "wins" in this case:
 
 ```python
 from stdlb import *
 
 datetime  # <module 'datetime' from '$PYTHON_HOME/lib/python3.9/datetime.py'>
 shlex     # <module 'shlex' from '$PYTHON_HOME/lib/python3.9/shlex.py'>
@@ -50,18 +72,20 @@
 
 A few names are disambiguated with the most sensible-seeming defaults:
 ```python
 path  # resolves to os.path, not sys.path
 join  # os.path.join, not shlex.join
 ```
 
+### Aliases <a id="aliases"></a>
+
 For convenience, `datetime.datetime` is also exposed as `dt`, and a few of its members are exported directly:
 ```python
 dt.now()       # datetime.datetime(2023, 8, 3, 10, 9, 43, 981458)
 fromtimestamp  # datetime.datetime.fromtimestamp
 fromisoformat  # datetime.datetime.fromisoformat
 ```
 
-### Custom `cached_property`
+### Custom `cached_property` <a id="cached-property"></a>
 One additional bit of functionality is [this custom `cached_property` decorator](stdlb/cached_property.py), which omits an unnecessary/unserializable lock found in `functools.cached_property`. [cpython#87634](https://github.com/python/cpython/issues/87634) has more info, seems like [a fix is coming in Python 3.12](https://github.com/python/cpython/issues/87634#issuecomment-1467140709).
```

