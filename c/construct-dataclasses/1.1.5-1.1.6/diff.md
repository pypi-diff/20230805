# Comparing `tmp/construct-dataclasses-1.1.5.tar.gz` & `tmp/construct-dataclasses-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "construct-dataclasses-1.1.5.tar", last modified: Fri Aug  4 17:58:10 2023, max compression
+gzip compressed data, was "construct-dataclasses-1.1.6.tar", last modified: Sat Aug  5 08:23:23 2023, max compression
```

## Comparing `construct-dataclasses-1.1.5.tar` & `construct-dataclasses-1.1.6.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:58:10.293928 construct-dataclasses-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-08-04 17:57:59.000000 construct-dataclasses-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-08-04 17:58:10.293928 construct-dataclasses-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-08-04 17:57:59.000000 construct-dataclasses-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:58:10.293928 construct-dataclasses-1.1.5/construct_dataclasses.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-08-04 17:58:10.000000 construct-dataclasses-1.1.5/construct_dataclasses.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-04 17:58:10.000000 construct-dataclasses-1.1.5/construct_dataclasses.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 17:58:10.000000 construct-dataclasses-1.1.5/construct_dataclasses.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-04 17:58:10.000000 construct-dataclasses-1.1.5/construct_dataclasses.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 17:58:10.000000 construct-dataclasses-1.1.5/construct_dataclasses.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-08-04 17:57:59.000000 construct-dataclasses-1.1.5/construct_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 17:58:10.293928 construct-dataclasses-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-08-04 17:57:59.000000 construct-dataclasses-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 08:23:23.848055 construct-dataclasses-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-08-05 08:23:05.000000 construct-dataclasses-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-08-05 08:23:23.844055 construct-dataclasses-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-08-05 08:23:05.000000 construct-dataclasses-1.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 08:23:23.844055 construct-dataclasses-1.1.6/construct_dataclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)    14753 2023-08-05 08:23:05.000000 construct-dataclasses-1.1.6/construct_dataclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-08-05 08:23:05.000000 construct-dataclasses-1.1.6/construct_dataclasses/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 08:23:05.000000 construct-dataclasses-1.1.6/construct_dataclasses/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 08:23:23.844055 construct-dataclasses-1.1.6/construct_dataclasses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-08-05 08:23:23.000000 construct-dataclasses-1.1.6/construct_dataclasses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-05 08:23:23.000000 construct-dataclasses-1.1.6/construct_dataclasses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 08:23:23.000000 construct-dataclasses-1.1.6/construct_dataclasses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-05 08:23:23.000000 construct-dataclasses-1.1.6/construct_dataclasses.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-05 08:23:23.000000 construct-dataclasses-1.1.6/construct_dataclasses.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 08:23:23.848055 construct-dataclasses-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-08-05 08:23:05.000000 construct-dataclasses-1.1.6/setup.py
```

### Comparing `construct-dataclasses-1.1.5/LICENSE` & `construct-dataclasses-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `construct-dataclasses-1.1.5/PKG-INFO` & `construct-dataclasses-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: construct-dataclasses
-Version: 1.1.5
+Version: 1.1.6
 Summary: enhancement for the python package 'construct' that adds support for dataclasses.
 Home-page: https://github.com/MatrixEditor/construct-dataclasses
 Author: MatrixEditor
 License: GNU GPLv3
 Keywords: construct,kaitai,declarative,data structure,struct,binary,symmetric,parser,builder,parsing,building,pack,unpack,packer,unpacker,bitstring,bytestring,dataclasses
 Platform: POSIX
 Platform: Windows
@@ -29,15 +29,15 @@
 ![License](https://img.shields.io:/static/v1?label=License&message=GNU+GPLv3&color=blue)
 [![PyPI](https://img.shields.io/pypi/v/construct-dataclasses)](https://pypi.org/project/construct-dataclasses/)
 
 This small repository is an enhancement of the python package [*construct*](https://pypi.org/project/construct/), which is a powerful tool to declare symmetrical parsers and builders for binary data. This project combines construct with python's dataclasses with support for nested structs.
 
 ## Installation
 
-You can install the package via pip or just copy the python file as it is only one.
+You can install the package via pip or just copy the python file (*\_\_init\_\_.py*) as it is only one.
 
 ```bash
 pip install construct-dataclasses
 ```
 
 ## Usage
```

