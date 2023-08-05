# Comparing `tmp/YzDB-0.0.1.tar.gz` & `tmp/YzDB-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YzDB-0.0.1.tar", last modified: Fri Jul 28 05:30:24 2023, max compression
+gzip compressed data, was "YzDB-0.0.2.tar", last modified: Sat Aug  5 07:58:46 2023, max compression
```

## Comparing `YzDB-0.0.1.tar` & `YzDB-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 yanzhong   (501) staff       (20)        0 2023-07-28 05:30:24.871947 YzDB-0.0.1/
--rw-r--r--   0 yanzhong   (501) staff       (20)     1070 2023-07-22 08:12:08.000000 YzDB-0.0.1/LICENSE
--rw-r--r--   0 yanzhong   (501) staff       (20)     2336 2023-07-28 05:30:24.871802 YzDB-0.0.1/PKG-INFO
--rw-r--r--   0 yanzhong   (501) staff       (20)     1913 2023-07-28 04:09:14.000000 YzDB-0.0.1/README.md
-drwxr-xr-x   0 yanzhong   (501) staff       (20)        0 2023-07-28 05:30:24.870597 YzDB-0.0.1/YzDB/
--rw-r--r--   0 yanzhong   (501) staff       (20)       56 2023-07-28 03:46:10.000000 YzDB-0.0.1/YzDB/__init__.py
--rw-r--r--   0 yanzhong   (501) staff       (20)     1571 2023-07-28 05:26:23.000000 YzDB-0.0.1/YzDB/conn_mysql.py
--rw-r--r--   0 yanzhong   (501) staff       (20)     2205 2023-07-27 10:01:43.000000 YzDB-0.0.1/YzDB/db_base.py
-drwxr-xr-x   0 yanzhong   (501) staff       (20)        0 2023-07-28 05:30:24.871224 YzDB-0.0.1/YzDB.egg-info/
--rw-r--r--   0 yanzhong   (501) staff       (20)     2336 2023-07-28 05:30:24.000000 YzDB-0.0.1/YzDB.egg-info/PKG-INFO
--rw-r--r--   0 yanzhong   (501) staff       (20)      426 2023-07-28 05:30:24.000000 YzDB-0.0.1/YzDB.egg-info/SOURCES.txt
--rw-r--r--   0 yanzhong   (501) staff       (20)        1 2023-07-28 05:30:24.000000 YzDB-0.0.1/YzDB.egg-info/dependency_links.txt
--rw-r--r--   0 yanzhong   (501) staff       (20)       78 2023-07-28 05:30:24.000000 YzDB-0.0.1/YzDB.egg-info/requires.txt
--rw-r--r--   0 yanzhong   (501) staff       (20)        5 2023-07-28 05:30:24.000000 YzDB-0.0.1/YzDB.egg-info/top_level.txt
--rw-r--r--   0 yanzhong   (501) staff       (20)       38 2023-07-28 05:30:24.872004 YzDB-0.0.1/setup.cfg
--rw-r--r--   0 yanzhong   (501) staff       (20)      977 2023-07-28 05:29:53.000000 YzDB-0.0.1/setup.py
-drwxr-xr-x   0 yanzhong   (501) staff       (20)        0 2023-07-28 05:30:24.871454 YzDB-0.0.1/tests/
--rw-r--r--   0 yanzhong   (501) staff       (20)     3760 2023-07-27 09:31:19.000000 YzDB-0.0.1/tests/test_db_base.py
--rw-r--r--   0 yanzhong   (501) staff       (20)     2699 2023-07-28 03:04:44.000000 YzDB-0.0.1/tests/test_mysql_operations.py
+drwxr-xr-x   0 huangyanzhong   (501) staff       (20)        0 2023-08-05 07:58:46.169814 YzDB-0.0.2/
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)     1070 2023-08-05 06:44:36.000000 YzDB-0.0.2/LICENSE
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)     2336 2023-08-05 07:58:46.169692 YzDB-0.0.2/PKG-INFO
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)     1913 2023-08-05 06:44:36.000000 YzDB-0.0.2/README.md
+drwxr-xr-x   0 huangyanzhong   (501) staff       (20)        0 2023-08-05 07:58:46.168599 YzDB-0.0.2/YzDB.egg-info/
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)     2336 2023-08-05 07:58:46.000000 YzDB-0.0.2/YzDB.egg-info/PKG-INFO
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)      322 2023-08-05 07:58:46.000000 YzDB-0.0.2/YzDB.egg-info/SOURCES.txt
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)        1 2023-08-05 07:58:46.000000 YzDB-0.0.2/YzDB.egg-info/dependency_links.txt
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)       78 2023-08-05 07:58:46.000000 YzDB-0.0.2/YzDB.egg-info/requires.txt
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)        5 2023-08-05 07:58:46.000000 YzDB-0.0.2/YzDB.egg-info/top_level.txt
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)       38 2023-08-05 07:58:46.169854 YzDB-0.0.2/setup.cfg
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)      977 2023-08-05 07:58:02.000000 YzDB-0.0.2/setup.py
+drwxr-xr-x   0 huangyanzhong   (501) staff       (20)        0 2023-08-05 07:58:46.168996 YzDB-0.0.2/tests/
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)     3760 2023-08-05 07:34:44.000000 YzDB-0.0.2/tests/test_db_base.py
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)     2699 2023-08-05 07:34:31.000000 YzDB-0.0.2/tests/test_mysql_operations.py
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)        0 2023-08-05 07:36:29.000000 YzDB-0.0.2/tests/test_sqlite_operations.py
+drwxr-xr-x   0 huangyanzhong   (501) staff       (20)        0 2023-08-05 07:58:46.169500 YzDB-0.0.2/yzdb/
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)      116 2023-08-05 07:57:43.000000 YzDB-0.0.2/yzdb/__init__.py
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)     1571 2023-08-05 07:51:42.000000 YzDB-0.0.2/yzdb/conn_mysql.py
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)      975 2023-08-05 07:57:30.000000 YzDB-0.0.2/yzdb/conn_sqlite.py
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)     2490 2023-08-05 07:30:39.000000 YzDB-0.0.2/yzdb/db_base.py
```

### Comparing `YzDB-0.0.1/LICENSE` & `YzDB-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `YzDB-0.0.1/PKG-INFO` & `YzDB-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YzDB
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for easy using database
 Home-page: https://github.com/Yanzhong-Hub/yzdb
 Author: Yanzhong Huang
 Author-email: yanzhong.huang@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `YzDB-0.0.1/README.md` & `YzDB-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `YzDB-0.0.1/YzDB/conn_mysql.py` & `YzDB-0.0.2/yzdb/conn_mysql.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 连接模块，外部调用接口
 """
 
-from YzDB.db_base import MySQLBase
+from yzdb.db_base import MySQLBase
 
-from YzDB.operations.add_mysql import AddDBMySQL, AddTableMySQL
-from YzDB.operations.drop_mysql import DropDBMySQL, DropTableMySQL
-from YzDB.operations.modify_mysql import ModifyDBMySQL, ModifyTableMySQL 
-from YzDB.operations.query_mysql import QueryDBMySQL, QueryTableMySQL 
+from yzdb.operations.add_mysql import AddDBMySQL, AddTableMySQL
+from yzdb.operations.drop_mysql import DropDBMySQL, DropTableMySQL
+from yzdb.operations.modify_mysql import ModifyDBMySQL, ModifyTableMySQL 
+from yzdb.operations.query_mysql import QueryDBMySQL, QueryTableMySQL 
 
 
 class MySQLConn(MySQLBase,
                 AddDBMySQL, AddTableMySQL,
                 DropDBMySQL, DropTableMySQL,
                 ModifyDBMySQL, ModifyTableMySQL,
                 QueryDBMySQL, QueryTableMySQL):
```

