# Comparing `tmp/example_package_linar2-0.0.1.tar.gz` & `tmp/example_package_linar2-0.1.1.tar.gz`

## Comparing `example_package_linar2-0.0.1.tar` & `example_package_linar2-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 example_package_linar2-0.0.1/src/example_package_linar2/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 example_package_linar2-0.0.1/src/example_package_linar2/example.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 example_package_linar2-0.0.1/LICENSE
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 example_package_linar2-0.0.1/README.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 example_package_linar2-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 example_package_linar2-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 example_package_linar2-0.1.1/src/example_package_linar2/__init__.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 example_package_linar2-0.1.1/src/example_package_linar2/example.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 example_package_linar2-0.1.1/LICENSE
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 example_package_linar2-0.1.1/README.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 example_package_linar2-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 example_package_linar2-0.1.1/PKG-INFO
```

### Comparing `example_package_linar2-0.0.1/LICENSE` & `example_package_linar2-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `example_package_linar2-0.0.1/pyproject.toml` & `example_package_linar2-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "example_package_linar2"
-version = "0.0.1"
+version = "0.1.1"
 authors = [
   { name="Linar Sharifullin"},
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

