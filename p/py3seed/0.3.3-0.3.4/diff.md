# Comparing `tmp/py3seed-0.3.3.tar.gz` & `tmp/py3seed-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3seed-0.3.3.tar", last modified: Wed Aug  2 06:17:03 2023, max compression
+gzip compressed data, was "py3seed-0.3.4.tar", last modified: Sat Aug  5 06:29:52 2023, max compression
```

## Comparing `py3seed-0.3.3.tar` & `py3seed-0.3.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-02 06:17:03.068670 py3seed-0.3.3/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.3.3/LICENSE
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-02 06:17:03.068834 py3seed-0.3.3/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.3.3/README.md
--rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.3.3/pyproject.toml
--rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-08-02 06:17:03.069778 py3seed-0.3.3/setup.cfg
--rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.3.3/setup.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-02 06:17:03.037302 py3seed-0.3.3/src/
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-02 06:17:03.060013 py3seed-0.3.3/src/py3seed/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.3.3/src/py3seed/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.3.3/src/py3seed/__main__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.3.3/src/py3seed/admin.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7571 2023-07-21 09:02:47.000000 py3seed-0.3.3/src/py3seed/cachesupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-02 06:17:03.064123 py3seed-0.3.3/src/py3seed/commands/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.3.3/src/py3seed/commands/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    22791 2023-08-02 06:16:01.000000 py3seed-0.3.3/src/py3seed/commands/gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.3.3/src/py3seed/error.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.3.3/src/py3seed/inflection.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.3.3/src/py3seed/log.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.3.3/src/py3seed/merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-31 04:55:20.000000 py3seed-0.3.3/src/py3seed/model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.3.3/src/py3seed/mongosupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14654 2023-08-02 02:06:33.000000 py3seed-0.3.3/src/py3seed/utils.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.3.3/src/py3seed/websupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-02 06:17:03.063123 py3seed-0.3.3/src/py3seed.egg-info/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-02 06:17:03.000000 py3seed-0.3.3/src/py3seed.egg-info/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-08-02 06:17:03.000000 py3seed-0.3.3/src/py3seed.egg-info/SOURCES.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-08-02 06:17:03.000000 py3seed-0.3.3/src/py3seed.egg-info/dependency_links.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-08-02 06:17:03.000000 py3seed-0.3.3/src/py3seed.egg-info/entry_points.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-08-02 06:17:03.000000 py3seed-0.3.3/src/py3seed.egg-info/requires.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-08-02 06:17:03.000000 py3seed-0.3.3/src/py3seed.egg-info/top_level.txt
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-02 06:17:03.067810 py3seed-0.3.3/tests/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     4032 2023-07-21 09:03:11.000000 py3seed-0.3.3/tests/test_cachesupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6832 2023-07-31 12:50:18.000000 py3seed-0.3.3/tests/test_gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.3.3/tests/test_merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.3.3/tests/test_model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.3.3/tests/test_mongosupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-05 06:29:52.211741 py3seed-0.3.4/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.3.4/LICENSE
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-05 06:29:52.211891 py3seed-0.3.4/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.3.4/README.md
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.3.4/pyproject.toml
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-08-05 06:29:52.212574 py3seed-0.3.4/setup.cfg
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.3.4/setup.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-05 06:29:52.189676 py3seed-0.3.4/src/
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-05 06:29:52.203769 py3seed-0.3.4/src/py3seed/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.3.4/src/py3seed/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.3.4/src/py3seed/__main__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.3.4/src/py3seed/admin.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7571 2023-07-21 09:02:47.000000 py3seed-0.3.4/src/py3seed/cachesupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-05 06:29:52.207472 py3seed-0.3.4/src/py3seed/commands/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.3.4/src/py3seed/commands/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    22814 2023-08-05 06:24:39.000000 py3seed-0.3.4/src/py3seed/commands/gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.3.4/src/py3seed/error.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.3.4/src/py3seed/inflection.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.3.4/src/py3seed/log.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.3.4/src/py3seed/merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-31 04:55:20.000000 py3seed-0.3.4/src/py3seed/model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.3.4/src/py3seed/mongosupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    15292 2023-08-03 03:55:39.000000 py3seed-0.3.4/src/py3seed/utils.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.3.4/src/py3seed/websupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-05 06:29:52.206408 py3seed-0.3.4/src/py3seed.egg-info/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-05 06:29:52.000000 py3seed-0.3.4/src/py3seed.egg-info/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-08-05 06:29:52.000000 py3seed-0.3.4/src/py3seed.egg-info/SOURCES.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-08-05 06:29:52.000000 py3seed-0.3.4/src/py3seed.egg-info/dependency_links.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-08-05 06:29:52.000000 py3seed-0.3.4/src/py3seed.egg-info/entry_points.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-08-05 06:29:52.000000 py3seed-0.3.4/src/py3seed.egg-info/requires.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-08-05 06:29:52.000000 py3seed-0.3.4/src/py3seed.egg-info/top_level.txt
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-05 06:29:52.211235 py3seed-0.3.4/tests/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     4032 2023-07-21 09:03:11.000000 py3seed-0.3.4/tests/test_cachesupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7225 2023-08-03 01:41:52.000000 py3seed-0.3.4/tests/test_gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.3.4/tests/test_merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.3.4/tests/test_model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.3.4/tests/test_mongosupport.py
```

### Comparing `py3seed-0.3.3/LICENSE` & `py3seed-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.3/PKG-INFO` & `py3seed-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.3.3
+Version: 0.3.4
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.3.3/setup.cfg` & `py3seed-0.3.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py3seed
-version = 0.3.3
+version = 0.3.4
 author = Samuel Feng
 author_email = okosioc@gmail.com
 description = A package that bootstraps your project by simple data models definition and auto api and user interface generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/okosioc/pyseed
 project_urls =
