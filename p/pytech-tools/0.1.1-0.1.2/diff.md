# Comparing `tmp/pytech_tools-0.1.1.tar.gz` & `tmp/pytech_tools-0.1.2.tar.gz`

## Comparing `pytech_tools-0.1.1.tar` & `pytech_tools-0.1.2.tar`

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
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytech_tools-0.1.2/pytech/datatypes/__init__.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 pytech_tools-0.1.2/pytech/datatypes/enums.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytech_tools-0.1.2/pytech/tools/__init__.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pytech_tools-0.1.2/pytech/tools/scheduler.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pytech_tools-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 pytech_tools-0.1.2/LICENCE
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pytech_tools-0.1.2/README.md
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pytech_tools-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 pytech_tools-0.1.2/PKG-INFO
```

### Comparing `pytech_tools-0.1.1/pytech/datatypes/enums.py` & `pytech_tools-0.1.2/pytech/datatypes/enums.py`

 * *Files identical despite different names*

### Comparing `pytech_tools-0.1.1/LICENCE` & `pytech_tools-0.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `pytech_tools-0.1.1/PKG-INFO` & `pytech_tools-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: pytech-tools
-Version: 0.1.1
+Version: 0.1.2
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
```

