# Comparing `tmp/amarium-0.1.7.tar.gz` & `tmp/amarium-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amarium-0.1.7.tar", last modified: Sat Aug  5 20:07:56 2023, max compression
+gzip compressed data, was "amarium-0.1.8.tar", last modified: Fri Apr  7 19:37:36 2023, max compression
```

## Comparing `amarium-0.1.7.tar` & `amarium-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dev       (1001) dev       (1001)        0 2023-08-05 20:07:56.834647 amarium-0.1.7/
--rw-r--r--   0 dev       (1001) dev       (1001)    34475 2023-08-04 18:53:38.000000 amarium-0.1.7/LICENSE
--rw-r--r--   0 dev       (1001) dev       (1001)     3450 2023-08-05 20:07:56.834647 amarium-0.1.7/PKG-INFO
--rw-r--r--   0 dev       (1001) dev       (1001)     2895 2023-08-04 18:53:53.000000 amarium-0.1.7/README.md
--rw-r--r--   0 dev       (1001) dev       (1001)      671 2023-08-05 20:07:49.000000 amarium-0.1.7/pyproject.toml
--rw-r--r--   0 dev       (1001) dev       (1001)       38 2023-08-05 20:07:56.834647 amarium-0.1.7/setup.cfg
-drwxr-xr-x   0 dev       (1001) dev       (1001)        0 2023-08-05 20:07:56.834647 amarium-0.1.7/src/
--rw-r--r--   0 dev       (1001) dev       (1001)        0 2023-08-04 19:58:16.000000 amarium-0.1.7/src/__init__.py
-drwxr-xr-x   0 dev       (1001) dev       (1001)        0 2023-08-05 20:07:56.834647 amarium-0.1.7/src/amarium/
--rw-r--r--   0 dev       (1001) dev       (1001)        0 2023-08-04 19:58:16.000000 amarium-0.1.7/src/amarium/__init__.py
--rw-r--r--   0 dev       (1001) dev       (1001)     2815 2023-08-05 20:06:17.000000 amarium-0.1.7/src/amarium/checks.py
--rw-r--r--   0 dev       (1001) dev       (1001)        0 2023-08-04 19:58:16.000000 amarium-0.1.7/src/amarium/csv_utils.py
--rw-r--r--   0 dev       (1001) dev       (1001)     3456 2023-08-04 19:58:17.000000 amarium-0.1.7/src/amarium/database.py
--rw-r--r--   0 dev       (1001) dev       (1001)     4964 2023-08-05 20:05:33.000000 amarium-0.1.7/src/amarium/encryption.py
--rw-r--r--   0 dev       (1001) dev       (1001)    11306 2023-08-05 20:05:23.000000 amarium-0.1.7/src/amarium/utils.py
-drwxr-xr-x   0 dev       (1001) dev       (1001)        0 2023-08-05 20:07:56.834647 amarium-0.1.7/src/amarium.egg-info/
--rw-r--r--   0 dev       (1001) dev       (1001)     3450 2023-08-05 20:07:56.000000 amarium-0.1.7/src/amarium.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1001) dev       (1001)      458 2023-08-05 20:07:56.000000 amarium-0.1.7/src/amarium.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1001) dev       (1001)        1 2023-08-05 20:07:56.000000 amarium-0.1.7/src/amarium.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1001) dev       (1001)        6 2023-08-05 20:07:56.000000 amarium-0.1.7/src/amarium.egg-info/requires.txt
--rw-r--r--   0 dev       (1001) dev       (1001)       17 2023-08-05 20:07:56.000000 amarium-0.1.7/src/amarium.egg-info/top_level.txt
-drwxr-xr-x   0 dev       (1001) dev       (1001)        0 2023-08-05 20:07:56.834647 amarium-0.1.7/tests/
--rw-r--r--   0 dev       (1001) dev       (1001)     2296 2023-08-05 20:06:32.000000 amarium-0.1.7/tests/test_checks.py
--rw-r--r--   0 dev       (1001) dev       (1001)        0 2023-08-04 18:53:53.000000 amarium-0.1.7/tests/test_database.py
--rw-r--r--   0 dev       (1001) dev       (1001)     2097 2023-08-04 19:24:19.000000 amarium-0.1.7/tests/test_encryption.py
--rw-r--r--   0 dev       (1001) dev       (1001)     9647 2023-08-04 19:29:07.000000 amarium-0.1.7/tests/test_file_utils.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-07 19:37:36.758845 amarium-0.1.8/
+-rw-r--r--   0 developer  (1001) developer  (1001)    34475 2023-03-31 13:19:24.000000 amarium-0.1.8/LICENSE
+-rw-r--r--   0 developer  (1001) developer  (1001)     3547 2023-04-07 19:37:36.758845 amarium-0.1.8/PKG-INFO
+-rw-r--r--   0 developer  (1001) developer  (1001)     2992 2023-04-07 19:34:55.000000 amarium-0.1.8/README.md
+-rw-r--r--   0 developer  (1001) developer  (1001)      671 2023-04-07 19:37:12.000000 amarium-0.1.8/pyproject.toml
+-rw-r--r--   0 developer  (1001) developer  (1001)       38 2023-04-07 19:37:36.758845 amarium-0.1.8/setup.cfg
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-07 19:37:36.758845 amarium-0.1.8/src/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-03-31 13:29:17.000000 amarium-0.1.8/src/__init__.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-07 19:37:36.758845 amarium-0.1.8/src/amarium/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-03-31 13:29:17.000000 amarium-0.1.8/src/amarium/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2528 2023-03-31 13:29:17.000000 amarium-0.1.8/src/amarium/checks.py
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-03-31 13:29:17.000000 amarium-0.1.8/src/amarium/csv_utils.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     3431 2023-04-04 20:47:05.000000 amarium-0.1.8/src/amarium/database.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     4608 2023-04-07 08:54:09.000000 amarium-0.1.8/src/amarium/encryption.py
+-rw-r--r--   0 developer  (1001) developer  (1001)    10740 2023-04-07 19:32:18.000000 amarium-0.1.8/src/amarium/utils.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-07 19:37:36.758845 amarium-0.1.8/src/amarium.egg-info/
+-rw-r--r--   0 developer  (1001) developer  (1001)     3547 2023-04-07 19:37:36.000000 amarium-0.1.8/src/amarium.egg-info/PKG-INFO
+-rw-r--r--   0 developer  (1001) developer  (1001)      458 2023-04-07 19:37:36.000000 amarium-0.1.8/src/amarium.egg-info/SOURCES.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)        1 2023-04-07 19:37:36.000000 amarium-0.1.8/src/amarium.egg-info/dependency_links.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)        6 2023-04-07 19:37:36.000000 amarium-0.1.8/src/amarium.egg-info/requires.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)       17 2023-04-07 19:37:36.000000 amarium-0.1.8/src/amarium.egg-info/top_level.txt
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-07 19:37:36.758845 amarium-0.1.8/tests/
+-rw-r--r--   0 developer  (1001) developer  (1001)     1992 2023-03-31 13:19:40.000000 amarium-0.1.8/tests/test_checks.py
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 19:34:02.000000 amarium-0.1.8/tests/test_database.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2095 2023-03-31 13:19:40.000000 amarium-0.1.8/tests/test_encryption.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     8438 2023-04-07 19:32:18.000000 amarium-0.1.8/tests/test_file_utils.py
```

### Comparing `amarium-0.1.7/LICENSE` & `amarium-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `amarium-0.1.7/PKG-INFO` & `amarium-0.1.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amarium
-Version: 0.1.7
+Version: 0.1.8
 Summary: Filesystem handling utilities
 Author-email: "Julian M. Kleber" <julian.m.kleber@gmail.com>
 Project-URL: Homepage, https://www.codeberg.org/cap_jmk/amarium.git
 Project-URL: Bug Tracker, https://www.codeberg.org/cap_jmk/amarium.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,15 @@
 
 # Amarium
 
 [![status-badge](https://ci.codeberg.org/api/badges/cap_jmk/amarium/status.svg)](https://ci.codeberg.org/cap_jmk/amarium)
 [![Downloads](https://static.pepy.tech/personalized-badge/amarium?period=total&units=international_system&left_color=orange&right_color=blue&left_text=Downloads)](https://pepy.tech/project/amarium)
 [![License: GPL v3](https://img.shields.io/badge/License-GPL_v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 ![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C-blue)
+[![PyPI - Version](https://img.shields.io/pypi/v/amarium.svg)](https://pypi.org/project/amarium)
 
 **Table of Content**
 
 <!-- TOC -->
 - [1. Why](#1-why)
 - [2. What](#2-what)
 - [3. Usage](#3-usage)
```

