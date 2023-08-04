# Comparing `tmp/uiclasses-2.4.0.tar.gz` & `tmp/uiclasses-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/uiclasses-2.4.0.tar", last modified: Mon Jul 19 21:38:56 2021, max compression
+gzip compressed data, was "uiclasses-3.0.0.tar", last modified: Fri Aug  4 22:12:22 2023, max compression
```

## Comparing `uiclasses-2.4.0.tar` & `uiclasses-3.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 gabrielfalcao   (502) staff       (20)        0 2021-07-19 21:38:56.000000 uiclasses-2.4.0/
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)     5402 2021-05-17 21:15:38.000000 uiclasses-2.4.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)     1877 2021-07-19 21:36:39.000000 uiclasses-2.4.0/CONTRIBUTING.rst
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)     1057 2021-07-19 21:36:23.000000 uiclasses-2.4.0/LICENSE
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)       30 2021-05-17 21:15:38.000000 uiclasses-2.4.0/MANIFEST.in
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)     4578 2021-07-19 21:38:56.000000 uiclasses-2.4.0/PKG-INFO
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)     3302 2021-07-19 21:38:49.000000 uiclasses-2.4.0/README.rst
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)      233 2021-07-19 21:38:49.000000 uiclasses-2.4.0/development.txt
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)       30 2021-05-17 21:15:38.000000 uiclasses-2.4.0/pyproject.toml
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)       79 2021-05-17 21:15:38.000000 uiclasses-2.4.0/requirements.txt
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)      295 2021-07-19 21:38:56.000000 uiclasses-2.4.0/setup.cfg
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)     2484 2021-07-19 21:37:02.000000 uiclasses-2.4.0/setup.py
-drwxr-xr-x   0 gabrielfalcao   (502) staff       (20)        0 2021-07-19 21:38:56.000000 uiclasses-2.4.0/uiclasses/
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)     1958 2021-07-19 21:36:23.000000 uiclasses-2.4.0/uiclasses/__init__.py
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)    16416 2021-07-19 21:36:23.000000 uiclasses-2.4.0/uiclasses/base.py
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)    10823 2021-07-19 21:36:23.000000 uiclasses-2.4.0/uiclasses/collections.py
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)     1513 2021-07-19 21:36:23.000000 uiclasses-2.4.0/uiclasses/errors.py
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)     2628 2021-07-19 21:36:23.000000 uiclasses-2.4.0/uiclasses/fs.py
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)     1426 2021-07-19 21:36:23.000000 uiclasses-2.4.0/uiclasses/meta.py
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)     2639 2021-07-19 21:36:23.000000 uiclasses-2.4.0/uiclasses/typing.py
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)     5232 2021-07-19 21:36:23.000000 uiclasses-2.4.0/uiclasses/utils.py
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)     1113 2021-07-19 21:38:49.000000 uiclasses-2.4.0/uiclasses/version.py
-drwxr-xr-x   0 gabrielfalcao   (502) staff       (20)        0 2021-07-19 21:38:56.000000 uiclasses-2.4.0/uiclasses.egg-info/
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)     4578 2021-07-19 21:38:56.000000 uiclasses-2.4.0/uiclasses.egg-info/PKG-INFO
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)      545 2021-07-19 21:38:56.000000 uiclasses-2.4.0/uiclasses.egg-info/SOURCES.txt
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)        1 2021-07-19 21:38:56.000000 uiclasses-2.4.0/uiclasses.egg-info/dependency_links.txt
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)       56 2021-07-19 21:38:56.000000 uiclasses-2.4.0/uiclasses.egg-info/entry_points.txt
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)        1 2021-07-19 21:03:46.000000 uiclasses-2.4.0/uiclasses.egg-info/not-zip-safe
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)       83 2021-07-19 21:38:56.000000 uiclasses-2.4.0/uiclasses.egg-info/requires.txt
--rw-r--r--   0 gabrielfalcao   (502) staff       (20)       10 2021-07-19 21:38:56.000000 uiclasses-2.4.0/uiclasses.egg-info/top_level.txt
+drwx------   0 gabrielfalcao   (504) staff       (20)        0 2023-08-04 22:12:22.147871 uiclasses-3.0.0/
+-rw-------   0 gabrielfalcao   (504) staff       (20)     5402 2023-08-04 22:01:17.000000 uiclasses-3.0.0/CODE_OF_CONDUCT.rst
+-rw-------   0 gabrielfalcao   (504) staff       (20)     1877 2023-08-04 22:01:16.000000 uiclasses-3.0.0/CONTRIBUTING.rst
+-rw-------   0 gabrielfalcao   (504) staff       (20)     1083 2023-08-04 22:01:16.000000 uiclasses-3.0.0/LICENSE
+-rw-------   0 gabrielfalcao   (504) staff       (20)       30 2023-08-04 22:01:16.000000 uiclasses-3.0.0/MANIFEST.in
+-rw-------   0 gabrielfalcao   (504) staff       (20)     4465 2023-08-04 22:12:22.147934 uiclasses-3.0.0/PKG-INFO
+-rw-------   0 gabrielfalcao   (504) staff       (20)     3126 2023-08-04 22:01:16.000000 uiclasses-3.0.0/README.rst
+-rw-------   0 gabrielfalcao   (504) staff       (20)      233 2023-08-04 22:01:17.000000 uiclasses-3.0.0/development.txt
+-rw-------   0 gabrielfalcao   (504) staff       (20)       30 2023-08-04 22:01:16.000000 uiclasses-3.0.0/pyproject.toml
+-rw-------   0 gabrielfalcao   (504) staff       (20)       79 2023-08-04 22:01:16.000000 uiclasses-3.0.0/requirements.txt
+-rw-------   0 gabrielfalcao   (504) staff       (20)      295 2023-08-04 22:12:22.148544 uiclasses-3.0.0/setup.cfg
+-rw-------   0 gabrielfalcao   (504) staff       (20)     2582 2023-08-04 22:01:16.000000 uiclasses-3.0.0/setup.py
+drwx------   0 gabrielfalcao   (504) staff       (20)        0 2023-08-04 22:12:22.146938 uiclasses-3.0.0/uiclasses/
+-rw-------   0 gabrielfalcao   (504) staff       (20)     1990 2023-08-04 22:01:16.000000 uiclasses-3.0.0/uiclasses/__init__.py
+-rw-------   0 gabrielfalcao   (504) staff       (20)    16448 2023-08-04 22:01:16.000000 uiclasses-3.0.0/uiclasses/base.py
+-rw-------   0 gabrielfalcao   (504) staff       (20)    10912 2023-08-04 22:01:16.000000 uiclasses-3.0.0/uiclasses/collections.py
+-rw-------   0 gabrielfalcao   (504) staff       (20)     1539 2023-08-04 22:01:16.000000 uiclasses-3.0.0/uiclasses/errors.py
+-rw-------   0 gabrielfalcao   (504) staff       (20)     2654 2023-08-04 22:01:16.000000 uiclasses-3.0.0/uiclasses/fs.py
+-rw-------   0 gabrielfalcao   (504) staff       (20)     1455 2023-08-04 22:01:16.000000 uiclasses-3.0.0/uiclasses/meta.py
+-rw-------   0 gabrielfalcao   (504) staff       (20)     2665 2023-08-04 22:01:16.000000 uiclasses-3.0.0/uiclasses/typing.py
+-rw-------   0 gabrielfalcao   (504) staff       (20)     5261 2023-08-04 22:01:16.000000 uiclasses-3.0.0/uiclasses/utils.py
+-rw-------   0 gabrielfalcao   (504) staff       (20)     1139 2023-08-04 22:01:16.000000 uiclasses-3.0.0/uiclasses/version.py
+drwx------   0 gabrielfalcao   (504) staff       (20)        0 2023-08-04 22:12:22.147775 uiclasses-3.0.0/uiclasses.egg-info/
+-rw-------   0 gabrielfalcao   (504) staff       (20)     4465 2023-08-04 22:12:22.000000 uiclasses-3.0.0/uiclasses.egg-info/PKG-INFO
+-rw-------   0 gabrielfalcao   (504) staff       (20)      545 2023-08-04 22:12:22.000000 uiclasses-3.0.0/uiclasses.egg-info/SOURCES.txt
+-rw-------   0 gabrielfalcao   (504) staff       (20)        1 2023-08-04 22:12:22.000000 uiclasses-3.0.0/uiclasses.egg-info/dependency_links.txt
+-rw-------   0 gabrielfalcao   (504) staff       (20)       55 2023-08-04 22:12:22.000000 uiclasses-3.0.0/uiclasses.egg-info/entry_points.txt
+-rw-------   0 gabrielfalcao   (504) staff       (20)        1 2023-08-04 22:04:47.000000 uiclasses-3.0.0/uiclasses.egg-info/not-zip-safe
+-rw-------   0 gabrielfalcao   (504) staff       (20)       83 2023-08-04 22:12:22.000000 uiclasses-3.0.0/uiclasses.egg-info/requires.txt
+-rw-------   0 gabrielfalcao   (504) staff       (20)       10 2023-08-04 22:12:22.000000 uiclasses-3.0.0/uiclasses.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `uiclasses-2.4.0/CODE_OF_CONDUCT.rst` & `uiclasses-3.0.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `uiclasses-2.4.0/CONTRIBUTING.rst` & `uiclasses-3.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `uiclasses-2.4.0/LICENSE` & `uiclasses-3.0.0/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2020 Gabriel Falcao
+Copyright (c) 2020-2023 Gabriel Falcão Gonçalves de Moura
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `uiclasses-2.4.0/PKG-INFO` & `uiclasses-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,50 @@
 Metadata-Version: 2.1
 Name: uiclasses
