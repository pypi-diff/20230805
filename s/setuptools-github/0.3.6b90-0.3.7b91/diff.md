# Comparing `tmp/setuptools-github-0.3.6b90.tar.gz` & `tmp/setuptools-github-0.3.7b91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-github-0.3.6b90.tar", last modified: Thu Aug  3 14:47:36 2023, max compression
+gzip compressed data, was "setuptools-github-0.3.7b91.tar", last modified: Fri Aug  4 19:54:42 2023, max compression
```

## Comparing `setuptools-github-0.3.6b90.tar` & `setuptools-github-0.3.7b91.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:47:36.243119 setuptools-github-0.3.6b90/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-08-03 14:47:36.243119 setuptools-github-0.3.6b90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-08-03 14:47:36.000000 setuptools-github-0.3.6b90/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 14:47:36.243119 setuptools-github-0.3.6b90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:47:36.239119 setuptools-github-0.3.6b90/setuptools_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-08-03 14:47:36.000000 setuptools-github-0.3.6b90/setuptools_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-03 14:47:36.000000 setuptools-github-0.3.6b90/setuptools_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:47:36.000000 setuptools-github-0.3.6b90/setuptools_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-03 14:47:36.000000 setuptools-github-0.3.6b90/setuptools_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-03 14:47:36.000000 setuptools-github-0.3.6b90/setuptools_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-03 14:47:36.000000 setuptools-github-0.3.6b90/setuptools_github.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:47:36.239119 setuptools-github-0.3.6b90/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:47:36.239119 setuptools-github-0.3.6b90/src/setuptools_github/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-03 14:47:36.000000 setuptools-github-0.3.6b90/src/setuptools_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/src/setuptools_github/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/src/setuptools_github/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/src/setuptools_github/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/src/setuptools_github/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    11363 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/src/setuptools_github/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:47:36.243119 setuptools-github-0.3.6b90/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/tests/test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:54:42.211853 setuptools-github-0.3.7b91/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-08-04 19:54:42.211853 setuptools-github-0.3.7b91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-08-04 19:54:42.000000 setuptools-github-0.3.7b91/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 19:54:42.211853 setuptools-github-0.3.7b91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:54:42.207853 setuptools-github-0.3.7b91/setuptools_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-08-04 19:54:42.000000 setuptools-github-0.3.7b91/setuptools_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-04 19:54:42.000000 setuptools-github-0.3.7b91/setuptools_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 19:54:42.000000 setuptools-github-0.3.7b91/setuptools_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-04 19:54:42.000000 setuptools-github-0.3.7b91/setuptools_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 19:54:42.000000 setuptools-github-0.3.7b91/setuptools_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-04 19:54:42.000000 setuptools-github-0.3.7b91/setuptools_github.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:54:42.207853 setuptools-github-0.3.7b91/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:54:42.211853 setuptools-github-0.3.7b91/src/setuptools_github/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-04 19:54:42.000000 setuptools-github-0.3.7b91/src/setuptools_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/src/setuptools_github/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/src/setuptools_github/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/src/setuptools_github/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/src/setuptools_github/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/src/setuptools_github/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:54:42.211853 setuptools-github-0.3.7b91/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11085 2023-08-04 19:54:06.000000 setuptools-github-0.3.7b91/tests/test_tools.py
```

### Comparing `setuptools-github-0.3.6b90/LICENSE` & `setuptools-github-0.3.7b91/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.6b90/PKG-INFO` & `setuptools-github-0.3.7b91/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.6b90
+Version: 0.3.7b91
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
 
-[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5752209245)
-[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.6/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.6)
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/workflows/master.yml)
+[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/master/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/master)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
 ## Quick start
@@ -43,15 +43,15 @@
   ├── .github
   │   └── workflows           <- workflow files for
   │       ├── beta.yml             * beta/N.M.O branches
   │       ├── master.yml           * master branch
   │       └── tags.yml             * release/N.M.O tags
   ├── src
   │   └── project_name        <- project name
