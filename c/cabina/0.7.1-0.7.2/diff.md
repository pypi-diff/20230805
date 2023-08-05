# Comparing `tmp/cabina-0.7.1.tar.gz` & `tmp/cabina-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cabina-0.7.1.tar", last modified: Sun Nov  6 18:14:51 2022, max compression
+gzip compressed data, was "cabina-0.7.2.tar", last modified: Sun Jun 11 07:47:18 2023, max compression
```

## Comparing `cabina-0.7.1.tar` & `cabina-0.7.2.tar`

### file list

```diff
@@ -1,24 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 18:14:51.226853 cabina-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-06 18:14:41.000000 cabina-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5626 2022-11-06 18:14:51.226853 cabina-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5013 2022-11-06 18:14:41.000000 cabina-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 18:14:51.222854 cabina-0.7.1/cabina/
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-11-06 18:14:41.000000 cabina-0.7.1/cabina/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-11-06 18:14:41.000000 cabina-0.7.1/cabina/_computed.py
--rw-r--r--   0 runner    (1001) docker     (121)     7956 2022-11-06 18:14:41.000000 cabina-0.7.1/cabina/_core.py
--rw-r--r--   0 runner    (1001) docker     (121)     3032 2022-11-06 18:14:41.000000 cabina-0.7.1/cabina/_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-11-06 18:14:41.000000 cabina-0.7.1/cabina/_future_value.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-06 18:14:41.000000 cabina-0.7.1/cabina/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 18:14:51.222854 cabina-0.7.1/cabina/errors/
--rw-r--r--   0 runner    (1001) docker     (121)      685 2022-11-06 18:14:41.000000 cabina-0.7.1/cabina/errors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 18:14:51.226853 cabina-0.7.1/cabina/parsers/
--rw-r--r--   0 runner    (1001) docker     (121)     1981 2022-11-06 18:14:41.000000 cabina-0.7.1/cabina/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-06 18:14:41.000000 cabina-0.7.1/cabina/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 18:14:51.222854 cabina-0.7.1/cabina.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5626 2022-11-06 18:14:51.000000 cabina-0.7.1/cabina.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-11-06 18:14:51.000000 cabina-0.7.1/cabina.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-06 18:14:51.000000 cabina-0.7.1/cabina.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-06 18:14:51.000000 cabina-0.7.1/cabina.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-06 18:14:51.000000 cabina-0.7.1/cabina.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-11-06 18:14:51.226853 cabina-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-11-06 18:14:41.000000 cabina-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 07:47:18.327519 cabina-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 07:47:07.000000 cabina-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-06-11 07:47:18.327519 cabina-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-06-11 07:47:07.000000 cabina-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 07:47:18.327519 cabina-0.7.2/cabina/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-11 07:47:07.000000 cabina-0.7.2/cabina/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-11 07:47:07.000000 cabina-0.7.2/cabina/_computed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-06-11 07:47:07.000000 cabina-0.7.2/cabina/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-11 07:47:07.000000 cabina-0.7.2/cabina/_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-11 07:47:07.000000 cabina-0.7.2/cabina/_future_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-11 07:47:07.000000 cabina-0.7.2/cabina/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 07:47:18.327519 cabina-0.7.2/cabina/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-11 07:47:07.000000 cabina-0.7.2/cabina/errors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 07:47:18.327519 cabina-0.7.2/cabina/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-11 07:47:07.000000 cabina-0.7.2/cabina/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 07:47:07.000000 cabina-0.7.2/cabina/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 07:47:18.327519 cabina-0.7.2/cabina.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-06-11 07:47:18.000000 cabina-0.7.2/cabina.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-11 07:47:18.000000 cabina-0.7.2/cabina.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 07:47:18.000000 cabina-0.7.2/cabina.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-11 07:47:18.000000 cabina-0.7.2/cabina.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 07:47:18.000000 cabina-0.7.2/cabina.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-11 07:47:18.331519 cabina-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-11 07:47:07.000000 cabina-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 07:47:18.327519 cabina-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-11 07:47:07.000000 cabina-0.7.2/tests/test_computed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-06-11 07:47:07.000000 cabina-0.7.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-11 07:47:07.000000 cabina-0.7.2/tests/test_config_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-11 07:47:07.000000 cabina-0.7.2/tests/test_env_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-11 07:47:07.000000 cabina-0.7.2/tests/test_env_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-11 07:47:07.000000 cabina-0.7.2/tests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-11 07:47:07.000000 cabina-0.7.2/tests/test_future_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-11 07:47:07.000000 cabina-0.7.2/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-06-11 07:47:07.000000 cabina-0.7.2/tests/test_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-06-11 07:47:07.000000 cabina-0.7.2/tests/test_section_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-11 07:47:07.000000 cabina-0.7.2/tests/test_section_inheritance.py
```

### Comparing `cabina-0.7.1/LICENSE` & `cabina-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cabina-0.7.1/PKG-INFO` & `cabina-0.7.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: cabina
-Version: 0.7.1
+Version: 0.7.2
 Summary: Configuration with typed env vars
