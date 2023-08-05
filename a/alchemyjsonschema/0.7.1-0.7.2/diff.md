# Comparing `tmp/alchemyjsonschema-0.7.1.tar.gz` & `tmp/alchemyjsonschema-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchemyjsonschema-0.7.1.tar", last modified: Fri Apr 23 12:05:52 2021, max compression
+gzip compressed data, was "alchemyjsonschema-0.7.2.tar", last modified: Tue May 30 10:54:12 2023, max compression
```

## Comparing `alchemyjsonschema-0.7.1.tar` & `alchemyjsonschema-0.7.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 nao        (501) staff       (20)        0 2021-04-23 12:05:52.000000 alchemyjsonschema-0.7.1/
--rw-r--r--   0 nao        (501) staff       (20)    12471 2021-04-23 12:05:52.000000 alchemyjsonschema-0.7.1/PKG-INFO
--rw-r--r--   0 nao        (501) staff       (20)     8956 2021-03-30 14:05:11.000000 alchemyjsonschema-0.7.1/README.rst
-drwxr-xr-x   0 nao        (501) staff       (20)        0 2021-04-23 12:05:52.000000 alchemyjsonschema-0.7.1/alchemyjsonschema/
--rw-r--r--   0 nao        (501) staff       (20)    15664 2021-04-23 12:04:34.000000 alchemyjsonschema-0.7.1/alchemyjsonschema/__init__.py
-drwxr-xr-x   0 nao        (501) staff       (20)        0 2021-04-23 12:05:52.000000 alchemyjsonschema-0.7.1/alchemyjsonschema/command/
--rw-r--r--   0 nao        (501) staff       (20)        0 2021-03-30 12:06:42.000000 alchemyjsonschema-0.7.1/alchemyjsonschema/command/__init__.py
--rw-r--r--   0 nao        (501) staff       (20)     2645 2021-03-30 12:06:42.000000 alchemyjsonschema-0.7.1/alchemyjsonschema/command/_transformer.py
--rw-r--r--   0 nao        (501) staff       (20)     2261 2021-03-30 12:06:42.000000 alchemyjsonschema-0.7.1/alchemyjsonschema/command/driver.py
--rw-r--r--   0 nao        (501) staff       (20)     1103 2021-03-30 12:06:42.000000 alchemyjsonschema-0.7.1/alchemyjsonschema/command/main.py
-drwxr-xr-x   0 nao        (501) staff       (20)        0 2021-04-23 12:05:52.000000 alchemyjsonschema-0.7.1/alchemyjsonschema/custom/
--rw-r--r--   0 nao        (501) staff       (20)       23 2021-03-30 12:06:42.000000 alchemyjsonschema-0.7.1/alchemyjsonschema/custom/__init__.py
--rw-r--r--   0 nao        (501) staff       (20)     2360 2021-03-30 14:05:11.000000 alchemyjsonschema-0.7.1/alchemyjsonschema/custom/format.py
--rw-r--r--   0 nao        (501) staff       (20)       23 2021-03-30 12:06:42.000000 alchemyjsonschema-0.7.1/alchemyjsonschema/custom/validator.py
--rw-r--r--   0 nao        (501) staff       (20)       89 2021-03-30 12:06:42.000000 alchemyjsonschema-0.7.1/alchemyjsonschema/debug.py
--rw-r--r--   0 nao        (501) staff       (20)    13297 2021-03-30 14:05:11.000000 alchemyjsonschema-0.7.1/alchemyjsonschema/dictify.py
--rw-r--r--   0 nao        (501) staff       (20)     3142 2021-03-30 12:06:42.000000 alchemyjsonschema-0.7.1/alchemyjsonschema/mapping.py
--rw-r--r--   0 nao        (501) staff       (20)     1684 2021-03-30 12:06:42.000000 alchemyjsonschema-0.7.1/alchemyjsonschema/parser.py
-drwxr-xr-x   0 nao        (501) staff       (20)        0 2021-04-23 12:05:52.000000 alchemyjsonschema-0.7.1/alchemyjsonschema.egg-info/
--rw-r--r--   0 nao        (501) staff       (20)    12471 2021-04-23 12:05:52.000000 alchemyjsonschema-0.7.1/alchemyjsonschema.egg-info/PKG-INFO
--rw-r--r--   0 nao        (501) staff       (20)      720 2021-04-23 12:05:52.000000 alchemyjsonschema-0.7.1/alchemyjsonschema.egg-info/SOURCES.txt
--rw-r--r--   0 nao        (501) staff       (20)        1 2021-04-23 12:05:52.000000 alchemyjsonschema-0.7.1/alchemyjsonschema.egg-info/dependency_links.txt
--rw-r--r--   0 nao        (501) staff       (20)       93 2021-04-23 12:05:52.000000 alchemyjsonschema-0.7.1/alchemyjsonschema.egg-info/entry_points.txt
--rw-r--r--   0 nao        (501) staff       (20)        1 2021-03-30 12:08:19.000000 alchemyjsonschema-0.7.1/alchemyjsonschema.egg-info/not-zip-safe
--rw-r--r--   0 nao        (501) staff       (20)      113 2021-04-23 12:05:52.000000 alchemyjsonschema-0.7.1/alchemyjsonschema.egg-info/requires.txt
--rw-r--r--   0 nao        (501) staff       (20)       18 2021-04-23 12:05:52.000000 alchemyjsonschema-0.7.1/alchemyjsonschema.egg-info/top_level.txt
--rw-r--r--   0 nao        (501) staff       (20)       67 2021-04-23 12:05:52.000000 alchemyjsonschema-0.7.1/setup.cfg
--rw-r--r--   0 nao        (501) staff       (20)     1488 2021-03-30 12:06:42.000000 alchemyjsonschema-0.7.1/setup.py
+drwxr-xr-x   0 podhmo    (1000) podhmo    (1000)        0 2023-05-30 10:54:12.330640 alchemyjsonschema-0.7.2/
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     1063 2023-05-30 10:47:25.000000 alchemyjsonschema-0.7.2/LICENSE
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     9788 2023-05-30 10:54:12.330640 alchemyjsonschema-0.7.2/PKG-INFO
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     8956 2023-05-30 10:47:25.000000 alchemyjsonschema-0.7.2/README.rst
+drwxr-xr-x   0 podhmo    (1000) podhmo    (1000)        0 2023-05-30 10:54:12.330640 alchemyjsonschema-0.7.2/alchemyjsonschema/
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)    15664 2023-05-30 10:47:25.000000 alchemyjsonschema-0.7.2/alchemyjsonschema/__init__.py
+drwxr-xr-x   0 podhmo    (1000) podhmo    (1000)        0 2023-05-30 10:54:12.330640 alchemyjsonschema-0.7.2/alchemyjsonschema/command/
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)        0 2023-05-30 10:47:25.000000 alchemyjsonschema-0.7.2/alchemyjsonschema/command/__init__.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     2645 2023-05-30 10:47:25.000000 alchemyjsonschema-0.7.2/alchemyjsonschema/command/_transformer.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     2261 2023-05-30 10:47:25.000000 alchemyjsonschema-0.7.2/alchemyjsonschema/command/driver.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     1103 2023-05-30 10:47:25.000000 alchemyjsonschema-0.7.2/alchemyjsonschema/command/main.py
+drwxr-xr-x   0 podhmo    (1000) podhmo    (1000)        0 2023-05-30 10:54:12.330640 alchemyjsonschema-0.7.2/alchemyjsonschema/custom/
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)       23 2023-05-30 10:47:25.000000 alchemyjsonschema-0.7.2/alchemyjsonschema/custom/__init__.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     2360 2023-05-30 10:47:25.000000 alchemyjsonschema-0.7.2/alchemyjsonschema/custom/format.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)       23 2023-05-30 10:47:25.000000 alchemyjsonschema-0.7.2/alchemyjsonschema/custom/validator.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)       89 2023-05-30 10:47:25.000000 alchemyjsonschema-0.7.2/alchemyjsonschema/debug.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)    13297 2023-05-30 10:47:25.000000 alchemyjsonschema-0.7.2/alchemyjsonschema/dictify.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     3142 2023-05-30 10:47:25.000000 alchemyjsonschema-0.7.2/alchemyjsonschema/mapping.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     1684 2023-05-30 10:47:25.000000 alchemyjsonschema-0.7.2/alchemyjsonschema/parser.py
+drwxr-xr-x   0 podhmo    (1000) podhmo    (1000)        0 2023-05-30 10:54:12.330640 alchemyjsonschema-0.7.2/alchemyjsonschema.egg-info/
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     9788 2023-05-30 10:54:12.000000 alchemyjsonschema-0.7.2/alchemyjsonschema.egg-info/PKG-INFO
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      728 2023-05-30 10:54:12.000000 alchemyjsonschema-0.7.2/alchemyjsonschema.egg-info/SOURCES.txt
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)        1 2023-05-30 10:54:12.000000 alchemyjsonschema-0.7.2/alchemyjsonschema.egg-info/dependency_links.txt
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)       93 2023-05-30 10:54:12.000000 alchemyjsonschema-0.7.2/alchemyjsonschema.egg-info/entry_points.txt
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)        1 2023-05-30 10:48:49.000000 alchemyjsonschema-0.7.2/alchemyjsonschema.egg-info/not-zip-safe
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      115 2023-05-30 10:54:12.000000 alchemyjsonschema-0.7.2/alchemyjsonschema.egg-info/requires.txt
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)       18 2023-05-30 10:54:12.000000 alchemyjsonschema-0.7.2/alchemyjsonschema.egg-info/top_level.txt
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)       67 2023-05-30 10:54:12.330640 alchemyjsonschema-0.7.2/setup.cfg
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     1490 2023-05-30 10:47:25.000000 alchemyjsonschema-0.7.2/setup.py
```

### Comparing `alchemyjsonschema-0.7.1/PKG-INFO` & `alchemyjsonschema-0.7.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,358 +1,365 @@
 Metadata-Version: 2.1
 Name: alchemyjsonschema
