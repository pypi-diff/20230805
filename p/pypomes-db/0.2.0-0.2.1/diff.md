# Comparing `tmp/pypomes_db-0.2.0.tar.gz` & `tmp/pypomes_db-0.2.1.tar.gz`

## Comparing `pypomes_db-0.2.0.tar` & `pypomes_db-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 pypomes_db-0.2.0/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    15547 2020-02-02 00:00:00.000000 pypomes_db-0.2.0/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 pypomes_db-0.2.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.2.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.2.0/README.md
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pypomes_db-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pypomes_db-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 pypomes_db-0.2.1/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    15500 2020-02-02 00:00:00.000000 pypomes_db-0.2.1/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pypomes_db-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.2.1/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.2.1/README.md
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pypomes_db-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pypomes_db-0.2.1/PKG-INFO
```

### Comparing `pypomes_db-0.2.0/src/pypomes_db/db_pomes.py` & `pypomes_db-0.2.1/src/pypomes_db/db_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,16 +151,15 @@
                     errors.append(f"{cursor.rowcount} tuples returned, "
                                   f"but {require_count} expected, in '{DB_NAME}' at '{DB_HOST}', "
                                   f"for '{__db_build_query_msg(sel_stmt, where_vals)}'")
 
                 else:
                     # obtain the returned tuples
                     rows: list[Row] = cursor.fetchall()
-                    for row in rows:
-                        result.append(tuple(row))
+                    result = [tuple(row) for row in rows]
             conn.commit()
     except Exception as e:
         errors.append(__db_except_msg(e))
 
     return result
 
 
@@ -276,16 +275,15 @@
                     # yes, report the error
                     errors.append(f"{cursor.rowcount} tuples returned, "
                                   f"but {require_count} expected, in '{DB_NAME}' at '{DB_HOST}', "
                                   f"for stored procedure '{proc_name}', with values '{proc_vals}'")
                 else:
                     # obtain the returned tuples
                     rows: list[Row] = cursor.fetchall()
-                    for row in rows:
-                        result.append(tuple(row))
+                    result = [tuple(row) for row in rows]
             conn.commit()
     except Exception as e:
         errors.append(__db_except_msg(e))
 
     return result
 
 
@@ -352,13 +350,13 @@
     :param where_vals: values associated with the search criteria
     :return: message indicative of empty search
     """
     result: str = __db_msg_clean(sel_stmt)
 
     for val in where_vals:
         if isinstance(val, str):
-            val = f"'{val}'"
+            sval: str = f"'{val}'"
         else:
-            val = str(val)
-        result = result.replace("?", val, 1)
+            sval: str = str(val)
+        result = result.replace("?", sval, 1)
 
     return result
```

### Comparing `pypomes_db-0.2.0/LICENSE` & `pypomes_db-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.2.0/pyproject.toml` & `pypomes_db-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (DB modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -18,15 +18,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "pip>=23.2.1",
     "psycopg2-binary>=2.9.6",
     "pyodbc>=4.0.39",
-    "pypomes_core>=0.2.1",
+    "pypomes_core>=0.2.3",
     "setuptools>=68.0.0",
     "wheel>=0.41.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-DB"
 "Bug Tracker" = "https://github.com/TheWiseCoder/PyPomes-DB/issues"
```

