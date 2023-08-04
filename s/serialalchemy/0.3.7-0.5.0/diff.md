# Comparing `tmp/SerialAlchemy-0.3.7.tar.gz` & `tmp/serialalchemy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SerialAlchemy-0.3.7.tar", max compression
+gzip compressed data, was "serialalchemy-0.5.0.tar", max compression
```

## Comparing `SerialAlchemy-0.3.7.tar` & `serialalchemy-0.5.0.tar`

### file list

```diff
@@ -1,4 +1,3 @@
--rw-r--r--   0        0        0      449 2022-08-08 18:29:23.354537 SerialAlchemy-0.3.7/pyproject.toml
--rw-r--r--   0        0        0    19383 2022-08-08 18:29:23.354537 SerialAlchemy-0.3.7/serialalchemy/__init__.py
--rw-r--r--   0        0        0      658 2022-08-08 18:30:43.542713 SerialAlchemy-0.3.7/setup.py
--rw-r--r--   0        0        0      501 2022-08-08 18:30:43.542865 SerialAlchemy-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0      449 2023-08-04 20:35:31.128227 serialalchemy-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    19148 2023-08-04 20:35:31.139060 serialalchemy-0.5.0/serialalchemy/__init__.py
+-rw-r--r--   0        0        0      622 1970-01-01 00:00:00.000000 serialalchemy-0.5.0/PKG-INFO
```

### Comparing `SerialAlchemy-0.3.7/serialalchemy/__init__.py` & `serialalchemy-0.5.0/serialalchemy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,69 @@
 '''SerialAlchemy
 Dead simple object serialization for SQLAlchemy
 
 '''
 
-from sqlalchemy import inspect, DateTime, Date, Time, processors, event
+from sqlalchemy import inspect, DateTime, Date, Time, event
 from decimal import Decimal
 from datetime import datetime, date, timedelta, time
 from sqlalchemy.ext.hybrid import hybrid_property
 
-import inspect as inspectPy
+# import inspect as inspectPy
 
 import re
 from collections import abc
 import json
 import base64
 
+from dateutil.parser import (
+    parse,
+    ParserError,
+)
+
+
 
 class SerialAlchemyError(Exception):
     pass
 
 __all__ = [
         'serializable_property',
+        'serializable_hybrid',
         'Serializable',
         ]
 
 first_cap_re = re.compile('(.)([A-Z][a-z]+)')
 all_cap_re = re.compile('([a-z0-9])([A-Z])')
 def convert_class(name):
     s1 = first_cap_re.sub(r'\1_\2', name)
     return all_cap_re.sub(r'\1_\2', s1).lower()
 
 
-primitives = (int, str, bytes, float, dict, list, type(None),)
-
 
 def _get_value(obj, field):
-    global primitives
+    '''Returns a value that can be serialized.
+
+    2023-07-10: Added docstring because I forgot what this did :P
+    '''
+
+    primitives = (int, str, bytes, float, dict, list, type(None),)
 
     value = getattr(obj, field)
 
     if isinstance(value, Decimal):
         return float(value)
     elif isinstance(value, datetime) or isinstance(value, date) or\
             isinstance(value, time):
         return str(value)
     elif isinstance(value, timedelta):
         return float(value.total_seconds())
     elif isinstance(value, (set, frozenset,)):
         return list(value)
     elif not isinstance(value, primitives):
+        # last ditch effort, try converting to string
         return str(value)
 
     return value
 
 
 def _get_serializable_properties(obj, attrs, loaded):
     all_members = set([f for f in dir(obj) if not f.startswith('_')])
@@ -63,16 +74,18 @@
 
     cls = obj.__class__
     propout = []
 
     obj_type = type(obj)
 
     for prop in properties:
-        if hasattr(obj_type, prop) and \
-                isinstance(getattr(obj_type, prop), serializable_property):
+        inst = getattr(obj_type, prop)
+        if inst and \
+                (isinstance(inst, serializable_property) or\
+                 isinstance(inst, serializable_hybrid)):
 
             propout.append(prop)
         else:
             attr = getattr(cls, prop)
             should_add = False
 
             try:
@@ -83,34 +96,59 @@
             if should_add and hasattr(obj, prop):
                 propout.append(prop)
 
     return propout
 
 
 class ExtJSONEncoder(json.JSONEncoder):
+    ''' Add a way to serialize bytes to base64.
+    '''
     def default(self, obj):
         if isinstance(obj, bytes):
             return base64.b64encode(obj).decode()
 
         # return json.JSONEncoder.default(self, obj)
         return super().default(obj)
 
 
+def _str_to_datetime(value):
+    try:
+        dt = parse(value)
+    except (ParserError, OverflowError) as ex:
+        raise SerialAlchemyError('Datetime parsing error', ex)
+    return dt
+
+def _str_to_date(value):
+    try:
+        dt = parse(value)
+    except (ParserError, OverflowError) as ex:
+        raise SerialAlchemyError('Date parsing error', ex)
+    return dt.date()
+
+def _str_to_time(value):
+    try:
+        dt = parse(value)
+    except (ParserError, OverflowError) as ex:
+        raise SerialAlchemyError('Date parsing error', ex)
+    return dt.time()
 
 
 class serializable_property(property):
     '''Simple wrapper for built-in `property` for explicit serialization of
     class/instance properties.
 
     As of version 0.2.0, SerialAlchemy will not include a property unless
     it is decorated with `serializable_property` or is a SQLAlchemy
     hybrid_attribute.
     '''
     pass
 
