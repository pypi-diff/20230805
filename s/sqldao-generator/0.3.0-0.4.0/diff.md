# Comparing `tmp/sqldao-generator-0.3.0.tar.gz` & `tmp/sqldao-generator-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqldao-generator-0.3.0.tar", last modified: Sun Jul 16 06:59:18 2023, max compression
+gzip compressed data, was "sqldao-generator-0.4.0.tar", last modified: Sat Aug  5 07:28:51 2023, max compression
```

## Comparing `sqldao-generator-0.3.0.tar` & `sqldao-generator-0.4.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 06:59:18.258346 sqldao-generator-0.3.0/
--rw-rw-rw-   0        0        0      440 2023-07-16 06:59:18.242719 sqldao-generator-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2558 2023-07-16 06:07:18.000000 sqldao-generator-0.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-16 06:59:18.258346 sqldao-generator-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      930 2023-07-16 06:11:26.000000 sqldao-generator-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 06:59:18.242719 sqldao-generator-0.3.0/sqldao_generator.egg-info/
--rw-rw-rw-   0        0        0      440 2023-07-16 06:59:18.000000 sqldao-generator-0.3.0/sqldao_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1057 2023-07-16 06:59:18.000000 sqldao-generator-0.3.0/sqldao_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 06:59:18.000000 sqldao-generator-0.3.0/sqldao_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-07-16 06:59:18.000000 sqldao-generator-0.3.0/sqldao_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-16 06:59:18.000000 sqldao-generator-0.3.0/sqldao_generator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-16 06:59:18.211470 sqldao-generator-0.3.0/sqldaogenerator/
-drwxrwxrwx   0        0        0        0 2023-07-16 06:59:18.227096 sqldao-generator-0.3.0/sqldaogenerator/common/
--rw-rw-rw-   0        0        0      575 2023-07-15 05:33:46.000000 sqldao-generator-0.3.0/sqldaogenerator/common/Criterion.py
--rw-rw-rw-   0        0        0      263 2023-07-09 05:32:41.000000 sqldao-generator-0.3.0/sqldaogenerator/common/Database.py
--rw-rw-rw-   0        0        0     2261 2023-07-16 06:42:12.000000 sqldao-generator-0.3.0/sqldaogenerator/common/TransactionManager.py
--rw-rw-rw-   0        0        0        0 2023-07-01 05:44:52.000000 sqldao-generator-0.3.0/sqldaogenerator/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 06:59:18.227096 sqldao-generator-0.3.0/sqldaogenerator/entity/
--rw-rw-rw-   0        0        0      245 2023-07-04 11:14:21.000000 sqldao-generator-0.3.0/sqldaogenerator/entity/General.py
--rw-rw-rw-   0        0        0      142 2023-07-04 12:50:50.000000 sqldao-generator-0.3.0/sqldaogenerator/entity/Page.py
--rw-rw-rw-   0        0        0        0 2023-07-01 13:43:56.000000 sqldao-generator-0.3.0/sqldaogenerator/entity/__init__.py
--rw-rw-rw-   0        0        0       86 2023-06-30 13:49:06.000000 sqldao-generator-0.3.0/sqldaogenerator/entity/base.py
-drwxrwxrwx   0        0        0        0 2023-07-16 06:59:18.227096 sqldao-generator-0.3.0/sqldaogenerator/generator/
--rw-rw-rw-   0        0        0        0 2023-06-28 05:41:54.000000 sqldao-generator-0.3.0/sqldaogenerator/generator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 06:59:18.242719 sqldao-generator-0.3.0/sqldaogenerator/generator/enums/
--rw-rw-rw-   0        0        0      324 2023-07-02 06:41:27.000000 sqldao-generator-0.3.0/sqldaogenerator/generator/enums/MySqlTypeEnum.py
--rw-rw-rw-   0        0        0        0 2023-06-28 06:35:09.000000 sqldao-generator-0.3.0/sqldaogenerator/generator/enums/__init__.py
--rw-rw-rw-   0        0        0     9478 2023-07-15 07:37:04.000000 sqldao-generator-0.3.0/sqldaogenerator/generator/mysql_generator.py
-drwxrwxrwx   0        0        0        0 2023-07-16 06:59:18.242719 sqldao-generator-0.3.0/sqldaogenerator/logger/
--rw-rw-rw-   0        0        0        0 2023-06-28 05:41:42.000000 sqldao-generator-0.3.0/sqldaogenerator/logger/__init__.py
--rw-rw-rw-   0        0        0      139 2023-07-02 12:44:00.000000 sqldao-generator-0.3.0/sqldaogenerator/logger/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-16 06:59:18.242719 sqldao-generator-0.3.0/sqldaogenerator/resources/
--rw-rw-rw-   0        0        0        0 2023-07-02 05:38:36.000000 sqldao-generator-0.3.0/sqldaogenerator/resources/__init__.py
--rw-rw-rw-   0        0        0      915 2023-07-15 07:41:08.000000 sqldao-generator-0.3.0/sqldaogenerator/resources/base_dao_template.txt
--rw-rw-rw-   0        0        0     1095 2023-07-15 05:33:47.000000 sqldao-generator-0.3.0/sqldaogenerator/resources/criterion_template.txt
--rw-rw-rw-   0        0        0     3018 2023-07-16 06:07:37.000000 sqldao-generator-0.3.0/sqldaogenerator/resources/dao_template.txt
--rw-rw-rw-   0        0        0      723 2023-07-15 05:28:29.000000 sqldao-generator-0.3.0/sqldaogenerator/resources/datasource_template.txt
--rw-rw-rw-   0        0        0      361 2023-07-15 05:28:29.000000 sqldao-generator-0.3.0/sqldaogenerator/resources/entity_template.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 07:28:51.288414 sqldao-generator-0.4.0/
+-rw-rw-rw-   0        0        0      440 2023-08-05 07:28:51.285396 sqldao-generator-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2552 2023-08-05 07:25:20.000000 sqldao-generator-0.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-05 07:28:51.288414 sqldao-generator-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      930 2023-08-05 07:25:20.000000 sqldao-generator-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:28:51.274386 sqldao-generator-0.4.0/sqldao_generator.egg-info/
+-rw-rw-rw-   0        0        0      440 2023-08-05 07:28:51.000000 sqldao-generator-0.4.0/sqldao_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1857 2023-08-05 07:28:51.000000 sqldao-generator-0.4.0/sqldao_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 07:28:51.000000 sqldao-generator-0.4.0/sqldao_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-08-05 07:28:51.000000 sqldao-generator-0.4.0/sqldao_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-05 07:28:51.000000 sqldao-generator-0.4.0/sqldao_generator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 07:28:51.174603 sqldao-generator-0.4.0/sqldaogenerator/
+drwxrwxrwx   0        0        0        0 2023-08-05 07:28:51.194408 sqldao-generator-0.4.0/sqldaogenerator/common/
+-rw-rw-rw-   0        0        0      575 2023-07-22 14:20:35.000000 sqldao-generator-0.4.0/sqldaogenerator/common/Criterion.py
+-rw-rw-rw-   0        0        0      263 2023-07-22 14:20:35.000000 sqldao-generator-0.4.0/sqldaogenerator/common/Database.py
+-rw-rw-rw-   0        0        0     2227 2023-08-05 06:57:57.000000 sqldao-generator-0.4.0/sqldaogenerator/common/TransactionManager.py
+-rw-rw-rw-   0        0        0        0 2023-07-22 14:20:35.000000 sqldao-generator-0.4.0/sqldaogenerator/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:28:51.201565 sqldao-generator-0.4.0/sqldaogenerator/entity/
+-rw-rw-rw-   0        0        0      245 2023-07-22 14:20:35.000000 sqldao-generator-0.4.0/sqldaogenerator/entity/General.py
+-rw-rw-rw-   0        0        0      137 2023-08-05 07:10:03.000000 sqldao-generator-0.4.0/sqldaogenerator/entity/Page.py
+-rw-rw-rw-   0        0        0        0 2023-07-22 14:20:35.000000 sqldao-generator-0.4.0/sqldaogenerator/entity/__init__.py
+-rw-rw-rw-   0        0        0       86 2023-07-22 14:20:35.000000 sqldao-generator-0.4.0/sqldaogenerator/entity/base.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:28:51.207839 sqldao-generator-0.4.0/sqldaogenerator/generator/
+-rw-rw-rw-   0        0        0        0 2023-07-22 14:20:35.000000 sqldao-generator-0.4.0/sqldaogenerator/generator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:28:51.212884 sqldao-generator-0.4.0/sqldaogenerator/generator/enums/
+-rw-rw-rw-   0        0        0      324 2023-07-22 14:20:35.000000 sqldao-generator-0.4.0/sqldaogenerator/generator/enums/MySqlTypeEnum.py
+-rw-rw-rw-   0        0        0        0 2023-07-22 14:20:35.000000 sqldao-generator-0.4.0/sqldaogenerator/generator/enums/__init__.py
+-rw-rw-rw-   0        0        0     9384 2023-08-05 06:59:30.000000 sqldao-generator-0.4.0/sqldaogenerator/generator/mysql_generator.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:28:51.212884 sqldao-generator-0.4.0/sqldaogenerator/logger/
+-rw-rw-rw-   0        0        0        0 2023-07-22 14:20:35.000000 sqldao-generator-0.4.0/sqldaogenerator/logger/__init__.py
+-rw-rw-rw-   0        0        0      139 2023-07-22 14:20:35.000000 sqldao-generator-0.4.0/sqldaogenerator/logger/logger.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:28:51.232373 sqldao-generator-0.4.0/sqldaogenerator/resources/
+-rw-rw-rw-   0        0        0        0 2023-07-22 14:20:35.000000 sqldao-generator-0.4.0/sqldaogenerator/resources/__init__.py
+-rw-rw-rw-   0        0        0      915 2023-07-22 14:20:35.000000 sqldao-generator-0.4.0/sqldaogenerator/resources/base_dao_template.txt
+-rw-rw-rw-   0        0        0     1095 2023-07-22 14:20:35.000000 sqldao-generator-0.4.0/sqldaogenerator/resources/criterion_template.txt
+-rw-rw-rw-   0        0        0     3052 2023-08-05 07:10:03.000000 sqldao-generator-0.4.0/sqldaogenerator/resources/dao_template.txt
+-rw-rw-rw-   0        0        0      723 2023-07-22 14:20:35.000000 sqldao-generator-0.4.0/sqldaogenerator/resources/datasource_template.txt
+-rw-rw-rw-   0        0        0      361 2023-07-22 14:20:35.000000 sqldao-generator-0.4.0/sqldaogenerator/resources/entity_template.txt
```

### Comparing `sqldao-generator-0.3.0/README.md` & `sqldao-generator-0.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 
 - See example/test/generator.py, SampleTest.py
 
 - Create a table first
 ```sql
 create table t_sample
 (
-    id           bigint unsigned auto_increment comment '主鍵'
+    id           bigint unsigned auto_increment comment 'ID'
         primary key,
-    col_var      varchar(100)  null comment '字串',
-    col_text     text          null comment '長字串',
-    col_tinyint  tinyint       null comment '微整數',
-    col_int      int           null comment '整數',
-    col_double   double(10, 2) null comment '浮點數',
-    col_datetime datetime      null comment '時間'
+    col_var      varchar(100)  null comment 'varchar',
+    col_text     text          null comment 'text',
+    col_tinyint  tinyint       null comment 'tinyint',
+    col_int      int           null comment 'int',
+    col_double   double(10, 2) null comment 'double',
+    col_datetime datetime      null comment 'datetime'
 );
 ```
 
 - Generate a dao and entity from a table
 
 ```python
 from example import dao, entity
@@ -37,65 +37,65 @@
          entity_package=entity, entity_name='Sample', table='t_sample', 
          override_datasource=True)
 ```
 
 - Select
 
 ```python
-criterion = SampleCriterion.builder()
+criterion = (SampleCriterion.builder()
     .col_var_like('df')
     .col_text_in(['6'])
     .col_tinyint_gte(1)
     .col_int_lte(5)
     .col_double(3.5)
     .col_datetime_start('2023-07-04 08:26:40')
     .col_datetime_end('2023-07-04 08:26:40')
     .page_no(1)
     .page_size(10)
-    .build()
+    .build())
 entities, total = sample_dao.select(criterion)
 ```
 
 - Insert
 
 ```python
 now = datetime.now().strftime(date_format)
-sample = SampleCriterion.builder()
+sample = (SampleCriterion.builder()
     .set_col_var('i')
     .set_col_text('6')
     .set_col_tinyint(1)
     .set_col_int(5)
     .set_col_double(3.5)
     .set_col_datetime(now)
-    .build()
+    .build())
 entity = sample_dao.insert(sample)
 print(entity.id)
 ```
 
 - Update
 
 ```python
-criterion = SampleCriterion.builder()
+criterion = (SampleCriterion.builder()
     .id_in([13, 15])
     .set_col_var('g')
     .set_col_text('m')
     .set_col_tinyint(3)
     .set_col_int(9)
     .set_col_double(6.5)
     .set_col_datetime(datetime.fromisoformat('2023-07-04T21:30:56'))
-    .build()
+    .build())
 total = sample_dao.update(criterion)
 ```
 
 - Delete
 
 ```python
-criterion = SampleCriterion.builder()
+criterion = (SampleCriterion.builder()
     .id(8)
-    .build()
+    .build())
 total = sample_dao.delete(criterion)
 ```
 
 - Execute in the same transaction
 
 ```python
 from sqldaogenerator.common.TransactionManager import transactional
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sqldao-generator-0.3.0/setup.py` & `sqldao-generator-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sqldao-generator',
-    version='0.3.0',
+    version='0.4.0',
     author='Daniel Hsu',
     description='SqlAlchemy DAO generator',
     long_description_content_type='text/markdown',
     url='https://github.com/davidhsusl/sqldao-generator',
     keywords='SQLAlchemy, mysql',
     python_requires='>=3.10, <4',
     py_modules=['sqldaogenerator'],  # Name of the python package
```

