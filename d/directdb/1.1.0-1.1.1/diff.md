# Comparing `tmp/directdb-1.1.0.tar.gz` & `tmp/directdb-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "directdb-1.1.0.tar", last modified: Sat Aug  5 11:06:54 2023, max compression
+gzip compressed data, was "directdb-1.1.1.tar", last modified: Sat Aug  5 11:09:02 2023, max compression
```

## Comparing `directdb-1.1.0.tar` & `directdb-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 11:06:54.162307 directdb-1.1.0/
--rw-rw-rw-   0        0        0    35182 2023-07-31 07:28:41.000000 directdb-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     2546 2023-08-05 11:06:54.161308 directdb-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1806 2023-08-01 16:32:26.000000 directdb-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-05 11:06:54.151307 directdb-1.1.0/directdb/
--rw-rw-rw-   0        0        0      605 2023-08-05 11:05:15.000000 directdb-1.1.0/directdb/__init__.py
--rw-rw-rw-   0        0        0     2412 2023-08-05 11:05:04.000000 directdb-1.1.0/directdb/exceptions.py
--rw-rw-rw-   0        0        0     5828 2023-08-05 11:04:58.000000 directdb-1.1.0/directdb/main.py
--rw-rw-rw-   0        0        0     5793 2023-08-05 11:05:10.000000 directdb-1.1.0/directdb/sqlite.py
-drwxrwxrwx   0        0        0        0 2023-08-05 11:06:54.159312 directdb-1.1.0/directdb.egg-info/
--rw-rw-rw-   0        0        0     2546 2023-08-05 11:06:53.000000 directdb-1.1.0/directdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-08-05 11:06:54.000000 directdb-1.1.0/directdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 11:06:54.000000 directdb-1.1.0/directdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-08-05 11:06:54.000000 directdb-1.1.0/directdb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-05 11:06:54.000000 directdb-1.1.0/directdb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-05 11:06:54.162307 directdb-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1144 2023-08-05 11:06:12.000000 directdb-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 11:09:02.340067 directdb-1.1.1/
+-rw-rw-rw-   0        0        0    35182 2023-07-31 07:28:41.000000 directdb-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2604 2023-08-05 11:09:02.339069 directdb-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1860 2023-08-05 11:08:18.000000 directdb-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 11:09:02.333067 directdb-1.1.1/directdb/
+-rw-rw-rw-   0        0        0      605 2023-08-05 11:05:15.000000 directdb-1.1.1/directdb/__init__.py
+-rw-rw-rw-   0        0        0     2412 2023-08-05 11:05:04.000000 directdb-1.1.1/directdb/exceptions.py
+-rw-rw-rw-   0        0        0     5828 2023-08-05 11:04:58.000000 directdb-1.1.1/directdb/main.py
+-rw-rw-rw-   0        0        0     5793 2023-08-05 11:05:10.000000 directdb-1.1.1/directdb/sqlite.py
+drwxrwxrwx   0        0        0        0 2023-08-05 11:09:02.338067 directdb-1.1.1/directdb.egg-info/
+-rw-rw-rw-   0        0        0     2604 2023-08-05 11:09:02.000000 directdb-1.1.1/directdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-08-05 11:09:02.000000 directdb-1.1.1/directdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 11:09:02.000000 directdb-1.1.1/directdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-05 11:09:02.000000 directdb-1.1.1/directdb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-05 11:09:02.000000 directdb-1.1.1/directdb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 11:09:02.340067 directdb-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1144 2023-08-05 11:08:49.000000 directdb-1.1.1/setup.py
```

### Comparing `directdb-1.1.0/LICENSE` & `directdb-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `directdb-1.1.0/PKG-INFO` & `directdb-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: directdb
-Version: 1.1.0
+Version: 1.1.1
 Summary: An async package that makes database handling extremely easy!
 Author: Cannonball Chris
 Author-email: cannonballchris8@gmail.com
 Keywords: db,bot,discord bot,database,postgresql,asyncpg,async,pgutils,nosql,sqlite,aiosqlite,discord.py
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,18 @@
 
 # directdb
 
 A simple library that makes handling SQL databases in python easy without the need to understand the syntax. The library would act like an interface between your code and the database server parsing the data to SQL format.
 
 If you enjoy using this project, consider giving it a star as it helps out a ton <3
 
+Currently Supported Databases:
+- PostgreSQL
+- SQLite
+
 ## Github Repository
 
 https://github.com/cannonballchris/directdb
 
 ## Installation
 
 To install the library, use `pip install directdb`
```

### Comparing `directdb-1.1.0/README.md` & `directdb-1.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 
 # directdb
 
 A simple library that makes handling SQL databases in python easy without the need to understand the syntax. The library would act like an interface between your code and the database server parsing the data to SQL format.
 
 If you enjoy using this project, consider giving it a star as it helps out a ton <3
 
+Currently Supported Databases:
+- PostgreSQL
+- SQLite
+
 ## Github Repository
 
 https://github.com/cannonballchris/directdb
 
 ## Installation
 
 To install the library, use `pip install directdb`
```

### Comparing `directdb-1.1.0/directdb/__init__.py` & `directdb-1.1.1/directdb/__init__.py`

 * *Files identical despite different names*

### Comparing `directdb-1.1.0/directdb/exceptions.py` & `directdb-1.1.1/directdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `directdb-1.1.0/directdb/main.py` & `directdb-1.1.1/directdb/main.py`

 * *Files identical despite different names*

### Comparing `directdb-1.1.0/directdb/sqlite.py` & `directdb-1.1.1/directdb/sqlite.py`

 * *Files identical despite different names*

### Comparing `directdb-1.1.0/directdb.egg-info/PKG-INFO` & `directdb-1.1.1/directdb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: directdb
-Version: 1.1.0
+Version: 1.1.1
 Summary: An async package that makes database handling extremely easy!
 Author: Cannonball Chris
 Author-email: cannonballchris8@gmail.com
 Keywords: db,bot,discord bot,database,postgresql,asyncpg,async,pgutils,nosql,sqlite,aiosqlite,discord.py
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,18 @@
 
 # directdb
 
 A simple library that makes handling SQL databases in python easy without the need to understand the syntax. The library would act like an interface between your code and the database server parsing the data to SQL format.
 
 If you enjoy using this project, consider giving it a star as it helps out a ton <3
 
+Currently Supported Databases:
+- PostgreSQL
+- SQLite
+
 ## Github Repository
 
 https://github.com/cannonballchris/directdb
 
 ## Installation
 
 To install the library, use `pip install directdb`
```

### Comparing `directdb-1.1.0/setup.py` & `directdb-1.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import codecs
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.0'
+VERSION = '1.1.1'
 DESCRIPTION = 'An async package that makes database handling extremely easy!'
 
 # Setting up
 setup(
     name="directdb",
     version=VERSION,
     author="Cannonball Chris",
```

