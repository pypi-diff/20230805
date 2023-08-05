# Comparing `tmp/pytech_rules-0.0.3.tar.gz` & `tmp/pytech_rules-0.0.4.tar.gz`

## Comparing `pytech_rules-0.0.3.tar` & `pytech_rules-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytech_rules-0.0.3/pytech/rules/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pytech_rules-0.0.3/.gitignore
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 pytech_rules-0.0.3/LICENCE
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pytech_rules-0.0.3/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pytech_rules-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 pytech_rules-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytech_rules-0.0.4/pytech/rules/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pytech_rules-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 pytech_rules-0.0.4/LICENCE
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pytech_rules-0.0.4/README.md
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 pytech_rules-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 pytech_rules-0.0.4/PKG-INFO
```

### Comparing `pytech_rules-0.0.3/LICENCE` & `pytech_rules-0.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `pytech_rules-0.0.3/pyproject.toml` & `pytech_rules-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pytech-rules"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name = "Alessandro Grandi", email = "alessandro.grandi@pytech.it" },
 ]
 description = "PyTech Rules Project"
 readme = "README.md"
-dependencies = [
-]
+dependencies = []
 requires-python = ">=3"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
```

### Comparing `pytech_rules-0.0.3/PKG-INFO` & `pytech_rules-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytech-rules
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyTech Rules Project
 Project-URL: Homepage, https://gitlab.com/pytech-srl/resources/pytech-rules/
 Project-URL: Bug Tracker, https://gitlab.com/pytech-srl/resources/pytech-rules/-/issues
 Project-URL: Documentation, https://pytech-srl.gitlab.io/resources/pytech-rules/
 Author-email: Alessandro Grandi <alessandro.grandi@pytech.it>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
```

