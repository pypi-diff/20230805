# Comparing `tmp/pytech_sqlalchemy_tools-0.1.2.tar.gz` & `tmp/pytech_sqlalchemy_tools-0.1.3.tar.gz`

## Comparing `pytech_sqlalchemy_tools-0.1.2.tar` & `pytech_sqlalchemy_tools-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytech_sqlalchemy_tools-0.1.2/pytech/sqlalchemy_tools/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 pytech_sqlalchemy_tools-0.1.2/pytech/sqlalchemy_tools/models.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pytech_sqlalchemy_tools-0.1.2/pytech/sqlalchemy_tools/services/__init__.py
--rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 pytech_sqlalchemy_tools-0.1.2/pytech/sqlalchemy_tools/services/build.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 pytech_sqlalchemy_tools-0.1.2/pytech/sqlalchemy_tools/services/retrieve.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pytech_sqlalchemy_tools-0.1.2/.gitignore
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 pytech_sqlalchemy_tools-0.1.2/LICENCE
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytech_sqlalchemy_tools-0.1.2/README.md
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 pytech_sqlalchemy_tools-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pytech_sqlalchemy_tools-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytech_sqlalchemy_tools-0.1.3/pytech/sqlalchemy_tools/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 pytech_sqlalchemy_tools-0.1.3/pytech/sqlalchemy_tools/models.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pytech_sqlalchemy_tools-0.1.3/pytech/sqlalchemy_tools/services/__init__.py
+-rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 pytech_sqlalchemy_tools-0.1.3/pytech/sqlalchemy_tools/services/build.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 pytech_sqlalchemy_tools-0.1.3/pytech/sqlalchemy_tools/services/retrieve.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pytech_sqlalchemy_tools-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 pytech_sqlalchemy_tools-0.1.3/LICENCE
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 pytech_sqlalchemy_tools-0.1.3/README.md
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 pytech_sqlalchemy_tools-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pytech_sqlalchemy_tools-0.1.3/PKG-INFO
```

### Comparing `pytech_sqlalchemy_tools-0.1.2/pytech/sqlalchemy_tools/services/build.py` & `pytech_sqlalchemy_tools-0.1.3/pytech/sqlalchemy_tools/services/build.py`

 * *Files identical despite different names*

### Comparing `pytech_sqlalchemy_tools-0.1.2/pytech/sqlalchemy_tools/services/retrieve.py` & `pytech_sqlalchemy_tools-0.1.3/pytech/sqlalchemy_tools/services/retrieve.py`

 * *Files identical despite different names*

### Comparing `pytech_sqlalchemy_tools-0.1.2/LICENCE` & `pytech_sqlalchemy_tools-0.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `pytech_sqlalchemy_tools-0.1.2/PKG-INFO` & `pytech_sqlalchemy_tools-0.1.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 Metadata-Version: 2.1
 Name: pytech-sqlalchemy-tools
-Version: 0.1.2
+Version: 0.1.3
 Summary: PyTech SQLAlchemy Tools Project
 Project-URL: Homepage, https://gitlab.com/pytech-srl/resources/pytech-sqlalchemy-tools
 Project-URL: Bug Tracker, https://gitlab.com/pytech-srl/resources/pytech-sqlalchemy-tools/-/issues
 Author-email: Alessandro Grandi <alessandro.grandi@pytech.it>
 License-File: LICENCE
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Requires-Dist: pytech-tools<0.2,>=0.1.3
 Requires-Dist: sqlalchemy==2.0.19
 Description-Content-Type: text/markdown
 
 # PyTech SQLAlchemy Tools
 
-Example package.
+## Description
+This project aims to provide basic tools to interact with SQL Alchemy.
+
+## Roadmap
+You may find some new features coming in the [Issue section](https://gitlab.com/pytech-srl/resources/pytech-sqlalchemy-tools/-/issues)
+
+## Authors and acknowledgment
+This package is provided thanks to:
+
+- Alessandro Grandi (PyTech srl)
```