-Version: 2.4.0
+Version: 3.0.0
 Summary: Data-Modeling for User Interfaces
 Home-page: https://github.com/gabrielfalcao/uiclasses
 Author: Gabriel Falcao
 Author-email: gabriel@nacaolivre.org
 Maintainer: Gabriel Falcão
 Maintainer-email: gabriel@nacaolivre.org
-License: UNKNOWN
 Project-URL: Documentation, https://uiclasses.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/gabrielfalcao/uiclasses
 Project-URL: Issue Tracker, https://github.com/gabrielfalcao/uiclasses/issues
 Project-URL: Test Coverage, https://codecov.io/gh/gabrielfalcao/uiclasses
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Handhelds/PDA's
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
 License-File: LICENSE
 
 UIClasses - Data-Modeling for User Interfaces
 ##############################################
 
 
 .. image:: https://img.shields.io/pypi/dm/uiclasses
    :target: https://pypi.org/project/uiclasses
 
 .. image:: https://img.shields.io/codecov/c/github/gabrielfalcao/uiclasses
    :target: https://codecov.io/gh/gabrielfalcao/uiclasses
 
-.. image:: https://img.shields.io/github/workflow/status/gabrielfalcao/uiclasses/python-3.6?label=python%203.6
-   :target: https://github.com/gabrielfalcao/uiclasses/actions
-
-.. image:: https://img.shields.io/github/workflow/status/gabrielfalcao/uiclasses/python-3.7?label=python%203.7
-   :target: https://github.com/gabrielfalcao/uiclasses/actions
+.. image:: https://github.com/gabrielfalcao/uiclasses/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/gabrielfalcao/uiclasses/actions/workflows/main.yml
 
 .. image:: https://img.shields.io/readthedocs/uiclasses
    :target: https://uiclasses.readthedocs.io/
 
 .. image:: https://img.shields.io/github/license/gabrielfalcao/uiclasses?label=Github%20License
    :target: https://github.com/gabrielfalcao/uiclasses/blob/master/LICENSE
 