### Comparing `YzDB-0.0.1/YzDB/db_base.py` & `YzDB-0.0.2/yzdb/db_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,31 @@
 数据库连接
 """
 
 from sqlalchemy import create_engine, text
 
 from sqlalchemy import Engine, Connection
 from abc import ABC, abstractmethod
-from typing import Any
+from typing import Any, Self
 
 
 class DBbase(ABC):
     """
     数据库连接基类
     """
+    __instance: Self | None = None
 
+    
+    def __new__(cls, *args, **kwargs) -> Self:  # type: ignore
+        if cls.__instance is None:
+            cls.__instance = super().__new__(cls)
+            return cls.__instance
+        else:
+            return cls.__instance
+        
     @abstractmethod
     def create_engine(self) -> Engine:
         ...
 
     def __init__(self) -> None:
         self.engine: Engine = self.create_engine()
```

### Comparing `YzDB-0.0.1/YzDB.egg-info/PKG-INFO` & `YzDB-0.0.2/YzDB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YzDB
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for easy using database
 Home-page: https://github.com/Yanzhong-Hub/yzdb
 Author: Yanzhong Huang
 Author-email: yanzhong.huang@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `YzDB-0.0.1/setup.py` & `YzDB-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # requirements
 with open("requirements.txt", "r") as f:
     requirements = f.read()
     requirements = requirements.split("\n")
 
 setup(
     name="YzDB",  # Need modify
-    version="0.0.1",  # Need modify
+    version="0.0.2",  # Need modify
     author="Yanzhong Huang",
     author_email="yanzhong.huang@outlook.com",
     description="A package for easy using database",  # Need modify
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Yanzhong-Hub/yzdb",  # Need modify
     packages=find_packages(),
```

### Comparing `YzDB-0.0.1/tests/test_db_base.py` & `YzDB-0.0.2/tests/test_db_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from YzDB.db_base import MySQLBase, SQLiteBase
+from yzdb.db_base import MySQLBase, SQLiteBase
 
 
 class TestMYSQLBase(unittest.TestCase):
     
     def test_execute(self):
         """测试execute方法"""
```

### Comparing `YzDB-0.0.1/tests/test_mysql_operations.py` & `YzDB-0.0.2/tests/test_mysql_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 
-from YzDB.db_base import MySQLBase
-from YzDB.operations.add_mysql import AddDBMySQL, AddTableMySQL
+from yzdb.db_base import MySQLBase
+from yzdb.operations.add_mysql import AddDBMySQL, AddTableMySQL
 
 class TestAddDBMySQL(unittest.TestCase):
 
     def test_add_db(self):
         # prepare
         mysql_base = MySQLBase(
             host='localhost',
```

