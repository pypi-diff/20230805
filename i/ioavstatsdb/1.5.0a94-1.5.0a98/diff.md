# Comparing `tmp/ioavstatsdb-1.5.0a94.tar.gz` & `tmp/ioavstatsdb-1.5.0a98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ioavstatsdb-1.5.0a94.tar", last modified: Sat Aug  5 12:37:04 2023, max compression
+gzip compressed data, was "ioavstatsdb-1.5.0a98.tar", last modified: Sat Aug  5 13:46:44 2023, max compression
```

## Comparing `ioavstatsdb-1.5.0a94.tar` & `ioavstatsdb-1.5.0a98.tar`

### file list

```diff
@@ -1,26 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 12:37:04.017115 ioavstatsdb-1.5.0a94/
--rw-rw-rw-   0        0        0     4170 2022-11-08 06:32:14.000000 ioavstatsdb-1.5.0a94/LICENSE.md
--rw-rw-rw-   0        0        0     7145 2023-08-05 12:37:04.017115 ioavstatsdb-1.5.0a94/PKG-INFO
--rw-rw-rw-   0        0        0     6013 2023-04-21 12:07:40.000000 ioavstatsdb-1.5.0a94/README.md
-drwxrwxrwx   0        0        0        0 2023-08-05 12:37:04.008116 ioavstatsdb-1.5.0a94/ioavstatsdb/
--rw-rw-rw-   0        0        0      165 2023-08-05 09:34:22.000000 ioavstatsdb-1.5.0a94/ioavstatsdb/__init__.py
--rw-rw-rw-   0        0        0    24538 2023-08-04 15:15:43.000000 ioavstatsdb-1.5.0a94/ioavstatsdb/avstats.py
--rw-rw-rw-   0        0        0     7150 2023-02-20 06:02:34.000000 ioavstatsdb-1.5.0a94/ioavstatsdb/code_generator.py
--rw-rw-rw-   0        0        0   181917 2023-04-29 03:25:19.000000 ioavstatsdb-1.5.0a94/ioavstatsdb/db_ddl_base.py
--rw-rw-rw-   0        0        0   206534 2023-08-04 02:28:33.000000 ioavstatsdb-1.5.0a94/ioavstatsdb/db_dml_base.py
--rw-rw-rw-   0        0        0    43648 2023-04-21 12:07:40.000000 ioavstatsdb-1.5.0a94/ioavstatsdb/db_dml_corr.py
--rw-rw-rw-   0        0        0     7766 2023-08-04 03:05:09.000000 ioavstatsdb-1.5.0a94/ioavstatsdb/db_utils.py
--rw-rw-rw-   0        0        0      435 2023-02-20 06:02:34.000000 ioavstatsdb-1.5.0a94/ioavstatsdb/io_config.py
--rw-rw-rw-   0        0        0    14122 2023-08-05 02:31:50.000000 ioavstatsdb-1.5.0a94/ioavstatsdb/io_glob.py
--rw-rw-rw-   0        0        0     5633 2023-02-20 06:02:33.000000 ioavstatsdb-1.5.0a94/ioavstatsdb/io_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-05 12:37:04.013116 ioavstatsdb-1.5.0a94/ioavstatsdb.egg-info/
--rw-rw-rw-   0        0        0     7145 2023-08-05 12:37:03.000000 ioavstatsdb-1.5.0a94/ioavstatsdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      498 2023-08-05 12:37:03.000000 ioavstatsdb-1.5.0a94/ioavstatsdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 12:37:03.000000 ioavstatsdb-1.5.0a94/ioavstatsdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-08-05 12:37:03.000000 ioavstatsdb-1.5.0a94/ioavstatsdb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1822 2023-08-05 12:25:55.000000 ioavstatsdb-1.5.0a94/pyproject.toml
--rw-rw-rw-   0        0        0      226 2023-08-05 12:37:04.019115 ioavstatsdb-1.5.0a94/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-05 12:37:04.016117 ioavstatsdb-1.5.0a94/tests/
--rw-rw-rw-   0        0        0      165 2023-08-04 19:41:42.000000 ioavstatsdb-1.5.0a94/tests/__init__.py
--rw-rw-rw-   0        0        0     6701 2023-08-05 02:54:01.000000 ioavstatsdb-1.5.0a94/tests/conftest.py
--rw-rw-rw-   0        0        0    13964 2023-08-05 02:54:01.000000 ioavstatsdb-1.5.0a94/tests/test_launcher.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:46:44.471929 ioavstatsdb-1.5.0a98/
+-rw-rw-rw-   0        0        0     4170 2022-11-08 06:32:14.000000 ioavstatsdb-1.5.0a98/LICENSE.md
+-rw-rw-rw-   0        0        0     7145 2023-08-05 13:46:44.471929 ioavstatsdb-1.5.0a98/PKG-INFO
+-rw-rw-rw-   0        0        0     6013 2023-04-21 12:07:40.000000 ioavstatsdb-1.5.0a98/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 13:46:44.467217 ioavstatsdb-1.5.0a98/ioavstatsdb/
+-rw-rw-rw-   0        0        0      165 2023-08-05 09:34:22.000000 ioavstatsdb-1.5.0a98/ioavstatsdb/__init__.py
+-rw-rw-rw-   0        0        0      165 2023-04-03 12:20:18.000000 ioavstatsdb-1.5.0a98/ioavstatsdb/__init__.pyi
+-rw-rw-rw-   0        0        0    24538 2023-08-04 15:15:43.000000 ioavstatsdb-1.5.0a98/ioavstatsdb/avstats.py
+-rw-rw-rw-   0        0        0     1527 2023-04-21 12:07:40.000000 ioavstatsdb-1.5.0a98/ioavstatsdb/avstats.pyi
+-rw-rw-rw-   0        0        0     7150 2023-02-20 06:02:34.000000 ioavstatsdb-1.5.0a98/ioavstatsdb/code_generator.py
+-rw-rw-rw-   0        0        0      265 2023-02-20 06:02:34.000000 ioavstatsdb-1.5.0a98/ioavstatsdb/code_generator.pyi
+-rw-rw-rw-   0        0        0   181917 2023-04-29 03:25:19.000000 ioavstatsdb-1.5.0a98/ioavstatsdb/db_ddl_base.py
+-rw-rw-rw-   0        0        0   206534 2023-08-04 02:28:33.000000 ioavstatsdb-1.5.0a98/ioavstatsdb/db_dml_base.py
+-rw-rw-rw-   0        0        0    43648 2023-04-21 12:07:40.000000 ioavstatsdb-1.5.0a98/ioavstatsdb/db_dml_corr.py
+-rw-rw-rw-   0        0        0     7766 2023-08-04 03:05:09.000000 ioavstatsdb-1.5.0a98/ioavstatsdb/db_utils.py
+-rw-rw-rw-   0        0        0      670 2023-08-04 06:32:37.000000 ioavstatsdb-1.5.0a98/ioavstatsdb/db_utils.pyi
+-rw-rw-rw-   0        0        0      435 2023-02-20 06:02:34.000000 ioavstatsdb-1.5.0a98/ioavstatsdb/io_config.py
+-rw-rw-rw-   0        0        0    14122 2023-08-05 02:31:50.000000 ioavstatsdb-1.5.0a98/ioavstatsdb/io_glob.py
+-rw-rw-rw-   0        0        0     5328 2023-07-31 18:14:14.000000 ioavstatsdb-1.5.0a98/ioavstatsdb/io_glob.pyi
+-rw-rw-rw-   0        0        0     5633 2023-02-20 06:02:33.000000 ioavstatsdb-1.5.0a98/ioavstatsdb/io_utils.py
+-rw-rw-rw-   0        0        0      554 2023-02-20 06:02:33.000000 ioavstatsdb-1.5.0a98/ioavstatsdb/io_utils.pyi
+drwxrwxrwx   0        0        0        0 2023-08-05 13:46:44.469926 ioavstatsdb-1.5.0a98/ioavstatsdb.egg-info/
+-rw-rw-rw-   0        0        0     7145 2023-08-05 13:46:44.000000 ioavstatsdb-1.5.0a98/ioavstatsdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      652 2023-08-05 13:46:44.000000 ioavstatsdb-1.5.0a98/ioavstatsdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 13:46:44.000000 ioavstatsdb-1.5.0a98/ioavstatsdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-05 13:46:44.000000 ioavstatsdb-1.5.0a98/ioavstatsdb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1881 2023-08-05 13:46:12.000000 ioavstatsdb-1.5.0a98/pyproject.toml
+-rw-rw-rw-   0        0        0      226 2023-08-05 13:46:44.472926 ioavstatsdb-1.5.0a98/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-05 13:46:44.470929 ioavstatsdb-1.5.0a98/tests/
+-rw-rw-rw-   0        0        0      165 2023-08-04 19:41:42.000000 ioavstatsdb-1.5.0a98/tests/__init__.py
+-rw-rw-rw-   0        0        0     6701 2023-08-05 02:54:01.000000 ioavstatsdb-1.5.0a98/tests/conftest.py
+-rw-rw-rw-   0        0        0    13964 2023-08-05 02:54:01.000000 ioavstatsdb-1.5.0a98/tests/test_launcher.py
```

### Comparing `ioavstatsdb-1.5.0a94/LICENSE.md` & `ioavstatsdb-1.5.0a98/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ioavstatsdb-1.5.0a94/PKG-INFO` & `ioavstatsdb-1.5.0a98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ioavstatsdb
-Version: 1.5.0a94
+Version: 1.5.0a98
 Summary: Aviation Event Statistics - Database Software
 Author-email: Team IO-Aero <info@io-aero.com>
 Maintainer-email: Team IO-Aero <info@io-aero.ch>
 Project-URL: Bug Tracker, https://github.com/io-aero/io-avstats-db/issues
 Project-URL: Documentation, https://io-aero.github.io/io-avstats-db/
 Project-URL: Homepage, https://github.com/io-aero/io-avstats-db
 Project-URL: Release History, https://io-aero.github.io/io-avstats-db/release_history/
