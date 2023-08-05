# Comparing `tmp/poetry_plugin_dotenv-0.5.1.tar.gz` & `tmp/poetry_plugin_dotenv-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_dotenv-0.5.1.tar", max compression
+gzip compressed data, was "poetry_plugin_dotenv-0.5.2.tar", max compression
```

## Comparing `poetry_plugin_dotenv-0.5.1.tar` & `poetry_plugin_dotenv-0.5.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1077 2023-07-22 22:05:45.441478 poetry_plugin_dotenv-0.5.1/LICENSE
--rw-r--r--   0        0        0     8943 2023-07-22 22:05:45.441478 poetry_plugin_dotenv-0.5.1/README.md
--rw-r--r--   0        0        0     5721 2023-07-22 22:05:45.445478 poetry_plugin_dotenv-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      699 2023-07-22 22:05:45.445478 poetry_plugin_dotenv-0.5.1/src/poetry_plugin_dotenv/__init__.py
--rw-r--r--   0        0        0      335 2023-07-22 22:05:45.445478 poetry_plugin_dotenv-0.5.1/src/poetry_plugin_dotenv/dotenv/__init__.py
--rw-r--r--   0        0        0     5235 2023-07-22 22:05:45.445478 poetry_plugin_dotenv-0.5.1/src/poetry_plugin_dotenv/dotenv/core.py
--rw-r--r--   0        0        0     5983 2023-07-22 22:05:45.445478 poetry_plugin_dotenv-0.5.1/src/poetry_plugin_dotenv/dotenv/parsers.py
--rw-r--r--   0        0        0     1445 2023-07-22 22:05:45.445478 poetry_plugin_dotenv-0.5.1/src/poetry_plugin_dotenv/dotenv/variables.py
--rw-r--r--   0        0        0     3469 2023-07-22 22:05:45.445478 poetry_plugin_dotenv-0.5.1/src/poetry_plugin_dotenv/plugin.py
--rw-r--r--   0        0        0        0 2023-07-22 22:05:45.445478 poetry_plugin_dotenv-0.5.1/src/poetry_plugin_dotenv/py.typed
--rw-r--r--   0        0        0    10880 1970-01-01 00:00:00.000000 poetry_plugin_dotenv-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-08-05 15:05:16.845614 poetry_plugin_dotenv-0.5.2/LICENSE
+-rw-r--r--   0        0        0     8970 2023-08-05 15:05:16.845614 poetry_plugin_dotenv-0.5.2/README.md
+-rw-r--r--   0        0        0     5727 2023-08-05 15:05:43.365590 poetry_plugin_dotenv-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      699 2023-08-05 15:05:16.849614 poetry_plugin_dotenv-0.5.2/src/poetry_plugin_dotenv/__init__.py
+-rw-r--r--   0        0        0      335 2023-08-05 15:05:16.849614 poetry_plugin_dotenv-0.5.2/src/poetry_plugin_dotenv/dotenv/__init__.py
+-rw-r--r--   0        0        0     5235 2023-08-05 15:05:16.849614 poetry_plugin_dotenv-0.5.2/src/poetry_plugin_dotenv/dotenv/core.py
+-rw-r--r--   0        0        0     5983 2023-08-05 15:05:16.849614 poetry_plugin_dotenv-0.5.2/src/poetry_plugin_dotenv/dotenv/parsers.py
+-rw-r--r--   0        0        0     1445 2023-08-05 15:05:16.849614 poetry_plugin_dotenv-0.5.2/src/poetry_plugin_dotenv/dotenv/variables.py
+-rw-r--r--   0        0        0     3469 2023-08-05 15:05:16.849614 poetry_plugin_dotenv-0.5.2/src/poetry_plugin_dotenv/plugin.py
+-rw-r--r--   0        0        0        0 2023-08-05 15:05:16.849614 poetry_plugin_dotenv-0.5.2/src/poetry_plugin_dotenv/py.typed
+-rw-r--r--   0        0        0    10907 1970-01-01 00:00:00.000000 poetry_plugin_dotenv-0.5.2/PKG-INFO
```

### Comparing `poetry_plugin_dotenv-0.5.1/LICENSE` & `poetry_plugin_dotenv-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-0.5.1/README.md` & `poetry_plugin_dotenv-0.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,20 @@
 - [⚙️ Installation](#️-installation)
 - [👩🏻‍💻 Usage](#-usage)
 
 # 🔮 Overview
 
 `poetry-plugin-dotenv` - is the plugin that automatically loads environment variables from a dotenv file into the environment before `poetry` commands are run.
 
-**This plugin doesn't have any dependencies, but therefore it also supports features that `python-dotenv` supports (e.g. templates, interpolating variables using `POSIX` variable expansions etc).**
+**Features**
+
+- 📦 Doesn't require any dependencies
+- 📝 Supports templates, interpolating variables using POSIX variable expansions
+- 🔮 Fully type safe
+- 🥷🏻 100% tests coverage and "A" grade for maintainability
 
 # ⚙️ Installation
 
 ```bash
 poetry self add poetry-plugin-dotenv
 ```
```

#### html2text {}

```diff
@@ -4,22 +4,22 @@
           [dependabot] [CI] [CD] [CodeQL] [Dependency_Review] [wheel]
             [coverage] [codeclimate] [downloads] [stars] [wakatime]
               [issues] [issues] [pr] [pr] [contributors] [commit]
              [buymeacoffee] [standwithukraine] [standwithukraine]
 - [ð® Overview](#-overview) - [âï¸ Installation](#ï¸-installation) -
 [ð©ð»âð» Usage](#-usage) # ð® Overview `poetry-plugin-dotenv` - is
 the plugin that automatically loads environment variables from a dotenv file
-into the environment before `poetry` commands are run. **This plugin doesn't
-have any dependencies, but therefore it also supports features that `python-
-dotenv` supports (e.g. templates, interpolating variables using `POSIX`
-variable expansions etc).** # âï¸ Installation ```bash poetry self add
-poetry-plugin-dotenv ``` # ð©ð»âð» Usage By default, plugin will load
-the `.env` file from the current working directory or "higher directories". To
-prevent ``poetry`` from loading the dotenv file, set the
-``POETRY_DONT_LOAD_DOTENV`` environment variable. If your dotenv file is
+into the environment before `poetry` commands are run. **Features** - ð¦
+Doesn't require any dependencies - ð Supports templates, interpolating
+variables using POSIX variable expansions - ð® Fully type safe - ð¥·ð»
+100% tests coverage and "A" grade for maintainability # âï¸ Installation
+```bash poetry self add poetry-plugin-dotenv ``` # ð©ð»âð» Usage By
+default, plugin will load the `.env` file from the current working directory or
+"higher directories". To prevent ``poetry`` from loading the dotenv file, set
+the ``POETRY_DONT_LOAD_DOTENV`` environment variable. If your dotenv file is
 located in a different path or has a different name you may set the
 ``POETRY_DOTENV_LOCATION`` environment variable. [logo] ```dotenv # .env
 DB__HOST=localhost DB__DBNAME=prod DB__USER=admin DB__PASSWORD=admin
 DB__ENGINE=postgresql://${DB__USER}:${DB__PASSWORD}@${DB__HOST}/${DB__DBNAME}
 ``` ```dotenv # .env.dev DB__HOST=localhost DB__DBNAME=dev DB__USER=root
 DB__PASSWORD=root DB__ENGINE=postgresql://${DB__USER}:${DB__PASSWORD}@$
 {DB__HOST}/${DB__DBNAME} ``` ```python # main.py import os if __name__ ==
```

### Comparing `poetry_plugin_dotenv-0.5.1/pyproject.toml` & `poetry_plugin_dotenv-0.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-dotenv"
-version = "0.5.1"
+version = "0.5.2"
 description = "poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."
 license = "MIT"
 authors = ["Volodymyr Pivoshenko <volodymyr.pivoshenko@gmail.com>"]
 maintainers = ["Volodymyr Pivoshenko <volodymyr.pivoshenko@gmail.com>"]
 keywords = [
     "python",
     "pypi",
@@ -62,15 +62,15 @@
 isort = "^5.12.0"
 black = "^23.3.0"
 pyupgrade = "^3.7.0"
 yesqa = "^1.5.0"
 
 [tool.poetry.group.linters.dependencies]
 mypy = "^1.4.0"
-ruff = "^0.0.275"
+ruff = ">=0.0.275,<0.0.281"
 deptry = "^0.12.0"
 memestra = "^0.2.1"
 codespell = "^2.2.5"
 
 [tool.poetry.group.tests.dependencies]
 pytest = "^7.4.0"
 xdoctest = "^1.1.1"
@@ -159,17 +159,18 @@
 order-by-type = false
 force-single-line = true
 force-sort-within-sections = true
 required-imports = ["from __future__ import annotations"]
 
 [tool.codespell]
 skip = "tests,pyproject.toml,poetry.lock,.git,.mypy_cache,.pytest_cache,.idea,.vscode"
+ignore-words-list="redunant"
 
 [tool.deptry]
-ignore_transitive = ["cleo", "poetry_plugin_dotenv"]
+ignore = ["DEP003"]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = ["src", "tests"]
 addopts = [
     "-l",
     "-vv",
```

### Comparing `poetry_plugin_dotenv-0.5.1/src/poetry_plugin_dotenv/__init__.py` & `poetry_plugin_dotenv-0.5.2/src/poetry_plugin_dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-0.5.1/src/poetry_plugin_dotenv/dotenv/core.py` & `poetry_plugin_dotenv-0.5.2/src/poetry_plugin_dotenv/dotenv/core.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-0.5.1/src/poetry_plugin_dotenv/dotenv/parsers.py` & `poetry_plugin_dotenv-0.5.2/src/poetry_plugin_dotenv/dotenv/parsers.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-0.5.1/src/poetry_plugin_dotenv/dotenv/variables.py` & `poetry_plugin_dotenv-0.5.2/src/poetry_plugin_dotenv/dotenv/variables.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-0.5.1/src/poetry_plugin_dotenv/plugin.py` & `poetry_plugin_dotenv-0.5.2/src/poetry_plugin_dotenv/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-0.5.1/PKG-INFO` & `poetry_plugin_dotenv-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-dotenv
-Version: 0.5.1
+Version: 0.5.2
 Summary: poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run.
 Home-page: https://github.com/volopivoshenko/poetry-plugin-dotenv
 License: MIT
 Keywords: python,pypi,poetry,plugin,plugins,poetry-plugin,poetry-plugins,env,dotenv,cross-platform,hacktoberfest
 Author: Volodymyr Pivoshenko
 Author-email: volodymyr.pivoshenko@gmail.com
 Maintainer: Volodymyr Pivoshenko
@@ -153,15 +153,20 @@
 - [⚙️ Installation](#️-installation)
 - [👩🏻‍💻 Usage](#-usage)
 
 # 🔮 Overview
 
 `poetry-plugin-dotenv` - is the plugin that automatically loads environment variables from a dotenv file into the environment before `poetry` commands are run.
 
-**This plugin doesn't have any dependencies, but therefore it also supports features that `python-dotenv` supports (e.g. templates, interpolating variables using `POSIX` variable expansions etc).**
+**Features**
+
+- 📦 Doesn't require any dependencies
+- 📝 Supports templates, interpolating variables using POSIX variable expansions
+- 🔮 Fully type safe
+- 🥷🏻 100% tests coverage and "A" grade for maintainability
 
 # ⚙️ Installation
 
 ```bash
 poetry self add poetry-plugin-dotenv
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poetry-plugin-dotenv Version: 0.5.1 Summary:
+Metadata-Version: 2.1 Name: poetry-plugin-dotenv Version: 0.5.2 Summary:
 poetry-plugin-dotenv - is the plugin that automatically loads environment
 variables from a dotenv file into the environment before poetry commands are
 run. Home-page: https://github.com/volopivoshenko/poetry-plugin-dotenv License:
 MIT Keywords: python,pypi,poetry,plugin,plugins,poetry-plugin,poetry-
 plugins,env,dotenv,cross-platform,hacktoberfest Author: Volodymyr Pivoshenko
 Author-email: volodymyr.pivoshenko@gmail.com Maintainer: Volodymyr Pivoshenko
 Maintainer-email: volodymyr.pivoshenko@gmail.com Requires-Python: >=3.8.1,<4.0
@@ -30,22 +30,22 @@
           [dependabot] [CI] [CD] [CodeQL] [Dependency_Review] [wheel]
             [coverage] [codeclimate] [downloads] [stars] [wakatime]
               [issues] [issues] [pr] [pr] [contributors] [commit]
              [buymeacoffee] [standwithukraine] [standwithukraine]
 - [ð® Overview](#-overview) - [âï¸ Installation](#ï¸-installation) -
 [ð©ð»âð» Usage](#-usage) # ð® Overview `poetry-plugin-dotenv` - is
 the plugin that automatically loads environment variables from a dotenv file
-into the environment before `poetry` commands are run. **This plugin doesn't
-have any dependencies, but therefore it also supports features that `python-
-dotenv` supports (e.g. templates, interpolating variables using `POSIX`
-variable expansions etc).** # âï¸ Installation ```bash poetry self add
-poetry-plugin-dotenv ``` # ð©ð»âð» Usage By default, plugin will load
-the `.env` file from the current working directory or "higher directories". To
-prevent ``poetry`` from loading the dotenv file, set the
-``POETRY_DONT_LOAD_DOTENV`` environment variable. If your dotenv file is
+into the environment before `poetry` commands are run. **Features** - ð¦
+Doesn't require any dependencies - ð Supports templates, interpolating
+variables using POSIX variable expansions - ð® Fully type safe - ð¥·ð»
+100% tests coverage and "A" grade for maintainability # âï¸ Installation
+```bash poetry self add poetry-plugin-dotenv ``` # ð©ð»âð» Usage By
+default, plugin will load the `.env` file from the current working directory or
+"higher directories". To prevent ``poetry`` from loading the dotenv file, set
+the ``POETRY_DONT_LOAD_DOTENV`` environment variable. If your dotenv file is
 located in a different path or has a different name you may set the
 ``POETRY_DOTENV_LOCATION`` environment variable. [logo] ```dotenv # .env
 DB__HOST=localhost DB__DBNAME=prod DB__USER=admin DB__PASSWORD=admin
 DB__ENGINE=postgresql://${DB__USER}:${DB__PASSWORD}@${DB__HOST}/${DB__DBNAME}
 ``` ```dotenv # .env.dev DB__HOST=localhost DB__DBNAME=dev DB__USER=root
 DB__PASSWORD=root DB__ENGINE=postgresql://${DB__USER}:${DB__PASSWORD}@$
 {DB__HOST}/${DB__DBNAME} ``` ```python # main.py import os if __name__ ==
```

