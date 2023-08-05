# Comparing `tmp/creart-0.2.2.tar.gz` & `tmp/creart-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creart-0.2.2.tar", last modified: Fri Aug 26 09:48:11 2022, max compression
+gzip compressed data, was "creart-0.3.0.tar", last modified: Sat Aug  5 09:46:14 2023, max compression
```

## Comparing `creart-0.2.2.tar` & `creart-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-08-26 09:47:52.913145 creart-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-26 09:47:52.913145 creart-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     2952 2022-08-26 09:47:52.913145 creart-0.2.2/creart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1148 2022-08-26 09:47:52.913145 creart-0.2.2/creart/creator.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-26 09:47:52.913145 creart-0.2.2/creart/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-08-26 09:47:52.913145 creart-0.2.2/pyproject.toml
--rw-------   0 runner    (1001) docker     (121)      299 2022-08-26 09:48:11.565497 creart-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-05 09:46:01.927530 creart-0.3.0/LICENSE
+-rw-r--r--   0        0        0       61 2023-08-05 09:46:01.927530 creart-0.3.0/README.md
+-rw-r--r--   0        0        0     3237 2023-08-05 09:46:01.927530 creart-0.3.0/creart/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 09:46:01.927530 creart-0.3.0/creart/builtins/__init__.py
+-rw-r--r--   0        0        0      875 2023-08-05 09:46:01.927530 creart-0.3.0/creart/builtins/loop.py
+-rw-r--r--   0        0        0     1148 2023-08-05 09:46:01.927530 creart-0.3.0/creart/creator.py
+-rw-r--r--   0        0        0        0 2023-08-05 09:46:01.927530 creart-0.3.0/creart/py.typed
+-rw-r--r--   0        0        0      664 2023-08-05 09:46:14.176204 creart-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      337 1970-01-01 00:00:00.000000 creart-0.3.0/PKG-INFO
```

### Comparing `creart-0.2.2/LICENSE` & `creart-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `creart-0.2.2/creart/__init__.py` & `creart-0.3.0/creart/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,25 @@
 _mapping: dict[str, type[AbstractCreator]] = {}
 
 T = TypeVar("T")
 
 
 def _env_scan():
     for entry in entry_points().select(group="creart.creators"):
-        creator = entry.load()
+        try:
+            creator = entry.load()
+        except ImportError:
+            import warnings
+
+            warnings.warn(
+                f"error throwed when creart attempt to import {entry}"
+                "please check your environment and report this problem."
+            )
+            continue
+
         if creator.available():
             add_creator(creator)
 
 
 def add_creator(creator: type[AbstractCreator]):
     intersection = {f"{i.module}:{i.identify}" for i in creator.targets}.intersection(_mapping.keys())
     if intersection:
@@ -95,9 +105,9 @@
             raise TypeError(f"no supported mixin for {type(target)}")
 
     return wrapper
 
 
 it = create
 
-if os.getenv("CREART_AUTO_SCAN") not in {"false", "False", "0", "no", "off"}:
+if os.getenv("CREART_AUTO_SCAN", "") not in {"false", "False", "0", "no", "off"}:
     _env_scan()
```

### Comparing `creart-0.2.2/creart/creator.py` & `creart-0.3.0/creart/creator.py`

 * *Files identical despite different names*

### Comparing `creart-0.2.2/pyproject.toml` & `creart-0.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "creart"
-version = "0.2.2"
+version = "0.3.0"
 description = "a universal, extensible class instantiation helper"
 authors = [
     { name = "GreyElaina", email = "GreyElaina@outlook.com" },
 ]
 dependencies = [
     "importlib-metadata>=3.6",
 ]
@@ -12,24 +12,27 @@
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 
+[project.entry-points."creart.creators"]
+loop = "creart.builtins.loop:EventLoopCreator"
+
 [tool.pdm.dev-dependencies]
 dev = [
     "black>=22.3.0",
     "isort>=5.10.1",
 ]
 
 [tool.black]
 line-length = 120
 
 [tool.isort]
 profile = "black"
 
 [build-system]
 requires = [
-    "pdm-pep517>=0.12.0",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
```