@@ -129,9 +126,7 @@
 Notes:
 ======
 
 
 - This is not designed to be fast, when adding data to models their
   types might cast and validated, which is costly.
   - filtering collections by string values cause glob match
-
-
```

### Comparing `uiclasses-2.4.0/README.rst` & `uiclasses-3.0.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,16 @@
 
 .. image:: https://img.shields.io/pypi/dm/uiclasses
    :target: https://pypi.org/project/uiclasses
 
 .. image:: https://img.shields.io/codecov/c/github/gabrielfalcao/uiclasses
    :target: https://codecov.io/gh/gabrielfalcao/uiclasses
 
-.. image:: https://img.shields.io/github/workflow/status/gabrielfalcao/uiclasses/python-3.6?label=python%203.6
-   :target: https://github.com/gabrielfalcao/uiclasses/actions
-
-.. image:: https://img.shields.io/github/workflow/status/gabrielfalcao/uiclasses/python-3.7?label=python%203.7
-   :target: https://github.com/gabrielfalcao/uiclasses/actions
+.. image:: https://github.com/gabrielfalcao/uiclasses/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/gabrielfalcao/uiclasses/actions/workflows/main.yml
 
 .. image:: https://img.shields.io/readthedocs/uiclasses
    :target: https://uiclasses.readthedocs.io/
 
 .. image:: https://img.shields.io/github/license/gabrielfalcao/uiclasses?label=Github%20License
    :target: https://github.com/gabrielfalcao/uiclasses/blob/master/LICENSE
