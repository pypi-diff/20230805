# Comparing `tmp/setuptools-github-0.3.7b92.tar.gz` & `tmp/setuptools-github-0.3.7b93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-github-0.3.7b92.tar", last modified: Fri Aug  4 22:21:41 2023, max compression
+gzip compressed data, was "setuptools-github-0.3.7b93.tar", last modified: Sat Aug  5 17:39:35 2023, max compression
```

## Comparing `setuptools-github-0.3.7b92.tar` & `setuptools-github-0.3.7b93.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:21:41.628932 setuptools-github-0.3.7b92/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-08-04 22:21:41.628932 setuptools-github-0.3.7b92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-08-04 22:21:41.000000 setuptools-github-0.3.7b92/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 22:21:41.628932 setuptools-github-0.3.7b92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:21:41.628932 setuptools-github-0.3.7b92/setuptools_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-08-04 22:21:41.000000 setuptools-github-0.3.7b92/setuptools_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-04 22:21:41.000000 setuptools-github-0.3.7b92/setuptools_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 22:21:41.000000 setuptools-github-0.3.7b92/setuptools_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-04 22:21:41.000000 setuptools-github-0.3.7b92/setuptools_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 22:21:41.000000 setuptools-github-0.3.7b92/setuptools_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-04 22:21:41.000000 setuptools-github-0.3.7b92/setuptools_github.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:21:41.624932 setuptools-github-0.3.7b92/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:21:41.628932 setuptools-github-0.3.7b92/src/setuptools_github/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-04 22:21:41.000000 setuptools-github-0.3.7b92/src/setuptools_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/src/setuptools_github/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/src/setuptools_github/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/src/setuptools_github/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/src/setuptools_github/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:21:41.628932 setuptools-github-0.3.7b92/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/tests/test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    11085 2023-08-04 22:20:51.000000 setuptools-github-0.3.7b92/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:39:35.623091 setuptools-github-0.3.7b93/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-05 17:38:50.000000 setuptools-github-0.3.7b93/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-05 17:38:50.000000 setuptools-github-0.3.7b93/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-08-05 17:39:35.619091 setuptools-github-0.3.7b93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-08-05 17:39:35.000000 setuptools-github-0.3.7b93/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-05 17:38:50.000000 setuptools-github-0.3.7b93/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 17:39:35.623091 setuptools-github-0.3.7b93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-08-05 17:38:50.000000 setuptools-github-0.3.7b93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:39:35.619091 setuptools-github-0.3.7b93/setuptools_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-08-05 17:39:35.000000 setuptools-github-0.3.7b93/setuptools_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-05 17:39:35.000000 setuptools-github-0.3.7b93/setuptools_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 17:39:35.000000 setuptools-github-0.3.7b93/setuptools_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-05 17:39:35.000000 setuptools-github-0.3.7b93/setuptools_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-05 17:39:35.000000 setuptools-github-0.3.7b93/setuptools_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-05 17:39:35.000000 setuptools-github-0.3.7b93/setuptools_github.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:39:35.619091 setuptools-github-0.3.7b93/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:39:35.619091 setuptools-github-0.3.7b93/src/setuptools_github/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-05 17:39:35.000000 setuptools-github-0.3.7b93/src/setuptools_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-05 17:38:50.000000 setuptools-github-0.3.7b93/src/setuptools_github/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-05 17:38:50.000000 setuptools-github-0.3.7b93/src/setuptools_github/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-08-05 17:38:50.000000 setuptools-github-0.3.7b93/src/setuptools_github/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11625 2023-08-05 17:38:50.000000 setuptools-github-0.3.7b93/src/setuptools_github/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:39:35.619091 setuptools-github-0.3.7b93/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-08-05 17:38:50.000000 setuptools-github-0.3.7b93/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-05 17:38:50.000000 setuptools-github-0.3.7b93/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-05 17:38:50.000000 setuptools-github-0.3.7b93/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-05 17:38:50.000000 setuptools-github-0.3.7b93/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-08-05 17:38:50.000000 setuptools-github-0.3.7b93/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-05 17:38:50.000000 setuptools-github-0.3.7b93/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11085 2023-08-05 17:38:50.000000 setuptools-github-0.3.7b93/tests/test_tools.py
```

### Comparing `setuptools-github-0.3.7b92/LICENSE` & `setuptools-github-0.3.7b93/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.7b92/PKG-INFO` & `setuptools-github-0.3.7b93/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.7b92
+Version: 0.3.7b93
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -19,16 +19,16 @@
 
 # setuptools-github
 
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
 
-[![Build](https://github.com/cav71/setuptools-github/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/workflows/master.yml)
-[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/master/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/master)
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5771985437)
+[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.7/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.7)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
 ## Quick start
```

### Comparing `setuptools-github-0.3.7b92/README.md` & `setuptools-github-0.3.7b93/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # setuptools-github
 
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
 
-[![Build](https://github.com/cav71/setuptools-github/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/workflows/master.yml)
-[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/master/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/master)
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5771985437)
+[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.7/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.7)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
 ## Quick start
```

### Comparing `setuptools-github-0.3.7b92/pyproject.toml` & `setuptools-github-0.3.7b93/pyproject.toml`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.7b92/setup.py` & `setuptools-github-0.3.7b93/setup.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.7b92/setuptools_github.egg-info/PKG-INFO` & `setuptools-github-0.3.7b93/setuptools_github.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.7b92
+Version: 0.3.7b93
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -19,16 +19,16 @@
 
 # setuptools-github
 
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
 
-[![Build](https://github.com/cav71/setuptools-github/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/workflows/master.yml)
-[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/master/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/master)
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5771985437)
+[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.7/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.7)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
 ## Quick start
```

### Comparing `setuptools-github-0.3.7b92/setuptools_github.egg-info/SOURCES.txt` & `setuptools-github-0.3.7b93/setuptools_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.7b92/src/setuptools_github/cli.py` & `setuptools-github-0.3.7b93/src/setuptools_github/cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.7b92/src/setuptools_github/scm.py` & `setuptools-github-0.3.7b93/src/setuptools_github/scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.7b92/src/setuptools_github/script.py` & `setuptools-github-0.3.7b93/src/setuptools_github/script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.7b92/src/setuptools_github/tools.py` & `setuptools-github-0.3.7b93/src/setuptools_github/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,13 +379,11 @@
     data = get_data(version_file, github_dump, abort)
     set_module_var(version_file, "__version__", data["version"])
     set_module_var(version_file, "__hash__", data["hash"])
 
     env = Environment(autoescape=True)
     env.filters["urlquote"] = partial(quote, safe="")
     for path in list_of_paths(paths):
-        txt = path.read_text()
-        for old, new in (fixers or {}).items():
-            txt = txt.replace(old, new, 1)
+        txt = apply_fixers(path.read_text(), fixers)
         tmpl = env.from_string(txt)
         path.write_text(tmpl.render(ctx=Context(**data)))
     return data
```

### Comparing `setuptools-github-0.3.7b92/tests/conftest.py` & `setuptools-github-0.3.7b93/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.7b92/tests/test_cli.py` & `setuptools-github-0.3.7b93/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.7b92/tests/test_conftest.py` & `setuptools-github-0.3.7b93/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.7b92/tests/test_scm.py` & `setuptools-github-0.3.7b93/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.7b92/tests/test_script.py` & `setuptools-github-0.3.7b93/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.7b92/tests/test_tools.py` & `setuptools-github-0.3.7b93/tests/test_tools.py`

 * *Files identical despite different names*