```

### Comparing `py3seed-0.3.3/src/py3seed/__init__.py` & `py3seed-0.3.4/src/py3seed/__init__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.3/src/py3seed/__main__.py` & `py3seed-0.3.4/src/py3seed/__main__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.3/src/py3seed/admin.py` & `py3seed-0.3.4/src/py3seed/admin.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.3/src/py3seed/cachesupport.py` & `py3seed-0.3.4/src/py3seed/cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.3/src/py3seed/commands/gen.py` & `py3seed-0.3.4/src/py3seed/commands/gen.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
                 # - admin/dashboard -> blueprint = admin, name = dashboard
                 if '/' in name:
                     blueprint, name = name.split('/')
                 else:
                     blueprint = 'public'
                 #
                 layout = v.strip()
-                logger.info(f'- {blueprint}/{name}: {layout}')
+                logger.info(f'- {"|".join(domains)}://{blueprint}/{name}: {layout}')
                 # Validate to make sure view name is unique
                 if name in view_names:
                     logger.error(f'View name {v["name"]} is not unique')
                     return False
                 #
                 view_names.add(name)
                 #
@@ -394,15 +394,15 @@
             # e.g,
             #   www/templates/{{#blueprints}}
             #     ->
             #     www/templates/public
             #     www/templates/dash
             #     www/templates/demo
             #     ...
-            logger.info(f'Render {o_name}')
+            logger.info(f'Render {o_name}/')
             o_path = os.path.join(o_base, o_name)
             if not os.path.exists(o_path):
                 os.mkdir(o_path)
             # if output is not the same as template, need to copy includes folder
             t_includes = os.path.join(t_path, INCLUDES_FOLDER)
             o_includes = os.path.join(o_path, INCLUDES_FOLDER)
             if t_path != o_path and os.path.exists(t_includes):
