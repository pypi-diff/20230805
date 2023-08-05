# Comparing `tmp/directdb-1.0.1.tar.gz` & `tmp/directdb-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "directdb-1.0.1.tar", last modified: Tue Aug  1 16:36:11 2023, max compression
+gzip compressed data, was "directdb-1.1.0.tar", last modified: Sat Aug  5 11:06:54 2023, max compression
```

## Comparing `directdb-1.0.1.tar` & `directdb-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 16:36:11.407807 directdb-1.0.1/
--rw-rw-rw-   0        0        0    35182 2023-07-31 07:28:41.000000 directdb-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2525 2023-08-01 16:36:11.406811 directdb-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1806 2023-08-01 16:32:26.000000 directdb-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 16:36:11.397810 directdb-1.0.1/directdb/
--rw-rw-rw-   0        0        0      536 2023-08-01 16:35:34.000000 directdb-1.0.1/directdb/__init__.py
--rw-rw-rw-   0        0        0     2371 2023-08-01 16:35:28.000000 directdb-1.0.1/directdb/exceptions.py
--rw-rw-rw-   0        0        0     5223 2023-08-01 16:35:16.000000 directdb-1.0.1/directdb/main.py
-drwxrwxrwx   0        0        0        0 2023-08-01 16:36:11.404807 directdb-1.0.1/directdb.egg-info/
--rw-rw-rw-   0        0        0     2525 2023-08-01 16:36:11.000000 directdb-1.0.1/directdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-08-01 16:36:11.000000 directdb-1.0.1/directdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 16:36:11.000000 directdb-1.0.1/directdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-08-01 16:36:11.000000 directdb-1.0.1/directdb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-01 16:36:11.000000 directdb-1.0.1/directdb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 16:36:11.407807 directdb-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1117 2023-08-01 14:43:36.000000 directdb-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 11:06:54.162307 directdb-1.1.0/
+-rw-rw-rw-   0        0        0    35182 2023-07-31 07:28:41.000000 directdb-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2546 2023-08-05 11:06:54.161308 directdb-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1806 2023-08-01 16:32:26.000000 directdb-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 11:06:54.151307 directdb-1.1.0/directdb/
+-rw-rw-rw-   0        0        0      605 2023-08-05 11:05:15.000000 directdb-1.1.0/directdb/__init__.py
+-rw-rw-rw-   0        0        0     2412 2023-08-05 11:05:04.000000 directdb-1.1.0/directdb/exceptions.py
+-rw-rw-rw-   0        0        0     5828 2023-08-05 11:04:58.000000 directdb-1.1.0/directdb/main.py
+-rw-rw-rw-   0        0        0     5793 2023-08-05 11:05:10.000000 directdb-1.1.0/directdb/sqlite.py
+drwxrwxrwx   0        0        0        0 2023-08-05 11:06:54.159312 directdb-1.1.0/directdb.egg-info/
+-rw-rw-rw-   0        0        0     2546 2023-08-05 11:06:53.000000 directdb-1.1.0/directdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-08-05 11:06:54.000000 directdb-1.1.0/directdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 11:06:54.000000 directdb-1.1.0/directdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-05 11:06:54.000000 directdb-1.1.0/directdb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-05 11:06:54.000000 directdb-1.1.0/directdb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 11:06:54.162307 directdb-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1144 2023-08-05 11:06:12.000000 directdb-1.1.0/setup.py
```

### Comparing `directdb-1.0.1/LICENSE` & `directdb-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `directdb-1.0.1/PKG-INFO` & `directdb-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: directdb
-Version: 1.0.1
+Version: 1.1.0
 Summary: An async package that makes database handling extremely easy!
 Author: Cannonball Chris
 Author-email: cannonballchris8@gmail.com
-Keywords: db,bot,discord bot,database,postgresql,asyncpg,async,pgutils,nosql,sqlite
+Keywords: db,bot,discord bot,database,postgresql,asyncpg,async,pgutils,nosql,sqlite,aiosqlite,discord.py
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `directdb-1.0.1/README.md` & `directdb-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `directdb-1.0.1/directdb/__init__.py` & `directdb-1.1.0/directdb/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # LICENSE
 # -----------------------------------------------------------------------
+# Copyright (c) CannonBall Chris,  2023
 # directdb is distributed under the terms of the GNU Affero General Public License (AGPL).
 # You can find a copy of the license in the LICENSE file included with this distribution.
 # The AGPL is a copyleft license that ensures the freedom to use, modify, and distribute the library's code, even in the case of web-based services.
 # By using directdb, you agree to comply with the terms and conditions of the AGPL.
 
 from .main import Postgresql
+from .sqlite import SQLite
```

