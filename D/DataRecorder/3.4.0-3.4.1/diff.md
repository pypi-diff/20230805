# Comparing `tmp/DataRecorder-3.4.0.tar.gz` & `tmp/DataRecorder-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DataRecorder-3.4.0.tar", last modified: Fri Aug  4 03:26:43 2023, max compression
+gzip compressed data, was "DataRecorder-3.4.1.tar", last modified: Sat Aug  5 04:34:32 2023, max compression
```

## Comparing `DataRecorder-3.4.0.tar` & `DataRecorder-3.4.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 03:26:43.864414 DataRecorder-3.4.0/
-drwxrwxrwx   0        0        0        0 2023-08-04 03:26:43.833138 DataRecorder-3.4.0/DataRecorder/
--rw-rw-rw-   0        0        0      138 2023-08-04 02:16:31.000000 DataRecorder-3.4.0/DataRecorder/__init__.py
--rw-rw-rw-   0        0        0     7043 2023-07-28 02:58:36.000000 DataRecorder-3.4.0/DataRecorder/base.py
--rw-rw-rw-   0        0        0     1967 2023-07-28 09:31:11.000000 DataRecorder-3.4.0/DataRecorder/base.pyi
--rw-rw-rw-   0        0        0     1721 2023-07-27 01:10:40.000000 DataRecorder-3.4.0/DataRecorder/byte_recorder.py
--rw-rw-rw-   0        0        0      487 2023-07-28 09:31:11.000000 DataRecorder-3.4.0/DataRecorder/byte_recorder.pyi
--rw-rw-rw-   0        0        0     5155 2023-07-28 09:42:09.000000 DataRecorder-3.4.0/DataRecorder/db_recorder.py
--rw-rw-rw-   0        0        0      929 2023-07-28 09:40:20.000000 DataRecorder-3.4.0/DataRecorder/db_recorder.pyi
--rw-rw-rw-   0        0        0    15875 2023-08-04 02:16:31.000000 DataRecorder-3.4.0/DataRecorder/filler.py
--rw-rw-rw-   0        0        0     2266 2023-08-04 02:16:31.000000 DataRecorder-3.4.0/DataRecorder/filler.pyi
--rw-rw-rw-   0        0        0     6488 2023-08-04 02:16:31.000000 DataRecorder-3.4.0/DataRecorder/recorder.py
--rw-rw-rw-   0        0        0      893 2023-08-04 02:16:31.000000 DataRecorder-3.4.0/DataRecorder/recorder.pyi
--rw-rw-rw-   0        0        0    11628 2023-08-03 00:50:54.000000 DataRecorder-3.4.0/DataRecorder/setter.py
--rw-rw-rw-   0        0        0     2839 2023-07-28 09:28:37.000000 DataRecorder-3.4.0/DataRecorder/setter.pyI
-drwxrwxrwx   0        0        0        0 2023-08-04 03:26:43.864414 DataRecorder-3.4.0/DataRecorder/style/
--rw-rw-rw-   0        0        0       77 2023-08-04 02:16:31.000000 DataRecorder-3.4.0/DataRecorder/style/__init__.py
--rw-rw-rw-   0        0        0    28558 2023-08-04 03:25:26.000000 DataRecorder-3.4.0/DataRecorder/style/cell_style.py
--rw-rw-rw-   0        0        0     8328 2023-08-03 01:26:58.000000 DataRecorder-3.4.0/DataRecorder/tools.py
--rw-rw-rw-   0        0        0      915 2023-07-28 09:42:09.000000 DataRecorder-3.4.0/DataRecorder/tools.pyi
-drwxrwxrwx   0        0        0        0 2023-08-04 03:26:43.864414 DataRecorder-3.4.0/DataRecorder.egg-info/
--rw-rw-rw-   0        0        0     4961 2023-08-04 03:26:43.000000 DataRecorder-3.4.0/DataRecorder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      657 2023-08-04 03:26:43.000000 DataRecorder-3.4.0/DataRecorder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 03:26:43.000000 DataRecorder-3.4.0/DataRecorder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-04 03:26:43.000000 DataRecorder-3.4.0/DataRecorder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-08-04 03:26:43.000000 DataRecorder-3.4.0/DataRecorder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2021-08-17 07:03:54.000000 DataRecorder-3.4.0/LICENSE
--rw-rw-rw-   0        0        0       26 2023-04-28 02:15:42.000000 DataRecorder-3.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4961 2023-08-04 03:26:43.864414 DataRecorder-3.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     4462 2023-05-26 08:55:32.000000 DataRecorder-3.4.0/README.md
--rw-rw-rw-   0        0        0       42 2023-08-04 03:26:43.864414 DataRecorder-3.4.0/setup.cfg
--rw-rw-rw-   0        0        0      863 2023-07-27 01:16:42.000000 DataRecorder-3.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 04:34:32.273028 DataRecorder-3.4.1/
+drwxrwxrwx   0        0        0        0 2023-08-05 04:34:32.258514 DataRecorder-3.4.1/DataRecorder/
+-rw-rw-rw-   0        0        0      138 2023-08-05 02:21:57.000000 DataRecorder-3.4.1/DataRecorder/__init__.py
+-rw-rw-rw-   0        0        0     7043 2023-07-31 14:26:40.000000 DataRecorder-3.4.1/DataRecorder/base.py
+-rw-rw-rw-   0        0        0     1967 2023-07-31 14:26:40.000000 DataRecorder-3.4.1/DataRecorder/base.pyi
+-rw-rw-rw-   0        0        0     1721 2023-07-31 14:26:40.000000 DataRecorder-3.4.1/DataRecorder/byte_recorder.py
+-rw-rw-rw-   0        0        0      487 2023-07-31 14:26:40.000000 DataRecorder-3.4.1/DataRecorder/byte_recorder.pyi
+-rw-rw-rw-   0        0        0     5360 2023-08-05 04:20:45.000000 DataRecorder-3.4.1/DataRecorder/db_recorder.py
+-rw-rw-rw-   0        0        0      929 2023-07-31 14:26:40.000000 DataRecorder-3.4.1/DataRecorder/db_recorder.pyi
+-rw-rw-rw-   0        0        0    15875 2023-08-05 02:21:57.000000 DataRecorder-3.4.1/DataRecorder/filler.py
+-rw-rw-rw-   0        0        0     2266 2023-08-05 02:21:57.000000 DataRecorder-3.4.1/DataRecorder/filler.pyi
+-rw-rw-rw-   0        0        0     6488 2023-08-05 02:21:57.000000 DataRecorder-3.4.1/DataRecorder/recorder.py
+-rw-rw-rw-   0        0        0      893 2023-08-05 02:21:57.000000 DataRecorder-3.4.1/DataRecorder/recorder.pyi
+-rw-rw-rw-   0        0        0    11628 2023-08-02 15:43:22.000000 DataRecorder-3.4.1/DataRecorder/setter.py
+-rw-rw-rw-   0        0        0     2839 2023-07-31 14:26:40.000000 DataRecorder-3.4.1/DataRecorder/setter.pyI
+drwxrwxrwx   0        0        0        0 2023-08-05 04:34:32.273028 DataRecorder-3.4.1/DataRecorder/style/
+-rw-rw-rw-   0        0        0       77 2023-08-05 02:21:57.000000 DataRecorder-3.4.1/DataRecorder/style/__init__.py
+-rw-rw-rw-   0        0        0    28558 2023-08-05 02:21:57.000000 DataRecorder-3.4.1/DataRecorder/style/cell_style.py
+-rw-rw-rw-   0        0        0     8328 2023-07-31 14:26:40.000000 DataRecorder-3.4.1/DataRecorder/tools.py
+-rw-rw-rw-   0        0        0      915 2023-07-31 14:26:40.000000 DataRecorder-3.4.1/DataRecorder/tools.pyi
+drwxrwxrwx   0        0        0        0 2023-08-05 04:34:32.271823 DataRecorder-3.4.1/DataRecorder.egg-info/
+-rw-rw-rw-   0        0        0     4961 2023-08-05 04:34:32.000000 DataRecorder-3.4.1/DataRecorder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      657 2023-08-05 04:34:32.000000 DataRecorder-3.4.1/DataRecorder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 04:34:32.000000 DataRecorder-3.4.1/DataRecorder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-05 04:34:32.000000 DataRecorder-3.4.1/DataRecorder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-05 04:34:32.000000 DataRecorder-3.4.1/DataRecorder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2022-01-26 11:22:47.000000 DataRecorder-3.4.1/LICENSE
+-rw-rw-rw-   0        0        0       26 2023-03-26 03:46:04.000000 DataRecorder-3.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4961 2023-08-05 04:34:32.273028 DataRecorder-3.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4462 2023-05-25 16:24:32.000000 DataRecorder-3.4.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-05 04:34:32.273028 DataRecorder-3.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      863 2023-08-05 04:23:24.000000 DataRecorder-3.4.1/setup.py
```

### Comparing `DataRecorder-3.4.0/DataRecorder/base.py` & `DataRecorder-3.4.1/DataRecorder/base.py`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.0/DataRecorder/base.pyi` & `DataRecorder-3.4.1/DataRecorder/base.pyi`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.0/DataRecorder/byte_recorder.py` & `DataRecorder-3.4.1/DataRecorder/byte_recorder.py`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.0/DataRecorder/db_recorder.py` & `DataRecorder-3.4.1/DataRecorder/db_recorder.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,38 +103,41 @@
                 name, cols = _create_table(self._cur, table, d)
                 tables[table] = cols
 
             now_data = (data,) if not isinstance(data[0], (list, tuple, dict)) else data
 
             for d in now_data:
                 long = len(d)
-                v = ','.join('?' * long)
                 if isinstance(d, dict):
+                    question_masks = ','.join('?' * long)
                     d = data_to_list_or_dict(self, d)
                     keys = d.keys()
 
                     for key in keys:  # 检查是否要新增列
                         if key not in tables[table]:
                             sql = f'ALTER TABLE {table} ADD COLUMN {key}'
                             self._cur.execute(sql)
                             tables[table].append(key)
 
                     keys_txt = ','.join(keys)
-                    values = d.values()
-                    sql = f'INSERT INTO {table} ({keys_txt}) values ({v})'
+                    values = list(d.values())
+                    sql = f'INSERT INTO {table} ({keys_txt}) values ({question_masks})'
 
                 else:
                     d = self._data_to_list(d)
-                    if long > len(tables[table]):
+                    cols_num = len(tables[table])
+                    if long > cols_num:
                         raise RuntimeError('数据个数大于列数。')
+                    d.extend([None] * (cols_num - long))
+                    question_masks = ','.join('?' * cols_num)
 
                     values = d
-                    sql = f'INSERT INTO {table} values ({v})'
+                    sql = f'INSERT INTO {table} values ({question_masks})'
 
-                self._cur.execute(sql, list(values))
+                self._cur.execute(sql, values)
 
         self._conn.commit()
 
 
 def _create_table(cursor, table_name: str, data: dict) -> tuple:
     """创建表格
     :param cursor: 数据库游标对象
```