### Comparing `sqldao-generator-0.3.0/sqldao_generator.egg-info/SOURCES.txt` & `sqldao-generator-0.4.0/sqldao_generator.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -20,8 +20,28 @@
 ./sqldaogenerator/resources/dao_template.txt
 ./sqldaogenerator/resources/datasource_template.txt
 ./sqldaogenerator/resources/entity_template.txt
 sqldao_generator.egg-info/PKG-INFO
 sqldao_generator.egg-info/SOURCES.txt
 sqldao_generator.egg-info/dependency_links.txt
 sqldao_generator.egg-info/requires.txt
-sqldao_generator.egg-info/top_level.txt
+sqldao_generator.egg-info/top_level.txt
+sqldaogenerator/common/Criterion.py
+sqldaogenerator/common/Database.py
+sqldaogenerator/common/TransactionManager.py
+sqldaogenerator/common/__init__.py
+sqldaogenerator/entity/General.py
+sqldaogenerator/entity/Page.py
+sqldaogenerator/entity/__init__.py
+sqldaogenerator/entity/base.py
+sqldaogenerator/generator/__init__.py
+sqldaogenerator/generator/mysql_generator.py
+sqldaogenerator/generator/enums/MySqlTypeEnum.py
+sqldaogenerator/generator/enums/__init__.py
+sqldaogenerator/logger/__init__.py
+sqldaogenerator/logger/logger.py
+sqldaogenerator/resources/__init__.py
+sqldaogenerator/resources/base_dao_template.txt
+sqldaogenerator/resources/criterion_template.txt
+sqldaogenerator/resources/dao_template.txt
+sqldaogenerator/resources/datasource_template.txt
+sqldaogenerator/resources/entity_template.txt
```

### Comparing `sqldao-generator-0.3.0/sqldaogenerator/common/Criterion.py` & `sqldao-generator-0.4.0/sqldaogenerator/common/Criterion.py`

 * *Files identical despite different names*

### Comparing `sqldao-generator-0.3.0/sqldaogenerator/common/TransactionManager.py` & `sqldao-generator-0.4.0/sqldaogenerator/common/TransactionManager.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,16 +42,15 @@
         else:
             raise LookupError('No existing transaction.')
 
     def new_transaction(self):
         return self.session_maker()
 
 
