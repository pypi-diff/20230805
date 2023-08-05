# Comparing `tmp/pypomes_store-0.1.8.tar.gz` & `tmp/pypomes_store-0.1.9.tar.gz`

## Comparing `pypomes_store-0.1.8.tar` & `pypomes_store-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pypomes_store-0.1.8/src/pypomes_store/__init__.py
--rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 pypomes_store-0.1.8/src/pypomes_store/azure_pomes.py
--rw-r--r--   0        0        0    13962 2020-02-02 00:00:00.000000 pypomes_store-0.1.8/src/pypomes_store/minio_pomes.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 pypomes_store-0.1.8/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_store-0.1.8/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_store-0.1.8/README.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pypomes_store-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 pypomes_store-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 pypomes_store-0.1.9/src/pypomes_store/__init__.py
+-rw-r--r--   0        0        0     7558 2020-02-02 00:00:00.000000 pypomes_store-0.1.9/src/pypomes_store/azure_pomes.py
+-rw-r--r--   0        0        0    14061 2020-02-02 00:00:00.000000 pypomes_store-0.1.9/src/pypomes_store/minio_pomes.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_store-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_store-0.1.9/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_store-0.1.9/README.md
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pypomes_store-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 pypomes_store-0.1.9/PKG-INFO
```

### Comparing `pypomes_store-0.1.8/src/pypomes_store/azure_pomes.py` & `pypomes_store-0.1.9/src/pypomes_store/azure_pomes.py`

 * *Files 5% similar despite different names*

```diff
@@ -165,47 +165,48 @@
     :param exception: A exceção levantada
     :return: A mensagem de erro formatada
     """
     # TODO
     return exc_format(exception, sys.exc_info())
 
 
-# testes do acesso ao Azure
-# if __name__ == "__main__":
-#
-#     # print errors
-#     def __print_errors(errors: list[str], op):
-#         if len(errors) > 0:
-#             print(f"\nErrors in '{op}':")
-#             for error in errors:
-#                 print(error)
-#
-#     errors: list[str] = []
-#     content: bytes = b"This is the content of a sample text file."
-#     file_path: str = "/temp/sample.txt"
-#
-#     # testa a verificação de existência do arquivo
-#     exists: bool = blob_exists(errors, file_path)
-#     __print_errors(errors, "blob_exists")
-#     assert exists is not None, "Failed verifying file"
-#
-#     # testa armazenamento de arquivo
-#     if not exists:
-#         success = blob_store(errors, content, file_path)
-#         __print_errors(errors, "blob_store")
-#         assert success, "Failed storing file"
-#
-#     # testa recuperação do tipo do arquivo
-#     mimetype: str = blob_get_mimetype(errors, file_path)
-#     __print_errors(errors, "blob_get_mimetype")
-#     assert mimetype is not None, "Failed retrieving file mimetype"
-#
-#     # testa recuperação do conteúdo do arquivo
-#     retrieved: bytes = blob_retrieve(errors, file_path)
-#     __print_errors(errors, "blob_retrieve")
-#     assert retrieved is not None, "Failed retrieving file content"
-#     print(f"Conteudo recuperado: {content}")
-#
-#     # testa a exclusão do arquivo
-#     success = blob_delete(errors, file_path)
-#     __print_errors(errors, "blob_delete")
-#     assert success, "Failed Deleting file"
+# test Azure operations
+if __name__ == "__main__":
+
+    # ruff: noqa: S101
+
+    def __print_errors(errors: list[str], op: str) -> None:
+        if len(errors) > 0:
+            print(f"\nErrors in '{op}':")
+            for error in errors:
+                print(error)
+
+    errors: list[str] = []
+    content: bytes = b"This is the content of a sample text file."
+    file_path: str = "/temp/sample.txt"
+
+    # verify if file exists
+    exists: bool = blob_exists(errors, file_path)
+    __print_errors(errors, "blob_exists")
+    assert exists is not None, "Failed verifying file"
+
+    # store file
+    if not exists:
+        success = blob_store(errors, content, file_path)
+        __print_errors(errors, "blob_store")
+        assert success, "Failed storing file"
+
+    # retrieve file type
+    mimetype: str = blob_get_mimetype(errors, file_path)
+    __print_errors(errors, "blob_get_mimetype")
+    assert mimetype is not None, "Failed retrieving file mimetype"
+
+    # retrieve file contents
+    retrieved: bytes = blob_retrieve(errors, file_path)
+    __print_errors(errors, "blob_retrieve")
+    assert retrieved is not None, "Failed retrieving file content"
+    print(f"Conteudo recuperado: {content}")
+
+    # remove the file
+    success = blob_delete(errors, file_path)
+    __print_errors(errors, "blob_delete")
+    assert success, "Failed Deleting file"
```

### Comparing `pypomes_store-0.1.8/src/pypomes_store/minio_pomes.py` & `pypomes_store-0.1.9/src/pypomes_store/minio_pomes.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 import pickle
 import tempfile
 import uuid
 from collections.abc import Iterator
 from minio import Minio
 from minio.datatypes import Object as MinioObject
 from minio.commonconfig import Tags
-from pypomes_core import APP_PREFIX, env_get_bool, env_get_str
+from pathlib import Path
+from pypomes_core import APP_PREFIX, env_get_bool, env_get_str, env_get_path
 from typing import Final
 from unidecode import unidecode
 
 MINIO_BUCKET: Final[str] = env_get_str(f"{APP_PREFIX}_MINIO_BUCKET")
 MINIO_HOST: Final[str] = env_get_str(f"{APP_PREFIX}_MINIO_HOST")
 MINIO_ACCESS_KEY: Final[str] = env_get_str(f"{APP_PREFIX}_MINIO_ACCESS_KEY")
 MINIO_SECRET_KEY: Final[str] = env_get_str(f"{APP_PREFIX}_MINIO_SECRET_KEY")
 MINIO_SECURE_ACCESS: Final[bool] = env_get_bool(F"{APP_PREFIX}_MINIO_SECURE_ACCESS")
-MINIO_TEMP_PATH: Final[str] = env_get_str(F"{APP_PREFIX}_MINIO_TEMP_PATH", tempfile.gettempdir())
+MINIO_TEMP_PATH: Final[Path] = env_get_path(f"{APP_PREFIX}_MINIO_TEMP_PATH", Path(tempfile.gettempdir()))
 
 
 def minio_setup(errors: list[str]) -> bool:
     """
     Prepare the *MinIO* client for operations.
 
     This function should be called just once, at startup,