```

### Comparing `py3seed-0.3.3/src/py3seed/error.py` & `py3seed-0.3.4/src/py3seed/error.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.3/src/py3seed/inflection.py` & `py3seed-0.3.4/src/py3seed/inflection.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.3/src/py3seed/log.py` & `py3seed-0.3.4/src/py3seed/log.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.3/src/py3seed/merge3.py` & `py3seed-0.3.4/src/py3seed/merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.3/src/py3seed/model.py` & `py3seed-0.3.4/src/py3seed/model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.3/src/py3seed/mongosupport.py` & `py3seed-0.3.4/src/py3seed/mongosupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.3/src/py3seed/utils.py` & `py3seed-0.3.4/src/py3seed/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         rows: [[                         # each column is a dict, which has name/params/format/span and inner rows
             {name: $, rows:[...]},
             {name: 0, rows:[...]},
         ]]
     }
     """
 
-    def _parse_lines(level, _lines, _schema):
+    def _parse_lines(level, _lines, _schema, _action):
         """ Recursively parse lines. """
         leading = '- ' * (level + 1)  # 2 spaces for each level
         # logger.debug('Parse lines:\n' + '\n'.join(_lines))
         _rows = []
         # Get the indexes of lines that has same indent with first line
         first_line = _lines[0]
         first_indent = len(first_line) - len(first_line.lstrip())
@@ -220,31 +220,39 @@
                 elif col_name == '-':
                     pass
                 # Group column
                 elif col_name.replace('.', '').isdigit():
                     if not col_lines:
                         raise LayoutError(f'Group {col_name} should have inner layout')
                     #
-                    column['rows'] = _parse_lines(level + 1, col_lines, _schema)
+                    column['rows'] = _parse_lines(level + 1, col_lines, _schema, _action)
                 else:
                     if col_name not in _schema['properties']:  # type of _schema is always a object
                         raise LayoutError(f'Field {col_name} not found in schema')
                     #
                     column_schema = _schema['properties'][col_name]
+                    if _action in ['create', 'update', 'upcreate']:
+                        # Can not edit back relation field as its value stores in counterpart
+                        if column_schema.get('is_back_relation', False):
+                            raise LayoutError(f'Field {col_name} is a back relation so can not be edited in {_action} action')
+                        # Can not edit non-editable field
+                        if not column_schema['editable']:
+                            raise LayoutError(f'Field {col_name} is not editable in {_action} action')
+                    #
                     column_type = column_schema['type']
                     inner_schema = None
                     if column_type == 'object':
                         inner_schema = column_schema
                     elif column_type == 'array':
                         inner_schema = column_schema['items'] if column_schema['items']['type'] == 'object' else None
                     #
                     if inner_schema:
                         # Inner layout is optional for inner object
                         if col_lines:
-                            column['rows'] = _parse_lines(level + 1, col_lines, inner_schema)  # Schema passing recursively should always be an object
+                            column['rows'] = _parse_lines(level + 1, col_lines, inner_schema, _action)  # Schema passing recursively should always be an object
                     else:
                         if col_lines:
                             raise LayoutError(f'{column_type.capitalize()} field {col_name} can not have inner layout')
                     #
                     column.pop('lines', None)
             #
             _rows.append(columns)
@@ -318,15 +326,15 @@
     if action_line.startswith('#!'):
         action_str = action_line[2:].strip()
         lines = lines[1:]
         # Parse params, e.g, form?param=1
         if '?' in action_str:
             action, params = _parse_query_str(action_str)
     #
-    rows = _parse_lines(0, lines, schema)
+    rows = _parse_lines(0, lines, schema, action)
     #
     return {
         'action': action,
         'params': params,
         'rows': rows
     }
```

### Comparing `py3seed-0.3.3/src/py3seed/websupport.py` & `py3seed-0.3.4/src/py3seed/websupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.3/src/py3seed.egg-info/PKG-INFO` & `py3seed-0.3.4/src/py3seed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.3.3
+Version: 0.3.4
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.3.3/src/py3seed.egg-info/SOURCES.txt` & `py3seed-0.3.4/src/py3seed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.3/tests/test_cachesupport.py` & `py3seed-0.3.4/tests/test_cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.3/tests/test_gen.py` & `py3seed-0.3.4/tests/test_gen.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,14 +37,20 @@
         1#summary,     members#8                                                  
           logo           avatar, name, status, roles, email, phone, team_join_time
           name         
           phone                                                                
           members                                                                   
           create_time  
     '''
+    team_members_layout_update = '''#!update?title=Team
+        logo
+        name, phone
+        members
+        remarks  
+    '''
     team_schema = Team.schema()
 
     #
     # Validation
     #
 
     # Validate invalid indent
@@ -67,14 +73,21 @@
     with pytest.raises(LayoutError) as exc_info:
         parse_layout(
             user_profile_layout.replace('intro', '  intro'),
             user_schema,
         )
     #
     assert 'phone can not have inner layout' in str(exc_info.value)
+    # Validate if back relation field can be updated
+    with pytest.raises(LayoutError) as exc_info:
+        parse_layout(
+            team_members_layout_update,
+            team_schema,
+        )
+    assert 'members is a back relation' in str(exc_info.value)
 
     #
     # Parsing
     #
 
     # User profile layout
     layout = parse_layout(user_profile_layout, user_schema)
```

### Comparing `py3seed-0.3.3/tests/test_merge3.py` & `py3seed-0.3.4/tests/test_merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.3/tests/test_model.py` & `py3seed-0.3.4/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.3/tests/test_mongosupport.py` & `py3seed-0.3.4/tests/test_mongosupport.py`

 * *Files identical despite different names*