-def register_transaction_manager(name: str,
-                                 transaction_manager: TransactionManager):
+def register_transaction_manager(name: str, transaction_manager: TransactionManager):
     transaction_managers.update({name: transaction_manager})
 
 
 def transactional(auto_commit=True):
     def decorator(func):
         def wrapper(*args, **kwargs):
             if transaction_managers[default_name].is_exists():
```

### Comparing `sqldao-generator-0.3.0/sqldaogenerator/generator/mysql_generator.py` & `sqldao-generator-0.4.0/sqldaogenerator/generator/mysql_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from types import ModuleType
 
 from sqlalchemy import create_engine, text
 
 from sqldaogenerator import resources
 from sqldaogenerator.generator.enums.MySqlTypeEnum import MySqlTypeEnum
 
-primary_key_template = "{column} = Column({type}, autoincrement=True, primary_key=True, comment='{comment}')"
+primary_key_template = "{column} = Column({type}, autoincrement=True, primary_key=True, " \
+                       "comment='{comment}')"
 column_template = "{column} = Column({type}, comment='{comment}')"
 set_template = """def set_{column}(self, value: {type}):
         self.values['{column}'] = value
         return self"""
 ifelse_filter_template = """def {column}{suffix}(self, value: {type} = None, reverse=False{other}):
         if value is not None{condition}:
             if not reverse:
@@ -88,30 +89,26 @@
 
 def generate(user: str, password: str, host: str, port: int, database: str,
              datasource_package: ModuleType, datasource_name: str,
              base_dao_package: ModuleType, base_dao_name: str,
              dao_package: ModuleType, entity_package: ModuleType,
              entity_name: str, table: str, override_datasource=False):
     # create a Datasource
-    datasource_file = pkg_resources.files(datasource_package) \
-        .joinpath(f"{datasource_name}.py")
+    datasource_file = pkg_resources.files(datasource_package).joinpath(f"{datasource_name}.py")
     if override_datasource or not datasource_file.is_file():
-        template = pkg_resources.files(resources) \
-            .joinpath('datasource_template.txt').read_text()
+        template = pkg_resources.files(resources).joinpath('datasource_template.txt').read_text()
         template = template.format(datasource_name=datasource_name,
                                    user=user, password=password, host=host,
                                    port=port, dbname=database)
         with datasource_file.open('w', encoding='utf-8') as file:
             file.write(template)
 
     # create a BaseDao
-    base_dao_file = pkg_resources.files(base_dao_package) \
-        .joinpath(f"{base_dao_name}.py")
-    template = pkg_resources.files(resources) \
-        .joinpath('base_dao_template.txt').read_text()
+    base_dao_file = pkg_resources.files(base_dao_package).joinpath(f"{base_dao_name}.py")
+    template = pkg_resources.files(resources).joinpath('base_dao_template.txt').read_text()
     template = template.format(base_dao_name=base_dao_name,
                                datasource_package=datasource_package.__package__,
                                datasource_name=datasource_name)
     with base_dao_file.open('w', encoding='utf-8') as file:
         file.write(template)
 
     connection_string = f"mysql+mysqlconnector://{user}:{password}@{host}:{port}/{database}"
@@ -131,16 +128,15 @@
     sets = []
     filters = []
     for result in results:
         column_name = result.COLUMN_NAME.lower()
         data_type = result.DATA_TYPE.decode() \
             if isinstance(result.DATA_TYPE, bytes) else result.DATA_TYPE
         comment = result.COLUMN_COMMENT.decode() \
-            if isinstance(result.COLUMN_COMMENT, bytes) \
-            else result.COLUMN_COMMENT
+            if isinstance(result.COLUMN_COMMENT, bytes) else result.COLUMN_COMMENT
 
         # column
         if result.COLUMN_KEY == 'PRI':
             template = primary_key_template
         else:
             template = column_template
         columns.append(template.format(
@@ -167,31 +163,27 @@
 
     # entity
     tab = '    '
     filter_intent = f"\n\n{tab}"
     for template_name, file_name \
             in [('entity_template.txt', entity_name),
                 ('criterion_template.txt', f"{entity_name}Criterion")]:
-        template = pkg_resources.files(resources) \
-            .joinpath(template_name).read_text()
+        template = pkg_resources.files(resources).joinpath(template_name).read_text()
         template = template.format(entity_name=entity_name, table=table,
                                    columns=f'\n{tab}'.join(columns),
                                    sets=filter_intent.join(sets),
                                    filters=filter_intent.join(filters),
                                    entity_package=entity_package.__package__)
-        entity_file = pkg_resources.files(entity_package) \
-            .joinpath(f"{file_name}.py")
+        entity_file = pkg_resources.files(entity_package).joinpath(f"{file_name}.py")
         with entity_file.open('w', encoding='utf-8') as file:
             file.write(template)
 
     # dao
-    template = pkg_resources.files(resources) \
-        .joinpath('dao_template.txt').read_text()
+    template = pkg_resources.files(resources).joinpath('dao_template.txt').read_text()
     template = template.format(base_dao_package=base_dao_package.__package__,
                                base_dao_name=base_dao_name,
                                entity_package=entity_package.__package__,
                                entity_name=entity_name,
                                entity_variable=underlined_word)
-    entity_file = pkg_resources.files(dao_package) \
-        .joinpath(f"{entity_name}Dao.py")
+    entity_file = pkg_resources.files(dao_package).joinpath(f"{entity_name}Dao.py")
     with entity_file.open('w', encoding='utf-8') as file:
         file.write(template)
```

### Comparing `sqldao-generator-0.3.0/sqldaogenerator/resources/base_dao_template.txt` & `sqldao-generator-0.4.0/sqldaogenerator/resources/base_dao_template.txt`

 * *Files identical despite different names*

### Comparing `sqldao-generator-0.3.0/sqldaogenerator/resources/criterion_template.txt` & `sqldao-generator-0.4.0/sqldaogenerator/resources/criterion_template.txt`

 * *Files identical despite different names*

### Comparing `sqldao-generator-0.3.0/sqldaogenerator/resources/dao_template.txt` & `sqldao-generator-0.4.0/sqldaogenerator/resources/dao_template.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,21 @@
     @transactional(auto_commit=False)
     def select(self, criterion: Criterion) -> tuple[list[{entity_name}], int]:
         criterion_list = criterion.to_list()
         assert self.is_in_modules(criterion_list, {entity_name}), \
             'The expressions must be created by the {entity_name} entity.'
         session = self.get_transaction()
         page = criterion.page
-        orders = page.order_by.split(' ')
-        query = session.query({entity_name}).filter(*criterion_list) \
-            .order_by(eval(f"{entity_name}.{{orders[0]}}.{{orders[1]}}()"))
+        query = session.query({entity_name}).filter(*criterion_list)
+        if page.order_by is not None:
+            orders = page.order_by.split(' ')
+            query = query.order_by(eval(f"{entity_name}.{{orders[0]}}.{{orders[1]}}()"))
         total = None
         if page.page_no is not None and page.page_size is not None:
-            query = query.offset((page.page_no - 1) * page.page_size) \
-                .limit(page.page_size)
+            query = query.offset((page.page_no - 1) * page.page_size).limit(page.page_size)
             total = session.query({entity_name}).filter(*criterion_list).count()
         entities = query.all()
         return entities, total or len(entities)
 
     @transactional()
     def insert(self, criterion: Criterion):
         session = self.get_transaction()
```

### Comparing `sqldao-generator-0.3.0/sqldaogenerator/resources/datasource_template.txt` & `sqldao-generator-0.4.0/sqldaogenerator/resources/datasource_template.txt`

 * *Files identical despite different names*