@@ -68,16 +69,16 @@
 
     except Exception as e:
         errors.append(__minio_except_msg(e))
 
     return result
 
 
-def minio_file_store(errors: list[str], basepath: str,
-                     identifier: str, filepath: str, mimetype: str, tags: dict = None) -> None:
+def minio_file_store(errors: list[str], basepath: Path | str,
+                     identifier: str, filepath: Path | str, mimetype: str, tags: dict = None) -> None:
     """
     Store a file at the *MinIO* store.
 
     :param errors: incidental error messages
     :param basepath: the path specifying the location to store the file at
     :param identifier: the file identifier, tipically a file name
     :param filepath: the path specifying where the file is
@@ -86,36 +87,37 @@
     """
     # obtain the MinIO client
     minio_client: Minio = minio_access(errors)
 
     # was the MinIO client obtained ?
     if minio_client is not None:
         # yes, store the file
-        remotepath: str = os.path.join(basepath, identifier)
+        remotepath: Path = Path(basepath) / identifier
         # have tags been defined ?
         if tags is None or len(tags) == 0:
             # no
             doc_tags = None
         else:
             # sim, store them
             doc_tags = Tags(for_object=True)
             for key, value in tags.items():
                 # normalize text, by removing all diacritics
                 doc_tags[key] = unidecode(value)
         try:
             minio_client.fput_object(bucket_name=MINIO_BUCKET,
-                                     object_name=remotepath,
+                                     object_name=f"{remotepath}",
                                      file_path=filepath,
                                      content_type=mimetype,
                                      tags=doc_tags)
         except Exception as e:
             errors.append(__minio_except_msg(e))
 
 
