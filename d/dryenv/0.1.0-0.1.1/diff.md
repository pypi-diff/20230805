# Comparing `tmp/dryenv-0.1.0.tar.gz` & `tmp/dryenv-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dryenv-0.1.0.tar", last modified: Fri May  1 08:45:40 2020, max compression
+gzip compressed data, was "dist/dryenv-0.1.1.tar", last modified: Sat Aug  5 12:13:50 2023, max compression
```

## Comparing `dryenv-0.1.0.tar` & `dryenv-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 me         (502) staff       (20)        0 2020-05-01 08:45:40.868721 dryenv-0.1.0/
--rw-r--r--   0 me         (502) staff       (20)     1066 2020-04-01 19:10:35.000000 dryenv-0.1.0/LICENSE.txt
--rw-r--r--   0 me         (502) staff       (20)       20 2019-12-25 16:35:55.000000 dryenv-0.1.0/MANIFEST.in
--rw-r--r--   0 me         (502) staff       (20)     8871 2020-05-01 08:45:40.868224 dryenv-0.1.0/PKG-INFO
--rw-r--r--   0 me         (502) staff       (20)     6838 2020-04-30 21:01:20.000000 dryenv-0.1.0/README.md
-drwxr-xr-x   0 me         (502) staff       (20)        0 2020-05-01 08:45:40.867455 dryenv-0.1.0/dryenv.egg-info/
--rw-r--r--   0 me         (502) staff       (20)     8871 2020-05-01 08:45:40.000000 dryenv-0.1.0/dryenv.egg-info/PKG-INFO
--rw-r--r--   0 me         (502) staff       (20)      201 2020-05-01 08:45:40.000000 dryenv-0.1.0/dryenv.egg-info/SOURCES.txt
--rw-r--r--   0 me         (502) staff       (20)        1 2020-05-01 08:45:40.000000 dryenv-0.1.0/dryenv.egg-info/dependency_links.txt
--rw-r--r--   0 me         (502) staff       (20)       25 2020-05-01 08:45:40.000000 dryenv-0.1.0/dryenv.egg-info/requires.txt
--rw-r--r--   0 me         (502) staff       (20)        7 2020-05-01 08:45:40.000000 dryenv-0.1.0/dryenv.egg-info/top_level.txt
--rw-r--r--   0 me         (502) staff       (20)     4438 2020-05-01 08:45:14.000000 dryenv-0.1.0/dryenv.py
--rw-r--r--   0 me         (502) staff       (20)       38 2020-05-01 08:45:40.868909 dryenv-0.1.0/setup.cfg
--rw-r--r--   0 me         (502) staff       (20)     1475 2020-05-01 08:30:11.000000 dryenv-0.1.0/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-08-05 12:13:50.016312 dryenv-0.1.1/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1066 2023-08-05 12:11:03.000000 dryenv-0.1.1/LICENSE.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       20 2023-08-05 12:11:03.000000 dryenv-0.1.1/MANIFEST.in
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9012 2023-08-05 12:13:50.016312 dryenv-0.1.1/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6827 2023-08-05 12:11:03.000000 dryenv-0.1.1/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-08-05 12:13:50.016312 dryenv-0.1.1/dryenv.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9012 2023-08-05 12:13:49.000000 dryenv-0.1.1/dryenv.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      201 2023-08-05 12:13:49.000000 dryenv-0.1.1/dryenv.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-08-05 12:13:49.000000 dryenv-0.1.1/dryenv.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       29 2023-08-05 12:13:49.000000 dryenv-0.1.1/dryenv.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-08-05 12:13:49.000000 dryenv-0.1.1/dryenv.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4426 2023-08-05 12:13:44.000000 dryenv-0.1.1/dryenv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-08-05 12:13:50.016312 dryenv-0.1.1/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1628 2023-08-05 12:13:34.000000 dryenv-0.1.1/setup.py
```

### Comparing `dryenv-0.1.0/LICENSE.txt` & `dryenv-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dryenv-0.1.0/PKG-INFO` & `dryenv-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: dryenv
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple DRY configuration with environment variables and pydantic.
 Home-page: http://github.com/alexmojaki/dryenv
 Author: Alex Hall
 Author-email: alex.mojaki@gmail.com
 License: MIT
 Description: # dryenv
         
         [![Build Status](https://travis-ci.org/alexmojaki/dryenv.svg?branch=master)](https://travis-ci.org/alexmojaki/dryenv) [![Coverage Status](https://coveralls.io/repos/github/alexmojaki/dryenv/badge.svg?branch=master)](https://coveralls.io/github/alexmojaki/dryenv?branch=master) [![Supports Python versions 3.6+](https://img.shields.io/pypi/pyversions/dryenv.svg)](https://pypi.python.org/pypi/dryenv)
         
         Simple configuration with environment variables and pydantic, without repeating yourself!
         
             pip install dryenv
         
-          * [Basic usage](#basic-usage)
-          * [Based on pydantic.](#based-on-pydantic)
-          * [Configuring DryEnv](#configuring-dryenv)
-          * [Additional features](#additional-features)
-          * [Usage with Django and PyCharm](#usage-with-django-and-pycharm)
+        - [Basic usage](#basic-usage)
+        - [Based on pydantic.](#based-on-pydantic)
+        - [Configuring DryEnv](#configuring-dryenv)
+        - [Additional features](#additional-features)
+        - [Usage with Django and PyCharm](#usage-with-django-and-pycharm)
         
         ## Basic usage
         
         For example, instead of writing:
         
         ```python
         # settings.py
@@ -99,15 +99,15 @@
         
         ## Based on pydantic.
         
         `DryEnv` is a thin wrapper around [`pydantic.BaseSettings`](https://pydantic-docs.helpmanual.io/usage/settings/), which does most of the heavy lifting. `DryEnv` makes things a little neater and more convenient by automatically:
         
         1. Setting `env_prefix` based on the class name, unless the class name is `Root` (case insensitive) in which case the prefix is empty.
         2. Instantiating the class to trigger the environment lookups.
-         
+        
         For example, this:
         
         ```python
         from dryenv import DryEnv
         
         class DATABASE(DryEnv):
             HOST = "localhost"
@@ -184,11 +184,14 @@
         Alternatively, you can add the line `DATABASE = DATABASE` or `DATABASE = DATABASE()` and then PyCharm will recognise this as a normal variable instead of a class.
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: tests
```

### Comparing `dryenv-0.1.0/README.md` & `dryenv-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 [![Build Status](https://travis-ci.org/alexmojaki/dryenv.svg?branch=master)](https://travis-ci.org/alexmojaki/dryenv) [![Coverage Status](https://coveralls.io/repos/github/alexmojaki/dryenv/badge.svg?branch=master)](https://coveralls.io/github/alexmojaki/dryenv?branch=master) [![Supports Python versions 3.6+](https://img.shields.io/pypi/pyversions/dryenv.svg)](https://pypi.python.org/pypi/dryenv)
 
 Simple configuration with environment variables and pydantic, without repeating yourself!
 
     pip install dryenv
 
-  * [Basic usage](#basic-usage)
-  * [Based on pydantic.](#based-on-pydantic)
-  * [Configuring DryEnv](#configuring-dryenv)
-  * [Additional features](#additional-features)
-  * [Usage with Django and PyCharm](#usage-with-django-and-pycharm)
+- [Basic usage](#basic-usage)
+- [Based on pydantic.](#based-on-pydantic)
+- [Configuring DryEnv](#configuring-dryenv)
+- [Additional features](#additional-features)
+- [Usage with Django and PyCharm](#usage-with-django-and-pycharm)
 
 ## Basic usage
 
 For example, instead of writing:
 
 ```python
 # settings.py
@@ -91,15 +91,15 @@
 
 ## Based on pydantic.
 
 `DryEnv` is a thin wrapper around [`pydantic.BaseSettings`](https://pydantic-docs.helpmanual.io/usage/settings/), which does most of the heavy lifting. `DryEnv` makes things a little neater and more convenient by automatically:
 
 1. Setting `env_prefix` based on the class name, unless the class name is `Root` (case insensitive) in which case the prefix is empty.
 2. Instantiating the class to trigger the environment lookups.
- 
+
 For example, this:
 
 ```python
 from dryenv import DryEnv
 
 class DATABASE(DryEnv):
     HOST = "localhost"
```

### Comparing `dryenv-0.1.0/dryenv.egg-info/PKG-INFO` & `dryenv-0.1.1/dryenv.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: dryenv
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple DRY configuration with environment variables and pydantic.
 Home-page: http://github.com/alexmojaki/dryenv
 Author: Alex Hall
 Author-email: alex.mojaki@gmail.com
 License: MIT
 Description: # dryenv
         
         [![Build Status](https://travis-ci.org/alexmojaki/dryenv.svg?branch=master)](https://travis-ci.org/alexmojaki/dryenv) [![Coverage Status](https://coveralls.io/repos/github/alexmojaki/dryenv/badge.svg?branch=master)](https://coveralls.io/github/alexmojaki/dryenv?branch=master) [![Supports Python versions 3.6+](https://img.shields.io/pypi/pyversions/dryenv.svg)](https://pypi.python.org/pypi/dryenv)
         
         Simple configuration with environment variables and pydantic, without repeating yourself!
         
             pip install dryenv
         
-          * [Basic usage](#basic-usage)
-          * [Based on pydantic.](#based-on-pydantic)
-          * [Configuring DryEnv](#configuring-dryenv)
-          * [Additional features](#additional-features)
-          * [Usage with Django and PyCharm](#usage-with-django-and-pycharm)
+        - [Basic usage](#basic-usage)
+        - [Based on pydantic.](#based-on-pydantic)
+        - [Configuring DryEnv](#configuring-dryenv)
+        - [Additional features](#additional-features)
+        - [Usage with Django and PyCharm](#usage-with-django-and-pycharm)
         
         ## Basic usage
         
         For example, instead of writing:
         
         ```python
         # settings.py
@@ -99,15 +99,15 @@
         
         ## Based on pydantic.
         
         `DryEnv` is a thin wrapper around [`pydantic.BaseSettings`](https://pydantic-docs.helpmanual.io/usage/settings/), which does most of the heavy lifting. `DryEnv` makes things a little neater and more convenient by automatically:
         
         1. Setting `env_prefix` based on the class name, unless the class name is `Root` (case insensitive) in which case the prefix is empty.
         2. Instantiating the class to trigger the environment lookups.
-         
+        
         For example, this:
         
         ```python
         from dryenv import DryEnv
         
         class DATABASE(DryEnv):
             HOST = "localhost"
@@ -184,11 +184,14 @@
         Alternatively, you can add the line `DATABASE = DATABASE` or `DATABASE = DATABASE()` and then PyCharm will recognise this as a normal variable instead of a class.
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: tests
```

### Comparing `dryenv-0.1.0/dryenv.py` & `dryenv-0.1.1/dryenv.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from collections import namedtuple
 from inspect import currentframe
-from typing import Dict, Any
+from typing import Any, Dict
 
 from pydantic import BaseSettings
 
 try:
     from pydantic.main import ModelMetaclass
 except ImportError:  # pragma: no cover
     ModelMetaclass = type(BaseSettings)
 
-__version__ = '0.1.0'
-__version_info__ = namedtuple(
-    'VersionInfo', ('major', 'minor', 'micro')
-)(*map(int, __version__.split('.')))
+__version__ = "0.1.1"
+__version_info__ = namedtuple("VersionInfo", ("major", "minor", "micro"))(
+    *map(int, __version__.split("."))
+)
 
 __all__ = ["DryEnvMeta", "populate_globals"]
 
 
 class DryEnvMeta(ModelMetaclass):
     def __new__(mcs, name, bases, namespace):
         Config = namespace.setdefault("Config", type("Config", (), {}))
@@ -104,16 +104,15 @@
                 HOST = "localhost"
                 USERNAME = "admin"
 
             assert DATABASE.dict() == {"HOST": "localhost", "USERNAME": "admin"}
             assert DATABASE.prefixed_dict() == {"DATABASE_HOST": "localhost", "DATABASE_USERNAME": "admin"}
         """
         return {
-            self.Config.env_prefix + k: v
-            for k, v in self.dict(*args, **kwargs).items()
+            self.Config.env_prefix + k: v for k, v in self.dict(*args, **kwargs).items()
         }
 
     def __call__(self, *args, **kwargs) -> "DryEnv":
         """
         Instantiate this class as if you were calling the class itself.
         """
         return type(self)(*args, **kwargs)
```

### Comparing `dryenv-0.1.0/setup.py` & `dryenv-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 import os
 import re
 from io import open
 
 from setuptools import setup
 
-package = 'dryenv'
+package = "dryenv"
 dirname = os.path.dirname(__file__)
 
 
 def file_to_string(*path):
-    with open(os.path.join(dirname, *path), encoding='utf8') as f:
+    with open(os.path.join(dirname, *path), encoding="utf8") as f:
         return f.read()
 
 
 # __version__ is defined inside the package, but we can't import
 # it because it imports dependencies which may not be installed yet,
 # so we extract it manually
 contents = file_to_string(package + ".py")
-__version__ = re.search(r"__version__ = '([.\d]+)'", contents).group(1)
+__version__ = re.search(r'__version__ = "([.\d]+)"', contents).group(1)
 
 install_requires = [
-    'pydantic',
+    "pydantic<2.0",
 ]
 
 tests_require = [
-    'pytest',
+    "pytest",
 ]
 
 setup(
     name=package,
     version=__version__,
     description="Simple DRY configuration with environment variables and pydantic.",
-    long_description=file_to_string('README.md'),
-    long_description_content_type='text/markdown',
-    url='http://github.com/alexmojaki/' + package,
-    author='Alex Hall',
-    author_email='alex.mojaki@gmail.com',
-    license='MIT',
+    long_description=file_to_string("README.md"),
+    long_description_content_type="text/markdown",
+    url="http://github.com/alexmojaki/" + package,
+    author="Alex Hall",
+    author_email="alex.mojaki@gmail.com",
+    license="MIT",
     include_package_data=True,
     py_modules=[package],
     install_requires=install_requires,
     tests_require=tests_require,
     extras_require={
-        'tests': tests_require,
+        "tests": tests_require,
     },
     classifiers=[
-        'Intended Audience :: Developers',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
     ],
 )
```

