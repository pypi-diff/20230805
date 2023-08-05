# Comparing `tmp/devtools_cli-0.1.0.tar.gz` & `tmp/devtools_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devtools_cli-0.1.0.tar", max compression
+gzip compressed data, was "devtools_cli-0.1.1.tar", max compression
```

## Comparing `devtools_cli-0.1.0.tar` & `devtools_cli-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1074 2023-08-05 20:54:13.832603 devtools_cli-0.1.0/LICENSE
--rw-r--r--   0        0        0       95 2023-08-05 20:54:13.832603 devtools_cli-0.1.0/README.md
--rw-r--r--   0        0        0      294 2023-08-05 20:54:13.832603 devtools_cli-0.1.0/devtools_cli/__init__.py
--rw-r--r--   0        0        0      294 2023-08-05 20:54:13.832603 devtools_cli-0.1.0/devtools_cli/commands/__init__.py
--rw-r--r--   0        0        0      294 2023-08-05 20:54:13.832603 devtools_cli-0.1.0/devtools_cli/commands/info/__init__.py
--rw-r--r--   0        0        0     1724 2023-08-05 20:54:13.832603 devtools_cli-0.1.0/devtools_cli/commands/info/main.py
--rw-r--r--   0        0        0      294 2023-08-05 20:54:13.832603 devtools_cli-0.1.0/devtools_cli/commands/license/__init__.py
--rw-r--r--   0        0        0     8013 2023-08-05 20:54:13.832603 devtools_cli-0.1.0/devtools_cli/commands/license/header.py
--rw-r--r--   0        0        0    11012 2023-08-05 20:54:13.836603 devtools_cli-0.1.0/devtools_cli/commands/license/helpers.py
--rw-r--r--   0        0        0     7234 2023-08-05 20:54:13.836603 devtools_cli-0.1.0/devtools_cli/commands/license/main.py
--rw-r--r--   0        0        0     2347 2023-08-05 20:54:13.836603 devtools_cli-0.1.0/devtools_cli/commands/license/models.py
--rw-r--r--   0        0        0     1007 2023-08-05 20:54:13.836603 devtools_cli-0.1.0/devtools_cli/main.py
--rw-r--r--   0        0        0     1810 2023-08-05 20:54:13.836603 devtools_cli-0.1.0/devtools_cli/models.py
--rw-r--r--   0        0        0     8089 2023-08-05 20:54:13.836603 devtools_cli-0.1.0/devtools_cli/utils.py
--rw-r--r--   0        0        0     2254 2023-08-05 20:54:13.836603 devtools_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1542 1970-01-01 00:00:00.000000 devtools_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-08-05 21:08:32.815425 devtools_cli-0.1.1/LICENSE
+-rw-r--r--   0        0        0       95 2023-08-05 21:08:32.815425 devtools_cli-0.1.1/README.md
+-rw-r--r--   0        0        0      294 2023-08-05 21:08:32.815425 devtools_cli-0.1.1/devtools_cli/__init__.py
+-rw-r--r--   0        0        0      294 2023-08-05 21:08:32.815425 devtools_cli-0.1.1/devtools_cli/commands/__init__.py
+-rw-r--r--   0        0        0      294 2023-08-05 21:08:32.819424 devtools_cli-0.1.1/devtools_cli/commands/info/__init__.py
+-rw-r--r--   0        0        0     1724 2023-08-05 21:08:32.819424 devtools_cli-0.1.1/devtools_cli/commands/info/main.py
+-rw-r--r--   0        0        0      294 2023-08-05 21:08:32.819424 devtools_cli-0.1.1/devtools_cli/commands/license/__init__.py
+-rw-r--r--   0        0        0     8041 2023-08-05 21:08:32.819424 devtools_cli-0.1.1/devtools_cli/commands/license/header.py
+-rw-r--r--   0        0        0    11012 2023-08-05 21:08:32.819424 devtools_cli-0.1.1/devtools_cli/commands/license/helpers.py
+-rw-r--r--   0        0        0     7234 2023-08-05 21:08:32.819424 devtools_cli-0.1.1/devtools_cli/commands/license/main.py
+-rw-r--r--   0        0        0     2347 2023-08-05 21:08:32.819424 devtools_cli-0.1.1/devtools_cli/commands/license/models.py
+-rw-r--r--   0        0        0     1007 2023-08-05 21:08:32.819424 devtools_cli-0.1.1/devtools_cli/main.py
+-rw-r--r--   0        0        0     1810 2023-08-05 21:08:32.819424 devtools_cli-0.1.1/devtools_cli/models.py
+-rw-r--r--   0        0        0     8089 2023-08-05 21:08:32.819424 devtools_cli-0.1.1/devtools_cli/utils.py
+-rw-r--r--   0        0        0     2254 2023-08-05 21:08:32.819424 devtools_cli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1542 1970-01-01 00:00:00.000000 devtools_cli-0.1.1/PKG-INFO
```

### Comparing `devtools_cli-0.1.0/LICENSE` & `devtools_cli-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `devtools_cli-0.1.0/devtools_cli/commands/info/main.py` & `devtools_cli-0.1.1/devtools_cli/commands/info/main.py`

 * *Files identical despite different names*

