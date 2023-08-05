# Comparing `tmp/pytech_tools-0.1.1.tar.gz` & `tmp/pytech_tools-0.1.3.tar.gz`

## Comparing `pytech_tools-0.1.1.tar` & `pytech_tools-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytech_tools-0.1.1/pytech/datatypes/__init__.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 pytech_tools-0.1.1/pytech/datatypes/enums.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytech_tools-0.1.1/pytech/tools/__init__.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pytech_tools-0.1.1/pytech/tools/scheduler.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pytech_tools-0.1.1/.gitignore
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 pytech_tools-0.1.1/LICENCE
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pytech_tools-0.1.1/README.md
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pytech_tools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 pytech_tools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytech_tools-0.1.3/pytech/datatypes/__init__.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 pytech_tools-0.1.3/pytech/datatypes/enums.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytech_tools-0.1.3/pytech/tools/__init__.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pytech_tools-0.1.3/pytech/tools/scheduler.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pytech_tools-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 pytech_tools-0.1.3/LICENCE
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 pytech_tools-0.1.3/README.md
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pytech_tools-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 pytech_tools-0.1.3/PKG-INFO
```

### Comparing `pytech_tools-0.1.1/pytech/datatypes/enums.py` & `pytech_tools-0.1.3/pytech/datatypes/enums.py`

 * *Files identical despite different names*

### Comparing `pytech_tools-0.1.1/LICENCE` & `pytech_tools-0.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `pytech_tools-0.1.1/pyproject.toml` & `pytech_tools-0.1.3/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pytech-tools"
-version = "0.1.1"
+version = "0.1.3"
 authors = [
   { name="Alessandro Grandi", email="alessandro.grandi@pytech.it" },
 ]
 description = "PyTech Tools Project"
 readme = "README.md"
 dependencies = [
     "apscheduler>=3",
 ]
 requires-python = ">=3"
 classifiers = [
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.com/pytech-srl/resources/pytech-tools"
 "Bug Tracker" = "https://gitlab.com/pytech-srl/resources/pytech-tools/-/issues"
-
-[tool.ruff]
-select = [
-  "E",   # pycodestyle
-  "F",   # pyflakes
-  "UP",  # pyupgrade
-]
+"Documentation" = "https://pytech-srl.gitlab.io/resources/pytech-tools/"
```

### Comparing `pytech_tools-0.1.1/PKG-INFO` & `pytech_tools-0.1.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: pytech-tools
-Version: 0.1.1
+Version: 0.1.3
 Summary: PyTech Tools Project
 Project-URL: Homepage, https://gitlab.com/pytech-srl/resources/pytech-tools
 Project-URL: Bug Tracker, https://gitlab.com/pytech-srl/resources/pytech-tools/-/issues
+Project-URL: Documentation, https://pytech-srl.gitlab.io/resources/pytech-tools/
 Author-email: Alessandro Grandi <alessandro.grandi@pytech.it>
 License-File: LICENCE
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Requires-Dist: apscheduler>=3
 Description-Content-Type: text/markdown
 
 # PyTech Tools
 
 ## Description
-This project aims to provide tools to handle dynamic data structure conversions through rules definition.
-
-The goal is to be able to define rules to translate data structs that may be incomplete and miss data.
+This project aims to provide basic tools that may be useful in general purpose projects.
 
 ## Roadmap
 You may find some new features coming in the [Issue section](https://gitlab.com/pytech-srl/resources/pytech-tools/-/issues)
 
 ## Authors and acknowledgment
 This package is provided thanks to:
```

