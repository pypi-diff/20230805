# Comparing `tmp/directdb-1.1.1.tar.gz` & `tmp/directdb-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "directdb-1.1.1.tar", last modified: Sat Aug  5 11:09:02 2023, max compression
+gzip compressed data, was "directdb-1.1.2.tar", last modified: Sat Aug  5 12:11:07 2023, max compression
```

## Comparing `directdb-1.1.1.tar` & `directdb-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 11:09:02.340067 directdb-1.1.1/
--rw-rw-rw-   0        0        0    35182 2023-07-31 07:28:41.000000 directdb-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     2604 2023-08-05 11:09:02.339069 directdb-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1860 2023-08-05 11:08:18.000000 directdb-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-05 11:09:02.333067 directdb-1.1.1/directdb/
--rw-rw-rw-   0        0        0      605 2023-08-05 11:05:15.000000 directdb-1.1.1/directdb/__init__.py
--rw-rw-rw-   0        0        0     2412 2023-08-05 11:05:04.000000 directdb-1.1.1/directdb/exceptions.py
--rw-rw-rw-   0        0        0     5828 2023-08-05 11:04:58.000000 directdb-1.1.1/directdb/main.py
--rw-rw-rw-   0        0        0     5793 2023-08-05 11:05:10.000000 directdb-1.1.1/directdb/sqlite.py
-drwxrwxrwx   0        0        0        0 2023-08-05 11:09:02.338067 directdb-1.1.1/directdb.egg-info/
--rw-rw-rw-   0        0        0     2604 2023-08-05 11:09:02.000000 directdb-1.1.1/directdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-08-05 11:09:02.000000 directdb-1.1.1/directdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 11:09:02.000000 directdb-1.1.1/directdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-08-05 11:09:02.000000 directdb-1.1.1/directdb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-05 11:09:02.000000 directdb-1.1.1/directdb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-05 11:09:02.340067 directdb-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1144 2023-08-05 11:08:49.000000 directdb-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 12:11:07.285707 directdb-1.1.2/
+-rw-rw-rw-   0        0        0    35182 2023-07-31 07:28:41.000000 directdb-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2604 2023-08-05 12:11:07.284675 directdb-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1860 2023-08-05 11:08:18.000000 directdb-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 12:11:07.277676 directdb-1.1.2/directdb/
+-rw-rw-rw-   0        0        0      605 2023-08-05 11:05:15.000000 directdb-1.1.2/directdb/__init__.py
+-rw-rw-rw-   0        0        0     2412 2023-08-05 11:05:04.000000 directdb-1.1.2/directdb/exceptions.py
+-rw-rw-rw-   0        0        0     5828 2023-08-05 11:04:58.000000 directdb-1.1.2/directdb/main.py
+-rw-rw-rw-   0        0        0     5793 2023-08-05 11:05:10.000000 directdb-1.1.2/directdb/sqlite.py
+drwxrwxrwx   0        0        0        0 2023-08-05 12:11:07.283675 directdb-1.1.2/directdb.egg-info/
+-rw-rw-rw-   0        0        0     2604 2023-08-05 12:11:07.000000 directdb-1.1.2/directdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-08-05 12:11:07.000000 directdb-1.1.2/directdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 12:11:07.000000 directdb-1.1.2/directdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-08-05 12:11:07.000000 directdb-1.1.2/directdb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-05 12:11:07.000000 directdb-1.1.2/directdb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 12:11:07.285707 directdb-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1157 2023-08-05 12:10:51.000000 directdb-1.1.2/setup.py
```

### Comparing `directdb-1.1.1/LICENSE` & `directdb-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `directdb-1.1.1/PKG-INFO` & `directdb-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: directdb
-Version: 1.1.1
+Version: 1.1.2
 Summary: An async package that makes database handling extremely easy!
 Author: Cannonball Chris
 Author-email: cannonballchris8@gmail.com
 Keywords: db,bot,discord bot,database,postgresql,asyncpg,async,pgutils,nosql,sqlite,aiosqlite,discord.py
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `directdb-1.1.1/README.md` & `directdb-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `directdb-1.1.1/directdb/__init__.py` & `directdb-1.1.2/directdb/__init__.py`

 * *Files identical despite different names*

### Comparing `directdb-1.1.1/directdb/exceptions.py` & `directdb-1.1.2/directdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `directdb-1.1.1/directdb/main.py` & `directdb-1.1.2/directdb/main.py`

 * *Files identical despite different names*

### Comparing `directdb-1.1.1/directdb/sqlite.py` & `directdb-1.1.2/directdb/sqlite.py`

 * *Files identical despite different names*

### Comparing `directdb-1.1.1/directdb.egg-info/PKG-INFO` & `directdb-1.1.2/directdb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: directdb
-Version: 1.1.1
+Version: 1.1.2
 Summary: An async package that makes database handling extremely easy!
 Author: Cannonball Chris
 Author-email: cannonballchris8@gmail.com
 Keywords: db,bot,discord bot,database,postgresql,asyncpg,async,pgutils,nosql,sqlite,aiosqlite,discord.py
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `directdb-1.1.1/setup.py` & `directdb-1.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 import codecs
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.1'
+VERSION = '1.1.2'
 DESCRIPTION = 'An async package that makes database handling extremely easy!'
 
 # Setting up
 setup(
     name="directdb",
     version=VERSION,
     author="Cannonball Chris",
     author_email="cannonballchris8@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['asyncpg'],
+    install_requires=['asyncpg', 'aiosqlite'],
     keywords=['db', 'bot', 'discord bot', 'database', 'postgresql', 'asyncpg', 'async', 'pgutils', 'nosql', 'sqlite', 'aiosqlite', 'discord.py'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