```

### Comparing `uiclasses-2.4.0/setup.py` & `uiclasses-3.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,11 +67,13 @@
         "Environment :: Win32 (MS Windows)",
         "Environment :: X11 Applications",
         "License :: OSI Approved :: MIT License",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: Implementation :: CPython",
     ],
     dependency_links=[],
 )
```

### Comparing `uiclasses-2.4.0/uiclasses/__init__.py` & `uiclasses-3.0.0/uiclasses/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020 Gabriel Falcao
+# Copyright (c) 2020-2023 Gabriel Falcão Gonçalves de Moura
 
 # Permission is hereby granted, free of charge, to any person
 # obtaining a copy of this software and associated documentation files
 # (the "Software"), to deal in the Software without restriction,
 # including without limitation the rights to use, copy, modify, merge,
 # publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so,
@@ -36,25 +36,25 @@
 
 from .base import (
     basic_dataclass,
     DataBag,
     DataBagChild,
     Model,
     repr_attributes,
-    traverse_dict_children,
+    traverse_dict_descendants,
     try_int,
     try_json,
     UserFriendlyObject,
 )
 from .collections import IterableCollection, ModelList, ModelSet
 
 
 __all__ = [
     "Model",
-    "traverse_dict_children",
+    "traverse_dict_descendants",
     "repr_attributes",
     "UserFriendlyObject",
     "DataBag",
     "DataBagChild",
     "basic_dataclass",
     "try_int",
     "try_json",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `uiclasses-2.4.0/uiclasses/base.py` & `uiclasses-3.0.0/uiclasses/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020 Gabriel Falcao
+# Copyright (c) 2020-2023 Gabriel Falcão Gonçalves de Moura
 
 # Permission is hereby granted, free of charge, to any person
 # obtaining a copy of this software and associated documentation files
 # (the "Software"), to deal in the Software without restriction,
 # including without limitation the rights to use, copy, modify, merge,
 # publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so,
@@ -43,15 +43,15 @@
     get_getter_by_name,
     get_setter_by_name,
     list_field_names_from_dataclass,
     list_getters_from_metaclass,
     list_setters_from_metaclass,
     list_visible_field_names_from_dataclass,
     repr_attributes,
-    traverse_dict_children,
+    traverse_dict_descendants,
     try_dict,
     try_int,
     try_json,
     unique,
 )
 
 
@@ -112,15 +112,15 @@
         return bool(self.__data__)
 
     def update(self, other: dict):
         self.__data__.update(other or {})
 
     def traverse(self, *keys, fallback=None):
         """attempts to retrieve the config value under the given nested keys"""
-        value = traverse_dict_children(self.__data__, *keys, fallback=fallback)
+        value = traverse_dict_descendants(self.__data__, *keys, fallback=fallback)
         if isinstance(value, dict):
             return DataBagChild(value, *keys)
 
         return value
 
     def __ui_attributes__(self):
         """converts self.__data__ to dict to prevent recursion error"""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `uiclasses-2.4.0/uiclasses/collections.py` & `uiclasses-3.0.0/uiclasses/collections.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020 Gabriel Falcao
+# Copyright (c) 2020-2023 Gabriel Falcão Gonçalves de Moura
 
 # Permission is hereby granted, free of charge, to any person
 # obtaining a copy of this software and associated documentation files
 # (the "Software"), to deal in the Software without restriction,
 # including without limitation the rights to use, copy, modify, merge,
 # publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so,
@@ -51,15 +51,15 @@
 class IterableCollection(UserFriendlyObject, Sized, IterableType[T]):
     """Base mixin for ModelList and ModelSet, provides methods to
     manipulate iterable collections in ways take advantage of the
     behavior of models.
 
 
     For example it supports filtering by instance attributes through a cal to the
-    :py:meth:`~uiclasses.base.Model.attribute_matches` method of each children.
+    :py:meth:`~uiclasses.base.Model.attribute_matches` method of each descendants.
 
     **Features:**
 
     - :py:meth:`~uiclasses.collections.IterableCollection.sorted_by` - sort by a single attribute
     - :py:meth:`~uiclasses.collections.IterableCollection.filter_by` - to filter by a single attribute
     - :py:meth:`~uiclasses.collections.IterableCollection.sorted` - alias to ``MyModel.List(sorted(my_model_collection))`` or ``.Set()``
     - :py:meth:`~uiclasses.collections.IterableCollection.filter` - alias to ``MyModel.List(filter(callback, my_model_collection))``
@@ -79,30 +79,30 @@
         for x in super().__iter__():
             yield x
 
     def __len__(self) -> int:
         return super().__len__()
 
     def sorted(self, **kw):
-        """returns a new ``ModelList`` with this collections' children sorted.
+        """returns a new ``ModelList`` with this collections' descendants sorted.
 
         Example:
 
         .. code::
 
            x = MyModel.List([MyModel({"id": 2}), MyModel({"id": 3})])
            result = x.sorted(key=lambda model: model.id)
 
         """
 
         items = sorted(self, **kw)
         return self.__class__(items)
 
     def sorted_by(self, attribute: str, **kw):
-        """sort by a single attribute of the model children.
+        """sort by a single attribute of the model descendants.
 
         Example:
 
         .. code::
 
            x = MyModel.List([MyModel({"id": 2}), MyModel({"id": 3})])
            result = x.sorted_by('id')
@@ -113,15 +113,15 @@
             or "",
             **kw,
         )
 
     def filter_by(
         self, attribute_name: str, fnmatch_pattern: str
     ) -> internal_typing.IterableCollection[Model]:
