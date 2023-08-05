# Comparing `tmp/modflow-devtools-0.3.0.tar.gz` & `tmp/modflow-devtools-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modflow-devtools-0.3.0.tar", last modified: Fri Aug  4 01:32:00 2023, max compression
+gzip compressed data, was "modflow-devtools-1.0.0.tar", last modified: Sat Aug  5 18:15:07 2023, max compression
```

## Comparing `modflow-devtools-0.3.0.tar` & `modflow-devtools-1.0.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-08-04 01:32:00.455114 modflow-devtools-0.3.0/
--rwxr-xr-x   0 wes        (501) staff       (20)     1627 2023-07-26 18:09:37.000000 modflow-devtools-0.3.0/LICENSE.md
--rw-r--r--   0 wes        (501) staff       (20)      163 2023-07-26 21:57:48.000000 modflow-devtools-0.3.0/MANIFEST.in
--rw-r--r--   0 wes        (501) staff       (20)     4768 2023-08-04 01:32:00.454710 modflow-devtools-0.3.0/PKG-INFO
--rw-r--r--   0 wes        (501) staff       (20)     3555 2023-08-04 01:30:58.000000 modflow-devtools-0.3.0/README.md
-drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-08-04 01:32:00.403262 modflow-devtools-0.3.0/modflow_devtools/
--rw-r--r--   0 wes        (501) staff       (20)      248 2023-08-04 01:31:17.000000 modflow-devtools-0.3.0/modflow_devtools/__init__.py
--rw-r--r--   0 wes        (501) staff       (20)      984 2023-07-26 18:09:37.000000 modflow-devtools-0.3.0/modflow_devtools/build.py
--rw-r--r--   0 wes        (501) staff       (20)     1029 2023-07-26 18:09:37.000000 modflow-devtools-0.3.0/modflow_devtools/case.py
--rw-r--r--   0 wes        (501) staff       (20)     7352 2023-07-26 21:57:48.000000 modflow-devtools-0.3.0/modflow_devtools/context.py
--rw-r--r--   0 wes        (501) staff       (20)    17656 2023-08-04 01:30:58.000000 modflow-devtools-0.3.0/modflow_devtools/download.py
--rw-r--r--   0 wes        (501) staff       (20)     2487 2023-07-26 21:57:48.000000 modflow-devtools-0.3.0/modflow_devtools/executables.py
--rw-r--r--   0 wes        (501) staff       (20)    11854 2023-07-26 21:57:48.000000 modflow-devtools-0.3.0/modflow_devtools/fixtures.py
--rw-r--r--   0 wes        (501) staff       (20)     1732 2023-07-26 18:09:37.000000 modflow-devtools-0.3.0/modflow_devtools/markers.py
--rw-r--r--   0 wes        (501) staff       (20)    11069 2023-07-26 21:57:48.000000 modflow-devtools-0.3.0/modflow_devtools/misc.py
-drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-08-04 01:32:00.453747 modflow-devtools-0.3.0/modflow_devtools/test/
--rw-r--r--   0 wes        (501) staff       (20)        0 2023-07-26 18:09:37.000000 modflow-devtools-0.3.0/modflow_devtools/test/__init__.py
--rw-r--r--   0 wes        (501) staff       (20)     1163 2023-07-26 18:09:37.000000 modflow-devtools-0.3.0/modflow_devtools/test/test_build.py
--rw-r--r--   0 wes        (501) staff       (20)     1788 2023-07-26 18:09:37.000000 modflow-devtools-0.3.0/modflow_devtools/test/test_case.py
--rw-r--r--   0 wes        (501) staff       (20)     3606 2023-07-26 21:57:48.000000 modflow-devtools-0.3.0/modflow_devtools/test/test_download.py
--rw-r--r--   0 wes        (501) staff       (20)     1148 2023-07-26 18:09:37.000000 modflow-devtools-0.3.0/modflow_devtools/test/test_executables.py
--rw-r--r--   0 wes        (501) staff       (20)     8043 2023-07-26 21:57:48.000000 modflow-devtools-0.3.0/modflow_devtools/test/test_fixtures.py
--rw-r--r--   0 wes        (501) staff       (20)      904 2023-07-26 18:09:37.000000 modflow-devtools-0.3.0/modflow_devtools/test/test_markers.py
--rw-r--r--   0 wes        (501) staff       (20)     8476 2023-07-26 21:57:48.000000 modflow-devtools-0.3.0/modflow_devtools/test/test_misc.py
--rw-r--r--   0 wes        (501) staff       (20)     2663 2023-07-26 21:57:48.000000 modflow-devtools-0.3.0/modflow_devtools/test/test_zip.py
--rw-r--r--   0 wes        (501) staff       (20)     5708 2023-07-26 21:57:48.000000 modflow-devtools-0.3.0/modflow_devtools/zip.py
-drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-08-04 01:32:00.436144 modflow-devtools-0.3.0/modflow_devtools.egg-info/
--rw-r--r--   0 wes        (501) staff       (20)     4768 2023-08-04 01:32:00.000000 modflow-devtools-0.3.0/modflow_devtools.egg-info/PKG-INFO
--rw-r--r--   0 wes        (501) staff       (20)      913 2023-08-04 01:32:00.000000 modflow-devtools-0.3.0/modflow_devtools.egg-info/SOURCES.txt
--rw-r--r--   0 wes        (501) staff       (20)        1 2023-08-04 01:32:00.000000 modflow-devtools-0.3.0/modflow_devtools.egg-info/dependency_links.txt
--rw-r--r--   0 wes        (501) staff       (20)        1 2022-07-22 15:19:26.000000 modflow-devtools-0.3.0/modflow_devtools.egg-info/not-zip-safe
--rw-r--r--   0 wes        (501) staff       (20)      235 2023-08-04 01:32:00.000000 modflow-devtools-0.3.0/modflow_devtools.egg-info/requires.txt
--rw-r--r--   0 wes        (501) staff       (20)       17 2023-08-04 01:32:00.000000 modflow-devtools-0.3.0/modflow_devtools.egg-info/top_level.txt
--rw-r--r--   0 wes        (501) staff       (20)     2164 2023-08-04 01:30:58.000000 modflow-devtools-0.3.0/pyproject.toml
--rw-r--r--   0 wes        (501) staff       (20)       38 2023-08-04 01:32:00.455233 modflow-devtools-0.3.0/setup.cfg
--rwxr-xr-x   0 wes        (501) staff       (20)       61 2023-07-26 21:57:48.000000 modflow-devtools-0.3.0/setup.py
--rw-r--r--   0 wes        (501) staff       (20)        5 2023-08-04 01:31:17.000000 modflow-devtools-0.3.0/version.txt
+drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-08-05 18:15:07.790226 modflow-devtools-1.0.0/
+-rwxr-xr-x   0 wes        (501) staff       (20)     1627 2023-07-26 18:09:37.000000 modflow-devtools-1.0.0/LICENSE.md
+-rw-r--r--   0 wes        (501) staff       (20)      163 2023-07-26 21:57:48.000000 modflow-devtools-1.0.0/MANIFEST.in
+-rw-r--r--   0 wes        (501) staff       (20)     4805 2023-08-05 18:15:07.789865 modflow-devtools-1.0.0/PKG-INFO
+-rw-r--r--   0 wes        (501) staff       (20)     3580 2023-08-05 18:14:37.000000 modflow-devtools-1.0.0/README.md
+drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-08-05 18:15:07.783076 modflow-devtools-1.0.0/modflow_devtools/
+-rw-r--r--   0 wes        (501) staff       (20)      248 2023-08-05 18:14:37.000000 modflow-devtools-1.0.0/modflow_devtools/__init__.py
+-rw-r--r--   0 wes        (501) staff       (20)      984 2023-07-26 18:09:37.000000 modflow-devtools-1.0.0/modflow_devtools/build.py
+-rw-r--r--   0 wes        (501) staff       (20)    17656 2023-08-04 01:30:58.000000 modflow-devtools-1.0.0/modflow_devtools/download.py
+-rw-r--r--   0 wes        (501) staff       (20)     1013 2023-08-05 18:14:37.000000 modflow-devtools-1.0.0/modflow_devtools/executables.py
+-rw-r--r--   0 wes        (501) staff       (20)    11951 2023-08-05 18:14:37.000000 modflow-devtools-1.0.0/modflow_devtools/fixtures.py
+-rw-r--r--   0 wes        (501) staff       (20)     5522 2023-08-05 18:14:37.000000 modflow-devtools-1.0.0/modflow_devtools/imports.py
+-rw-r--r--   0 wes        (501) staff       (20)     1829 2023-08-05 18:14:37.000000 modflow-devtools-1.0.0/modflow_devtools/markers.py
+-rw-r--r--   0 wes        (501) staff       (20)    11069 2023-07-26 21:57:48.000000 modflow-devtools-1.0.0/modflow_devtools/misc.py
+-rw-r--r--   0 wes        (501) staff       (20)     3440 2023-08-05 18:14:37.000000 modflow-devtools-1.0.0/modflow_devtools/ostags.py
+drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-08-05 18:15:07.789240 modflow-devtools-1.0.0/modflow_devtools/test/
+-rw-r--r--   0 wes        (501) staff       (20)        0 2023-07-26 18:09:37.000000 modflow-devtools-1.0.0/modflow_devtools/test/__init__.py
+-rw-r--r--   0 wes        (501) staff       (20)     1163 2023-07-26 18:09:37.000000 modflow-devtools-1.0.0/modflow_devtools/test/test_build.py
+-rw-r--r--   0 wes        (501) staff       (20)     3606 2023-07-26 21:57:48.000000 modflow-devtools-1.0.0/modflow_devtools/test/test_download.py
+-rw-r--r--   0 wes        (501) staff       (20)     1119 2023-08-05 18:14:37.000000 modflow-devtools-1.0.0/modflow_devtools/test/test_executables.py
+-rw-r--r--   0 wes        (501) staff       (20)     8043 2023-07-26 21:57:48.000000 modflow-devtools-1.0.0/modflow_devtools/test/test_fixtures.py
+-rw-r--r--   0 wes        (501) staff       (20)      904 2023-07-26 18:09:37.000000 modflow-devtools-1.0.0/modflow_devtools/test/test_markers.py
+-rw-r--r--   0 wes        (501) staff       (20)     8476 2023-07-26 21:57:48.000000 modflow-devtools-1.0.0/modflow_devtools/test/test_misc.py
+-rw-r--r--   0 wes        (501) staff       (20)     1499 2023-08-05 18:14:37.000000 modflow-devtools-1.0.0/modflow_devtools/test/test_ostags.py
+-rw-r--r--   0 wes        (501) staff       (20)     2663 2023-07-26 21:57:48.000000 modflow-devtools-1.0.0/modflow_devtools/test/test_zip.py
+-rw-r--r--   0 wes        (501) staff       (20)     5708 2023-07-26 21:57:48.000000 modflow-devtools-1.0.0/modflow_devtools/zip.py
+drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-08-05 18:15:07.785888 modflow-devtools-1.0.0/modflow_devtools.egg-info/
+-rw-r--r--   0 wes        (501) staff       (20)     4805 2023-08-05 18:15:07.000000 modflow-devtools-1.0.0/modflow_devtools.egg-info/PKG-INFO
+-rw-r--r--   0 wes        (501) staff       (20)      917 2023-08-05 18:15:07.000000 modflow-devtools-1.0.0/modflow_devtools.egg-info/SOURCES.txt
+-rw-r--r--   0 wes        (501) staff       (20)        1 2023-08-05 18:15:07.000000 modflow-devtools-1.0.0/modflow_devtools.egg-info/dependency_links.txt
+-rw-r--r--   0 wes        (501) staff       (20)        1 2022-07-22 15:19:26.000000 modflow-devtools-1.0.0/modflow_devtools.egg-info/not-zip-safe
+-rw-r--r--   0 wes        (501) staff       (20)      235 2023-08-05 18:15:07.000000 modflow-devtools-1.0.0/modflow_devtools.egg-info/requires.txt
+-rw-r--r--   0 wes        (501) staff       (20)       17 2023-08-05 18:15:07.000000 modflow-devtools-1.0.0/modflow_devtools.egg-info/top_level.txt
+-rw-r--r--   0 wes        (501) staff       (20)     2176 2023-08-05 18:14:37.000000 modflow-devtools-1.0.0/pyproject.toml
+-rw-r--r--   0 wes        (501) staff       (20)       38 2023-08-05 18:15:07.790320 modflow-devtools-1.0.0/setup.cfg
+-rwxr-xr-x   0 wes        (501) staff       (20)       61 2023-07-26 21:57:48.000000 modflow-devtools-1.0.0/setup.py
+-rw-r--r--   0 wes        (501) staff       (20)        5 2023-08-05 18:14:37.000000 modflow-devtools-1.0.0/version.txt
```

### Comparing `modflow-devtools-0.3.0/LICENSE.md` & `modflow-devtools-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.3.0/PKG-INFO` & `modflow-devtools-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: modflow-devtools
-Version: 0.3.0
+Version: 1.0.0
 Summary: Python tools for MODFLOW development
 Author-email: "Joseph D. Hughes" <modflow@usgs.gov>
 Maintainer-email: "Joseph D. Hughes" <modflow@usgs.gov>
 License: CC0
 Project-URL: Documentation, https://modflow-devtools.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/MODFLOW-USGS/modflow-devtools/issues
 Project-URL: Source Code, https://github.com/MODFLOW-USGS/modflow-devtools
 Keywords: MODFLOW,development,utilities,groundwater,hydrogeology
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -48,15 +48,15 @@
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
 ## Use cases
 
 This is a small toolkit for developing MODFLOW 6, FloPy, and related projects. It includes standalone utilities and optional [Pytest](https://github.com/pytest-dev/pytest) extensions.
 
-Standalone utilities include a very minimal GitHub API client, mainly for retrieving release information and downloading assets, and a `ZipFile` subclass that [preserves file permissions](https://stackoverflow.com/questions/39296101/python-zipfile-removes-execute-permissions-from-binaries) (workaround for [Python #15795](https://bugs.python.org/issue15795))
+The former include a very minimal GitHub API client for retrieving release information and downloading assets, a `ZipFile` subclass that [preserves file permissions](https://stackoverflow.com/questions/39296101/python-zipfile-removes-execute-permissions-from-binaries) (workaround for [Python #15795](https://bugs.python.org/issue15795)), and other release/distribution-related tools.
 
 Pytest features include:
 
 - `--keep <path>` tempdir fixtures for [each scope](https://docs.pytest.org/en/stable/how-to/fixtures.html#scope-sharing-fixtures-across-classes-modules-packages-or-session)
 - a [`--smoke` test](https://en.wikipedia.org/wiki/Smoke_testing_(software)) (abbrev. `-S`) CLI option shortcut
 - markers to skip test cases conditional on
   - operating system
```

### Comparing `modflow-devtools-0.3.0/README.md` & `modflow-devtools-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
 ## Use cases
 
 This is a small toolkit for developing MODFLOW 6, FloPy, and related projects. It includes standalone utilities and optional [Pytest](https://github.com/pytest-dev/pytest) extensions.
 
-Standalone utilities include a very minimal GitHub API client, mainly for retrieving release information and downloading assets, and a `ZipFile` subclass that [preserves file permissions](https://stackoverflow.com/questions/39296101/python-zipfile-removes-execute-permissions-from-binaries) (workaround for [Python #15795](https://bugs.python.org/issue15795))
+The former include a very minimal GitHub API client for retrieving release information and downloading assets, a `ZipFile` subclass that [preserves file permissions](https://stackoverflow.com/questions/39296101/python-zipfile-removes-execute-permissions-from-binaries) (workaround for [Python #15795](https://bugs.python.org/issue15795)), and other release/distribution-related tools.
 
 Pytest features include:
 
 - `--keep <path>` tempdir fixtures for [each scope](https://docs.pytest.org/en/stable/how-to/fixtures.html#scope-sharing-fixtures-across-classes-modules-packages-or-session)
 - a [`--smoke` test](https://en.wikipedia.org/wiki/Smoke_testing_(software)) (abbrev. `-S`) CLI option shortcut
 - markers to skip test cases conditional on
   - operating system
```

### Comparing `modflow-devtools-0.3.0/modflow_devtools/build.py` & `modflow-devtools-1.0.0/modflow_devtools/build.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.3.0/modflow_devtools/download.py` & `modflow-devtools-1.0.0/modflow_devtools/download.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.3.0/modflow_devtools/fixtures.py` & `modflow-devtools-1.0.0/modflow_devtools/fixtures.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from collections import OrderedDict
 from itertools import groupby
 from os import PathLike, environ
 from pathlib import Path
 from shutil import copytree, rmtree
 from typing import Dict, List, Optional
 
-import pytest
+from modflow_devtools.imports import import_optional_dependency
 from modflow_devtools.misc import get_namefile_paths, get_packages
 
+pytest = import_optional_dependency("pytest")
+
 # temporary directory fixtures
 
 
 @pytest.fixture(scope="function")
 def function_tmpdir(tmpdir_factory, request) -> Path:
     node = (
         request.node.name.replace("/", "_")
```

### Comparing `modflow-devtools-0.3.0/modflow_devtools/markers.py` & `modflow-devtools-1.0.0/modflow_devtools/markers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from platform import system
 
-import pytest
+from modflow_devtools.imports import import_optional_dependency
 from modflow_devtools.misc import (
     get_current_branch,
     has_exe,
     has_pkg,
     is_connected,
     is_in_ci,
 )
 
+pytest = import_optional_dependency("pytest")
+
 
 def requires_exe(*exes):
     missing = {exe for exe in exes if not has_exe(exe)}
     return pytest.mark.skipif(
         missing,
         reason=f"missing executable{'s' if len(missing) != 1 else ''}: "
         + ", ".join(missing),
```

### Comparing `modflow-devtools-0.3.0/modflow_devtools/misc.py` & `modflow-devtools-1.0.0/modflow_devtools/misc.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.3.0/modflow_devtools/test/test_build.py` & `modflow-devtools-1.0.0/modflow_devtools/test/test_build.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.3.0/modflow_devtools/test/test_download.py` & `modflow-devtools-1.0.0/modflow_devtools/test/test_download.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.3.0/modflow_devtools/test/test_executables.py` & `modflow-devtools-1.0.0/modflow_devtools/test/test_executables.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 import subprocess
 import sys
 from os import environ
 from pathlib import Path
 
 import pytest
-from modflow_devtools.executables import Executables, build_default_exe_dict
+from modflow_devtools.executables import Executables
 from modflow_devtools.misc import add_sys_path, get_suffixes
 
 _bin_path = Path(environ.get("BIN_PATH")).expanduser().absolute()
 _ext, _ = get_suffixes(sys.platform)
 
 
 @pytest.fixture
 def exes():
     if not _bin_path.is_dir():
         pytest.skip(f"BIN_PATH ({_bin_path}) is not a directory")
 
     with add_sys_path(str(_bin_path)):
-        yield Executables(**build_default_exe_dict(_bin_path))
+        yield Executables(
+            **{
+                "mf6": _bin_path / f"mf6{_ext}",
+            }
+        )
 
 
 def test_get_version(exes):
     ver_str = Executables.get_version(exes.mf6)
     version = (
         subprocess.check_output([f"{exes.mf6}", "-v"])
         .decode("utf-8")
@@ -34,8 +38,7 @@
 
 def test_mapping(exes):
     print(exes.mf6)
     assert (
         exes.mf6 == exes["mf6"]
     )  # should support both attribute and dictionary access
     assert exes.mf6 == _bin_path / f"mf6{_ext}"  # should be the correct path
-    assert exes.mf6_regression.parent.parent == _bin_path
```

### Comparing `modflow-devtools-0.3.0/modflow_devtools/test/test_fixtures.py` & `modflow-devtools-1.0.0/modflow_devtools/test/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.3.0/modflow_devtools/test/test_markers.py` & `modflow-devtools-1.0.0/modflow_devtools/test/test_markers.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.3.0/modflow_devtools/test/test_misc.py` & `modflow-devtools-1.0.0/modflow_devtools/test/test_misc.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.3.0/modflow_devtools/test/test_zip.py` & `modflow-devtools-1.0.0/modflow_devtools/test/test_zip.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.3.0/modflow_devtools/zip.py` & `modflow-devtools-1.0.0/modflow_devtools/zip.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.3.0/modflow_devtools.egg-info/PKG-INFO` & `modflow-devtools-1.0.0/modflow_devtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: modflow-devtools
-Version: 0.3.0
+Version: 1.0.0
 Summary: Python tools for MODFLOW development
 Author-email: "Joseph D. Hughes" <modflow@usgs.gov>
 Maintainer-email: "Joseph D. Hughes" <modflow@usgs.gov>
 License: CC0
 Project-URL: Documentation, https://modflow-devtools.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/MODFLOW-USGS/modflow-devtools/issues
 Project-URL: Source Code, https://github.com/MODFLOW-USGS/modflow-devtools
 Keywords: MODFLOW,development,utilities,groundwater,hydrogeology
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -48,15 +48,15 @@
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
 ## Use cases
 
 This is a small toolkit for developing MODFLOW 6, FloPy, and related projects. It includes standalone utilities and optional [Pytest](https://github.com/pytest-dev/pytest) extensions.
 
-Standalone utilities include a very minimal GitHub API client, mainly for retrieving release information and downloading assets, and a `ZipFile` subclass that [preserves file permissions](https://stackoverflow.com/questions/39296101/python-zipfile-removes-execute-permissions-from-binaries) (workaround for [Python #15795](https://bugs.python.org/issue15795))
+The former include a very minimal GitHub API client for retrieving release information and downloading assets, a `ZipFile` subclass that [preserves file permissions](https://stackoverflow.com/questions/39296101/python-zipfile-removes-execute-permissions-from-binaries) (workaround for [Python #15795](https://bugs.python.org/issue15795)), and other release/distribution-related tools.
 
 Pytest features include:
 
 - `--keep <path>` tempdir fixtures for [each scope](https://docs.pytest.org/en/stable/how-to/fixtures.html#scope-sharing-fixtures-across-classes-modules-packages-or-session)
 - a [`--smoke` test](https://en.wikipedia.org/wiki/Smoke_testing_(software)) (abbrev. `-S`) CLI option shortcut
 - markers to skip test cases conditional on
   - operating system
```

### Comparing `modflow-devtools-0.3.0/modflow_devtools.egg-info/SOURCES.txt` & `modflow-devtools-1.0.0/modflow_devtools.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 version.txt
 modflow_devtools/__init__.py
 modflow_devtools/build.py
-modflow_devtools/case.py
-modflow_devtools/context.py
 modflow_devtools/download.py
 modflow_devtools/executables.py
 modflow_devtools/fixtures.py
+modflow_devtools/imports.py
 modflow_devtools/markers.py
 modflow_devtools/misc.py
+modflow_devtools/ostags.py
 modflow_devtools/zip.py
 modflow_devtools.egg-info/PKG-INFO
 modflow_devtools.egg-info/SOURCES.txt
 modflow_devtools.egg-info/dependency_links.txt
 modflow_devtools.egg-info/not-zip-safe
 modflow_devtools.egg-info/requires.txt
 modflow_devtools.egg-info/top_level.txt
 modflow_devtools/test/__init__.py
 modflow_devtools/test/test_build.py
-modflow_devtools/test/test_case.py
 modflow_devtools/test/test_download.py
 modflow_devtools/test/test_executables.py
 modflow_devtools/test/test_fixtures.py
 modflow_devtools/test/test_markers.py
 modflow_devtools/test/test_misc.py
+modflow_devtools/test/test_ostags.py
 modflow_devtools/test/test_zip.py
```

### Comparing `modflow-devtools-0.3.0/pyproject.toml` & `modflow-devtools-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "utilities",
     "groundwater",
     "hydrogeology"
 ]
 readme = "README.md"
 license = {text = "CC0"}
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
     "License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

