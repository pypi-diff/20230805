# Comparing `tmp/graphene-django-optimizer-0.9.0.tar.gz` & `tmp/graphene-django-optimizer-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene-django-optimizer-0.9.0.tar", last modified: Wed Aug 18 23:45:11 2021, max compression
+gzip compressed data, was "graphene-django-optimizer-0.9.1.tar", last modified: Fri Oct 15 00:50:30 2021, max compression
```

## Comparing `graphene-django-optimizer-0.9.0.tar` & `graphene-django-optimizer-0.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-08-18 23:45:11.331657 graphene-django-optimizer-0.9.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1077 2021-08-18 23:44:57.000000 graphene-django-optimizer-0.9.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     6912 2021-08-18 23:45:11.331657 graphene-django-optimizer-0.9.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     5909 2021-08-18 23:44:57.000000 graphene-django-optimizer-0.9.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-08-18 23:45:11.327655 graphene-django-optimizer-0.9.0/graphene_django_optimizer/
--rw-rw-r--   0 travis    (2000) travis    (2000)      188 2021-08-18 23:44:57.000000 graphene-django-optimizer-0.9.0/graphene_django_optimizer/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      676 2021-08-18 23:44:57.000000 graphene-django-optimizer-0.9.0/graphene_django_optimizer/field.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      858 2021-08-18 23:44:57.000000 graphene-django-optimizer-0.9.0/graphene_django_optimizer/hints.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16609 2021-08-18 23:44:57.000000 graphene-django-optimizer-0.9.0/graphene_django_optimizer/query.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      291 2021-08-18 23:44:57.000000 graphene-django-optimizer-0.9.0/graphene_django_optimizer/resolver.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      717 2021-08-18 23:44:57.000000 graphene-django-optimizer-0.9.0/graphene_django_optimizer/types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      125 2021-08-18 23:44:57.000000 graphene-django-optimizer-0.9.0/graphene_django_optimizer/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-08-18 23:45:11.331657 graphene-django-optimizer-0.9.0/graphene_django_optimizer.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6912 2021-08-18 23:45:11.000000 graphene-django-optimizer-0.9.0/graphene_django_optimizer.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      483 2021-08-18 23:45:11.000000 graphene-django-optimizer-0.9.0/graphene_django_optimizer.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-08-18 23:45:11.000000 graphene-django-optimizer-0.9.0/graphene_django_optimizer.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       26 2021-08-18 23:45:11.000000 graphene-django-optimizer-0.9.0/graphene_django_optimizer.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      321 2021-08-18 23:45:11.331657 graphene-django-optimizer-0.9.0/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1457 2021-08-18 23:44:57.000000 graphene-django-optimizer-0.9.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-10-15 00:50:30.512824 graphene-django-optimizer-0.9.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1077 2021-10-15 00:50:15.000000 graphene-django-optimizer-0.9.1/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7035 2021-10-15 00:50:30.512824 graphene-django-optimizer-0.9.1/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6032 2021-10-15 00:50:15.000000 graphene-django-optimizer-0.9.1/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-10-15 00:50:30.512824 graphene-django-optimizer-0.9.1/graphene_django_optimizer/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      188 2021-10-15 00:50:15.000000 graphene-django-optimizer-0.9.1/graphene_django_optimizer/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      676 2021-10-15 00:50:15.000000 graphene-django-optimizer-0.9.1/graphene_django_optimizer/field.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      858 2021-10-15 00:50:15.000000 graphene-django-optimizer-0.9.1/graphene_django_optimizer/hints.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16701 2021-10-15 00:50:15.000000 graphene-django-optimizer-0.9.1/graphene_django_optimizer/query.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      291 2021-10-15 00:50:15.000000 graphene-django-optimizer-0.9.1/graphene_django_optimizer/resolver.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      717 2021-10-15 00:50:15.000000 graphene-django-optimizer-0.9.1/graphene_django_optimizer/types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      125 2021-10-15 00:50:15.000000 graphene-django-optimizer-0.9.1/graphene_django_optimizer/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-10-15 00:50:30.512824 graphene-django-optimizer-0.9.1/graphene_django_optimizer.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7035 2021-10-15 00:50:30.000000 graphene-django-optimizer-0.9.1/graphene_django_optimizer.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      483 2021-10-15 00:50:30.000000 graphene-django-optimizer-0.9.1/graphene_django_optimizer.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-10-15 00:50:30.000000 graphene-django-optimizer-0.9.1/graphene_django_optimizer.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       26 2021-10-15 00:50:30.000000 graphene-django-optimizer-0.9.1/graphene_django_optimizer.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      321 2021-10-15 00:50:30.516824 graphene-django-optimizer-0.9.1/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1457 2021-10-15 00:50:15.000000 graphene-django-optimizer-0.9.1/setup.py
```

### Comparing `graphene-django-optimizer-0.9.0/LICENSE` & `graphene-django-optimizer-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene-django-optimizer-0.9.0/PKG-INFO` & `graphene-django-optimizer-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django-optimizer
-Version: 0.9.0
+Version: 0.9.1
 Summary: Optimize database access inside graphene queries.
 Home-page: https://github.com/tfoxy/graphene-django-optimizer
 Author: Tomás Fox
 Author-email: tomas.c.fox@gmail.com
 License: MIT
 Keywords: graphene django optimizer optimize graphql query prefetch select related
 Platform: UNKNOWN