-        """filter by a single attribute of the model children.
+        """filter by a single attribute of the model descendants.
 
         Example:
 
         .. code::
 
            x = MyModel.List([MyModel({"name": 'chucknorris'}), MyModel({"name": 'foobar'})])
            result = x.filter_by('name', '*norris*')
@@ -130,15 +130,15 @@
         return self.filter(
             lambda model: model.attribute_matches(
                 attribute_name, fnmatch_pattern
             )
         )
 
     def filter(self, check: Callable[[Model], bool]) -> IterableType[Model]:
-        """returns a new ``ModelList`` with this collections' children filter.
+        """returns a new ``ModelList`` with this collections' descendants filter.
 
         Example:
 
         .. code::
 
            x = MyModel.List([MyModel({"id": 2}), MyModel({"id": 3})])
            result = x.filter(key=lambda model: model.id)
@@ -209,47 +209,47 @@
                 f"the following columns are not available "
                 f"for {self.__of_model__}: {mismatched_columns}"
             )
 
         return columns
 
     def to_dict(self, only_visible: bool = False) -> IterableType[dict]:
-        """calls ``.to_dict()`` in each children of this collection."""
+        """calls ``.to_dict()`` in each descendants of this collection."""
         return [m.to_dict(only_visible=only_visible) for m in self]
 
     def serialize(self, only_visible: bool = False) -> IterableType[dict]:
-        """calls ``.serialize()`` in each children of this collection."""
+        """calls ``.serialize()`` in each descendants of this collection."""
         return [m.serialize(only_visible=only_visible) for m in self]
 
     def serialize_visible(self) -> IterableType[dict]:
-        """calls ``.serialize_visible()`` in each children of this collection."""
+        """calls ``.serialize_visible()`` in each descendants of this collection."""
         return [m.serialize_visible() for m in self]
 
     def serialize_all(self) -> IterableType[dict]:
-        """calls ``.serialize_all()`` in each children of this collection."""
+        """calls ``.serialize_all()`` in each descendants of this collection."""
         return [m.serialize_all() for m in self]
 
 
 class ModelList(list, IterableCollection[T]):
     """Implementation of :py:class:`~uiclasses.collections.IterableCollection` for the
     :py:class:`list` type.
 
     """
 
-    def __init__(self, children: IterableType[T]):
+    def __init__(self, descendants: IterableType[T]):
         model_class = self.__of_model__
 
-        if not is_iterable(children):
+        if not is_iterable(descendants):
             raise TypeError(
-                f"{self.__class__.__name__} requires the 'children' attribute to be "
-                f"a valid iterable, got {children!r} {type(children)} instead"
+                f"{self.__class__.__name__} requires the 'descendants' attribute to be "
+                f"a valid iterable, got {descendants!r} {type(descendants)} instead"
             )
 
         items = []