### Comparing `directdb-1.0.1/directdb/exceptions.py` & `directdb-1.1.0/directdb/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # LICENSE
 # -----------------------------------------------------------------------
+# Copyright (c) CannonBall Chris,  2023
 # directdb is distributed under the terms of the GNU Affero General Public License (AGPL).
 # You can find a copy of the license in the LICENSE file included with this distribution.
 # The AGPL is a copyleft license that ensures the freedom to use, modify, and distribute the library's code, even in the case of web-based services.
 # By using directdb, you agree to comply with the terms and conditions of the AGPL.
 
 import datetime
```

### Comparing `directdb-1.0.1/directdb/main.py` & `directdb-1.1.0/directdb/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # LICENSE
 # -----------------------------------------------------------------------
+# Copyright (c) CannonBall Chris,  2023
 # directdb is distributed under the terms of the GNU Affero General Public License (AGPL).
 # You can find a copy of the license in the LICENSE file included with this distribution.
 # The AGPL is a copyleft license that ensures the freedom to use, modify, and distribute the library's code, even in the case of web-based services.
 # By using directdb, you agree to comply with the terms and conditions of the AGPL.
 
 import asyncio
 
@@ -103,37 +104,51 @@
 			columns = ', '.join(data.keys())
 			values = ', '.join(['${}'.format(i + 1) for i in range(len(data))])
 			query = 'INSERT INTO {} ({}) VALUES ({})'.format(table, columns, values)
 			await self.pool.execute(query, *data.values())
 		except Exception as e:
 			raise DatabaseInsertionException(e)
 
-	async def fetch(self, table:str, *, data_filter:dict = None) -> list:
+	async def fetch(self, table:str, *, data_filter:dict = None, **sorting) -> list:
 		""" Fetches data from the database.
 		
 		Parameters
 		----------
 		table: str
 			The table to fetch data from.
 		data_filter: dict [Optional]
 			The data_filter to use in format {'column name':data}.
+		sort_by: str
+			The column to sort the data by.The data which will be sorted will be always in descending order.
+		sort : str
+			The order to sort the data by. Can be either 'ASC' or 'DESC'.
 
 		Returns
 		-------
 		list
 			A list of data fetched from the database.
 
 		"""
 		try:
 			if not data_filter:
 				query = 'SELECT * FROM {}'.format(table)
+				if sorting:
+					sort_by = sorting.get('sort_by', None)
+					sort = sorting.get('sort', None)
+					if sort_by and sort:
+						query += ' ORDER BY {} {}'.format(sort_by, sort)
 				return await self.pool.fetch(query)
 			else:
 				data_filters = ' AND '.join(['{} = ${}'.format(column, i + 1) for i, column in enumerate(data_filter)])
 				query = 'SELECT * FROM {} WHERE {}'.format(table, data_filters)
+				if sorting:
+					sort_by = sorting.get('sort_by')
+					sort = sorting.get('sort')
+					if sort_by and sort:
+						query += ' ORDER BY {} {}'.format(sort_by, sort)
 				return await self.pool.fetch(query, *data_filter.values())
 
 		except Exception as e:
 			raise DatabaseFetchException(e)
 
 	async def update(self, table:str, data:dict, data_filter:dict) -> None:
 		""" Updates data in the database.
```

### Comparing `directdb-1.0.1/directdb.egg-info/PKG-INFO` & `directdb-1.1.0/directdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: directdb
-Version: 1.0.1
+Version: 1.1.0
 Summary: An async package that makes database handling extremely easy!
 Author: Cannonball Chris
 Author-email: cannonballchris8@gmail.com
-Keywords: db,bot,discord bot,database,postgresql,asyncpg,async,pgutils,nosql,sqlite
+Keywords: db,bot,discord bot,database,postgresql,asyncpg,async,pgutils,nosql,sqlite,aiosqlite,discord.py
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `directdb-1.0.1/setup.py` & `directdb-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import codecs
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.1'
+VERSION = '1.1.0'
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
     install_requires=['asyncpg'],
-    keywords=['db', 'bot', 'discord bot', 'database', 'postgresql', 'asyncpg', 'async', 'pgutils', 'nosql', 'sqlite'],
+    keywords=['db', 'bot', 'discord bot', 'database', 'postgresql', 'asyncpg', 'async', 'pgutils', 'nosql', 'sqlite', 'aiosqlite', 'discord.py'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