### Comparing `amarium-0.1.7/README.md` & `amarium-0.1.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Amarium
 
 [![status-badge](https://ci.codeberg.org/api/badges/cap_jmk/amarium/status.svg)](https://ci.codeberg.org/cap_jmk/amarium)
 [![Downloads](https://static.pepy.tech/personalized-badge/amarium?period=total&units=international_system&left_color=orange&right_color=blue&left_text=Downloads)](https://pepy.tech/project/amarium)
 [![License: GPL v3](https://img.shields.io/badge/License-GPL_v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 ![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C-blue)
+[![PyPI - Version](https://img.shields.io/pypi/v/amarium.svg)](https://pypi.org/project/amarium)
 
 **Table of Content**
 
 <!-- TOC -->
 - [1. Why](#1-why)
 - [2. What](#2-what)
 - [3. Usage](#3-usage)
```

### Comparing `amarium-0.1.7/pyproject.toml` & `amarium-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "amarium"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="Julian M. Kleber", email="julian.m.kleber@gmail.com" },
 ]
 description = "Filesystem handling utilities"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `amarium-0.1.7/src/amarium/checks.py` & `amarium-0.1.8/src/amarium/checks.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 """Module to provide sanity checks for user inputs and other routine quality
 checks during execution.
 
 :author: Julian M. Kleber
 """
 import os
-from collections.abc import Iterable
 from typing import List, Any
 import shutil
-
-
 import logging
 
-LOGGER = logging.getLogger(__name__)
-
 
 def check_header_and_data(data: List[Any], header: List[Any]) -> None:
     """The check_header_and_data function checks that the length of the data
     and header lists are equal. If they are not, it raises a RuntimeError with
     an appropriate message.
 
-    :param data: List[Any]: Used to Pass in the data to be written.
-    :param header: List[Any]: Used to Ensure that the header and data
-        have the same number of fields.
-    :return: A boolean value.  :doc-author: Julian M. Kleber
+    :param data:List[Any]: Used to Pass in the data to be written.
+    :param header:List[Any]: Used to Ensure that the header and data have the same number of fields.
+    :return: A boolean value.
+
+    :doc-author: Julian M. Kleber
     """
 
     if len(data) == len(header):
         pass
     else:
         raise RuntimeError(
             "Input data and input header do not have the "
@@ -36,62 +32,54 @@
 
 
 def check_make_file_name_suffix(file_name: str, suffix: str = "") -> str:
     """The check_name_plot function checks that the file_name ends with .png.
     If it does not, then check_name_plot appends .png to the end of the
     file_name.
 
-    :param file_name: Used to Specify the name of the file to be
-        plotted.
-    :return: The file_name with the correct file extension. :doc-
-        author: Trelent
+    :param file_name: Used to Specify the name of the file to be plotted.
+    :return: The file_name with the correct file extension.
+
+    :doc-author: Trelent
     """
     name = file_name
     ext = os.path.splitext(file_name)[1]
     if not ext:
         if not suffix.startswith("."):
             suffix = "." + suffix
         name += suffix
     return name
 
 
-def check_make_subdirs(dir_names: Iterable[str]) -> str:
-    
-    from .utils import attach_slash
-    final_dir = ""
-    for directory in dir_names:
-        final_dir += attach_slash(directory)
-
-    check_make_dir(final_dir)
-    logging.info("Created dir " + final_dir)
-    return final_dir
-
 def check_delete_dir(dir_name: str) -> None:
     """The check_delete_dir function checks if a directory exists and deletes
     it.
 
-    :param dir_name: str: Used to Specify the directory name.
-    :return: None. :doc-author: Julian M. Kleber
+    :param dir_name:str: Used to Specify the directory name.
+    :return: None.
+    :doc-author: Julian M. Kleber
     """
 
     if os.path.isdir(dir_name):
         shutil.rmtree(dir_name)
 
 
 def check_make_dir(dir_name: str) -> None:
     """The check_make_dir function checks if a directory exists. If it does not
     exist, the function creates it.
 
-    :param dir_name: str: Used to Specify the folder name.
-    :return: None.  :doc-author: Trelent
+    :param dir_name:str: Used to Specify the folder name.
+    :return: None.
+
+    :doc-author: Trelent
     """
 
-    
+    # You should change 'test' to your preferred folder.
     check_folder = os.path.isdir(dir_name)
     logging.info("Checked the directory %s", dir_name)
-    
+    # If folder doesn't exist, then create it.
     if not check_folder:
         os.makedirs(dir_name)
         logging.info("Created folder : %s", dir_name)
 
     else:
         logging.info("%s folder already exists.", dir_name)
```

### Comparing `amarium-0.1.7/src/amarium/database.py` & `amarium-0.1.8/src/amarium/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,52 @@
-"""The file collects common CRUD operations interacting with databases.  The
-functions aim to provide a simplified API.
+"""
+The file collects common CRUD operations interacting with 
+databases.  The functions aim to provide a simplified API. 
 
-:author: Julian M. Kleber
+:author: Julian M. Kleber 
 """
 
 from typing import Optional, Any
 import sys
 
 import psycopg2
 import psycopg2.extras
 from sqlalchemy import create_engine
 
 import pandas as pd
 
 
 def connect_pg_db(host: str, dbname: str, user: str, password: str) -> None:
-    """The connect_pg_db function connects to a PostgreSQL database.
+    """
+    The connect_pg_db function connects to a PostgreSQL database.
+
+    :param host:str: Used to specify the hostname of the server to connect to.
+    :param dbname:str: Used to specify the name of the database that you want to connect to.
+    :param user:str: Used to specify the user name of the database.
+    :param password:str: Used to specify the password for the database.
+    :return: A connection object.
 
-    :param host: str: Used to specify the hostname of the server to
-        connect to.
-    :param dbname: str: Used to specify the name of the database that
-        you want to connect to.
-    :param user: str: Used to specify the user name of the database.
-    :param password: str: Used to specify the password for the database.
-    :return: A connection object.  :doc-author: Julian M. Kleber
+    :doc-author: Julian M. Kleber
     """
 
     if password is not None:
         conn_string = (
             f"host={host}' dbname='{dbname}' user='{user}' password='{password}'"
         )
     else:
         conn_string = f"host={host}' dbname='{dbname}' user='{user}'"
     print("Connecting to database\n	->%s" % (conn_string))
 
     conn = psycopg2.connect(conn_string)
     return conn
 
 
-def fetch_data(table: str, where_clause: str, limit: int, rows: str, conn: Any) -> iter:
-    """The fetch_data function is used to fetch data from a PostgreSQL
-    database.
+def fetch_data(table: str, where_clause: str, limit: int, rows: str, conn:) -> iter:
+    """
+    The fetch_data function is used to fetch data from a PostgreSQL database.
 
     The function takes in the following parameters:
 
 
     :param table:str: Used to Specify the table name.
     :param where_clause:str: Used to Filter the data that is returned.
     :param limit:int: Used to Limit the number of rows returned by the query.
@@ -53,52 +55,53 @@
 
     :doc-author: Trelent
     """
 
     cursor = conn.cursor(
         "cursor_unique_name", cursor_factory=psycopg2.extras.DictCursor
     )
-    cursor.execute(f"SELECT {rows} FROM {table} WHERE {where_clause} LIMIT {limit}")
+    cursor.execute(
+        f"SELECT {rows} FROM {table} WHERE {where_clause} LIMIT {limit}")
     row_count = 0
     for row in cursor:
         row_count += 1
         print("row: %s    %s\n" % (row_count, row))
 
 
 def make_conn_sqla(
     host: str, dbname: str, user: str, port: int, password: Optional[str] = None
 ) -> Any:
-    """The make_conn_sqla function creates a connection to the database using
-    SQLAlchemy.
+    """
+    The make_conn_sqla function creates a connection to the database using SQLAlchemy.
 
-    :param host: str: Used to Specify the host name or ip address of the
-        server.
-    :param dbname: str: Used to Specify the name of the database to
-        connect to.
-    :param user: str: Used to Specify the username for the database.
-    :param port: int: Used to Specify the port number that is used to
-        connect to the database.
-    :param password: Optional[str]=None: Used to Make the password
-        parameter optional.
-    :return: A connection object.  :doc-author: Trelent
+    :param host:str: Used to Specify the host name or ip address of the server.
+    :param dbname:str: Used to Specify the name of the database to connect to.
+    :param user:str: Used to Specify the username for the database.
+    :param port:int: Used to Specify the port number that is used to connect to the database.
+    :param password:Optional[str]=None: Used to Make the password parameter optional.
+    :return: A connection object.
+
+    :doc-author: Trelent
     """
 
     if password is None:
         password = ""
 
     conn_string = f"postgresql+psycopg2://{user}:{password}@{host}:{port}/{dbname}"
     db = create_engine(conn_string)
     conn = db.connect()
     return conn
 
 
 def get_filename_no_ext(filename: str) -> str:
-    """The get_filename_no_ext function takes a filename as input and returns
-    the filename without its extension. For example, if the input is
-    'myfile.txt', then the output will be 'myfile'.
+    """
+    The get_filename_no_ext function takes a filename as input and returns the filename without its extension.
+        For example, if the input is 'myfile.txt', then the output will be 'myfile'.
 
-    :param filename: str: Used to Pass the filename to the function.
-    :return: The filename without the extension.  :doc-author: Trelent
+    :param filename:str: Used to Pass the filename to the function.
+    :return: The filename without the extension.
+
+    :doc-author: Trelent
     """
 
     filename = filename.split(".")
     return filename[0]
```

### Comparing `amarium-0.1.7/src/amarium/encryption.py` & `amarium-0.1.8/src/amarium/encryption.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 from .utils import prepare_file_name_saving
 
 
 def decrypt_file(encrypted_file: str, private_key_path: str):
     """The decrypt_file function takes in an encrypted file and a private key,
     then decrypts the file using the private key.
 
-    :param encrypted_file: str: Used to Pass the file name of the
-        encrypted file to be decrypted.
-    :param private_key: str: Used to Read the private key file and
-        decrypt the encrypted message.
-    :return: The original message.  :doc-author: Julian M. Kleber
+    :param encrypted_file:str: Used to Pass the file name of the encrypted file to be decrypted.
+    :param private_key:str: Used to Read the private key file and decrypt the encrypted message.
+    :return: The original message.
+
+    :doc-author: Julian M. Kleber
     """
 
     with open(encrypted_file, "rb") as ecf:
         encrypted = (
             ecf.read()
         )  # From before (could have been stored then read back here)
 
@@ -49,28 +49,22 @@
 ) -> None:
     """The encrypt_file function takes a file name, public key, and optional
     in-place flag. It then encrypts the contents of the file using the provided
     public key. If in_place is True, it will overwrite the original file with
     its encrypted version. Otherwise it will create a new encrypted version of
     that file.
 
-    :param file_name:str: Used to Specify the name of the file to be
-    encrypted. :param public_key:str: Used to Specify the name of the
-    public key file. :param in_place:bool=False: Used to Determine
-    whether the file should be overwritten or not. :param save_
-    file:Optional[str]=None:
-    :param file_name: str: Used to Specify the name of the file to be
-        encrypted.
-    :param public_key: str: Used to Specify the name of the public key
-        file.
-    :param in_place: bool=False: Used to Determine whether the file
-        should be overwritten or not.
-    :param save_file: Optional[str]=None: Used to Allow the user to
-        specify a file name for saving the encrypted file.
-    :return: None.  :doc-author: Julian M. Kleber
+    :param file_name:str: Used to Specify the name of the file to be encrypted.
+    :param public_key:str: Used to Specify the name of the public key file.
+    :param in_place:bool=False: Used to Determine whether the file should be overwritten or not.
+    :param save_file:Optional[str]=None: Used to Allow the user to specify a file name for saving
+    the encrypted file.
+    :return: None.
+
+    :doc-author: Julian M. Kleber
     """
 
     with open(public_key_file, "rb") as key_file:
         public_key = serialization.load_pem_public_key(
             key_file.read(), backend=default_backend()
         )
 
@@ -96,20 +90,20 @@
 def generate_asymmetric_keys(
     key_size: int, private_key_name: str, public_key_name: str, write_secret: bool
 ) -> Tuple[bytes, bytes]:
     """The generate_asymmetric_keys function generates a private key and public
     key pair. The keys are generated using the RSA algorithm with a specified
     bit size. The keys are then written to files in PEM format.
 
-    :param key_size: int: Used to specify the size of the key that will
-        be generated.
-    :param private_key_name: str: Used to Name the private key file.
-    :param public_key_name: str: Used to specify the name of the public
-        key file.
-    :return: The private and public keys.  :doc-author: Julian M. Kleber
+    :param key_size:int: Used to specify the size of the key that will be generated.
+    :param private_key_name:str: Used to Name the private key file.
+    :param public_key_name:str: Used to specify the name of the public key file.
+    :return: The private and public keys.
+
+    :doc-author: Julian M. Kleber
     """
 
     private_key_name = prepare_file_name_saving(private_key_name)
     public_key_name = prepare_file_name_saving(public_key_name)
     private_key = rsa.generate_private_key(
         public_exponent=65537, key_size=key_size, backend=default_backend()
     )
```

### Comparing `amarium-0.1.7/src/amarium/utils.py` & `amarium-0.1.8/src/amarium/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,42 +19,28 @@
 import numpy.typing as npt
 
 from .checks import check_make_file_name_suffix, check_make_dir
 
 LOGGER = logging.getLogger(__name__)
 
 
-def read_file(file_name: str, encoding="ISO-8859-1") -> str:
-    with open(file_name, "r", encoding=encoding) as f:
-        content = f.read()
-    return content
-
-
-def write_txt_file(content: str, file_name: str, encoding: str = "ISO-8859-1"):
-    file_name = prepare_file_name_saving(file_name=file_name)
-    with open(file_name, "w", encoding=encoding) as txt_file:
-        txt_file.write(content)
-    logging.info("Wrote txt file to " + file_name)
-
-
 def prepare_file_name_saving(
     file_name: str,
     prefix: Optional[str | Type[None]] = None,
     suffix: Optional[str | Type[None]] = None,
 ) -> str:
     """The prepare_file_name_saving function takes a prefix and file name as
     input. It checks to see if the directory exists, and makes it if not. Then
     it returns the full path of the file.
 
-    :param prefix: str: Used to specify the folder where the file will
-        be saved.
-    :param file_name: str: Used to specify the name of the file to be
-        saved.
-    :return: The full path of the file name. :doc-author: Julian M.
-        Kleber
+    :param prefix:str: Used to specify the folder where the file will be saved.
+    :param file_name:str: Used to specify the name of the file to be saved.
+    :return: The full path of the file name.
+
+    :doc-author: Julian M. Kleber
     """
     if suffix == "" or suffix is None:
         file_name, suffix = os.path.splitext(file_name)
 
     if prefix == "" or prefix is None:
         prefix, file_name = os.path.split(file_name)
 
@@ -66,20 +52,20 @@
 
 def insert_string_in_file_name(file_name: str, insertion: str, suffix: str) -> str:
     """The insert_string_in_file_name function takes a file_name and inserts a
     string into the name. The insertion is placed before the extension of the
     file_name, or if there is no extension, it will be placed at the end of the
     file_name with an suffix specified by you.
 
-    :param file_name: str: Used to Specify the file name that you want
-        to insert a string into.
-    :param insertion: str: Used to Specify the string that will be
-        inserted into the file name.
-    :param suffix: str: Used to Specify the file suffix.
-    :return: A string.  :doc-author: Julian M. Kleber
+    :param file_name:str: Used to Specify the file name that you want to insert a string into.
+    :param insertion:str: Used to Specify the string that will be inserted into the file name.
+    :param suffix:str: Used to Specify the file suffix.
+    :return: A string.
+
+    :doc-author: Julian M. Kleber
     """
 
     root, ext = os.path.splitext(file_name)
 
     if suffix is None and not ext:
         raise ValueError(
             "You must either specify an suffix in the file_name or pass an suffix through the\
@@ -122,44 +108,47 @@
     return file_name
 
 
 def load_json_from_file(file_name: str) -> Dict[Any, Any]:
     """The load_json_from_file function takes a file name as input and returns
     the contents of that file in JSON format.
 
-    :param file_name: str: Used to Specify the file name of the json
-        file to be loaded.
-    :return: A dictionary of the data in the file. :doc-author: Julian
-        M. Kleber
+    :param file_name:str: Used to Specify the file name of the json file to be loaded.
+    :return: A dictionary of the data in the file.
+
+    :doc-author: Julian M. Kleber
     """
 
     with open(file_name, "r", encoding="utf-8") as json_file:
         data = dict(json.load(json_file))
     return data
 
 
 def save_json_to_file(dictionary: Dict[Any, Any], file_name: str) -> None:
     """The save_json function saves a dictionary to a json file.
 
     :param dictionary: Used to store the data that will be saved.
-    :param file_name: str=None: Used to specify a file name.
+    :param file_name:str=None: Used to specify a file name.
     :return: A string with the name of the file that was just created.
-        :doc-author: Julian M. Kleber
+
+    :doc-author: Julian M. Kleber
     """
 
     def convert(np_data: Union[npt.NDArray[Any], Type[np.generic]]) -> Any:
         """The convert function takes in a numpy object and returns the value
         of that object. If the input is an array, it will return a list of
         values. If it is not an array, it will return just the value.
 
-        :param o: Union[Type(np.ndarray): Used to Specify the type of
-            object that will be passed to the function. :param
-            Type(np.generic)]: Used to Specify the type of object that
-            is being passed into the function.
-        :return: The value of the input object.  :doc-author: Trelent
+        :param o:Union[Type(np.ndarray): Used to Specify the type of object that will be passed to
+        the function.
+        :param Type(np.generic)]: Used to Specify the type of object that is being passed into
+        the function.
+        :return: The value of the input object.
+
+        :doc-author: Trelent
         """
 
         val = None
         if isinstance(np_data, np.generic):
             val = np_data.item()
         elif isinstance(np_data, np.ndarray):
             val = list(np_data)
@@ -175,19 +164,20 @@
     time stamp in the format YYYY-MM-DD_HH:MM:SS.out.  The prefix, file_name,
     and suffix are optional arguments that can be used to specify what string
     should precede the date stamp in the file_name (prefix), what string should
     be appended after the date stamp (suffix), or both (file_name).   If no
     arguments are provided, then make_date_file_name will use default values
     for all three arguments.
 
-    :param prefix: str="": Used to ddd a prefix to the file name.
-    :param file_name: str="": Used to specify the name of the file.
-    :param suffix: str=".out": Used to specify the file extension.
-    :return: A string that is the combination of prefix, file_name and
-        suffix. :doc-author: Julian M. Kleber
+    :param prefix:str="": Used to ddd a prefix to the file name.
+    :param file_name:str="": Used to specify the name of the file.
+    :param suffix:str=".out": Used to specify the file extension.
+    :return: A string that is the combination of prefix, file_name and suffix.
+
+    :doc-author: Julian M. Kleber
     """
     time_str = time.strftime("%Y%m%d-%H%M%S" + prefix + file_name + suffix)
     return time_str
 
 
 def delete_file(file_name: str) -> None:
     """The delete_file function deletes a file from the local directory.
@@ -212,17 +202,18 @@
 
 def search_subdirs(dir_name: str) -> Tuple[List[str], List[str]]:
     """The search_subdirs function takes a directory name as input and returns
     a tuple of two lists. The first list contains all the files in the
     directory, including those in subdirectories. The second list contains all
     the subdirectories.
 
-    :param dir_name: str: Used to Specify the directory that we want to
-        search.
-    :return: A tuple of two lists.  :doc-author: Julian M. Kleber
+    :param dir_name:str: Used to Specify the directory that we want to search.
+    :return: A tuple of two lists.
+
+    :doc-author: Julian M. Kleber
     """
     if not dir_name.endswith("/"):
         dir_name += "/"
 
     result_files = []
     sub_dirs = []
     for path, subdirs, files in os.walk(dir_name):
@@ -235,19 +226,19 @@
 
 
 def write_tar(target_dir: str, file_name: str) -> None:
     """The write_tar function takes a target directory and an output name as
     arguments. It then creates a tar file with the given output name, and adds
     all files in the target directory to it.
 
-    :param target_dir: str: Used to Specify the directory that you want
-        to compress.
-    :param out_name: str: Used to Specify the name of the tar file that
-        will be created.
-    :return: None.  :doc-author: Julian M. Kleber
+    :param target_dir:str: Used to Specify the directory that you want to compress.
+    :param out_name:str: Used to Specify the name of the tar file that will be created.
+    :return: None.
+
+    :doc-author: Julian M. Kleber
     """
 
     with tarfile.open(file_name, "w") as tar:
         for root, directory, files in os.walk(target_dir):
             for file in files:
                 fullpath = os.path.join(root, file)
                 tar.add(fullpath, arcname=file)
@@ -256,19 +247,19 @@
 
 
 def copy_dir(old_dir: str, new_dir: str, overwrite=True) -> None:
     """The copy_dir function takes two arguments, old_dir and new_dir. It
     copies all files from the old directory to the new directory. If either of
     these directories do not end with a "/", it will be added.
 
-    :param old_dir: str: Used to Specify the directory that you want to
-        copy from.
-    :param new_dir: str: Used to Specify the new directory that you want
-        to copy your files into.
-    :return: None.  :doc-author: Julian M. Kleber
+    :param old_dir:str: Used to Specify the directory that you want to copy from.
+    :param new_dir:str: Used to Specify the new directory that you want to copy your files into.
+    :return: None.
+
+    :doc-author: Julian M. Kleber
     """
 
     check_make_dir(new_dir)
     if not old_dir.endswith("/"):
         old_dir += "/"
     if not new_dir.endswith("/"):
         new_dir += "/"
@@ -278,33 +269,34 @@
 
 
 def convert_str_to_bool(bool_str: str) -> None:
     """The convert_str_to_bool function takes a string and converts it to a
     boolean. The function is used in the main() function to convert the
     override value from a string to a boolean.
 
-    :param bool_str: str: Used to Specify the type of data that will be
-        passed into the function.
-    :return: None.  :doc-author: Julian M. Kleber
+    :param bool_str:str: Used to Specify the type of data that will be passed into the function.
+    :return: None.
+
+    :doc-author: Julian M. Kleber
     """
 
     if bool_str == "True":
         bool_str = True
     if bool_str == "False":
         bool_str = False
     return bool_str
 
 
-def attach_slash(raw_string: str) -> str:
-    """The attach_slash function takes a string as input and returns the same
+def append_slash(raw_string: str) -> str:
+    """The append_slash function takes a string as input and returns the same
     string with a slash appended to it. If the input already ends in a slash,
     then no change is made.
 
-    :param raw_string: str: Used to Specify the type of data that is
-        being passed into the function.
-    :return: A string with a trailing slash. :doc-author: Julian M.
-        Kleber
+    :param raw_string:str: Used to Specify the type of data that is being passed into the function.
+    :return: A string with a trailing slash.
+
+    :doc-author: Julian M. Kleber
     """
 
     if not raw_string.endswith("/"):
         raw_string += "/"
     return raw_string
```

### Comparing `amarium-0.1.7/src/amarium.egg-info/PKG-INFO` & `amarium-0.1.8/src/amarium.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amarium
-Version: 0.1.7
+Version: 0.1.8
 Summary: Filesystem handling utilities
 Author-email: "Julian M. Kleber" <julian.m.kleber@gmail.com>
 Project-URL: Homepage, https://www.codeberg.org/cap_jmk/amarium.git
 Project-URL: Bug Tracker, https://www.codeberg.org/cap_jmk/amarium.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,15 @@
 
 # Amarium
 
 [![status-badge](https://ci.codeberg.org/api/badges/cap_jmk/amarium/status.svg)](https://ci.codeberg.org/cap_jmk/amarium)
 [![Downloads](https://static.pepy.tech/personalized-badge/amarium?period=total&units=international_system&left_color=orange&right_color=blue&left_text=Downloads)](https://pepy.tech/project/amarium)
 [![License: GPL v3](https://img.shields.io/badge/License-GPL_v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 ![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C-blue)
+[![PyPI - Version](https://img.shields.io/pypi/v/amarium.svg)](https://pypi.org/project/amarium)
 
 **Table of Content**
 
 <!-- TOC -->
 - [1. Why](#1-why)
 - [2. What](#2-what)
 - [3. Usage](#3-usage)
```

### Comparing `amarium-0.1.7/tests/test_checks.py` & `amarium-0.1.8/tests/test_checks.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 import pytest
 
 from src.amarium.checks import (
     check_header_and_data,
     check_make_dir,
     check_make_file_name_suffix,
     check_delete_dir,
-    check_make_subdirs
 )
 
 
 def test_check_header_and_data():
+
     header = ["a", "b", "c"]
     data = [1, 2, 3]
     check_header_and_data(data=data, header=header)
     data = [1, 2, 3, 4]
     with pytest.raises(RuntimeError) as run_time_error:
         check_header_and_data(data=data, header=header)
 
@@ -30,26 +30,28 @@
     assert (
         str(run_time_error.value)
         == "Input data and input header do not have the same number of fields. Please ensure an appropriate data structure."
     )
 
 
 def test_check_make_dir():
+
     test_dir = "tests/test_utils"
     test_folder = "test_utils"
     check_make_dir(test_dir)
     dirs = os.listdir("tests/")
     assert test_folder in dirs
     check_make_dir(test_dir)
     os.rmdir(test_dir)
     dirs = os.listdir("tests/")
     assert test_folder not in dirs
 
 
 def test_check_file_name():
+
     file_name = "test"
     suffix = ".csv"
     res1 = check_make_file_name_suffix(file_name, suffix)
     assert res1 == file_name + suffix
 
     suffix = "csv"
     res1 = check_make_file_name_suffix(file_name, suffix)
@@ -57,28 +59,18 @@
 
     file_name = "test.csv"
     res1 = check_make_file_name_suffix(file_name)
     assert res1 == file_name
 
 
 def test_check_delete_dir():
+
     test_dir = "tests/test_utils"
     test_folder = "test_utils"
     check_make_dir(test_dir)
     dirs = os.listdir("tests/")
 
     assert test_folder in dirs
     check_delete_dir(test_dir)
     assert os.path.isdir(test_dir) == False
     check_delete_dir(test_dir)
     assert os.path.isdir(test_dir) == False
-
-
-def test_check_make_sub_dirs(): 
-
-    test_iter = ["tests", "A", "B/", "C", "D/"]
-    control = "tests/A/B/C/D/"
-    result = check_make_subdirs(test_iter)
-    assert result == control
-    assert os.path.isdir(result)
-    check_delete_dir(result)
-    assert not os.path.isdir(result)
```

### Comparing `amarium-0.1.7/tests/test_encryption.py` & `amarium-0.1.8/tests/test_encryption.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import pytest
 
 from amarium.encryption import generate_asymmetric_keys, encrypt_file, decrypt_file
 
 
 def test_asymmetric_key_generation():
+
     # case 1
     key_size = 2048
     public_key_name = "tests/public_test.pem"
     private_key_name = "tests/private_test.pem"
     if os.path.isfile(public_key_name):
         os.remove(public_key_name)
 
@@ -33,14 +34,15 @@
         write_secret=True,
     )
     assert "public_test.pem" in os.listdir("tests")
     assert "private_test.pem" in os.listdir("tests")
 
 
 def test_file_encryption():
+
     message = "Amarium is a decent library to write and read files"
 
     file_name = "test_encryption_files/test_encrypt.txt"
     if os.path.isfile(file_name):
         os.remove(file_name)
     with open(file_name, "w") as test_file:
         test_file.write(message)
@@ -60,15 +62,15 @@
 
     in_place = True
     encrypt_file(
         file_name=file_name, public_key_file=public_key_file, in_place=in_place
     )
 
 
-def test_decryption():
+def test_decryption(): 
+
     encrypted_file = "test_encryption_files/test_encrypted_test_file.txt"
     private_key_path = "tests/private_test.pem"
-
-    message = decrypt_file(
-        encrypted_file=encrypted_file, private_key_path=private_key_path
-    )
-    assert message == b"Amarium is a decent library to write and read files"
+    
+    message = decrypt_file(encrypted_file=encrypted_file, 
+    private_key_path=private_key_path)
+    assert message == b"Amarium is a decent library to write and read files"
```

### Comparing `amarium-0.1.7/tests/test_file_utils.py` & `amarium-0.1.8/tests/test_file_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,26 +9,25 @@
     prepare_file_name_saving,
     make_date_file_name,
     load_json_from_file,
     convert_str_to_bool,
     make_full_filename,
     save_json_to_file,
     search_subdirs,
-    write_txt_file,
-    attach_slash,
+    append_slash,
     delete_file,
     write_tar,
-    read_file,
     copy_dir,
 )
 
 from src.amarium.checks import check_make_file_name_suffix, check_make_dir
 
 
 def test_delete_file():
+
     file_name = "./tests/empty.txt"
     with pytest.raises(Exception) as e:
         delete_file(file_name)
 
     with open(file_name, "w") as fp:
         pass
 
@@ -95,32 +94,36 @@
     prefix = "tests/data"
     file_name = "testfile.png"
     expectation = "tests/data/testfile.png"
     make_name(prefix, file_name, expectation)
 
 
 def test_prepare_file_name_saving():
+
     # case 1
     test_dir = "tests/data"
     name = "test_file_name_saving"
     suffix = ".txt"
-    file_name = prepare_file_name_saving(prefix=test_dir, file_name=name, suffix=suffix)
+    file_name = prepare_file_name_saving(
+        prefix=test_dir, file_name=name, suffix=suffix)
     assert file_name == "tests/data/test_file_name_saving.txt"
     # case 2
     test_dir = "tests/data/"
-    file_name = prepare_file_name_saving(prefix=test_dir, file_name=name, suffix=suffix)
+    file_name = prepare_file_name_saving(
+        prefix=test_dir, file_name=name, suffix=suffix)
     assert file_name == "tests/data/test_file_name_saving.txt"
     # case 3
     file_name = "tests/data/test_file_name_saving.txt"
     file_name = prepare_file_name_saving(file_name)
     assert file_name == "tests/data/test_file_name_saving.txt"
 
 
 def test_insert_string_in_file_name():
     def make_name(file_name, insertions, suffix, expectation):
+
         new_file_name = insert_string_in_file_name(
             file_name=file_name, insertion=insertion, suffix=suffix
         )
         assert new_file_name == expectation, (
             str(file_name)
             + " old file_name "
             + str(insertion)
@@ -130,15 +133,16 @@
         )
 
     # case 1
     file_name = "foo.bar"
     insertion = "fantastic"
     suffix = None
     expectation = "foo_fantastic.bar"
-    result_name = make_name(file_name, insertion, suffix, expectation=expectation)
+    result_name = make_name(file_name, insertion,
+                            suffix, expectation=expectation)
 
     # case2
     file_name = "foo"
     suffix = ".bar"
     insertion = "fantastic"
     ending = None
     expectation = "foo_fantastic.bar"
@@ -236,83 +240,56 @@
 
     search_dir = "tests/test_dir_search"
     result_files, result_dirs = search_subdirs(dir_name=search_dir)
     check_output(result_files, result_dirs)
 
 
 def test_tar_writer():
+
     target_dir = "tests/test_dir_search"
     file_name = "tests/test.tar"
     write_tar(target_dir=target_dir, file_name=file_name)
     assert os.path.isfile(file_name)
     os.remove(file_name)
     assert not os.path.isfile(file_name)
 
 
 def test_copy_dir():
+
     import shutil
 
     target_dir = "tests/test_dir_copy"
     old_dir = "tests/test_dir_search"
     copy_dir(old_dir, new_dir=target_dir)
     assert os.path.isdir(target_dir)
     shutil.rmtree(target_dir)
     assert not os.path.isdir(target_dir)
 
 
 def test_str_convert_to_bool():
+
     test_string = "False"
     test_bool = convert_str_to_bool(test_string)
     assert test_bool is False
     test_string = "True"
     test_bool = convert_str_to_bool(test_string)
     assert test_bool is True
 
 
 def test_make_date_file_name():
+
     time_str = time.strftime("%Y%m%d-%H%M%S")
     date_file_name = make_date_file_name(prefix="", file_name="", suffix="")  #
     assert (
         date_file_name == time_str
     ), "The time strings do not match, it could be the function is too slow. That means anyways that the system is not suitable for tests."
 
 
 def test_attach_string():
-    test_string = "test_dir_or_file"
-    test_string_mod = attach_slash(test_string)
+
+    test_string ="test_dir_or_file"
+    test_string_mod = append_slash(test_string)
     assert test_string_mod == test_string + "/"
 
     test_string = "test_dir_or_file/"
-    test_string_mod = attach_slash(test_string)
-    assert test_string_mod == test_string
-
-
-def test_read_file():
-    test_string = "Testing a txt write file"
-    file_name = "tests/test_files/test.txt"
-    write_txt_file(content=test_string, file_name=file_name, encoding="utf-8")
-    res_content = read_file(file_name=file_name, encoding="utf-8")
-    assert res_content == test_string
-    delete_file(file_name=file_name)
-
-
-def test_write_txt():
-    test_string = "Testing a txt write file"
-    file_name = "tests/test_files/test.txt"
-    write_txt_file(content=test_string, file_name=file_name, encoding="utf-8")
-    res_content = read_file(file_name=file_name, encoding="utf-8")
-    assert res_content == test_string
-    delete_file(file_name=file_name)
-
-    test_string = "Testing a txt write file"
-    file_name = "tests/test_files/test.txt"
-    write_txt_file(content=test_string, file_name=file_name)
-    res_content = read_file(file_name=file_name)
-    assert res_content == test_string
-    delete_file(file_name=file_name)
-
-    test_string = "Testing a txt write file"
-    file_name = "tests/non_existent_folder/test.txt"
-    write_txt_file(content=test_string, file_name=file_name)
-    res_content = read_file(file_name=file_name)
-    assert res_content == test_string
-    delete_file(file_name=file_name)
+    test_string_mod = append_slash(test_string)
+    assert test_string_mod == test_string
```