-        for index, child in enumerate(children):
+        for index, child in enumerate(descendants):
             if isinstance(child, dict):
                 child = self.__of_model__(child)
             if not isinstance(child, model_class):
                 raise TypeError(
                     f"cannot create {self.__class__.__name__} because value at index [{index}] is not a {model_class}: {child!r} {type(child)}"
                 )
             items.append(child)
@@ -269,24 +269,24 @@
 
 
 class ModelSet(OrderedSet, IterableCollection):
     """Implementation of :py:class:`~uiclasses.collections.IterableCollection` for the
     `OrderedSet <https://pypi.org/project/ordered-set/>`_ type.
     """
 
-    def __init__(self, children: IterableType[Model]):
+    def __init__(self, descendants: IterableType[Model]):
         model_class = getattr(self, "__of_model__", None)
 
-        if not is_iterable(children):
+        if not is_iterable(descendants):
             raise TypeError(
-                f"{self.__class__.__name__} requires the 'children' attribute to be "
-                f"a valid iterable, got {children!r} {type(children)} instead"
+                f"{self.__class__.__name__} requires the 'descendants' attribute to be "
+                f"a valid iterable, got {descendants!r} {type(descendants)} instead"
             )
         items = []
-        for index, child in enumerate(children):
+        for index, child in enumerate(descendants):
             if isinstance(child, dict):
                 child = self.__of_model__(child)
 
             if not isinstance(child, model_class):
                 raise TypeError(
                     f"cannot create {self.__class__.__name__} because value at index [{index}] is not a {model_class}: {child!r} {type(child)}"
                 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `uiclasses-2.4.0/uiclasses/errors.py` & `uiclasses-3.0.0/uiclasses/errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020 Gabriel Falcao
+# Copyright (c) 2020-2023 Gabriel Falcão Gonçalves de Moura
 
 # Permission is hereby granted, free of charge, to any person
 # obtaining a copy of this software and associated documentation files
 # (the "Software"), to deal in the Software without restriction,
 # including without limitation the rights to use, copy, modify, merge,
 # publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `uiclasses-2.4.0/uiclasses/fs.py` & `uiclasses-3.0.0/uiclasses/fs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020 Gabriel Falcao
+# Copyright (c) 2020-2023 Gabriel Falcão Gonçalves de Moura
 
 # Permission is hereby granted, free of charge, to any person
 # obtaining a copy of this software and associated documentation files
 # (the "Software"), to deal in the Software without restriction,
 # including without limitation the rights to use, copy, modify, merge,
 # publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `uiclasses-2.4.0/uiclasses/meta.py` & `uiclasses-3.0.0/uiclasses/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020 Gabriel Falcao
+# Copyright (c) 2020-2023 Gabriel Falcão Gonçalves de Moura
 
 # Permission is hereby granted, free of charge, to any person
 # obtaining a copy of this software and associated documentation files
 # (the "Software"), to deal in the Software without restriction,
 # including without limitation the rights to use, copy, modify, merge,
 # publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so,
@@ -16,18 +16,8 @@
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
 # BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
 # ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-
-from typing import List
-
-
-def is_builtin_class_except(target: type, except_names: List[str]) -> bool:
-    """returns ``True`` if the given class children of one of metaclasses built in :py:mod:`uiclasses.base`'."""
-
-    return (
-        target.__module__.startswith("uiclasses.")
-        and target.__name__ in except_names
-    )
+version = "3.0.0"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `uiclasses-2.4.0/uiclasses/typing.py` & `uiclasses-3.0.0/uiclasses/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020 Gabriel Falcao
+# Copyright (c) 2020-2023 Gabriel Falcão Gonçalves de Moura
 
 # Permission is hereby granted, free of charge, to any person
 # obtaining a copy of this software and associated documentation files
 # (the "Software"), to deal in the Software without restriction,
 # including without limitation the rights to use, copy, modify, merge,
 # publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `uiclasses-2.4.0/uiclasses/utils.py` & `uiclasses-3.0.0/uiclasses/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020 Gabriel Falcao
+# Copyright (c) 2020-2023 Gabriel Falcão Gonçalves de Moura
 
 # Permission is hereby granted, free of charge, to any person
 # obtaining a copy of this software and associated documentation files
 # (the "Software"), to deal in the Software without restriction,
 # including without limitation the rights to use, copy, modify, merge,
 # publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so,
@@ -86,15 +86,15 @@
     Does not emit logs.
     """
     if not isinstance(value, str):
         return value
     return try_convert(value, json.loads)
 
 
-def traverse_dict_children(data, *keys, fallback=None):
+def traverse_dict_descendants(data, *keys, fallback=None):
     """attempts to retrieve the config value under the given nested keys"""
     value = reduce(lambda d, l: d.get(l, None) or {}, keys, data)
     return value or fallback
 
 
 def repr_attributes(attributes: dict, separator: str = " "):
     """used for pretty-printing the attributes of a model
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `uiclasses-2.4.0/uiclasses/version.py` & `uiclasses-3.0.0/uiclasses/meta.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020 Gabriel Falcao
+# Copyright (c) 2020-2023 Gabriel Falcão Gonçalves de Moura
 
 # Permission is hereby granted, free of charge, to any person
 # obtaining a copy of this software and associated documentation files
 # (the "Software"), to deal in the Software without restriction,
 # including without limitation the rights to use, copy, modify, merge,
 # publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so,
@@ -16,8 +16,18 @@
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
 # BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
 # ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-version = "2.4.0"
+
+from typing import List
+
+
+def is_builtin_class_except(target: type, except_names: List[str]) -> bool:
+    """returns ``True`` if the given class descendants of one of metaclasses built in :py:mod:`uiclasses.base`'."""
+
+    return (
+        target.__module__.startswith("uiclasses.")
+        and target.__name__ in except_names
+    )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `uiclasses-2.4.0/uiclasses.egg-info/PKG-INFO` & `uiclasses-3.0.0/uiclasses.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,50 @@
 Metadata-Version: 2.1
 Name: uiclasses
-Version: 2.4.0
+Version: 3.0.0
 Summary: Data-Modeling for User Interfaces
 Home-page: https://github.com/gabrielfalcao/uiclasses
 Author: Gabriel Falcao
 Author-email: gabriel@nacaolivre.org
 Maintainer: Gabriel Falcão
 Maintainer-email: gabriel@nacaolivre.org
-License: UNKNOWN
 Project-URL: Documentation, https://uiclasses.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/gabrielfalcao/uiclasses
 Project-URL: Issue Tracker, https://github.com/gabrielfalcao/uiclasses/issues
 Project-URL: Test Coverage, https://codecov.io/gh/gabrielfalcao/uiclasses
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Handhelds/PDA's
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
 License-File: LICENSE
 
 UIClasses - Data-Modeling for User Interfaces
 ##############################################
 
 
 .. image:: https://img.shields.io/pypi/dm/uiclasses
    :target: https://pypi.org/project/uiclasses
 
 .. image:: https://img.shields.io/codecov/c/github/gabrielfalcao/uiclasses
    :target: https://codecov.io/gh/gabrielfalcao/uiclasses
 
-.. image:: https://img.shields.io/github/workflow/status/gabrielfalcao/uiclasses/python-3.6?label=python%203.6
-   :target: https://github.com/gabrielfalcao/uiclasses/actions
-
-.. image:: https://img.shields.io/github/workflow/status/gabrielfalcao/uiclasses/python-3.7?label=python%203.7
-   :target: https://github.com/gabrielfalcao/uiclasses/actions
+.. image:: https://github.com/gabrielfalcao/uiclasses/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/gabrielfalcao/uiclasses/actions/workflows/main.yml
 
 .. image:: https://img.shields.io/readthedocs/uiclasses
    :target: https://uiclasses.readthedocs.io/
 
 .. image:: https://img.shields.io/github/license/gabrielfalcao/uiclasses?label=Github%20License
    :target: https://github.com/gabrielfalcao/uiclasses/blob/master/LICENSE
 
@@ -129,9 +126,7 @@
 Notes:
 ======
 
 
 - This is not designed to be fast, when adding data to models their
   types might cast and validated, which is costly.
   - filtering collections by string values cause glob match
-
-
```

### Comparing `uiclasses-2.4.0/uiclasses.egg-info/SOURCES.txt` & `uiclasses-3.0.0/uiclasses.egg-info/SOURCES.txt`

 * *Files identical despite different names*