-  │       └── __init__.py     <- initfile
+  │       └── __init__.py     <- version_file
   └── tests                   <- tests (pytest)
       ├── conftest.py
       └── requirements.txt    <- requirement file for tests
 ```
 
 > **NOTE** for a pyproject.toml / hatch enabled version of this, please use
 > [hatch-ci plugin](https://pypi.org/project/hatch-ci)
@@ -60,28 +60,28 @@
 #### install the package
 ```bash
 pip install setuptools-github
  or
 conda install -c conda-forge setuptools-github
 ```
 
-#### put the initial version info in the initfile
+#### put the initial version info in the version_file
 Create a new `src/project_name/__init__.py` file to store the package information:
 ```
 __version__ = "N.M.O"  # replace N, M and O with numerical values (eg. 0.0.0)
 __hash__ = ""  # leave this empty
 ```
 
 #### Fix the setup.py file
 ```
 from setuptools_github import tools
 
 setup(
   name="project-name",
-  version=tools.update_version(initfile, os.getenv("GITHUB_DUMP")),
+  version=tools.update_version(version_file, os.getenv("GITHUB_DUMP")),
   ...
 ```
 > **NOTE**: there's an advanced function `tools.process` that can update 
 > and process files like the readmes (see an example in [setup.py](https://raw.githubusercontent.com/cav71/setuptools-github/master/setup.py))
 
 #### Add the github workflow files
 - [github/workflows/master.yml](https://github.com/cav71/setuptools-github/blob/master/.github/workflows/master.yml)
@@ -152,15 +152,15 @@
 ```python
 
 python -m setuptools_github.script micro src/project_name/__init__.py
 or
 setuptools-github make-beta micro src/project_name/__init__.py
 ```
 This will tag the HEAD on **beta/N.M.O** branch 
-with the **release/N.M.O** tag and increment the **initfile** with the
+with the **release/N.M.O** tag and increment the **version_file** with the
 next version N.M.O+1 (using micro).
 
 Once done, you'll need to push it the tag.
 ```bash
 git push release/N.M.O
 ```
 This will:
```

### Comparing `setuptools-github-0.3.6b90/README.md` & `setuptools-github-0.3.7b91/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # setuptools-github
 
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
 
-[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5752209245)
-[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.6/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.6)
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/workflows/master.yml)
+[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/master/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/master)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
 ## Quick start
@@ -24,15 +24,15 @@
   ├── .github
   │   └── workflows           <- workflow files for
   │       ├── beta.yml             * beta/N.M.O branches
   │       ├── master.yml           * master branch
   │       └── tags.yml             * release/N.M.O tags
   ├── src
   │   └── project_name        <- project name
-  │       └── __init__.py     <- initfile
+  │       └── __init__.py     <- version_file
   └── tests                   <- tests (pytest)
       ├── conftest.py
       └── requirements.txt    <- requirement file for tests
 ```
 
 > **NOTE** for a pyproject.toml / hatch enabled version of this, please use
 > [hatch-ci plugin](https://pypi.org/project/hatch-ci)
@@ -41,28 +41,28 @@
 #### install the package
 ```bash
 pip install setuptools-github
  or
 conda install -c conda-forge setuptools-github
 ```
 
-#### put the initial version info in the initfile
+#### put the initial version info in the version_file
 Create a new `src/project_name/__init__.py` file to store the package information:
 ```
 __version__ = "N.M.O"  # replace N, M and O with numerical values (eg. 0.0.0)
 __hash__ = ""  # leave this empty
 ```
 
 #### Fix the setup.py file
 ```
 from setuptools_github import tools
 
 setup(
   name="project-name",
-  version=tools.update_version(initfile, os.getenv("GITHUB_DUMP")),
+  version=tools.update_version(version_file, os.getenv("GITHUB_DUMP")),
   ...
 ```
 > **NOTE**: there's an advanced function `tools.process` that can update 
 > and process files like the readmes (see an example in [setup.py](https://raw.githubusercontent.com/cav71/setuptools-github/master/setup.py))
 
 #### Add the github workflow files
 - [github/workflows/master.yml](https://github.com/cav71/setuptools-github/blob/master/.github/workflows/master.yml)
@@ -133,15 +133,15 @@
 ```python
 
 python -m setuptools_github.script micro src/project_name/__init__.py
 or
 setuptools-github make-beta micro src/project_name/__init__.py
 ```
 This will tag the HEAD on **beta/N.M.O** branch 
-with the **release/N.M.O** tag and increment the **initfile** with the
+with the **release/N.M.O** tag and increment the **version_file** with the
 next version N.M.O+1 (using micro).
 
 Once done, you'll need to push it the tag.
 ```bash
 git push release/N.M.O
 ```
 This will:
```

### Comparing `setuptools-github-0.3.6b90/pyproject.toml` & `setuptools-github-0.3.7b91/pyproject.toml`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.6b90/setuptools_github.egg-info/PKG-INFO` & `setuptools-github-0.3.7b91/setuptools_github.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.6b90
+Version: 0.3.7b91
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
 
-[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5752209245)
-[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.6/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.6)
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/workflows/master.yml)
+[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/master/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/master)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
 ## Quick start