```

### Comparing `ioavstatsdb-1.5.0a94/README.md` & `ioavstatsdb-1.5.0a98/README.md`

 * *Files identical despite different names*

### Comparing `ioavstatsdb-1.5.0a94/ioavstatsdb/avstats.py` & `ioavstatsdb-1.5.0a98/ioavstatsdb/avstats.py`

 * *Files identical despite different names*

### Comparing `ioavstatsdb-1.5.0a94/ioavstatsdb/code_generator.py` & `ioavstatsdb-1.5.0a98/ioavstatsdb/code_generator.py`

 * *Files identical despite different names*

### Comparing `ioavstatsdb-1.5.0a94/ioavstatsdb/db_ddl_base.py` & `ioavstatsdb-1.5.0a98/ioavstatsdb/db_ddl_base.py`

 * *Files identical despite different names*

### Comparing `ioavstatsdb-1.5.0a94/ioavstatsdb/db_dml_base.py` & `ioavstatsdb-1.5.0a98/ioavstatsdb/db_dml_base.py`

 * *Files identical despite different names*

### Comparing `ioavstatsdb-1.5.0a94/ioavstatsdb/db_dml_corr.py` & `ioavstatsdb-1.5.0a98/ioavstatsdb/db_dml_corr.py`

 * *Files identical despite different names*

### Comparing `ioavstatsdb-1.5.0a94/ioavstatsdb/db_utils.py` & `ioavstatsdb-1.5.0a98/ioavstatsdb/db_utils.py`

 * *Files identical despite different names*

### Comparing `ioavstatsdb-1.5.0a94/ioavstatsdb/io_glob.py` & `ioavstatsdb-1.5.0a98/ioavstatsdb/io_glob.py`

 * *Files identical despite different names*

### Comparing `ioavstatsdb-1.5.0a94/ioavstatsdb/io_utils.py` & `ioavstatsdb-1.5.0a98/ioavstatsdb/io_utils.py`

 * *Files identical despite different names*

### Comparing `ioavstatsdb-1.5.0a94/ioavstatsdb.egg-info/PKG-INFO` & `ioavstatsdb-1.5.0a98/ioavstatsdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ioavstatsdb
-Version: 1.5.0a94
+Version: 1.5.0a98
 Summary: Aviation Event Statistics - Database Software
 Author-email: Team IO-Aero <info@io-aero.com>
 Maintainer-email: Team IO-Aero <info@io-aero.ch>
 Project-URL: Bug Tracker, https://github.com/io-aero/io-avstats-db/issues
 Project-URL: Documentation, https://io-aero.github.io/io-avstats-db/
 Project-URL: Homepage, https://github.com/io-aero/io-avstats-db
 Project-URL: Release History, https://io-aero.github.io/io-avstats-db/release_history/