-Home-page: https://github.com/nikitanovosibirsk/cabina
+Home-page: https://github.com/tsv1/cabina
 Author: Nikita Tsvetkov
-Author-email: nikitanovosibirsk@yandex.com
+Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cabina
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/cabina/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/cabina)
+[![Codecov](https://img.shields.io/codecov/c/github/tsv1/cabina/master.svg?style=flat-square)](https://codecov.io/gh/tsv1/cabina)
 [![PyPI](https://img.shields.io/pypi/v/cabina.svg?style=flat-square)](https://pypi.python.org/pypi/cabina/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/cabina?style=flat-square)](https://pypi.python.org/pypi/cabina/)
 [![Python Version](https://img.shields.io/pypi/pyversions/cabina.svg?style=flat-square)](https://pypi.python.org/pypi/cabina/)
 
 
 ## Installation
```

### Comparing `cabina-0.7.1/README.md` & `cabina-0.7.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # cabina
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/cabina/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/cabina)
+[![Codecov](https://img.shields.io/codecov/c/github/tsv1/cabina/master.svg?style=flat-square)](https://codecov.io/gh/tsv1/cabina)
 [![PyPI](https://img.shields.io/pypi/v/cabina.svg?style=flat-square)](https://pypi.python.org/pypi/cabina/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/cabina?style=flat-square)](https://pypi.python.org/pypi/cabina/)
 [![Python Version](https://img.shields.io/pypi/pyversions/cabina.svg?style=flat-square)](https://pypi.python.org/pypi/cabina/)
 
 
 ## Installation
```

### Comparing `cabina-0.7.1/cabina/_core.py` & `cabina-0.7.2/cabina/_core.py`

 * *Files identical despite different names*

### Comparing `cabina-0.7.1/cabina/_environment.py` & `cabina-0.7.2/cabina/_environment.py`

 * *Files identical despite different names*

### Comparing `cabina-0.7.1/cabina/_future_value.py` & `cabina-0.7.2/cabina/_future_value.py`

 * *Files identical despite different names*

### Comparing `cabina-0.7.1/cabina/errors/__init__.py` & `cabina-0.7.2/cabina/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `cabina-0.7.1/cabina/parsers/__init__.py` & `cabina-0.7.2/cabina/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `cabina-0.7.1/cabina.egg-info/PKG-INFO` & `cabina-0.7.2/cabina.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: cabina
-Version: 0.7.1
+Version: 0.7.2
 Summary: Configuration with typed env vars
-Home-page: https://github.com/nikitanovosibirsk/cabina
+Home-page: https://github.com/tsv1/cabina
 Author: Nikita Tsvetkov
-Author-email: nikitanovosibirsk@yandex.com
+Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cabina
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/cabina/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/cabina)
+[![Codecov](https://img.shields.io/codecov/c/github/tsv1/cabina/master.svg?style=flat-square)](https://codecov.io/gh/tsv1/cabina)
 [![PyPI](https://img.shields.io/pypi/v/cabina.svg?style=flat-square)](https://pypi.python.org/pypi/cabina/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/cabina?style=flat-square)](https://pypi.python.org/pypi/cabina/)
 [![Python Version](https://img.shields.io/pypi/pyversions/cabina.svg?style=flat-square)](https://pypi.python.org/pypi/cabina/)
 
 
 ## Installation
```

### Comparing `cabina-0.7.1/setup.cfg` & `cabina-0.7.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.7.1
+current_version = 0.7.2
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `cabina-0.7.1/setup.py` & `cabina-0.7.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,29 +9,30 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="cabina",
-    version="0.7.1",
+    version="0.7.2",
     description="Configuration with typed env vars",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
-    author_email="nikitanovosibirsk@yandex.com",
+    author_email="tsv1@fastmail.com",
     python_requires=">=3.7",
-    url="https://github.com/nikitanovosibirsk/cabina",
+    url="https://github.com/tsv1/cabina",
     license="Apache-2.0",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"cabina": ["py.typed"]},
     install_requires=find_required(),
     tests_require=find_dev_required(),
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
     ],
 )
```