+class serializable_hybrid(hybrid_property):
+    pass
+
 
 class Serializable:
     '''Provides serialization and deserialization for data-mapped classes.
 
     This is a mixin class that provides serializaiton to python dicts and
     object population (deserialization). A method for creating a streaming
     json generator from a result set is also defined.
@@ -233,15 +271,16 @@
                 if 'serializable' in col.info and not col.info['serializable']:
                     continue
 
             output[field] = _get_value(self, field)
 
 
         if relationships:
-            for field, relation in info.mapper.relationships.items():
+            relations = info.mapper.relationships.items()
+            for field, relation in relations:
                 if includes and field not in includes:
                     continue
                 elif excludes and field in excludes:
                     continue
 
                 data = getattr(self, field)
                 relout = None
@@ -301,15 +340,16 @@
                 continue
 
             if hasattr(self, prop):
                 output[prop] = _get_value(self, prop)
 
         return output
 
-    def populate(self, data, skip_fields=None, swallow_exceptions=False):
+    def populate(self, data, skip_fields=None, swallow_exceptions=False,
+                 strict_typing=True):
         '''Populate object from a dict of fields.
 
         *This method does not populate relationships*. It is recommended
         to override the method and handle them manually.
 
         Values for relationship attributes can be supplied in the `data`
         parameter and will be safely ignored.
@@ -331,23 +371,28 @@
         errors = []
 
         for col in mapper.columns:
             if col.name in skip_fields:
                 continue
             elif col.name in data:
                 if isinstance(col.type, DateTime):
-                    value = processors.str_to_datetime(data[col.name])
+                    value = _str_to_datetime(data[col.name])
                 elif isinstance(col.type, Date):
-                    value = processors.str_to_date(data[col.name])
+                    value = _str_to_date(data[col.name])
                 elif isinstance(col.type, Time):
-                    value = processors.str_to_time(data[col.name])
+                    value = _str_to_time(data[col.name])
                 else:
                     value = data[col.name]
 
+                col_pytype = col.type.python_type
                 try:
+                    if strict_typing and not isinstance(value, col_pytype):
+                        raise TypeError(col.name,
+                                        f'Value {value} {type(value)} does '\
+                                        f'not match type {str(col_pytype)}')
                     setattr(self, col.name, value)
                 except Exception as ex:
                     if not swallow_exceptions:
                         raise ex
                     errors.append(ex)
 
         return errors
@@ -430,72 +475,19 @@
             return json.dumps({cls.__plural__: seritems}, cls=ExtJSONEncoder)
         elif resultset is not None:
             return json.dumps({cls.__single__: resultset.to_dict(fields,
                 relationships, mtm_pkonly)}, cls=ExtJSONEncoder)
         else:
             return json.dumps({cls.__single__: None})
 
-    @classmethod
-    def schema_info(cls):
-        '''Return schema metadata as a dict.
-
-        This classmethod returns information about the table columns.
-
-        *Note*: this function is experimental and may not stay in the library
-        '''
-        info = inspect(cls)
-
-        metainfo = {}
-
-        for name, col in info.c.items():
-            if 'serializable' in col.info and not col.info['serializable']:
-                continue
-
-            try:
-                pytype = col.type.python_type.__qualname__
-            except NotImplementedError:
-                pytype = 'bytes'
-
-            m = {
-                "type": pytype,
-                "auto": col.autoincrement,
-                "pk": col.primary_key,
-                "default": col.default,
-                "nullable": col.nullable,
-            }
-
-            if hasattr(col.type, 'length'):
-                m['length'] = col.type.length
-            if hasattr(col.type, 'precision'):
-                m['precision'] = col.type.precision
-                m['scale'] = col.type.scale
-            if hasattr(col.type, 'enums'):
-                m['enums'] = col.type.enums
-
-            metainfo[name] = m
-
-        for name, rel in info.relationships.items():
-            if 'serializable' in col.info and not col.info['serializable']:
-                continue
-
-            m = {
-                "type": "relationship",
-                "target": rel.target.name,
-                "many": rel.uselist,
-                "manytomany": rel.secondary is not None,
-            }
-
-            metainfo[name] = m
-
-        return metainfo
 
     @classmethod
     async def async_factory(cls, resultset, fields=None, relationships=True,
             mtm_pkonly=True, encoding='utf-8'):
-        '''Create an async generator to serialize a result or result set to JSON.
+        '''Experimental: Create an async generator to serialize a result or result set to JSON.
 
         This classmethod creates a generator that streams JSON data, wrapping
         the set in the pluralized name if the object is iterable (i.e. a list),
         or in the singular name if not.
 
         :param resultset: An iterable (e.g. list or SQLAlchemy query), or a
             single mapped instance.
```