-def minio_file_retrieve(errors: list[str], basepath: str, identifier: str, filepath: str) -> any:
+def minio_file_retrieve(errors: list[str], basepath: Path | str,
+                        identifier: str, filepath: Path | str) -> any:
     """
     Retrieve a file from the *MinIO* store.
 
     :param errors: incidental error messages
     :param basepath: the path specifying the location to retrieve the file from
     :param identifier: the file identifier, tipically a file name
     :param filepath: the path to save the retrieved file at
@@ -126,27 +128,27 @@
 
     # obtain the MinIO client
     minio_client: Minio = minio_access(errors)
 
     # was the MinIO client obtained ?
     if minio_client is not None:
         # yes, retrieve the file
-        remotepath: str = os.path.join(basepath, identifier)
+        remotepath: Path = Path(basepath) / identifier
         try:
             result = minio_client.fget_object(bucket_name=MINIO_BUCKET,
-                                              object_name=remotepath,
+                                              object_name=f"{remotepath}",
                                               file_path=filepath)
         except Exception as e:
             if not hasattr(e, "code") or e.code != "NoSuchKey":
                 errors.append(__minio_except_msg(e))
 
     return result
 
 
-def minio_object_exists(errors: list[str], basepath: str, identifier: str = None) -> bool:
+def minio_object_exists(errors: list[str], basepath: Path | str, identifier: str = None) -> bool:
     """
     Determine if a given object exists in the *MinIO* store.
 
     :param errors: incidental error messages
     :param basepath: the path specifying the location to locate the object at
     :param identifier: the object identifier
     :return: True if the object was found
@@ -157,23 +159,22 @@
     # was the identifier provided ?
     if identifier is None:
         # no, object is a folder
         objs: Iterator = minio_objects_list(errors, basepath)
         for _ in objs:
             result = True
             break
-    else:
-        # yes, verify the status of the object
-        if minio_object_stat(errors, basepath, identifier) is not None:
-            result = True
+    # verify the status of the object
+    elif minio_object_stat(errors, basepath, identifier) is not None:
+        result = True
 
     return result
 
 
-def minio_object_stat(errors: list[str], basepath: str, identifier: str) -> MinioObject:
+def minio_object_stat(errors: list[str], basepath: Path | str, identifier: str) -> MinioObject:
     """
     Retrieve and return the information about an object in the *MinIO* store.
 
     :param errors: incidental error messages
     :param basepath: the path specifying where to locate the object
     :param identifier: the object identifier
     :return: metadata and information about the object
@@ -183,26 +184,26 @@
 
     # obtain the MinIO client
     minio_client: Minio = minio_access(errors)
 
     # was the MinIO client obtained ?
     if minio_client is not None:
         # yes, retrieve the object's information
-        remotepath: str = os.path.join(basepath, identifier)
+        remotepath: Path = Path(basepath) / identifier
         try:
             result = minio_client.stat_object(bucket_name=MINIO_BUCKET,
-                                              object_name=remotepath)
+                                              object_name=f"{remotepath}")
         except Exception as e:
             if not hasattr(e, "code") or e.code != "NoSuchKey":
                 errors.append(__minio_except_msg(e))
 
     return result
 
 
-def minio_object_store(errors: list[str], basepath: str,
+def minio_object_store(errors: list[str], basepath: Path | str,
                        identifier: str, obj: any, tags: dict = None) -> None:
     """
     Store an object at the *MinIO* store.
 
     :param errors: incidental error messages
     :param basepath: the path specifying the location to store the object at
     :param identifier: the object identifier
@@ -212,45 +213,45 @@
     # obtain the MinIO client
     minio_client: Minio = minio_access(errors)
 
     # proceed, if the MinIO client was obtained
     if minio_client is not None:
 
         # serialize the object into a file
-        filepath: str = os.path.join(MINIO_TEMP_PATH, str(uuid.uuid4()) + ".pickle")
-        with open(filepath, "wb") as f:
+        filepath: Path = Path(MINIO_TEMP_PATH) / f"{uuid.uuid4()}.pickle"
+        with Path.open(filepath, "wb") as f:
             pickle.dump(obj, f)
 
         # store the file and remove it
         minio_file_store(errors, basepath, identifier, filepath, "application/octet-stream", tags)