-Version: 0.7.1
+Version: 0.7.2
 Summary: mapping jsonschema for sqlalchemy models
 Home-page: https://github.com/podhmo/alchemyjsonschema
 Author: podhmo
 Author-email: 
 License: mit
-Description: alchemyjsonschema
-        =================
-        
-        .. |Python package| image:: https://github.com/podhmo/alchemyjsonschema/actions/workflows/python-package.yml/badge.svg
-            :target: https://github.com/podhmo/alchemyjsonschema/actions/workflows/python-package.yml
-        
-        features
-        ----------------------------------------
-        
-        alchemyjsonschema is the library for converting sqlalchemys's model to jsonschema.
-        
-        - using alchemyjsonschema as command
-        - using alchemyjsonschema as library
-        
-        as library
-        ----------------------------------------
-        
-        having three output styles.
-        
-        - NoForeignKeyWalker -- ignore relationships
-        - ForeignKeyWalker -- expecting the information about relationship is foreign key
-        - StructuralWalker -- fullset output(expecting the information about relationship is full JSON data)
-        
-        examples
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        dumping json with above three output styles.
-        
-        target models are here. Group and User.
-        
-        .. code:: python
-        
-           # -*- coding:utf-8 -*-
-           import sqlalchemy as sa
-           import sqlalchemy.orm as orm
-           from sqlalchemy.ext.declarative import declarative_base
-        
-           Base = declarative_base()
-        
-        
-           class Group(Base):
-               """model for test"""
-               __tablename__ = "Group"
-        
-               pk = sa.Column(sa.Integer, primary_key=True, doc="primary key")
-               name = sa.Column(sa.String(255), default="", nullable=False)
-        
-        
-           class User(Base):
-               __tablename__ = "User"
-        
-               pk = sa.Column(sa.Integer, primary_key=True, doc="primary key")
-               name = sa.Column(sa.String(255), default="", nullable=True)
-               group_id = sa.Column(sa.Integer, sa.ForeignKey(Group.pk), nullable=False)
-               group = orm.relationship(Group, uselist=False, backref="users")
-        
-        
-        NoForeignKeyWalker
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: python
-        
-           import pprint as pp
-           from alchemyjsonschema import SchemaFactory
-           from alchemyjsonschema import NoForeignKeyWalker
-        
-           factory = SchemaFactory(NoForeignKeyWalker)
-           pp.pprint(factory(User))
-        
-           """
-           {'properties': {'name': {'maxLength': 255, 'type': 'string'},
-                           'pk': {'description': 'primary key', 'type': 'integer'}},
-            'required': ['pk'],
-            'title': 'User',
-            'type': 'object'}
-           """
-        
-        
-        ForeignKeyWalker
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: python
-        
-           import pprint as pp
-           from alchemyjsonschema import SchemaFactory
-           from alchemyjsonschema import ForeignKeyWalker
-        
-           factory = SchemaFactory(ForeignKeyWalker)
-           pp.pprint(factory(User))
-        
-           """
-           {'properties': {'group_id': {'type': 'integer'},
-                           'name': {'maxLength': 255, 'type': 'string'},
-                           'pk': {'description': 'primary key', 'type': 'integer'}},
-            'required': ['pk', 'group_id'],
-            'title': 'User',
-            'type': 'object'}
-           """
-        
-        
-        StructuralWalker
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        
-        .. code:: python
-        
-           import pprint as pp
-           from alchemyjsonschema import SchemaFactory
-           from alchemyjsonschema import StructuralWalker
-        
-           factory = SchemaFactory(StructuralWalker)
-           pp.pprint(factory(User))
-        
-           """
-           {'definitions': {'Group': {'properties': {'pk': {'description': 'primary key',
-                                                            'type': 'integer'},
-                                                     'name': {'maxLength': 255,
-                                                              'type': 'string'}},
-                                      'type': 'object'}},
-            'properties': {'pk': {'description': 'primary key', 'type': 'integer'},
-                           'name': {'maxLength': 255, 'type': 'string'},
-                           'group': {'$ref': '#/definitions/Group'}},
-            'required': ['pk'],
-            'title': 'User',
-            'type': 'object'}
-           """
-        
-           pp.pprint(factory(Group))
-        
-           """
-           {'definitions': {'User': {'properties': {'pk': {'description': 'primary key',
-                                                           'type': 'integer'},
-                                                    'name': {'maxLength': 255,
-                                                             'type': 'string'}},
-                                     'type': 'object'}},
-            'description': 'model for test',
-            'properties': {'pk': {'description': 'primary key', 'type': 'integer'},
-                           'name': {'maxLength': 255, 'type': 'string'},
-                           'users': {'items': {'$ref': '#/definitions/User'},
-                                     'type': 'array'}},
-            'required': ['pk', 'name'],
-            'title': 'Group',
-            'type': 'object'}
-           """
-        
-        as command
-        ----------------------------------------
-        
-        using alchemyjsonschema as command (the command name is also `alchemyjsonschema`).
-        
-        help
-        
-        .. code:: bash
-        
-            $ alchemyjsonschema --help
-            usage: alchemyjsonschema [-h] [--walker {noforeignkey,foreignkey,structural}]
-                                     [--decision {default,fullset}] [--depth DEPTH]
-                                     [--out OUT]
-                                     target
-        
-            positional arguments:
-              target                the module or class to extract schemas from
-        
-            optional arguments:
-              -h, --help            show this help message and exit
-              --walker {noforeignkey,foreignkey,structural}
-              --decision {default,fullset}
-              --depth DEPTH
-              --out OUT             output to file
-        
-        If above two model definitions (User,Group) are existed in `alchemyjsonschema.tests.models` .
-        
-        Target is the class position or module position. for example,
-        
-        - class position -- `alchemyjsonschema.tests.models:User`
-        - module position -- `alchemyjsonschema.tests.models`
-        
-        example
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        Using StructuralWalker via command line (--walker structural).
-        Of course, NoForeignKeyWalker is noforeignkey, and ForeignKeyWalker is foreignkey.
-        
-        .. code:: bash
-        
-            $ alchemyjsonschema --walker structural alchemyjsonschema.tests.models:Group
-        
-            {
-              "definitions": {
-                "Group": {
-                  "properties": {
-                    "color": {
-                      "enum": [
-                        "red",
-                        "green",
-                        "yellow",
-                        "blue"
-                      ],
-                      "maxLength": 6,
-                      "type": "string"
-                    },
-                    "created_at": {
-                      "format": "date-time",
-                      "type": "string"
-                    },
-                    "name": {
-                      "maxLength": 255,
-                      "type": "string"
-                    },
-                    "pk": {
-                      "description": "primary key",
-                      "type": "integer"
-                    },
-                    "users": {
-                      "items": {
-                        "$ref": "#/definitions/User"
-                      },
-                      "type": "array"
-                    }
-                  },
-                  "required": [
-                    "pk"
-                  ],
-                  "title": "Group",
-                  "type": "object"
-                },
-                "User": {
-                  "properties": {
-                    "created_at": {
-                      "format": "date-time",
-                      "type": "string"
-                    },
-                    "name": {
-                      "maxLength": 255,
-                      "type": "string"
-                    },
-                    "pk": {
-                      "description": "primary key",
-                      "type": "integer"
-                    }
-                  },
-                  "required": [
-                    "pk"
-                  ],
-                  "type": "object"
-                }
-              }
-            }
-        
-        Output is not same when using Walker-class, directly. This is handy output for something like a swagger(OpenAPI 2.0)'s tool.
-        
-        appendix: what is `--decision` ?
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        what is `--decision`? (TODO: gentle description)
-        
-        .. code-block:: bash
-        
-           $ alchemyjsonschema --walker structural alchemyjsonschema.tests.models:User | jq . -S > /tmp/default.json
-           $ alchemyjsonschema --decision useforeignkey --walker structural alchemyjsonschema.tests.models:User | jq . -S > /tmp/useforeignkey.json
-           $ diff -u /tmp/default.json /tmp/useforeignkey.json
-        
-        .. code-block:: diff
-        
-          --- /tmp/default.json	2017-01-02 22:49:44.000000000 +0900
-          +++ /tmp/useforeignkey.json	2017-01-02 22:53:13.000000000 +0900
-          @@ -1,43 +1,14 @@
-           {
-             "definitions": {
-          -    "Group": {
-          -      "properties": {
-          -        "color": {
-          -          "enum": [
-          -            "red",
-          -            "green",
-          -            "yellow",
-          -            "blue"
-          -          ],
-          -          "maxLength": 6,
-          -          "type": "string"
-          -        },
-          -        "created_at": {
-          -          "format": "date-time",
-          -          "type": "string"
-          -        },
-          -        "name": {
-          -          "maxLength": 255,
-          -          "type": "string"
-          -        },
-          -        "pk": {
-          -          "description": "primary key",
-          -          "type": "integer"
-          -        }
-          -      },
-          -      "required": [
-          -        "pk"
-          -      ],
-          -      "type": "object"
-          -    },
-               "User": {
-                 "properties": {
-                   "created_at": {
-                     "format": "date-time",
-                     "type": "string"
-                   },
-          -        "group": {
-          -          "$ref": "#/definitions/Group"
-          +        "group_id": {
-          +          "relation": "group",
-          +          "type": "integer"
-                   },
-                   "name": {
-                     "maxLength": 255,
-        
-        
-        0.7.1
-        
-        - adjust_required() option
-        
-        0.7.0
-        
-        - see server_default
-        - omit python 2.x
-        
-        0.6.1
-        
-        - catch up magicalimport 0.8.1
-        
-        0.6.0
-        
-        - fix for jsonschema-update
-        
-        0.4.2
-        
-        - fix bug calling command with module (not model class)
-        
-        0.4.0
-        
-        - remove needless feature(#11)
-        
-        0.3
-        
-        - swagger support(thanks of isysd)
-        
 Keywords: alchemyjsonschema sqlalchemy jsonschema schema-generation
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Provides-Extra: testing
 Provides-Extra: docs
+Provides-Extra: testing
+License-File: LICENSE
+
+alchemyjsonschema
+=================
+
+.. |Python package| image:: https://github.com/podhmo/alchemyjsonschema/actions/workflows/python-package.yml/badge.svg
+    :target: https://github.com/podhmo/alchemyjsonschema/actions/workflows/python-package.yml
+
+features
+----------------------------------------
+
+alchemyjsonschema is the library for converting sqlalchemys's model to jsonschema.
+
+- using alchemyjsonschema as command
+- using alchemyjsonschema as library
+
+as library
+----------------------------------------
+
+having three output styles.
+
+- NoForeignKeyWalker -- ignore relationships
+- ForeignKeyWalker -- expecting the information about relationship is foreign key
+- StructuralWalker -- fullset output(expecting the information about relationship is full JSON data)
+
+examples
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+dumping json with above three output styles.
+
+target models are here. Group and User.
+
+.. code:: python
+
+   # -*- coding:utf-8 -*-
+   import sqlalchemy as sa
+   import sqlalchemy.orm as orm
+   from sqlalchemy.ext.declarative import declarative_base
+
+   Base = declarative_base()
+
+
+   class Group(Base):
+       """model for test"""
+       __tablename__ = "Group"
+
+       pk = sa.Column(sa.Integer, primary_key=True, doc="primary key")
+       name = sa.Column(sa.String(255), default="", nullable=False)
+
+
+   class User(Base):
+       __tablename__ = "User"
+
+       pk = sa.Column(sa.Integer, primary_key=True, doc="primary key")
+       name = sa.Column(sa.String(255), default="", nullable=True)
+       group_id = sa.Column(sa.Integer, sa.ForeignKey(Group.pk), nullable=False)
+       group = orm.relationship(Group, uselist=False, backref="users")
+
+
+NoForeignKeyWalker
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+   import pprint as pp
+   from alchemyjsonschema import SchemaFactory
+   from alchemyjsonschema import NoForeignKeyWalker
+
+   factory = SchemaFactory(NoForeignKeyWalker)
+   pp.pprint(factory(User))
+
+   """
+   {'properties': {'name': {'maxLength': 255, 'type': 'string'},
+                   'pk': {'description': 'primary key', 'type': 'integer'}},
+    'required': ['pk'],
+    'title': 'User',
+    'type': 'object'}
+   """
+
+
+ForeignKeyWalker
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+   import pprint as pp
+   from alchemyjsonschema import SchemaFactory
+   from alchemyjsonschema import ForeignKeyWalker
+
+   factory = SchemaFactory(ForeignKeyWalker)
+   pp.pprint(factory(User))
+
+   """
+   {'properties': {'group_id': {'type': 'integer'},
+                   'name': {'maxLength': 255, 'type': 'string'},
+                   'pk': {'description': 'primary key', 'type': 'integer'}},
+    'required': ['pk', 'group_id'],
+    'title': 'User',
+    'type': 'object'}
+   """
+
+
+StructuralWalker
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+
+.. code:: python
+
+   import pprint as pp
+   from alchemyjsonschema import SchemaFactory
+   from alchemyjsonschema import StructuralWalker
+
+   factory = SchemaFactory(StructuralWalker)
+   pp.pprint(factory(User))
+
+   """
+   {'definitions': {'Group': {'properties': {'pk': {'description': 'primary key',
+                                                    'type': 'integer'},
+                                             'name': {'maxLength': 255,
+                                                      'type': 'string'}},
+                              'type': 'object'}},
+    'properties': {'pk': {'description': 'primary key', 'type': 'integer'},
+                   'name': {'maxLength': 255, 'type': 'string'},
+                   'group': {'$ref': '#/definitions/Group'}},
+    'required': ['pk'],
+    'title': 'User',
+    'type': 'object'}
+   """
+
+   pp.pprint(factory(Group))
+
+   """
+   {'definitions': {'User': {'properties': {'pk': {'description': 'primary key',
+                                                   'type': 'integer'},
+                                            'name': {'maxLength': 255,
+                                                     'type': 'string'}},
+                             'type': 'object'}},
+    'description': 'model for test',
+    'properties': {'pk': {'description': 'primary key', 'type': 'integer'},
+                   'name': {'maxLength': 255, 'type': 'string'},
+                   'users': {'items': {'$ref': '#/definitions/User'},
+                             'type': 'array'}},
+    'required': ['pk', 'name'],
+    'title': 'Group',
+    'type': 'object'}
+   """
+
+as command
+----------------------------------------
+
+using alchemyjsonschema as command (the command name is also `alchemyjsonschema`).
+
+help
+
+.. code:: bash
+
+    $ alchemyjsonschema --help
+    usage: alchemyjsonschema [-h] [--walker {noforeignkey,foreignkey,structural}]
+                             [--decision {default,fullset}] [--depth DEPTH]
+                             [--out OUT]
+                             target
+
+    positional arguments:
+      target                the module or class to extract schemas from
+
+    optional arguments:
+      -h, --help            show this help message and exit
+      --walker {noforeignkey,foreignkey,structural}
+      --decision {default,fullset}
+      --depth DEPTH
+      --out OUT             output to file
+
+If above two model definitions (User,Group) are existed in `alchemyjsonschema.tests.models` .
+
+Target is the class position or module position. for example,
+
+- class position -- `alchemyjsonschema.tests.models:User`
+- module position -- `alchemyjsonschema.tests.models`
+
+example
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Using StructuralWalker via command line (--walker structural).
+Of course, NoForeignKeyWalker is noforeignkey, and ForeignKeyWalker is foreignkey.
+
+.. code:: bash
+
+    $ alchemyjsonschema --walker structural alchemyjsonschema.tests.models:Group
+
+    {
+      "definitions": {
+        "Group": {
+          "properties": {
+            "color": {
+              "enum": [
+                "red",
+                "green",
+                "yellow",
+                "blue"
+              ],
+              "maxLength": 6,
+              "type": "string"
+            },
+            "created_at": {
+              "format": "date-time",
+              "type": "string"
+            },
+            "name": {
+              "maxLength": 255,
+              "type": "string"
+            },
+            "pk": {
+              "description": "primary key",
+              "type": "integer"
+            },
+            "users": {
+              "items": {
+                "$ref": "#/definitions/User"
+              },
+              "type": "array"
+            }
+          },
+          "required": [
+            "pk"
+          ],
+          "title": "Group",
+          "type": "object"
+        },
+        "User": {
+          "properties": {
+            "created_at": {
+              "format": "date-time",
+              "type": "string"
+            },
+            "name": {
+              "maxLength": 255,
+              "type": "string"
+            },
+            "pk": {
+              "description": "primary key",
+              "type": "integer"
+            }
+          },
+          "required": [
+            "pk"
+          ],
+          "type": "object"
+        }
+      }
+    }
+
+Output is not same when using Walker-class, directly. This is handy output for something like a swagger(OpenAPI 2.0)'s tool.
+
+appendix: what is `--decision` ?
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+what is `--decision`? (TODO: gentle description)
+
+.. code-block:: bash
+
+   $ alchemyjsonschema --walker structural alchemyjsonschema.tests.models:User | jq . -S > /tmp/default.json
+   $ alchemyjsonschema --decision useforeignkey --walker structural alchemyjsonschema.tests.models:User | jq . -S > /tmp/useforeignkey.json
+   $ diff -u /tmp/default.json /tmp/useforeignkey.json
+
+.. code-block:: diff
+
+  --- /tmp/default.json	2017-01-02 22:49:44.000000000 +0900
+  +++ /tmp/useforeignkey.json	2017-01-02 22:53:13.000000000 +0900
+  @@ -1,43 +1,14 @@
+   {
+     "definitions": {
+  -    "Group": {
+  -      "properties": {
+  -        "color": {
+  -          "enum": [
+  -            "red",
+  -            "green",
+  -            "yellow",
+  -            "blue"
+  -          ],
+  -          "maxLength": 6,
+  -          "type": "string"
+  -        },
+  -        "created_at": {
+  -          "format": "date-time",
+  -          "type": "string"
+  -        },
+  -        "name": {
+  -          "maxLength": 255,
+  -          "type": "string"
+  -        },
+  -        "pk": {
+  -          "description": "primary key",
+  -          "type": "integer"
+  -        }
+  -      },
+  -      "required": [
+  -        "pk"
+  -      ],
+  -      "type": "object"
+  -    },
+       "User": {
+         "properties": {
+           "created_at": {
+             "format": "date-time",
+             "type": "string"
+           },
+  -        "group": {
+  -          "$ref": "#/definitions/Group"
+  +        "group_id": {
+  +          "relation": "group",
+  +          "type": "integer"
+           },
+           "name": {
+             "maxLength": 255,
+
+
+0.7.2
+
+- Pin version of SQLAlchemy below 2.0 #31
+
+0.7.1
+
+- adjust_required() option
+
+0.7.0
+
+- see server_default
+- omit python 2.x
+
+0.6.1
+
+- catch up magicalimport 0.8.1
+
+0.6.0
+
+- fix for jsonschema-update
+
+0.4.2
+
+- fix bug calling command with module (not model class)
+
+0.4.0
+
+- remove needless feature(#11)
+
+0.3
+
+- swagger support(thanks of isysd)
+
+
```

### Comparing `alchemyjsonschema-0.7.1/README.rst` & `alchemyjsonschema-0.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `alchemyjsonschema-0.7.1/alchemyjsonschema/__init__.py` & `alchemyjsonschema-0.7.2/alchemyjsonschema/__init__.py`

 * *Files identical despite different names*

### Comparing `alchemyjsonschema-0.7.1/alchemyjsonschema/command/_transformer.py` & `alchemyjsonschema-0.7.2/alchemyjsonschema/command/_transformer.py`

 * *Files identical despite different names*

### Comparing `alchemyjsonschema-0.7.1/alchemyjsonschema/command/driver.py` & `alchemyjsonschema-0.7.2/alchemyjsonschema/command/driver.py`

 * *Files identical despite different names*

### Comparing `alchemyjsonschema-0.7.1/alchemyjsonschema/command/main.py` & `alchemyjsonschema-0.7.2/alchemyjsonschema/command/main.py`

 * *Files identical despite different names*

### Comparing `alchemyjsonschema-0.7.1/alchemyjsonschema/custom/format.py` & `alchemyjsonschema-0.7.2/alchemyjsonschema/custom/format.py`

 * *Files identical despite different names*

### Comparing `alchemyjsonschema-0.7.1/alchemyjsonschema/dictify.py` & `alchemyjsonschema-0.7.2/alchemyjsonschema/dictify.py`

 * *Files identical despite different names*

### Comparing `alchemyjsonschema-0.7.1/alchemyjsonschema/mapping.py` & `alchemyjsonschema-0.7.2/alchemyjsonschema/mapping.py`

 * *Files identical despite different names*

### Comparing `alchemyjsonschema-0.7.1/alchemyjsonschema/parser.py` & `alchemyjsonschema-0.7.2/alchemyjsonschema/parser.py`

 * *Files identical despite different names*

### Comparing `alchemyjsonschema-0.7.1/alchemyjsonschema.egg-info/PKG-INFO` & `alchemyjsonschema-0.7.2/alchemyjsonschema.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,358 +1,365 @@
 Metadata-Version: 2.1
 Name: alchemyjsonschema
-Version: 0.7.1
+Version: 0.7.2
 Summary: mapping jsonschema for sqlalchemy models
 Home-page: https://github.com/podhmo/alchemyjsonschema
 Author: podhmo
 Author-email: 
 License: mit
-Description: alchemyjsonschema
-        =================
-        
-        .. |Python package| image:: https://github.com/podhmo/alchemyjsonschema/actions/workflows/python-package.yml/badge.svg
-            :target: https://github.com/podhmo/alchemyjsonschema/actions/workflows/python-package.yml
-        
-        features
-        ----------------------------------------
-        
-        alchemyjsonschema is the library for converting sqlalchemys's model to jsonschema.
-        
-        - using alchemyjsonschema as command
-        - using alchemyjsonschema as library
-        
-        as library
-        ----------------------------------------
-        
-        having three output styles.
-        
-        - NoForeignKeyWalker -- ignore relationships
-        - ForeignKeyWalker -- expecting the information about relationship is foreign key
-        - StructuralWalker -- fullset output(expecting the information about relationship is full JSON data)
-        
-        examples
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        dumping json with above three output styles.
-        
-        target models are here. Group and User.
-        
-        .. code:: python
-        
-           # -*- coding:utf-8 -*-
-           import sqlalchemy as sa
-           import sqlalchemy.orm as orm
-           from sqlalchemy.ext.declarative import declarative_base
-        
-           Base = declarative_base()
-        
-        
-           class Group(Base):
-               """model for test"""
-               __tablename__ = "Group"
-        
-               pk = sa.Column(sa.Integer, primary_key=True, doc="primary key")
-               name = sa.Column(sa.String(255), default="", nullable=False)
-        
-        
-           class User(Base):
-               __tablename__ = "User"
-        
-               pk = sa.Column(sa.Integer, primary_key=True, doc="primary key")
-               name = sa.Column(sa.String(255), default="", nullable=True)
-               group_id = sa.Column(sa.Integer, sa.ForeignKey(Group.pk), nullable=False)
-               group = orm.relationship(Group, uselist=False, backref="users")
-        
-        
-        NoForeignKeyWalker
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: python
-        
-           import pprint as pp
-           from alchemyjsonschema import SchemaFactory
-           from alchemyjsonschema import NoForeignKeyWalker
-        
-           factory = SchemaFactory(NoForeignKeyWalker)
-           pp.pprint(factory(User))
-        
-           """
-           {'properties': {'name': {'maxLength': 255, 'type': 'string'},
-                           'pk': {'description': 'primary key', 'type': 'integer'}},
-            'required': ['pk'],
-            'title': 'User',
-            'type': 'object'}
-           """
-        
-        
-        ForeignKeyWalker
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: python
-        
-           import pprint as pp
-           from alchemyjsonschema import SchemaFactory
-           from alchemyjsonschema import ForeignKeyWalker
-        
-           factory = SchemaFactory(ForeignKeyWalker)
-           pp.pprint(factory(User))
-        
-           """
-           {'properties': {'group_id': {'type': 'integer'},
-                           'name': {'maxLength': 255, 'type': 'string'},
-                           'pk': {'description': 'primary key', 'type': 'integer'}},
-            'required': ['pk', 'group_id'],
-            'title': 'User',
-            'type': 'object'}
-           """
-        
-        
-        StructuralWalker
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        
-        .. code:: python
-        
-           import pprint as pp
-           from alchemyjsonschema import SchemaFactory
-           from alchemyjsonschema import StructuralWalker
-        
-           factory = SchemaFactory(StructuralWalker)
-           pp.pprint(factory(User))
-        
-           """
-           {'definitions': {'Group': {'properties': {'pk': {'description': 'primary key',
-                                                            'type': 'integer'},
-                                                     'name': {'maxLength': 255,
-                                                              'type': 'string'}},
-                                      'type': 'object'}},
-            'properties': {'pk': {'description': 'primary key', 'type': 'integer'},
-                           'name': {'maxLength': 255, 'type': 'string'},
-                           'group': {'$ref': '#/definitions/Group'}},
-            'required': ['pk'],
-            'title': 'User',
-            'type': 'object'}
-           """
-        
-           pp.pprint(factory(Group))
-        
-           """
-           {'definitions': {'User': {'properties': {'pk': {'description': 'primary key',
-                                                           'type': 'integer'},
-                                                    'name': {'maxLength': 255,
-                                                             'type': 'string'}},
-                                     'type': 'object'}},
-            'description': 'model for test',
-            'properties': {'pk': {'description': 'primary key', 'type': 'integer'},
-                           'name': {'maxLength': 255, 'type': 'string'},
-                           'users': {'items': {'$ref': '#/definitions/User'},
-                                     'type': 'array'}},
-            'required': ['pk', 'name'],
-            'title': 'Group',
-            'type': 'object'}
-           """
-        
-        as command
-        ----------------------------------------
-        
-        using alchemyjsonschema as command (the command name is also `alchemyjsonschema`).
-        
-        help
-        
-        .. code:: bash
-        
-            $ alchemyjsonschema --help
-            usage: alchemyjsonschema [-h] [--walker {noforeignkey,foreignkey,structural}]
-                                     [--decision {default,fullset}] [--depth DEPTH]
-                                     [--out OUT]
-                                     target
-        
-            positional arguments:
-              target                the module or class to extract schemas from
-        
-            optional arguments:
-              -h, --help            show this help message and exit
-              --walker {noforeignkey,foreignkey,structural}
-              --decision {default,fullset}
-              --depth DEPTH
-              --out OUT             output to file
-        
-        If above two model definitions (User,Group) are existed in `alchemyjsonschema.tests.models` .
-        
-        Target is the class position or module position. for example,
-        
-        - class position -- `alchemyjsonschema.tests.models:User`
-        - module position -- `alchemyjsonschema.tests.models`
-        
-        example
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        Using StructuralWalker via command line (--walker structural).
-        Of course, NoForeignKeyWalker is noforeignkey, and ForeignKeyWalker is foreignkey.
-        
-        .. code:: bash
-        
-            $ alchemyjsonschema --walker structural alchemyjsonschema.tests.models:Group
-        
-            {
-              "definitions": {
-                "Group": {
-                  "properties": {
-                    "color": {
-                      "enum": [
-                        "red",
-                        "green",
-                        "yellow",
-                        "blue"
-                      ],
-                      "maxLength": 6,
-                      "type": "string"
-                    },
-                    "created_at": {
-                      "format": "date-time",
-                      "type": "string"
-                    },
-                    "name": {
-                      "maxLength": 255,
-                      "type": "string"
-                    },
-                    "pk": {
-                      "description": "primary key",
-                      "type": "integer"
-                    },
-                    "users": {
-                      "items": {
-                        "$ref": "#/definitions/User"
-                      },
-                      "type": "array"
-                    }
-                  },
-                  "required": [
-                    "pk"
-                  ],
-                  "title": "Group",
-                  "type": "object"
-                },
-                "User": {
-                  "properties": {
-                    "created_at": {
-                      "format": "date-time",
-                      "type": "string"
-                    },
-                    "name": {
-                      "maxLength": 255,
-                      "type": "string"
-                    },
-                    "pk": {
-                      "description": "primary key",
-                      "type": "integer"
-                    }
-                  },
-                  "required": [
-                    "pk"
-                  ],
-                  "type": "object"
-                }
-              }
-            }
-        
-        Output is not same when using Walker-class, directly. This is handy output for something like a swagger(OpenAPI 2.0)'s tool.
-        
-        appendix: what is `--decision` ?
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        what is `--decision`? (TODO: gentle description)
-        
-        .. code-block:: bash
-        
-           $ alchemyjsonschema --walker structural alchemyjsonschema.tests.models:User | jq . -S > /tmp/default.json
-           $ alchemyjsonschema --decision useforeignkey --walker structural alchemyjsonschema.tests.models:User | jq . -S > /tmp/useforeignkey.json
-           $ diff -u /tmp/default.json /tmp/useforeignkey.json
-        
-        .. code-block:: diff
-        
-          --- /tmp/default.json	2017-01-02 22:49:44.000000000 +0900
-          +++ /tmp/useforeignkey.json	2017-01-02 22:53:13.000000000 +0900
-          @@ -1,43 +1,14 @@
-           {
-             "definitions": {
-          -    "Group": {
-          -      "properties": {
-          -        "color": {
-          -          "enum": [
-          -            "red",
-          -            "green",
-          -            "yellow",
-          -            "blue"
-          -          ],
-          -          "maxLength": 6,
-          -          "type": "string"
-          -        },
-          -        "created_at": {
-          -          "format": "date-time",
-          -          "type": "string"
-          -        },
-          -        "name": {
-          -          "maxLength": 255,
-          -          "type": "string"
-          -        },
-          -        "pk": {
-          -          "description": "primary key",
-          -          "type": "integer"
-          -        }
-          -      },
-          -      "required": [
-          -        "pk"
-          -      ],
-          -      "type": "object"
-          -    },
-               "User": {
-                 "properties": {
-                   "created_at": {
-                     "format": "date-time",
-                     "type": "string"
-                   },
-          -        "group": {
-          -          "$ref": "#/definitions/Group"
-          +        "group_id": {
-          +          "relation": "group",
-          +          "type": "integer"
-                   },
-                   "name": {
-                     "maxLength": 255,
-        
-        
-        0.7.1
-        
-        - adjust_required() option
-        
-        0.7.0
-        
-        - see server_default
-        - omit python 2.x
-        
-        0.6.1
-        
-        - catch up magicalimport 0.8.1
-        
-        0.6.0
-        
-        - fix for jsonschema-update
-        
-        0.4.2
-        
-        - fix bug calling command with module (not model class)
-        
-        0.4.0
-        
-        - remove needless feature(#11)
-        
-        0.3
-        
-        - swagger support(thanks of isysd)
-        
 Keywords: alchemyjsonschema sqlalchemy jsonschema schema-generation
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Provides-Extra: testing
 Provides-Extra: docs
+Provides-Extra: testing
+License-File: LICENSE
+
+alchemyjsonschema
+=================
+
+.. |Python package| image:: https://github.com/podhmo/alchemyjsonschema/actions/workflows/python-package.yml/badge.svg
+    :target: https://github.com/podhmo/alchemyjsonschema/actions/workflows/python-package.yml
+
+features
+----------------------------------------
+
+alchemyjsonschema is the library for converting sqlalchemys's model to jsonschema.
+
+- using alchemyjsonschema as command
+- using alchemyjsonschema as library
+
+as library
+----------------------------------------
+
+having three output styles.
+
+- NoForeignKeyWalker -- ignore relationships
+- ForeignKeyWalker -- expecting the information about relationship is foreign key
+- StructuralWalker -- fullset output(expecting the information about relationship is full JSON data)
+
+examples
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+dumping json with above three output styles.
+
+target models are here. Group and User.
+
+.. code:: python
+
+   # -*- coding:utf-8 -*-
+   import sqlalchemy as sa
+   import sqlalchemy.orm as orm
+   from sqlalchemy.ext.declarative import declarative_base
+
+   Base = declarative_base()
+
+
+   class Group(Base):
+       """model for test"""
+       __tablename__ = "Group"
+
+       pk = sa.Column(sa.Integer, primary_key=True, doc="primary key")
+       name = sa.Column(sa.String(255), default="", nullable=False)
+
+
+   class User(Base):
+       __tablename__ = "User"
+
+       pk = sa.Column(sa.Integer, primary_key=True, doc="primary key")
+       name = sa.Column(sa.String(255), default="", nullable=True)
+       group_id = sa.Column(sa.Integer, sa.ForeignKey(Group.pk), nullable=False)
+       group = orm.relationship(Group, uselist=False, backref="users")
+
+
+NoForeignKeyWalker
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+   import pprint as pp
+   from alchemyjsonschema import SchemaFactory
+   from alchemyjsonschema import NoForeignKeyWalker
+
+   factory = SchemaFactory(NoForeignKeyWalker)
+   pp.pprint(factory(User))
+
+   """
+   {'properties': {'name': {'maxLength': 255, 'type': 'string'},
+                   'pk': {'description': 'primary key', 'type': 'integer'}},
+    'required': ['pk'],
+    'title': 'User',
+    'type': 'object'}
+   """
+
+
+ForeignKeyWalker
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+   import pprint as pp
+   from alchemyjsonschema import SchemaFactory
+   from alchemyjsonschema import ForeignKeyWalker
+
+   factory = SchemaFactory(ForeignKeyWalker)
+   pp.pprint(factory(User))
+
+   """
+   {'properties': {'group_id': {'type': 'integer'},
+                   'name': {'maxLength': 255, 'type': 'string'},
+                   'pk': {'description': 'primary key', 'type': 'integer'}},
+    'required': ['pk', 'group_id'],
+    'title': 'User',
+    'type': 'object'}
+   """
+
+
+StructuralWalker
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+
+.. code:: python
+
+   import pprint as pp
+   from alchemyjsonschema import SchemaFactory
+   from alchemyjsonschema import StructuralWalker
+
+   factory = SchemaFactory(StructuralWalker)
+   pp.pprint(factory(User))
+
+   """
+   {'definitions': {'Group': {'properties': {'pk': {'description': 'primary key',
+                                                    'type': 'integer'},
+                                             'name': {'maxLength': 255,
+                                                      'type': 'string'}},
+                              'type': 'object'}},
+    'properties': {'pk': {'description': 'primary key', 'type': 'integer'},
+                   'name': {'maxLength': 255, 'type': 'string'},
+                   'group': {'$ref': '#/definitions/Group'}},
+    'required': ['pk'],
+    'title': 'User',
+    'type': 'object'}
+   """
+
+   pp.pprint(factory(Group))
+
+   """
+   {'definitions': {'User': {'properties': {'pk': {'description': 'primary key',
+                                                   'type': 'integer'},
+                                            'name': {'maxLength': 255,
+                                                     'type': 'string'}},
+                             'type': 'object'}},
+    'description': 'model for test',
+    'properties': {'pk': {'description': 'primary key', 'type': 'integer'},
+                   'name': {'maxLength': 255, 'type': 'string'},
+                   'users': {'items': {'$ref': '#/definitions/User'},
+                             'type': 'array'}},
+    'required': ['pk', 'name'],
+    'title': 'Group',
+    'type': 'object'}
+   """
+
+as command
+----------------------------------------
+
+using alchemyjsonschema as command (the command name is also `alchemyjsonschema`).
+
+help
+
+.. code:: bash
+
+    $ alchemyjsonschema --help
+    usage: alchemyjsonschema [-h] [--walker {noforeignkey,foreignkey,structural}]
+                             [--decision {default,fullset}] [--depth DEPTH]
+                             [--out OUT]
+                             target
+
+    positional arguments:
+      target                the module or class to extract schemas from
+
+    optional arguments:
+      -h, --help            show this help message and exit
+      --walker {noforeignkey,foreignkey,structural}
+      --decision {default,fullset}
+      --depth DEPTH
+      --out OUT             output to file
+
+If above two model definitions (User,Group) are existed in `alchemyjsonschema.tests.models` .
+
+Target is the class position or module position. for example,
+
+- class position -- `alchemyjsonschema.tests.models:User`
+- module position -- `alchemyjsonschema.tests.models`
+
+example
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Using StructuralWalker via command line (--walker structural).
+Of course, NoForeignKeyWalker is noforeignkey, and ForeignKeyWalker is foreignkey.
+
+.. code:: bash
+
+    $ alchemyjsonschema --walker structural alchemyjsonschema.tests.models:Group
+
+    {
+      "definitions": {
+        "Group": {
+          "properties": {
+            "color": {
+              "enum": [
+                "red",
+                "green",
+                "yellow",
+                "blue"
+              ],
+              "maxLength": 6,
+              "type": "string"
+            },
+            "created_at": {
+              "format": "date-time",
+              "type": "string"
+            },
+            "name": {
+              "maxLength": 255,
+              "type": "string"
+            },
+            "pk": {
+              "description": "primary key",
+              "type": "integer"
+            },
+            "users": {
+              "items": {
+                "$ref": "#/definitions/User"
+              },
+              "type": "array"
+            }
+          },
+          "required": [
+            "pk"
+          ],
+          "title": "Group",
+          "type": "object"
+        },
+        "User": {
+          "properties": {
+            "created_at": {
+              "format": "date-time",
+              "type": "string"
+            },
+            "name": {
+              "maxLength": 255,
+              "type": "string"
+            },
+            "pk": {
+              "description": "primary key",
+              "type": "integer"
+            }
+          },
+          "required": [
+            "pk"
+          ],
+          "type": "object"
+        }
+      }
+    }
+
+Output is not same when using Walker-class, directly. This is handy output for something like a swagger(OpenAPI 2.0)'s tool.
+
+appendix: what is `--decision` ?
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+what is `--decision`? (TODO: gentle description)
+
+.. code-block:: bash
+
+   $ alchemyjsonschema --walker structural alchemyjsonschema.tests.models:User | jq . -S > /tmp/default.json
+   $ alchemyjsonschema --decision useforeignkey --walker structural alchemyjsonschema.tests.models:User | jq . -S > /tmp/useforeignkey.json
+   $ diff -u /tmp/default.json /tmp/useforeignkey.json
+
+.. code-block:: diff
+
+  --- /tmp/default.json	2017-01-02 22:49:44.000000000 +0900
+  +++ /tmp/useforeignkey.json	2017-01-02 22:53:13.000000000 +0900
+  @@ -1,43 +1,14 @@
+   {
+     "definitions": {
+  -    "Group": {
+  -      "properties": {
+  -        "color": {
+  -          "enum": [
+  -            "red",
+  -            "green",
+  -            "yellow",
+  -            "blue"
+  -          ],
+  -          "maxLength": 6,
+  -          "type": "string"
+  -        },
+  -        "created_at": {
+  -          "format": "date-time",
+  -          "type": "string"
+  -        },
+  -        "name": {
+  -          "maxLength": 255,
+  -          "type": "string"
+  -        },
+  -        "pk": {
+  -          "description": "primary key",
+  -          "type": "integer"
+  -        }
+  -      },
+  -      "required": [
+  -        "pk"
+  -      ],
+  -      "type": "object"
+  -    },
+       "User": {
+         "properties": {
+           "created_at": {
+             "format": "date-time",
+             "type": "string"
+           },
+  -        "group": {
+  -          "$ref": "#/definitions/Group"
+  +        "group_id": {
+  +          "relation": "group",
+  +          "type": "integer"
+           },
+           "name": {
+             "maxLength": 255,
+
+
+0.7.2
+
+- Pin version of SQLAlchemy below 2.0 #31
+
+0.7.1
+
+- adjust_required() option
+
+0.7.0
+
+- see server_default
+- omit python 2.x
+
+0.6.1
+
+- catch up magicalimport 0.8.1
+
+0.6.0
+
+- fix for jsonschema-update
+
+0.4.2
+
+- fix bug calling command with module (not model class)
+
+0.4.0
+
+- remove needless feature(#11)
+
+0.3
+
+- swagger support(thanks of isysd)
+
+
```

### Comparing `alchemyjsonschema-0.7.1/alchemyjsonschema.egg-info/SOURCES.txt` & `alchemyjsonschema-0.7.2/alchemyjsonschema.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.rst
 setup.cfg
 setup.py
 alchemyjsonschema/__init__.py
 alchemyjsonschema/debug.py
 alchemyjsonschema/dictify.py
 alchemyjsonschema/mapping.py
```

### Comparing `alchemyjsonschema-0.7.1/setup.py` & `alchemyjsonschema-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         README = f.read()
     with open(os.path.join(here, "CHANGES.txt")) as f:
         CHANGES = f.read()
 except IOError:
     README = CHANGES = ""
 
 install_requires = [
-    "sqlalchemy",
+    "sqlalchemy<2",
     "jsonschema",
     "strict-rfc3339",
     "isodate",  # hmm.
     "pytz",
     "magicalimport",
     "dictknife>=0.7.2",
 ]
```

