# Comparing `tmp/alembic_postgresql_enum-0.1.4a0.tar.gz` & `tmp/alembic_postgresql_enum-0.1.4a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alembic_postgresql_enum-0.1.4a0.tar", max compression
+gzip compressed data, was "alembic_postgresql_enum-0.1.4a2.tar", max compression
```

## Comparing `alembic_postgresql_enum-0.1.4a0.tar` & `alembic_postgresql_enum-0.1.4a2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1082 2023-05-26 08:19:49.153846 alembic_postgresql_enum-0.1.4a0/LICENSE
--rw-r--r--   0        0        0     3985 2023-07-26 19:58:44.754677 alembic_postgresql_enum-0.1.4a0/README.md
--rw-r--r--   0        0        0       32 2023-07-26 19:11:56.863336 alembic_postgresql_enum-0.1.4a0/alembic_postgresql_enum/__init__.py
--rw-r--r--   0        0        0     1718 2023-07-26 19:11:56.863336 alembic_postgresql_enum-0.1.4a0/alembic_postgresql_enum/compare_dispatch.py
--rw-r--r--   0        0        0     6270 2023-07-26 19:58:15.881837 alembic_postgresql_enum-0.1.4a0/alembic_postgresql_enum/enum_alteration.py
--rw-r--r--   0        0        0     1145 2023-07-26 19:11:56.863336 alembic_postgresql_enum-0.1.4a0/alembic_postgresql_enum/enum_creation.py
--rw-r--r--   0        0        0     1174 2023-07-26 19:11:56.863336 alembic_postgresql_enum-0.1.4a0/alembic_postgresql_enum/enum_deletion.py
--rw-r--r--   0        0        0      606 2023-07-26 19:11:55.927316 alembic_postgresql_enum-0.1.4a0/alembic_postgresql_enum/enum_op_base.py
--rw-r--r--   0        0        0     4799 2023-07-27 07:02:52.233793 alembic_postgresql_enum-0.1.4a0/alembic_postgresql_enum/get_enum_data.py
--rw-r--r--   0        0        0      902 2023-07-27 07:13:19.051159 alembic_postgresql_enum-0.1.4a0/pyproject.toml
--rw-r--r--   0        0        0     4824 1970-01-01 00:00:00.000000 alembic_postgresql_enum-0.1.4a0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-26 08:19:49.153846 alembic_postgresql_enum-0.1.4a2/LICENSE
+-rw-r--r--   0        0        0     3985 2023-07-26 19:58:44.754677 alembic_postgresql_enum-0.1.4a2/README.md
+-rw-r--r--   0        0        0       32 2023-07-26 19:11:56.863336 alembic_postgresql_enum-0.1.4a2/alembic_postgresql_enum/__init__.py
+-rw-r--r--   0        0        0     1718 2023-07-26 19:11:56.863336 alembic_postgresql_enum-0.1.4a2/alembic_postgresql_enum/compare_dispatch.py
+-rw-r--r--   0        0        0     6303 2023-07-27 07:39:19.179602 alembic_postgresql_enum-0.1.4a2/alembic_postgresql_enum/enum_alteration.py
+-rw-r--r--   0        0        0     1145 2023-07-26 19:11:56.863336 alembic_postgresql_enum-0.1.4a2/alembic_postgresql_enum/enum_creation.py
+-rw-r--r--   0        0        0     1174 2023-07-26 19:11:56.863336 alembic_postgresql_enum-0.1.4a2/alembic_postgresql_enum/enum_deletion.py
+-rw-r--r--   0        0        0      606 2023-07-26 19:11:55.927316 alembic_postgresql_enum-0.1.4a2/alembic_postgresql_enum/enum_op_base.py
+-rw-r--r--   0        0        0     4799 2023-07-27 07:02:52.233793 alembic_postgresql_enum-0.1.4a2/alembic_postgresql_enum/get_enum_data.py
+-rw-r--r--   0        0        0      903 2023-07-27 07:52:30.045850 alembic_postgresql_enum-0.1.4a2/pyproject.toml
+-rw-r--r--   0        0        0     4824 1970-01-01 00:00:00.000000 alembic_postgresql_enum-0.1.4a2/PKG-INFO
```

### Comparing `alembic_postgresql_enum-0.1.4a0/LICENSE` & `alembic_postgresql_enum-0.1.4a2/LICENSE`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.4a0/README.md` & `alembic_postgresql_enum-0.1.4a2/README.md`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.4a0/alembic_postgresql_enum/compare_dispatch.py` & `alembic_postgresql_enum-0.1.4a2/alembic_postgresql_enum/compare_dispatch.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.4a0/alembic_postgresql_enum/enum_alteration.py` & `alembic_postgresql_enum-0.1.4a2/alembic_postgresql_enum/enum_alteration.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,14 @@
     def sync_enum_values(
             cls,
             operations,
             schema: str,
             enum_name: str,
             new_values: List[str],
             affected_columns: 'List[Tuple[str, str]]' = None,
-            *,
             enum_values_to_rename: 'Iterable[Tuple[str, str]]' = tuple()
     ):
         """
         Replace enum values with `new_values`
         :param operations:
             ...
         :param str schema:
@@ -138,15 +137,16 @@
 
     def to_diff_tuple(self) -> 'Tuple[Any, ...]':
         return self.operation_name, self.old_values, self.new_values, self.affected_columns
 
 
 @alembic.autogenerate.render.renderers.dispatch_for(SyncEnumValuesOp)
 def render_sync_enum_value_op(autogen_context: AutogenContext, op: SyncEnumValuesOp):
-    return f"op.sync_enum_values({op.schema!r}, {op.name!r}, {op.new_values!r}, {op.affected_columns!r})"
+    return (f"op.sync_enum_values({op.schema!r}, {op.name!r}, {op.new_values!r}, {op.affected_columns!r}, \n"
+            f"  enum_values_to_rename=())")
 
 
 def sync_changed_enums(defined_enums: EnumNamesToValues, declared_enums: EnumNamesToValues,
                        table_references: EnumNamesToTableReferences,
                        schema: str, upgrade_ops: UpgradeOps):
     for enum_name, new_values in declared_enums.items():
         if enum_name not in defined_enums:
```

### Comparing `alembic_postgresql_enum-0.1.4a0/alembic_postgresql_enum/enum_creation.py` & `alembic_postgresql_enum-0.1.4a2/alembic_postgresql_enum/enum_creation.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.4a0/alembic_postgresql_enum/enum_deletion.py` & `alembic_postgresql_enum-0.1.4a2/alembic_postgresql_enum/enum_deletion.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.4a0/alembic_postgresql_enum/enum_op_base.py` & `alembic_postgresql_enum-0.1.4a2/alembic_postgresql_enum/enum_op_base.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.4a0/alembic_postgresql_enum/get_enum_data.py` & `alembic_postgresql_enum-0.1.4a2/alembic_postgresql_enum/get_enum_data.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.4a0/pyproject.toml` & `alembic_postgresql_enum-0.1.4a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alembic-postgresql-enum"
-version = "0.1.4a"
+version = "0.1.4a2"
 description = "Alembic autogenerate support for creation, alteration and deletion of enums"
 authors = ["RustyGuard"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "alembic_postgresql_enum" }]
 classifiers = [
     'Development Status :: 4 - Beta',
```

### Comparing `alembic_postgresql_enum-0.1.4a0/PKG-INFO` & `alembic_postgresql_enum-0.1.4a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alembic-postgresql-enum
-Version: 0.1.4a0
+Version: 0.1.4a2
 Summary: Alembic autogenerate support for creation, alteration and deletion of enums
 License: MIT
 Author: RustyGuard
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

