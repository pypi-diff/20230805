# Comparing `tmp/json_pydantic-1.0.0.tar.gz` & `tmp/json_pydantic-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_pydantic-1.0.0.tar", last modified: Thu Aug  3 13:02:26 2023, max compression
+gzip compressed data, was "json_pydantic-1.1.0.tar", last modified: Sat Aug  5 17:28:45 2023, max compression
```

## Comparing `json_pydantic-1.0.0.tar` & `json_pydantic-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 13:02:26.894254 json_pydantic-1.0.0/
--rw-rw-rw-   0        0        0    35819 2023-08-03 12:40:01.000000 json_pydantic-1.0.0/LICENCE
--rw-rw-rw-   0        0        0      194 2023-08-03 13:02:26.894254 json_pydantic-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      608 2023-08-03 12:56:28.000000 json_pydantic-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 13:02:26.888254 json_pydantic-1.0.0/json_pydantic/
--rw-rw-rw-   0        0        0        0 2023-08-02 19:40:01.000000 json_pydantic-1.0.0/json_pydantic/__init__.py
--rw-rw-rw-   0        0        0      580 2023-08-02 19:40:01.000000 json_pydantic-1.0.0/json_pydantic/__main__.py
--rw-rw-rw-   0        0        0      189 2023-08-02 19:40:01.000000 json_pydantic-1.0.0/json_pydantic/classes.py
--rw-rw-rw-   0        0        0     2653 2023-08-02 20:04:29.000000 json_pydantic-1.0.0/json_pydantic/conventer.py
--rw-rw-rw-   0        0        0      560 2023-08-02 19:40:01.000000 json_pydantic-1.0.0/json_pydantic/functions.py
--rw-rw-rw-   0        0        0       61 2023-08-02 19:40:01.000000 json_pydantic-1.0.0/json_pydantic/variables.py
-drwxrwxrwx   0        0        0        0 2023-08-03 13:02:26.893254 json_pydantic-1.0.0/json_pydantic.egg-info/
--rw-rw-rw-   0        0        0      194 2023-08-03 13:02:26.000000 json_pydantic-1.0.0/json_pydantic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-08-03 13:02:26.000000 json_pydantic-1.0.0/json_pydantic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 13:02:26.000000 json_pydantic-1.0.0/json_pydantic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-08-03 13:02:26.000000 json_pydantic-1.0.0/json_pydantic.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-08-03 13:02:26.000000 json_pydantic-1.0.0/json_pydantic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 13:02:26.894254 json_pydantic-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      505 2023-08-03 13:01:49.000000 json_pydantic-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 17:28:45.203358 json_pydantic-1.1.0/
+-rw-rw-rw-   0        0        0    35819 2023-08-03 12:40:01.000000 json_pydantic-1.1.0/LICENCE
+-rw-rw-rw-   0        0        0      246 2023-08-05 17:28:45.202359 json_pydantic-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      620 2023-08-04 10:38:08.000000 json_pydantic-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 17:28:45.189358 json_pydantic-1.1.0/json_pydantic/
+-rw-rw-rw-   0        0        0        0 2023-08-02 19:40:01.000000 json_pydantic-1.1.0/json_pydantic/__init__.py
+-rw-rw-rw-   0        0        0      580 2023-08-02 19:40:01.000000 json_pydantic-1.1.0/json_pydantic/__main__.py
+-rw-rw-rw-   0        0        0      106 2023-08-05 12:13:25.000000 json_pydantic-1.1.0/json_pydantic/classes.py
+-rw-rw-rw-   0        0        0     2495 2023-08-05 17:08:29.000000 json_pydantic-1.1.0/json_pydantic/conventer.py
+-rw-rw-rw-   0        0        0      560 2023-08-02 19:40:01.000000 json_pydantic-1.1.0/json_pydantic/functions.py
+-rw-rw-rw-   0        0        0      117 2023-08-05 17:07:16.000000 json_pydantic-1.1.0/json_pydantic/variables.py
+drwxrwxrwx   0        0        0        0 2023-08-05 17:28:45.202359 json_pydantic-1.1.0/json_pydantic.egg-info/
+-rw-rw-rw-   0        0        0      246 2023-08-05 17:28:45.000000 json_pydantic-1.1.0/json_pydantic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2023-08-05 17:28:45.000000 json_pydantic-1.1.0/json_pydantic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 17:28:45.000000 json_pydantic-1.1.0/json_pydantic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-08-05 17:28:45.000000 json_pydantic-1.1.0/json_pydantic.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-08-05 17:28:45.000000 json_pydantic-1.1.0/json_pydantic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-05 17:28:45.000000 json_pydantic-1.1.0/json_pydantic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 17:28:45.203358 json_pydantic-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      614 2023-08-05 17:28:43.000000 json_pydantic-1.1.0/setup.py
```

### Comparing `json_pydantic-1.0.0/LICENCE` & `json_pydantic-1.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `json_pydantic-1.0.0/README.md` & `json_pydantic-1.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 Json_Pydantic is a utility for converting json files to Pydantic models
 
 ## Install
 
 ```commandline