### Comparing `devtools_cli-0.1.0/devtools_cli/commands/license/header.py` & `devtools_cli-0.1.1/devtools_cli/commands/license/header.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,14 +258,16 @@
 
 			if content[0].startswith(header.symbols.first):
 				end = 0
 				if header.symbols.identical:
 					for i, line in enumerate(content):
 						if line.startswith(header.symbols.first):
 							end += 1
+							continue
+						break
 				else:
 					for i, line in enumerate(content):
 						if line.startswith(header.symbols.last):
 							end += 1
 							break
 						elif (
 							line.startswith(header.symbols.middle) or
```

### Comparing `devtools_cli-0.1.0/devtools_cli/commands/license/helpers.py` & `devtools_cli-0.1.1/devtools_cli/commands/license/helpers.py`

 * *Files identical despite different names*

### Comparing `devtools_cli-0.1.0/devtools_cli/commands/license/main.py` & `devtools_cli-0.1.1/devtools_cli/commands/license/main.py`

 * *Files identical despite different names*

### Comparing `devtools_cli-0.1.0/devtools_cli/commands/license/models.py` & `devtools_cli-0.1.1/devtools_cli/commands/license/models.py`

 * *Files identical despite different names*

### Comparing `devtools_cli-0.1.0/devtools_cli/main.py` & `devtools_cli-0.1.1/devtools_cli/main.py`

 * *Files identical despite different names*

### Comparing `devtools_cli-0.1.0/devtools_cli/models.py` & `devtools_cli-0.1.1/devtools_cli/models.py`

 * *Files identical despite different names*

### Comparing `devtools_cli-0.1.0/devtools_cli/utils.py` & `devtools_cli-0.1.1/devtools_cli/utils.py`

 * *Files identical despite different names*

### Comparing `devtools_cli-0.1.0/pyproject.toml` & `devtools_cli-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "devtools-cli"
-version = "0.1.0"
+version = "0.1.1"
 description = "A toolbox of cross-language utility scripts for efficient software development."
 license = "MIT"
 authors = ["Mattias Aabmets <mattias.aabmets@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/aabmets/devtools-cli"
 keywords = ["toolbox", "cross-language", "utility", "scripts", "software", "development"]
 classifiers = [
```

### Comparing `devtools_cli-0.1.0/PKG-INFO` & `devtools_cli-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devtools-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: A toolbox of cross-language utility scripts for efficient software development.
 Home-page: https://github.com/aabmets/devtools-cli
 License: MIT
 Keywords: toolbox,cross-language,utility,scripts,software,development
 Author: Mattias Aabmets
 Author-email: mattias.aabmets@gmail.com
 Requires-Python: >=3.11,<4.0
```