### Comparing `construct-dataclasses-1.1.5/README.md` & `construct-dataclasses-1.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ![License](https://img.shields.io:/static/v1?label=License&message=GNU+GPLv3&color=blue)
 [![PyPI](https://img.shields.io/pypi/v/construct-dataclasses)](https://pypi.org/project/construct-dataclasses/)
 
 This small repository is an enhancement of the python package [*construct*](https://pypi.org/project/construct/), which is a powerful tool to declare symmetrical parsers and builders for binary data. This project combines construct with python's dataclasses with support for nested structs.
 
 ## Installation
 
-You can install the package via pip or just copy the python file as it is only one.
+You can install the package via pip or just copy the python file (*\_\_init\_\_.py*) as it is only one.
 
 ```bash
 pip install construct-dataclasses
 ```
 
 ## Usage
```

### Comparing `construct-dataclasses-1.1.5/construct_dataclasses.egg-info/PKG-INFO` & `construct-dataclasses-1.1.6/construct_dataclasses.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: construct-dataclasses
-Version: 1.1.5
+Version: 1.1.6
 Summary: enhancement for the python package 'construct' that adds support for dataclasses.
 Home-page: https://github.com/MatrixEditor/construct-dataclasses
 Author: MatrixEditor
 License: GNU GPLv3
 Keywords: construct,kaitai,declarative,data structure,struct,binary,symmetric,parser,builder,parsing,building,pack,unpack,packer,unpacker,bitstring,bytestring,dataclasses
 Platform: POSIX
 Platform: Windows
@@ -29,15 +29,15 @@
 ![License](https://img.shields.io:/static/v1?label=License&message=GNU+GPLv3&color=blue)
 [![PyPI](https://img.shields.io/pypi/v/construct-dataclasses)](https://pypi.org/project/construct-dataclasses/)
 
 This small repository is an enhancement of the python package [*construct*](https://pypi.org/project/construct/), which is a powerful tool to declare symmetrical parsers and builders for binary data. This project combines construct with python's dataclasses with support for nested structs.
 
 ## Installation
 
-You can install the package via pip or just copy the python file as it is only one.
+You can install the package via pip or just copy the python file (*\_\_init\_\_.py*) as it is only one.
 
 ```bash
 pip install construct-dataclasses
 ```
 
 ## Usage
```

### Comparing `construct-dataclasses-1.1.5/construct_dataclasses.py` & `construct-dataclasses-1.1.6/construct_dataclasses/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,16 +347,17 @@
     else:
         ds_struct = DataclassStruct(cls, depth, reverse, union=union)
 
     setattr(new_cls, "parser", ds_struct)
     setattr(new_cls, "struct", ds_struct.subcon)
     return new_cls
 
+
 def dataclass_struct(
-    cls = None, /, *, bitwise=False, depth=None, reverse=False, union=False
+    cls=None, /, *, bitwise=False, depth=None, reverse=False, union=False
 ):
     """Creates a dataclass that stores a class-parser instance.
 
     Example::
 
         >>> @dataclass_struct
         ... class Blob:
```

### Comparing `construct-dataclasses-1.1.5/setup.py` & `construct-dataclasses-1.1.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 from setuptools import setup
 
-version_string = "1.1.5"
+version_string = "1.1.6"
 
 setup(
     name="construct-dataclasses",
     version=version_string,
-    package_data={"construct_dataclasses": ["construct_dataclasses.pyi"]},
-    py_modules=["construct_dataclasses"],
+    package_data={"construct_dataclasses": ["*.pyi", "py.typed"]},
+    packages=["construct_dataclasses"],
     license="GNU GPLv3",
     license_files=("LICENSE",),
     description="enhancement for the python package 'construct' that adds support for dataclasses.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     platforms=["POSIX", "Windows"],
     url="https://github.com/MatrixEditor/construct-dataclasses",
```