### Comparing `DataRecorder-3.4.0/DataRecorder/db_recorder.pyi` & `DataRecorder-3.4.1/DataRecorder/db_recorder.pyi`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.0/DataRecorder/filler.py` & `DataRecorder-3.4.1/DataRecorder/filler.py`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.0/DataRecorder/filler.pyi` & `DataRecorder-3.4.1/DataRecorder/filler.pyi`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.0/DataRecorder/recorder.py` & `DataRecorder-3.4.1/DataRecorder/recorder.py`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.0/DataRecorder/recorder.pyi` & `DataRecorder-3.4.1/DataRecorder/recorder.pyi`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.0/DataRecorder/setter.py` & `DataRecorder-3.4.1/DataRecorder/setter.py`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.0/DataRecorder/setter.pyI` & `DataRecorder-3.4.1/DataRecorder/setter.pyI`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.0/DataRecorder/style/cell_style.py` & `DataRecorder-3.4.1/DataRecorder/style/cell_style.py`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.0/DataRecorder/tools.py` & `DataRecorder-3.4.1/DataRecorder/tools.py`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.0/DataRecorder/tools.pyi` & `DataRecorder-3.4.1/DataRecorder/tools.pyi`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.0/DataRecorder.egg-info/PKG-INFO` & `DataRecorder-3.4.1/DataRecorder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataRecorder
-Version: 3.4.0
+Version: 3.4.1
 Summary: 用于记录数据的模块。
 Home-page: https://gitee.com/g1879/DataRecorder
 Author: g1879
 Author-email: g1879@qq.com
 License: MIT
 Keywords: DataRecorder
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `DataRecorder-3.4.0/DataRecorder.egg-info/SOURCES.txt` & `DataRecorder-3.4.1/DataRecorder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.0/LICENSE` & `DataRecorder-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.0/PKG-INFO` & `DataRecorder-3.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataRecorder
-Version: 3.4.0
+Version: 3.4.1
 Summary: 用于记录数据的模块。
 Home-page: https://gitee.com/g1879/DataRecorder
 Author: g1879
 Author-email: g1879@qq.com
 License: MIT
 Keywords: DataRecorder
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `DataRecorder-3.4.0/README.md` & `DataRecorder-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.0/setup.py` & `DataRecorder-3.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="DataRecorder",
-    version="3.4.0",
+    version="3.4.1",
     author="g1879",
     author_email="g1879@qq.com",
     description="用于记录数据的模块。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     keywords="DataRecorder",
```