```

### Comparing `ioavstatsdb-1.5.0a94/pyproject.toml` & `ioavstatsdb-1.5.0a98/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ]
 maintainers = [
     { name = "Team IO-Aero", email = "info@io-aero.ch" },
 ]
 name = "ioavstatsdb"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "1.5.0a94"
+version = "1.5.0a98"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/io-aero/io-avstats-db/issues"
 "Documentation" = "https://io-aero.github.io/io-avstats-db/"
 "Homepage" = "https://github.com/io-aero/io-avstats-db"
 "Release History" = "https://io-aero.github.io/io-avstats-db/release_history/"
 "Release Notes" = "https://io-aero.github.io/io-avstats-db/release_notes/"
@@ -62,7 +62,10 @@
 markers = ["issue"]
 norecursedirs = "./tests/helpers"
 pythonpath = "./ioavstatsdb/"
 testpaths = "./tests/"
 
 [tool.setuptools]
 packages = ["ioavstatsdb"]
+
+[tool.setuptools.package-data]
+ioavstatsdb = ["*.pyi"]
```

### Comparing `ioavstatsdb-1.5.0a94/tests/conftest.py` & `ioavstatsdb-1.5.0a98/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ioavstatsdb-1.5.0a94/tests/test_launcher.py` & `ioavstatsdb-1.5.0a98/tests/test_launcher.py`

 * *Files identical despite different names*