@@ -22,29 +22,31 @@
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # graphene-django-optimizer
 
-[![build status](https://img.shields.io/travis/tfoxy/graphene-django-optimizer.svg)](https://travis-ci.org/tfoxy/graphene-django-optimizer)
+[![build status](https://img.shields.io/travis/tfoxy/graphene-django-optimizer.svg)](https://travis-ci.com/github/tfoxy/graphene-django-optimizer)
 [![coverage](https://img.shields.io/codecov/c/github/tfoxy/graphene-django-optimizer.svg)](https://codecov.io/gh/tfoxy/graphene-django-optimizer)
 [![PyPI version](https://img.shields.io/pypi/v/graphene-django-optimizer.svg)](https://pypi.org/project/graphene-django-optimizer/)
 ![python version](https://img.shields.io/pypi/pyversions/graphene-django-optimizer.svg)
 ![django version](https://img.shields.io/pypi/djversions/graphene-django-optimizer.svg)
 
 Optimize queries executed by [graphene-django](https://github.com/graphql-python/graphene-django) automatically, using [`select_related`](https://docs.djangoproject.com/en/2.0/ref/models/querysets/#select-related), [`prefetch_related`](https://docs.djangoproject.com/en/2.0/ref/models/querysets/#prefetch-related) and [`only`](https://docs.djangoproject.com/en/2.0/ref/models/querysets/#only) methods of Django QuerySet.
 
 
+
 ## Install
 
 ```bash
 pip install graphene-django-optimizer
 ```
 
+*Note: If you are using Graphene V2, please install version `0.8`. v0.9 and forward will support only Graphene V3*
 
 ## Usage
 
 Having the following schema based on [the tutorial of graphene-django](http://docs.graphene-python.org/projects/django/en/latest/tutorial-plain/#hello-graphql-schema-and-object-types) (notice the use of `gql_optimizer`)
 
 ```py
 # cookbook/ingredients/schema.py
```

### Comparing `graphene-django-optimizer-0.9.0/README.md` & `graphene-django-optimizer-0.9.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # graphene-django-optimizer
 
-[![build status](https://img.shields.io/travis/tfoxy/graphene-django-optimizer.svg)](https://travis-ci.org/tfoxy/graphene-django-optimizer)
+[![build status](https://img.shields.io/travis/tfoxy/graphene-django-optimizer.svg)](https://travis-ci.com/github/tfoxy/graphene-django-optimizer)
 [![coverage](https://img.shields.io/codecov/c/github/tfoxy/graphene-django-optimizer.svg)](https://codecov.io/gh/tfoxy/graphene-django-optimizer)
 [![PyPI version](https://img.shields.io/pypi/v/graphene-django-optimizer.svg)](https://pypi.org/project/graphene-django-optimizer/)
 ![python version](https://img.shields.io/pypi/pyversions/graphene-django-optimizer.svg)
 ![django version](https://img.shields.io/pypi/djversions/graphene-django-optimizer.svg)
 
 Optimize queries executed by [graphene-django](https://github.com/graphql-python/graphene-django) automatically, using [`select_related`](https://docs.djangoproject.com/en/2.0/ref/models/querysets/#select-related), [`prefetch_related`](https://docs.djangoproject.com/en/2.0/ref/models/querysets/#prefetch-related) and [`only`](https://docs.djangoproject.com/en/2.0/ref/models/querysets/#only) methods of Django QuerySet.
 
 
+
 ## Install
 
 ```bash
 pip install graphene-django-optimizer
 ```
 
+*Note: If you are using Graphene V2, please install version `0.8`. v0.9 and forward will support only Graphene V3*
 
 ## Usage
 
 Having the following schema based on [the tutorial of graphene-django](http://docs.graphene-python.org/projects/django/en/latest/tutorial-plain/#hello-graphql-schema-and-object-types) (notice the use of `gql_optimizer`)
 
 ```py
 # cookbook/ingredients/schema.py
```

### Comparing `graphene-django-optimizer-0.9.0/graphene_django_optimizer/field.py` & `graphene-django-optimizer-0.9.1/graphene_django_optimizer/field.py`

 * *Files identical despite different names*

### Comparing `graphene-django-optimizer-0.9.0/graphene_django_optimizer/hints.py` & `graphene-django-optimizer-0.9.1/graphene_django_optimizer/hints.py`

 * *Files identical despite different names*

### Comparing `graphene-django-optimizer-0.9.0/graphene_django_optimizer/query.py` & `graphene-django-optimizer-0.9.1/graphene_django_optimizer/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,15 +265,17 @@
             )
         return True
 
     def _add_optimization_hints(self, source, target):
         if source:
             if not is_iterable(source):
                 source = (source,)
-            target += source
+            target += [
+                source_item for source_item in source if source_item not in target
+            ]
 
     def _get_name_from_resolver(self, resolver):
         optimization_hints = self._get_optimization_hints(resolver)
         if optimization_hints:
             name_fn = optimization_hints.model_field
             if name_fn:
                 return name_fn()
```

### Comparing `graphene-django-optimizer-0.9.0/graphene_django_optimizer/types.py` & `graphene-django-optimizer-0.9.1/graphene_django_optimizer/types.py`

 * *Files identical despite different names*

### Comparing `graphene-django-optimizer-0.9.0/graphene_django_optimizer.egg-info/PKG-INFO` & `graphene-django-optimizer-0.9.1/graphene_django_optimizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django-optimizer
-Version: 0.9.0
+Version: 0.9.1
 Summary: Optimize database access inside graphene queries.
 Home-page: https://github.com/tfoxy/graphene-django-optimizer
 Author: Tomás Fox
 Author-email: tomas.c.fox@gmail.com
 License: MIT
 Keywords: graphene django optimizer optimize graphql query prefetch select related
 Platform: UNKNOWN
@@ -22,29 +22,31 @@
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # graphene-django-optimizer
 
-[![build status](https://img.shields.io/travis/tfoxy/graphene-django-optimizer.svg)](https://travis-ci.org/tfoxy/graphene-django-optimizer)
+[![build status](https://img.shields.io/travis/tfoxy/graphene-django-optimizer.svg)](https://travis-ci.com/github/tfoxy/graphene-django-optimizer)
 [![coverage](https://img.shields.io/codecov/c/github/tfoxy/graphene-django-optimizer.svg)](https://codecov.io/gh/tfoxy/graphene-django-optimizer)
 [![PyPI version](https://img.shields.io/pypi/v/graphene-django-optimizer.svg)](https://pypi.org/project/graphene-django-optimizer/)
 ![python version](https://img.shields.io/pypi/pyversions/graphene-django-optimizer.svg)
 ![django version](https://img.shields.io/pypi/djversions/graphene-django-optimizer.svg)
 
 Optimize queries executed by [graphene-django](https://github.com/graphql-python/graphene-django) automatically, using [`select_related`](https://docs.djangoproject.com/en/2.0/ref/models/querysets/#select-related), [`prefetch_related`](https://docs.djangoproject.com/en/2.0/ref/models/querysets/#prefetch-related) and [`only`](https://docs.djangoproject.com/en/2.0/ref/models/querysets/#only) methods of Django QuerySet.
 
 
+
 ## Install
 
 ```bash
 pip install graphene-django-optimizer
 ```
 
+*Note: If you are using Graphene V2, please install version `0.8`. v0.9 and forward will support only Graphene V3*
 
 ## Usage
 
 Having the following schema based on [the tutorial of graphene-django](http://docs.graphene-python.org/projects/django/en/latest/tutorial-plain/#hello-graphql-schema-and-object-types) (notice the use of `gql_optimizer`)
 
 ```py
 # cookbook/ingredients/schema.py
```

### Comparing `graphene-django-optimizer-0.9.0/setup.py` & `graphene-django-optimizer-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="graphene-django-optimizer",
-    version="0.9.0",
+    version="0.9.1",
     author="Tomás Fox",
     author_email="tomas.c.fox@gmail.com",
     description="Optimize database access inside graphene queries.",
     license="MIT",
     keywords="graphene django optimizer optimize graphql query prefetch select related",
     url="https://github.com/tfoxy/graphene-django-optimizer",
     packages=["graphene_django_optimizer"],
```

