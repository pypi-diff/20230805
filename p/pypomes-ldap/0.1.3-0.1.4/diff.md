# Comparing `tmp/pypomes_ldap-0.1.3.tar.gz` & `tmp/pypomes_ldap-0.1.4.tar.gz`

## Comparing `pypomes_ldap-0.1.3.tar` & `pypomes_ldap-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0  1418839 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.3/python_ldap-3.4.0-cp310-cp310-win_amd64.whl
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.3/src/pypomes_ldap/__init__.py
--rw-r--r--   0        0        0    18287 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.3/src/pypomes_ldap/ldap_pomes.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.3/README.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0  1418839 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.4/python_ldap-3.4.0-cp310-cp310-win_amd64.whl
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.4/src/pypomes_ldap/__init__.py
+-rw-r--r--   0        0        0    18391 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.4/src/pypomes_ldap/ldap_pomes.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.4/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.4/README.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.4/PKG-INFO
```

### Comparing `pypomes_ldap-0.1.3/python_ldap-3.4.0-cp310-cp310-win_amd64.whl` & `pypomes_ldap-0.1.4/python_ldap-3.4.0-cp310-cp310-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `pypomes_ldap-0.1.3/src/pypomes_ldap/ldap_pomes.py` & `pypomes_ldap-0.1.4/src/pypomes_ldap/ldap_pomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import ldap
-import os
 import sys
 import tempfile
 from ldap import LDAPError, modlist
 from ldap.ldapobject import LDAPObject
+from pathlib import Path
 from typing import Final, TextIO
-from pypomes_core import APP_PREFIX, env_get_str, env_get_int, exc_format
+from pypomes_core import APP_PREFIX, env_get_str, env_get_int, env_get_path, exc_format
 
 _val: str = env_get_str(f"{APP_PREFIX}_LDAP_BASE_DN")
 LDAP_BASE_DN: Final[str] = None if _val is None else _val.replace(":", "=")
 _val = env_get_str(f"{APP_PREFIX}_LDAP_BIND_DN")
 LDAP_BIND_DN:  Final[str] = None if _val is None else _val.replace(":", "=")
 LDAP_BIND_PWD:  Final[str] = env_get_str(f"{APP_PREFIX}_LDAP_BIND_PWD")
 LDAP_SERVER_URI:  Final[str] = env_get_str(f"{APP_PREFIX}_LDAP_SERVER_URI")
 LDAP_TIMEOUT:  Final[int] = env_get_int(f"{APP_PREFIX}_LDAP_TIMEOUT", 30)
-LDAP_TRACE_FILE:  Final[str] = env_get_str(f"{APP_PREFIX}_LDAP_TRACE_FILEPATH",
-                                           os.path.join(tempfile.gettempdir(), f"{APP_PREFIX}_ldap.log"))
+LDAP_TRACE_FILEPATH:  Final[Path] = env_get_path(f"{APP_PREFIX}_LDAP_TRACE_FILEPATH",
+                                                 Path(tempfile.gettempdir()) / f"{APP_PREFIX}_ldap.log")
 LDAP_TRACE_LEVEL:  Final[int] = env_get_int(f"{APP_PREFIX}_LDAP_TRACE_LEVEL", 0)
 
 
 def ldap_init(errors: list[str], server_uri: str = LDAP_SERVER_URI,
-              trace_filepath: str = LDAP_TRACE_FILE, trace_level: int = LDAP_TRACE_LEVEL) -> LDAPObject:
+              trace_filepath: Path = LDAP_TRACE_FILEPATH, trace_level: int = LDAP_TRACE_LEVEL) -> LDAPObject:
     """
     Initialize and return the LDAP client object.
     
     :param errors: incidental error messages
     :param server_uri: URI to access the LDAP server
     :param trace_filepath: path for the trace log file
     :param trace_level: level for the trace log
@@ -38,15 +38,15 @@
         trace_out: TextIO
         match trace_filepath:
             case "sys.stdout" | None:
                 trace_out = sys.stdout
             case "sys.stderr":
                 trace_out = sys.stderr
             case _:
-                trace_out = open(trace_filepath, "a")
+                trace_out = Path.open(trace_filepath, "a")
 
         if not isinstance(trace_level, int):
             trace_level = 0
 
         # obtem a conexão
         result = ldap.initialize(uri=server_uri,
                                  trace_level=trace_level,
@@ -82,34 +82,34 @@
         result = True
     except Exception as e:
         errors.append(f"Error binding with the LDAP server: {__ldap_except_msg(e)}")
 
     return result
 
 
-def ldap_unbind(errors: list[str], ldap_client: LDAPObject):
+def ldap_unbind(errors: list[str], ldap_client: LDAPObject) -> None:
     """
     Unbind the given LDAP client object *conn* with the LDAP server.
     
     :param errors: incidental error messages
     :param ldap_client: the LDAP client object
     """
     try:
         ldap_client.unbind_s()
         # is the log device 'stdout' ou 'stderr' ?
         # noinspection PyProtectedMember
-        if ldap_client._trace_file.name not in ["<stdout>", "<stderr>"]:
+        if ldap_client._trace_file.name not in ["<stdout>", "<stderr>"]: # noqa SLF001
             # no, close the log device
             # noinspection PyProtectedMember
-            ldap_client._trace_file.close()
+            ldap_client._trace_file.close() # noqa SLF001
     except Exception as e:
         errors.append(f"Error unbinding with the LDAP server: {__ldap_except_msg(e)}")
 
 
-def ldap_add_entry(errors: list[str], entry_dn: str, attrs: dict):
+def ldap_add_entry(errors: list[str], entry_dn: str, attrs: dict) -> None:
     """
     Add an entry to the LDAP store.
     
     :param errors: incidental error messages
     :param entry_dn: the entry DN
     :param attrs: the entry attributes
     """
@@ -133,15 +133,15 @@
             errors.append(f"Error on the LDAP add entry operation: {__ldap_except_msg(e)}")
 
     # unbind the LDAP client, if applicable
     if bound:
         ldap_unbind(errors, ldap_client)
 
 
-def ldap_modify_entry(errors: list[str], entry_dn: str, mod_entry: list[tuple[int, str, any]]):
+def ldap_modify_entry(errors: list[str], entry_dn: str, mod_entry: list[tuple[int, str, any]]) -> None:
     """
     Add an entry to the LDAP store.
     
     :param errors: incidental error messages
     :param entry_dn: the entry DN
     :param mod_entry: the list of modified entry attributes
     """
@@ -164,15 +164,15 @@
             errors.append(f"Error on the LDAP modify entry operation: {__ldap_except_msg(e)}")
 
     # unbind the LDAP client, if applicable
     if bound:
         ldap_unbind(errors, conn)
 
 
-def ldap_delete_entry(errors: list[str], entry_dn: str):
+def ldap_delete_entry(errors: list[str], entry_dn: str) -> None:
     """
     Remove an entry to the LDAP store.
     
     :param errors: incidental error messages
     :param entry_dn: the entry DN
     """
     # obtain the LDAP client object
@@ -193,15 +193,15 @@
             errors.append(f"Error on the LDAP delete entry operation: {__ldap_except_msg(e)}")
 
     # unbind the LDAP client, if applicable
     if bound:
         ldap_unbind(errors, conn)
 
 
-def ldap_modify_user(errors: list[str], user_id: str, attrs: list[tuple[str, bytes | None]]):
+def ldap_modify_user(errors: list[str], user_id: str, attrs: list[tuple[str, bytes | None]]) -> None:
     """
     Modify a user entry at the LDAP store.
     
     :param errors: incidental error messages
     :param user_id: id of the user
     :param attrs: the list of modified attributes
     """
@@ -352,29 +352,29 @@
     """
     data: list[bytes] = ldap_get_value_list(errors, entry_dn, attr)
     result: bytes = data[0] if isinstance(data, list) and len(data) > 0 else None
 
     return result
 
 
-def ldap_add_value(errors: list[str], entry_dn: str, attr: str, value: bytes):
+def ldap_add_value(errors: list[str], entry_dn: str, attr: str, value: bytes) -> None:
     """
     Add a value to an attribute at the LDAP store.
 
     :param errors: incidental error messages
     :param entry_dn: the DN entry
     :param attr: target attribute
     :param value: value to add to the target attribute
     :return: the target attribute's value
     """
     mod_entries: list[tuple[int, str, bytes]] = [(ldap.MOD_ADD, attr, value)]
     ldap_modify_entry(errors, entry_dn, mod_entries)
 
 
-def ldap_set_value(errors: list[str], entry_dn: str, attr: str, value: bytes | None):
+def ldap_set_value(errors: list[str], entry_dn: str, attr: str, value: bytes | None) -> None:
     """
     Add a value to an attribute at the LDAP store.
 
     :param errors: incidental error messages
     :param entry_dn: the DN entry
     :param attr: target attribute
     :param value: value to add to the target attribute
@@ -465,26 +465,24 @@
     # perform the search operation
     search_data: list[tuple[str, dict]] = ldap_search(errors, entry_dn, attrs)
 
     # did the search operation return data ?
     if isinstance(search_data, list) and len(search_data) > 0:
         # yes, proceed
         user_data: dict = search_data[0][1]
-        items: list[list[bytes]] = []
-        for attr in attrs:
-            items.append(user_data.get(attr))
+        items: list[list[bytes]] = [user_data.get(attr) for attr in attrs]
         result = tuple(items)
 
     return result
 
 
 def __is_secure(conn: LDAPObject) -> bool:
 
     # noinspection PyProtectedMember
-    return conn._uri.startswith("ldaps:")
+    return conn._uri.startswith("ldaps:") # noqa SLF001
 
 
 # constrói a mensagem de erro a partir da exceção produzida
 def __ldap_except_msg(exc: Exception) -> str:
 
     if isinstance(exc, LDAPError):
         err_data: any = exc.args[0]
```

### Comparing `pypomes_ldap-0.1.3/LICENSE` & `pypomes_ldap-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_ldap-0.1.3/pyproject.toml` & `pypomes_ldap-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_ldap"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (LDAP module)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "pip>=23.1.2",
-    "pypomes_core>=0.2.1",
+    "pypomes_core>=0.2.3",
     "python-ldap>=3.4.0",
     "setuptools>=68.0.0",
     "wheel>=0.41.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-LDAP"
```

### Comparing `pypomes_ldap-0.1.3/PKG-INFO` & `pypomes_ldap-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pypomes_ldap
-Version: 0.1.3
+Version: 0.1.4
 Summary: A collection of Python pomes, pennyeach (LDAP module)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-LDAP
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-LDAP/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: pip>=23.1.2
-Requires-Dist: pypomes-core>=0.2.1
+Requires-Dist: pypomes-core>=0.2.3
 Requires-Dist: python-ldap>=3.4.0
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.41.0
```

