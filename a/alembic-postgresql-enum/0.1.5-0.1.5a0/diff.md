# Comparing `tmp/alembic_postgresql_enum-0.1.5.tar.gz` & `tmp/alembic_postgresql_enum-0.1.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alembic_postgresql_enum-0.1.5.tar", max compression
+gzip compressed data, was "alembic_postgresql_enum-0.1.5a0.tar", max compression
```

## Comparing `alembic_postgresql_enum-0.1.5.tar` & `alembic_postgresql_enum-0.1.5a0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1082 2023-05-26 08:19:49.153846 alembic_postgresql_enum-0.1.5/LICENSE
--rw-r--r--   0        0        0     6074 2023-08-05 06:01:32.666075 alembic_postgresql_enum-0.1.5/README.md
--rw-r--r--   0        0        0       32 2023-07-26 19:11:56.863336 alembic_postgresql_enum-0.1.5/alembic_postgresql_enum/__init__.py
--rw-r--r--   0        0        0     1718 2023-07-26 19:11:56.863336 alembic_postgresql_enum-0.1.5/alembic_postgresql_enum/compare_dispatch.py
--rw-r--r--   0        0        0     8237 2023-08-05 06:01:31.742062 alembic_postgresql_enum-0.1.5/alembic_postgresql_enum/enum_alteration.py
--rw-r--r--   0        0        0     1145 2023-07-26 19:11:56.863336 alembic_postgresql_enum-0.1.5/alembic_postgresql_enum/enum_creation.py
--rw-r--r--   0        0        0     1174 2023-07-26 19:11:56.863336 alembic_postgresql_enum-0.1.5/alembic_postgresql_enum/enum_deletion.py
--rw-r--r--   0        0        0      606 2023-07-26 19:11:55.927316 alembic_postgresql_enum-0.1.5/alembic_postgresql_enum/enum_op_base.py
--rw-r--r--   0        0        0     4799 2023-07-27 07:02:52.233793 alembic_postgresql_enum-0.1.5/alembic_postgresql_enum/get_enum_data.py
--rw-r--r--   0        0        0      901 2023-08-05 06:17:57.598241 alembic_postgresql_enum-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     6911 1970-01-01 00:00:00.000000 alembic_postgresql_enum-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-26 08:19:49.153846 alembic_postgresql_enum-0.1.5a0/LICENSE
+-rw-r--r--   0        0        0     6074 2023-08-05 06:01:32.666075 alembic_postgresql_enum-0.1.5a0/README.md
+-rw-r--r--   0        0        0       32 2023-07-26 19:11:56.863336 alembic_postgresql_enum-0.1.5a0/alembic_postgresql_enum/__init__.py
+-rw-r--r--   0        0        0     1718 2023-07-26 19:11:56.863336 alembic_postgresql_enum-0.1.5a0/alembic_postgresql_enum/compare_dispatch.py
+-rw-r--r--   0        0        0     8237 2023-08-05 06:01:31.742062 alembic_postgresql_enum-0.1.5a0/alembic_postgresql_enum/enum_alteration.py
+-rw-r--r--   0        0        0     1145 2023-07-26 19:11:56.863336 alembic_postgresql_enum-0.1.5a0/alembic_postgresql_enum/enum_creation.py
+-rw-r--r--   0        0        0     1174 2023-07-26 19:11:56.863336 alembic_postgresql_enum-0.1.5a0/alembic_postgresql_enum/enum_deletion.py
+-rw-r--r--   0        0        0      606 2023-07-26 19:11:55.927316 alembic_postgresql_enum-0.1.5a0/alembic_postgresql_enum/enum_op_base.py
+-rw-r--r--   0        0        0     4799 2023-07-27 07:02:52.233793 alembic_postgresql_enum-0.1.5a0/alembic_postgresql_enum/get_enum_data.py
+-rw-r--r--   0        0        0      903 2023-08-05 06:06:47.218351 alembic_postgresql_enum-0.1.5a0/pyproject.toml
+-rw-r--r--   0        0        0     6913 1970-01-01 00:00:00.000000 alembic_postgresql_enum-0.1.5a0/PKG-INFO
```

### Comparing `alembic_postgresql_enum-0.1.5/LICENSE` & `alembic_postgresql_enum-0.1.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.5/README.md` & `alembic_postgresql_enum-0.1.5a0/README.md`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.5/alembic_postgresql_enum/compare_dispatch.py` & `alembic_postgresql_enum-0.1.5a0/alembic_postgresql_enum/compare_dispatch.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.5/alembic_postgresql_enum/enum_alteration.py` & `alembic_postgresql_enum-0.1.5a0/alembic_postgresql_enum/enum_alteration.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.5/alembic_postgresql_enum/enum_creation.py` & `alembic_postgresql_enum-0.1.5a0/alembic_postgresql_enum/enum_creation.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.5/alembic_postgresql_enum/enum_deletion.py` & `alembic_postgresql_enum-0.1.5a0/alembic_postgresql_enum/enum_deletion.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.5/alembic_postgresql_enum/enum_op_base.py` & `alembic_postgresql_enum-0.1.5a0/alembic_postgresql_enum/enum_op_base.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.5/alembic_postgresql_enum/get_enum_data.py` & `alembic_postgresql_enum-0.1.5a0/alembic_postgresql_enum/get_enum_data.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.5/pyproject.toml` & `alembic_postgresql_enum-0.1.5a0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alembic-postgresql-enum"
-version = "0.1.5"
+version = "0.1.5a0"
 description = "Alembic autogenerate support for creation, alteration and deletion of enums"
 authors = ["RustyGuard"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "alembic_postgresql_enum" }]
 classifiers = [
     'Development Status :: 4 - Beta',
```

### Comparing `alembic_postgresql_enum-0.1.5/PKG-INFO` & `alembic_postgresql_enum-0.1.5a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alembic-postgresql-enum
-Version: 0.1.5
+Version: 0.1.5a0
 Summary: Alembic autogenerate support for creation, alteration and deletion of enums
 License: MIT
 Author: RustyGuard
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