-        os.remove(filepath)
+        Path.unlink(filepath)
 
 
-def minio_object_retrieve(errors: list[str], basepath: str, identifier: str) -> any:
+def minio_object_retrieve(errors: list[str], basepath: Path, identifier: str) -> any:
     """
     Retrieve an object from the *MinIO* store.
 
     :param errors: incidental error messages
     :param basepath: the path specifying the location to retrieve the object from
     :param identifier: the object identifier
     :return: the object retrieved
     """
     # initialize the return variable
     result: any = None
 
     # retrieve the file containg the serialized object
-    filepath: str = os.path.join(MINIO_TEMP_PATH, str(uuid.uuid4()) + ".pickle")
+    filepath: Path = Path(MINIO_TEMP_PATH) / f"{uuid.uuid4()}.pickle"
     stat: any = minio_file_retrieve(errors, basepath, identifier, filepath)
 
     # was the file retrieved ?
     if stat is not None:
         # yes, umarshall the corresponding object
-        with open(filepath, "rb") as f:
+        with Path.open(filepath, "rb") as f:
             result = pickle.load(f)
-        os.remove(filepath)
+        Path.unlink(filepath)
 
     return result
 
 
 def minio_object_delete(errors: list[str], basepath: str, identifier: str = None) -> None:
     """
     Remove an object from the *MinIO* store.
@@ -353,26 +354,26 @@
     #
     try:
         objs: Iterator = minio_objects_list(errors, basepath, True)
         for obj in objs:
             try:
                 minio_client.remove_object(bucket_name=MINIO_BUCKET,
                                            object_name=obj.object_name)
-            except Exception as e:
+            except Exception as e:  # noqa: PERF203
                 # SANITY CHECK: in case of concurrent exclusion
                 if not hasattr(e, "code") or e.code != "NoSuchKey":
                     errors.append(__minio_except_msg(e))
     except Exception as e:
         errors.append(__minio_except_msg(e))
 
 
 def __minio_except_msg(exception: Exception) -> str:
     """
     Format and return an error message from *exception*.
 
     :param exception: the reference exception
     :return: the error message
     """
-    # interaction with MinIO raised the exception "<class 'classe-da-exceção'>"
+    # interaction with MinIO raised the exception "<class 'exception_class'>"
     cls: str = str(exception.__class__)
     exc_msg: str = f"{cls[7:-1]} - {exception}"
     return f"Error accessing the object storer: {exc_msg}"
```

### Comparing `pypomes_store-0.1.8/LICENSE` & `pypomes_store-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_store-0.1.8/pyproject.toml` & `pypomes_store-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_store"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (object storage modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -21,15 +21,15 @@
 dependencies = [
     "azure-common>=1.1.28",
     "azure-core>=1.28.0",
     "azure-identity>=1.13.0",
     "azure-storage-blob>=12.17.0",
     "minio>=7.1.15",
     "pip>=23.2.1",
-    "pypomes_core>=0.2.2",
+    "pypomes_core>=0.2.3",
     "setuptools>=68.0.0",
     "Unidecode>=1.3.6",
     "wheel>=0.41.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-Store"
```

### Comparing `pypomes_store-0.1.8/PKG-INFO` & `pypomes_store-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypomes_store
-Version: 0.1.8
+Version: 0.1.9
 Summary: A collection of Python pomes, pennyeach (object storage modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Store
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Store/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,11 +12,11 @@
 Requires-Python: >=3.10
 Requires-Dist: azure-common>=1.1.28
 Requires-Dist: azure-core>=1.28.0
 Requires-Dist: azure-identity>=1.13.0
 Requires-Dist: azure-storage-blob>=12.17.0
 Requires-Dist: minio>=7.1.15
 Requires-Dist: pip>=23.2.1
-Requires-Dist: pypomes-core>=0.2.2
+Requires-Dist: pypomes-core>=0.2.3
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: unidecode>=1.3.6
 Requires-Dist: wheel>=0.41.0
```