@@ -43,15 +43,15 @@
   ├── .github
   │   └── workflows           <- workflow files for
   │       ├── beta.yml             * beta/N.M.O branches
   │       ├── master.yml           * master branch
   │       └── tags.yml             * release/N.M.O tags
   ├── src
   │   └── project_name        <- project name
-  │       └── __init__.py     <- initfile
+  │       └── __init__.py     <- version_file
   └── tests                   <- tests (pytest)
       ├── conftest.py
       └── requirements.txt    <- requirement file for tests
 ```
 
 > **NOTE** for a pyproject.toml / hatch enabled version of this, please use
 > [hatch-ci plugin](https://pypi.org/project/hatch-ci)
@@ -60,28 +60,28 @@
 #### install the package
 ```bash
 pip install setuptools-github
  or
 conda install -c conda-forge setuptools-github
 ```
 
-#### put the initial version info in the initfile
+#### put the initial version info in the version_file
 Create a new `src/project_name/__init__.py` file to store the package information:
 ```
 __version__ = "N.M.O"  # replace N, M and O with numerical values (eg. 0.0.0)
 __hash__ = ""  # leave this empty
 ```
 
 #### Fix the setup.py file
 ```
 from setuptools_github import tools
 
 setup(
   name="project-name",
-  version=tools.update_version(initfile, os.getenv("GITHUB_DUMP")),
+  version=tools.update_version(version_file, os.getenv("GITHUB_DUMP")),
   ...
 ```
 > **NOTE**: there's an advanced function `tools.process` that can update 
 > and process files like the readmes (see an example in [setup.py](https://raw.githubusercontent.com/cav71/setuptools-github/master/setup.py))
 
 #### Add the github workflow files
 - [github/workflows/master.yml](https://github.com/cav71/setuptools-github/blob/master/.github/workflows/master.yml)
@@ -152,15 +152,15 @@
 ```python
 
 python -m setuptools_github.script micro src/project_name/__init__.py
 or
 setuptools-github make-beta micro src/project_name/__init__.py
 ```
 This will tag the HEAD on **beta/N.M.O** branch 
-with the **release/N.M.O** tag and increment the **initfile** with the
+with the **release/N.M.O** tag and increment the **version_file** with the
 next version N.M.O+1 (using micro).
 
 Once done, you'll need to push it the tag.
 ```bash
 git push release/N.M.O
 ```
 This will:
```

### Comparing `setuptools-github-0.3.6b90/setuptools_github.egg-info/SOURCES.txt` & `setuptools-github-0.3.7b91/setuptools_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.6b90/src/setuptools_github/checks.py` & `setuptools-github-0.3.7b91/src/setuptools_github/checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.6b90/src/setuptools_github/cli.py` & `setuptools-github-0.3.7b91/src/setuptools_github/cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.6b90/src/setuptools_github/scm.py` & `setuptools-github-0.3.7b91/src/setuptools_github/scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.6b90/src/setuptools_github/script.py` & `setuptools-github-0.3.7b91/src/setuptools_github/script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.6b90/src/setuptools_github/tools.py` & `setuptools-github-0.3.7b91/src/setuptools_github/tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -93,14 +93,24 @@
     return [Path(s) for s in ([paths] if isinstance(paths, (str, Path)) else paths)]
 
 
 def lstrip(txt: str, left: str) -> str:
     return txt[len(left) :] if txt.startswith(left) else txt
 
 
+def apply_fixers(txt: str, fixers: dict[str, str] | None = None) -> str:
+    result = txt
+    for src, dst in (fixers or {}).items():
+        if src.startswith("re:"):
+            result = re.sub(src[3:], dst, result)
+        else:
+            result = result.replace(src, dst)
+    return result
+
+
 def get_module_var(
     path: Path | str, var: str = "__version__", abort=True
 ) -> str | None:
     """extract from a python module in path the module level <var> variable
 
     Args:
         path (str,Path): python module file to parse using ast (no code-execution)
@@ -162,15 +172,15 @@
     path: str | Path, var: str, value: Any, create: bool = True
 ) -> tuple[Any, str]:
     """replace var in path with value
 
     Args:
         path (str,Path): python module file to parse
         var (str): module level variable name to extract
-        value (None or Any): if not None replace var in initfile
+        value (None or Any): if not None replace var in version_file
         create (bool): create path if not present
 
     Returns:
         (str, str) the (<previous-var-value|None>, <the new text>)
     """
 
     # validate the var
@@ -234,36 +244,36 @@
         newver[-1] = 0
     elif mode == "micro":
         newver[-1] += 1
     return ".".join(str(v) for v in newver)
 
 
 def get_data(
-    initfile: str | Path, github_dump: str | None = None, abort: bool = True
+    version_file: str | Path, github_dump: str | None = None, abort: bool = True
 ) -> dict[str, str | None]:
-    """extracts version information from github_dump and updates initfile in-place
+    """extracts version information from github_dump and updates version_file in-place
 
     Args:
-        initfile (str, Path): path to the __init__.py file with a __version__ variable
+        version_file (str, Path): path to a file  with a __version__ variable
         github_dump (str): the os.getenv("GITHUB_DUMP") value
 
     Returns:
         dict[str,str|None]: a dict with the current config
     """
     result = {
-        "version": get_module_var(initfile, "__version__"),
-        "current": get_module_var(initfile, "__version__"),
+        "version": get_module_var(version_file, "__version__"),
+        "current": get_module_var(version_file, "__version__"),
         "branch": None,
         "hash": None,
         "build": None,
         "runid": None,
         "workflow": None,
     }
 
-    path = Path(initfile)
+    path = Path(version_file)
     repo = scm.lookup(path)
 
     if not (repo or github_dump):
         if abort:
             raise scm.InvalidGitRepoError(f"cannot find a valid git repo for {path}")
         return result
 
@@ -305,44 +315,44 @@
             result["workflow"] = "beta"
         else:
             result["workflow"] = "tags"
     return result
 
 
 def update_version(
-    initfile: str | Path, github_dump: str | None = None, abort: bool = True
+    version_file: str | Path, github_dump: str | None = None, abort: bool = True
 ) -> str | None:
-    """extracts version information from github_dump and updates initfile in-place
+    """extracts version information from github_dump and updates version_file in-place
 
     Args:
-        initfile (str, Path): path to the __init__.py file with a __version__ variable
+        version_file (str, Path): path to a file with a __version__ variable
         github_dump (str): the os.getenv("GITHUB_DUMP") value
 
     Returns:
         str: the new version for the package
     """
 
-    data = get_data(initfile, github_dump, abort)
-    set_module_var(initfile, "__version__", data["version"])
-    set_module_var(initfile, "__hash__", data["hash"])
+    data = get_data(version_file, github_dump, abort)
+    set_module_var(version_file, "__version__", data["version"])
+    set_module_var(version_file, "__hash__", data["hash"])
     return data["version"]
 
 
 def process(
-    initfile: str | Path,
+    version_file: str | Path,
     github_dump: str | None = None,
     paths: str | Path | list[str | Path] | None = None,
     fixers: dict[str, str] | None = None,
     abort: bool = True,
 ) -> dict[str, str | None]:
-    """get version from github_dump and updates initfile/paths
+    """get version from github_dump and updates version_file/paths
 
     Args:
         paths (str, Path): path(s) to files jinja2 processeable
-        initfile (str, Path): path to the __init__.py file with a __version__ variable
+        version_file (str, Path): path to a file with __version__ variable
         github_dump (str): the os.getenv("GITHUB_DUMP") value
 
     Returns:
         str: the new version for the package
 
     Example:
         {'branch': 'beta/0.3.1',
@@ -362,17 +372,17 @@
     class Context(Namespace):
         def items(self):
             for name, value in self.__dict__.items():
                 if name.startswith("_"):
                     continue
                 yield (name, value)
 
-    data = get_data(initfile, github_dump, abort)
-    set_module_var(initfile, "__version__", data["version"])
-    set_module_var(initfile, "__hash__", data["hash"])
+    data = get_data(version_file, github_dump, abort)
+    set_module_var(version_file, "__version__", data["version"])
+    set_module_var(version_file, "__hash__", data["hash"])
 
     env = Environment(autoescape=True)
     env.filters["urlquote"] = partial(quote, safe="")
     for path in list_of_paths(paths):
         txt = path.read_text()
         for old, new in (fixers or {}).items():
             txt = txt.replace(old, new, 1)
```

### Comparing `setuptools-github-0.3.6b90/tests/conftest.py` & `setuptools-github-0.3.7b91/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.6b90/tests/test_checks.py` & `setuptools-github-0.3.7b91/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.6b90/tests/test_cli.py` & `setuptools-github-0.3.7b91/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.6b90/tests/test_conftest.py` & `setuptools-github-0.3.7b91/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.6b90/tests/test_scm.py` & `setuptools-github-0.3.7b91/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.6b90/tests/test_script.py` & `setuptools-github-0.3.7b91/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.6b90/tests/test_tools.py` & `setuptools-github-0.3.7b91/tests/test_tools.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# ruff: noqa: E501
+
 import pytest
 from setuptools_github import tools
 
 # this is the output from ${{ toJson(github) }}
 GITHUB = {
     "beta": {
         "ref": "refs/heads/beta/0.0.4",
@@ -131,14 +133,52 @@
     ]
 
 
 def test_lstrip():
     assert tools.lstrip("/a/b/c/d/e", "/a/b") == "/c/d/e"
 
 
+def test_apply_fixers():
+    fixers = {
+        "abc": "def",
+    }
+    assert tools.apply_fixers("abcdef abc123", fixers) == "defdef def123"
+    fixers = {
+        "re:([ab])cde": "x\\1",
+    }
+    assert tools.apply_fixers("acde bcde123", fixers) == "xa xb123"
+
+    fixers = {
+        # for the github actions
+        "re:(https://github.com/.+/actions/workflows/)(master)(.yml/badge.svg)": "\\1{{ ctx.workflow }}\\3",
+        "re:(https://github.com/.+/actions)/(workflows/)(master.yml)(?!/)": "\\1/runs/{{ ctx.runid }}",
+        # for the codecov part
+        "re:(https://codecov.io/gh/.+/tree)/master(/graph/badge.svg[?]token=.+)": "\\1/{{ ctx.branch|urlquote }}\\2",
+        "re:(https://codecov.io/gh/.+/tree)/master(?!/)": "\\1/{{ ctx.branch|urlquote }}",
+    }
+
+    txt = "https://github.com/cav71/setuptools-github/actions/workflows/master.yml/badge.svg"
+    expected = "https://github.com/cav71/setuptools-github/actions/workflows/{{ ctx.workflow }}.yml/badge.svg"
+    assert tools.apply_fixers(txt, fixers) == expected
+
+    txt = "https://github.com/cav71/setuptools-github/actions/workflows/master.yml"
+    expected = "https://github.com/cav71/setuptools-github/actions/runs/{{ ctx.runid }}"
+    assert tools.apply_fixers(txt, fixers) == expected
+
+    txt = "https://codecov.io/gh/cav71/setuptools-github/tree/master/graph/badge.svg?token=RANDOM123"
+    expected = "https://codecov.io/gh/cav71/setuptools-github/tree/{{ ctx.branch|urlquote }}/graph/badge.svg?token=RANDOM123"
+    assert tools.apply_fixers(txt, fixers) == expected
+
+    txt = "https://codecov.io/gh/cav71/setuptools-github/tree/master"
+    expected = (
+        "https://codecov.io/gh/cav71/setuptools-github/tree/{{ ctx.branch|urlquote }}"
+    )
+    assert tools.apply_fixers(txt, fixers) == expected
+
+
 def test_get_module_var(tmp_path):
     "pulls variables from a file"
     path = tmp_path / "in0.txt"
     path.write_text(
         """
 # a test file
 A = 12
@@ -338,50 +378,58 @@
     assert tools.get_module_var(repo.initfile) == "0.0.3"
     assert tools.get_module_var(repo.initfile, "__hash__") == "5547365c82"
     repo.revert(repo.initfile)
 
 
 def test_process(git_project_factory):
     def write_tfile(tfile):
-        tfile.write_text("""
+        tfile.write_text(
+            """
 {% for k, v in ctx.items() | sort -%}
 Key[{{k}}] = {{v}}
 {% endfor %}
-""")
+"""
+        )
         return tfile
 
     repo = git_project_factory().create("1.2.3")
 
     # tfile won't appear in the repo.status() because is untracked
     tfile = write_tfile(repo.workdir / "test.txt")
 
     data = tools.process(repo.initfile, None, tfile)
 
     assert data["hash"][-1] != "*"
 
-    assert tfile.read_text() == f"""
+    assert (
+        tfile.read_text()
+        == f"""
 Key[branch] = master
 Key[build] = 0
 Key[current] = 1.2.3
 Key[hash] = {data['hash']}
 Key[runid] = 0
 Key[version] = 1.2.3
 Key[workflow] = master
 """
+    )
 
     # clean and switch to new branch
     repo.revert(repo.initfile)
     write_tfile(tfile)
     repo.branch("beta/1.2.3", "master")
 
     data = tools.process(repo.initfile, None, tfile)
     assert data["hash"][-1] != "*"
 
-    assert tfile.read_text() == f"""
+    assert (
+        tfile.read_text()
+        == f"""
 Key[branch] = beta/1.2.3
 Key[build] = 0
 Key[current] = 1.2.3
 Key[hash] = {data['hash']}
 Key[runid] = 0
 Key[version] = 1.2.3b0
 Key[workflow] = beta
 """
+    )
```