-pip install .
+pip install json-pydantic
 ```
 
 ## Usage
 
 You can use this tool with two ways
 
 - As module
```

### Comparing `json_pydantic-1.0.0/json_pydantic/__main__.py` & `json_pydantic-1.1.0/json_pydantic/__main__.py`

 * *Files identical despite different names*

### Comparing `json_pydantic-1.0.0/json_pydantic/conventer.py` & `json_pydantic-1.1.0/json_pydantic/conventer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from jinja2 import Environment, FileSystemLoader
+
 from .classes import ClassStruct
-from .variables import CLASS_TEMPLATE
 from .functions import get_type, load_json, save_models
+from .variables import models_template_name, templates_path
 
 
 def parse_types(data: dict) -> dict[str, ...]:
     result = {}
 
     if isinstance(data, list) and len(data):
         result['content_list'] = [parse_types(data[0])]
@@ -18,58 +20,49 @@
         elif isinstance(value, list):
             result[key] = [parse_types(i) if isinstance(i, dict) else get_type(i) for i in value]
         else:
             result[key] = get_type(value)
     return result
 
 
-def parse_classes(data: dict[str, ...] | list, name: str = 'Root') -> ClassStruct:
-    class_struct: ClassStruct = {
-        'name': name,
-        'args': {},
-        'inner_classes': []
-    }
+def parse_classes(data: dict[str, ...] | list, name: str = 'Root') -> list[ClassStruct]:
+    result_classes: list[ClassStruct] = []
 
+    buffer: ClassStruct = {'name': name, 'args': {}}
     if not isinstance(data, dict):
         return get_type(data)
 
     for key, value in data.items():
         class_name = key.title().replace('_', '')
         if isinstance(value, dict):
-            if len(value):
-                class_struct['inner_classes'].append(parse_classes(value, class_name))
-                class_struct['args'][key] = class_name
+            if value:
+                new_classes = parse_classes(value, class_name)
+                result_classes = new_classes + result_classes
+                buffer['args'][key] = class_name
             else:
-                class_struct['args'][key] = 'dict'
+                buffer['args'][key] = 'dict'
         elif isinstance(value, list):
-            if len(value):
-                class_struct['inner_classes'].append(parse_classes(value[0], class_name))
-                class_struct['args'][key] = f'list[{class_name}]'
-            else:
-                class_struct['args'][key] = 'list'
+            if value:
+                if value:
+                    new_classes = parse_classes(value[0], class_name)
+                    result_classes = new_classes + result_classes
+                    buffer['args'][key] = f'list[{class_name}]'
+                else:
+                    buffer['args'][key] = 'list'
         else:
-            class_struct['args'][key] = value
-    return class_struct
-
+            buffer['args'][key] = value
+    result_classes.append(buffer)
 
-def _generate_models(class_struct: ClassStruct) -> str:
-    inner = class_struct['inner_classes']
-    result_string = ''
-    if inner:
-        for class_ in inner:
-            result_string += _generate_models(class_)
-    name = class_struct['name']
-    args = class_struct['args']
-    args = '\n\t'.join(f'{k}: {v}' for k, v in sorted(args.items()))
-    result_string += CLASS_TEMPLATE.format(name=name, args=args)
-    return result_string
+    return result_classes
 
 
-def generate_models(class_struct: ClassStruct):
-    return 'from pydantic import BaseModel\n\n\n' + _generate_models(class_struct)
+def generate_models(classes: list[ClassStruct]):
+    environment = Environment(loader=FileSystemLoader(templates_path))
+    models_template = environment.get_template(models_template_name)
+    return models_template.render(classes=classes)
 
 
 def run(input_file: str, output_file: str, first_class_name: str):
     input_json = load_json(input_file)
     parsed_types = parse_types(input_json)
     class_struct = parse_classes(parsed_types, first_class_name)
     models = generate_models(class_struct)
```

### Comparing `json_pydantic-1.0.0/json_pydantic/functions.py` & `json_pydantic-1.1.0/json_pydantic/functions.py`

 * *Files identical despite different names*

