# Comparing `tmp/curies-0.5.7.tar.gz` & `tmp/curies-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curies-0.5.7.tar", last modified: Sat Jul 22 23:20:19 2023, max compression
+gzip compressed data, was "curies-0.6.0.tar", last modified: Sat Aug  5 13:07:58 2023, max compression
```

## Comparing `curies-0.5.7.tar` & `curies-0.6.0.tar`

### file list

```diff
@@ -1,62 +1,69 @@
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-22 23:20:19.931929 curies-0.5.7/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2022-07-31 23:04:00.000000 curies-0.5.7/LICENSE
--rw-r--r--   0 cthoyt     (501) staff       (20)      394 2023-04-28 13:05:54.000000 curies-0.5.7/MANIFEST.in
--rw-r--r--   0 cthoyt     (501) staff       (20)    11777 2023-07-22 23:20:19.932093 curies-0.5.7/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)    10308 2023-05-05 11:46:12.000000 curies-0.5.7/README.md
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-22 23:20:19.903582 curies-0.5.7/docs/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-22 23:20:19.907299 curies-0.5.7/docs/source/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-22 23:20:19.919090 curies-0.5.7/docs/source/api/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1864 2023-04-13 07:20:08.000000 curies-0.5.7/docs/source/api/curies.Converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      101 2023-04-13 07:20:08.000000 curies-0.5.7/docs/source/api/curies.DuplicatePrefixes.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      110 2023-04-13 07:20:08.000000 curies-0.5.7/docs/source/api/curies.DuplicateURIPrefixes.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      107 2023-04-13 07:20:08.000000 curies-0.5.7/docs/source/api/curies.DuplicateValueError.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       86 2023-04-13 07:20:08.000000 curies-0.5.7/docs/source/api/curies.Record.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       64 2023-04-13 07:20:08.000000 curies-0.5.7/docs/source/api/curies.chain.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      124 2023-04-13 07:20:08.000000 curies-0.5.7/docs/source/api/curies.get_bioregistry_converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       94 2023-04-13 07:20:08.000000 curies-0.5.7/docs/source/api/curies.get_fastapi_app.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      103 2023-04-13 07:20:08.000000 curies-0.5.7/docs/source/api/curies.get_fastapi_router.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       88 2023-04-13 07:20:08.000000 curies-0.5.7/docs/source/api/curies.get_flask_app.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      106 2023-04-13 07:20:08.000000 curies-0.5.7/docs/source/api/curies.get_flask_blueprint.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       97 2023-04-13 07:20:08.000000 curies-0.5.7/docs/source/api/curies.get_go_converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      112 2023-04-13 07:20:08.000000 curies-0.5.7/docs/source/api/curies.get_monarch_converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      100 2023-04-13 07:20:08.000000 curies-0.5.7/docs/source/api/curies.get_obo_converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      130 2023-04-13 07:20:08.000000 curies-0.5.7/docs/source/api/curies.get_prefixcommons_converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       82 2023-04-13 07:20:08.000000 curies-0.5.7/docs/source/api/curies.get_version.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      141 2023-04-13 07:20:08.000000 curies-0.5.7/docs/source/api/curies.mapping_service.MappingServiceGraph.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      332 2023-04-13 07:20:08.000000 curies-0.5.7/docs/source/api/curies.mapping_service.MappingServiceSPARQLProcessor.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      134 2023-04-13 07:20:08.000000 curies-0.5.7/docs/source/api/curies.mapping_service.get_fastapi_mapping_app.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      119 2023-04-13 07:20:08.000000 curies-0.5.7/docs/source/api/curies.mapping_service.get_fastapi_router.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      128 2023-04-13 07:20:08.000000 curies-0.5.7/docs/source/api/curies.mapping_service.get_flask_mapping_app.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      146 2023-04-13 07:20:08.000000 curies-0.5.7/docs/source/api/curies.mapping_service.get_flask_mapping_blueprint.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)     7469 2023-07-22 23:20:18.000000 curies-0.5.7/docs/source/conf.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2538 2023-03-10 11:58:39.000000 curies-0.5.7/docs/source/index.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      377 2023-07-02 15:23:36.000000 curies-0.5.7/pyproject.toml
--rw-r--r--   0 cthoyt     (501) staff       (20)     2647 2023-07-22 23:20:19.933249 curies-0.5.7/setup.cfg
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-22 23:20:19.904259 curies-0.5.7/src/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-22 23:20:19.923356 curies-0.5.7/src/curies/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1015 2023-05-15 10:11:51.000000 curies-0.5.7/src/curies/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      146 2023-02-21 22:19:21.000000 curies-0.5.7/src/curies/__main__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    44826 2023-07-22 23:17:39.000000 curies-0.5.7/src/curies/api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     5065 2023-04-13 07:17:14.000000 curies-0.5.7/src/curies/cli.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-22 23:20:19.928210 curies-0.5.7/src/curies/mapping_service/
--rw-r--r--   0 cthoyt     (501) staff       (20)     4478 2023-04-13 07:57:38.000000 curies-0.5.7/src/curies/mapping_service/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     8224 2023-05-05 11:46:12.000000 curies-0.5.7/src/curies/mapping_service/api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3343 2023-03-26 20:29:12.000000 curies-0.5.7/src/curies/mapping_service/rdflib_custom.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     4637 2023-05-05 11:46:12.000000 curies-0.5.7/src/curies/mapping_service/utils.py
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-07-31 23:04:01.000000 curies-0.5.7/src/curies/py.typed
--rw-r--r--   0 cthoyt     (501) staff       (20)     2033 2023-03-04 12:32:17.000000 curies-0.5.7/src/curies/sources.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      255 2023-07-22 23:20:18.000000 curies-0.5.7/src/curies/version.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     9669 2023-07-02 15:23:36.000000 curies-0.5.7/src/curies/web.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-22 23:20:19.925889 curies-0.5.7/src/curies.egg-info/
--rw-r--r--   0 cthoyt     (501) staff       (20)    11777 2023-07-22 23:20:19.000000 curies-0.5.7/src/curies.egg-info/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     1837 2023-07-22 23:20:19.000000 curies-0.5.7/src/curies.egg-info/SOURCES.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-07-22 23:20:19.000000 curies-0.5.7/src/curies.egg-info/dependency_links.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-07-31 23:04:24.000000 curies-0.5.7/src/curies.egg-info/not-zip-safe
--rw-r--r--   0 cthoyt     (501) staff       (20)      290 2023-07-22 23:20:19.000000 curies-0.5.7/src/curies.egg-info/requires.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        7 2023-07-22 23:20:19.000000 curies-0.5.7/src/curies.egg-info/top_level.txt
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-22 23:20:19.931445 curies-0.5.7/tests/
--rw-r--r--   0 cthoyt     (501) staff       (20)       56 2022-07-31 23:04:00.000000 curies-0.5.7/tests/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    19293 2023-07-22 23:17:39.000000 curies-0.5.7/tests/test_api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     5198 2023-04-13 10:20:39.000000 curies-0.5.7/tests/test_federated_sparql.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    13426 2023-04-13 07:57:38.000000 curies-0.5.7/tests/test_mapping_service.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3273 2023-07-02 15:23:36.000000 curies-0.5.7/tests/test_web.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-08-05 13:07:58.498147 curies-0.6.0/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2022-07-31 23:04:00.000000 curies-0.6.0/LICENSE
+-rw-r--r--   0 cthoyt     (501) staff       (20)      394 2023-04-28 13:05:54.000000 curies-0.6.0/MANIFEST.in
+-rw-r--r--   0 cthoyt     (501) staff       (20)    11908 2023-08-05 13:07:58.498358 curies-0.6.0/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)    10467 2023-08-05 13:07:02.000000 curies-0.6.0/README.md
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-08-05 13:07:58.462143 curies-0.6.0/docs/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-08-05 13:07:58.468562 curies-0.6.0/docs/source/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-08-05 13:07:58.483208 curies-0.6.0/docs/source/api/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2228 2023-07-31 12:30:08.000000 curies-0.6.0/docs/source/api/curies.Converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      101 2023-07-31 12:30:08.000000 curies-0.6.0/docs/source/api/curies.DuplicatePrefixes.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      110 2023-07-31 12:30:08.000000 curies-0.6.0/docs/source/api/curies.DuplicateURIPrefixes.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      107 2023-07-31 12:30:08.000000 curies-0.6.0/docs/source/api/curies.DuplicateValueError.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      345 2023-07-31 12:30:08.000000 curies-0.6.0/docs/source/api/curies.Record.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      445 2023-07-31 12:30:08.000000 curies-0.6.0/docs/source/api/curies.Reference.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      110 2023-07-31 12:30:08.000000 curies-0.6.0/docs/source/api/curies.ReferenceTuple.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       64 2023-07-31 12:30:08.000000 curies-0.6.0/docs/source/api/curies.chain.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      124 2023-07-31 12:30:08.000000 curies-0.6.0/docs/source/api/curies.get_bioregistry_converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       97 2023-07-31 12:30:08.000000 curies-0.6.0/docs/source/api/curies.get_go_converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      112 2023-07-31 12:30:08.000000 curies-0.6.0/docs/source/api/curies.get_monarch_converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      100 2023-07-31 12:30:08.000000 curies-0.6.0/docs/source/api/curies.get_obo_converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      130 2023-07-31 12:30:08.000000 curies-0.6.0/docs/source/api/curies.get_prefixcommons_converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       82 2023-07-31 12:30:08.000000 curies-0.6.0/docs/source/api/curies.get_version.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      141 2023-07-31 12:30:08.000000 curies-0.6.0/docs/source/api/curies.mapping_service.MappingServiceGraph.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      332 2023-07-31 12:30:08.000000 curies-0.6.0/docs/source/api/curies.mapping_service.MappingServiceSPARQLProcessor.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      134 2023-07-31 12:30:08.000000 curies-0.6.0/docs/source/api/curies.mapping_service.get_fastapi_mapping_app.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      119 2023-07-31 12:30:08.000000 curies-0.6.0/docs/source/api/curies.mapping_service.get_fastapi_router.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      128 2023-07-31 12:30:08.000000 curies-0.6.0/docs/source/api/curies.mapping_service.get_flask_mapping_app.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      146 2023-07-31 12:30:08.000000 curies-0.6.0/docs/source/api/curies.mapping_service.get_flask_mapping_blueprint.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      111 2023-07-31 12:30:08.000000 curies-0.6.0/docs/source/api/curies.resolver_service.get_fastapi_app.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      120 2023-07-31 12:30:08.000000 curies-0.6.0/docs/source/api/curies.resolver_service.get_fastapi_router.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      105 2023-07-31 12:30:08.000000 curies-0.6.0/docs/source/api/curies.resolver_service.get_flask_app.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      123 2023-07-31 12:30:08.000000 curies-0.6.0/docs/source/api/curies.resolver_service.get_flask_blueprint.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1313 2023-08-05 12:42:27.000000 curies-0.6.0/docs/source/api.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       47 2023-08-05 12:42:27.000000 curies-0.6.0/docs/source/cli.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7437 2023-08-05 13:07:57.000000 curies-0.6.0/docs/source/conf.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      666 2023-08-05 13:07:02.000000 curies-0.6.0/docs/source/index.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      137 2023-08-05 12:42:27.000000 curies-0.6.0/docs/source/mapping_service.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      118 2023-08-05 12:42:27.000000 curies-0.6.0/docs/source/resolver_service.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      197 2023-08-05 12:42:27.000000 curies-0.6.0/docs/source/struct.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      377 2023-07-02 15:23:36.000000 curies-0.6.0/pyproject.toml
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2576 2023-08-05 13:07:58.499553 curies-0.6.0/setup.cfg
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-08-05 13:07:58.462823 curies-0.6.0/src/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-08-05 13:07:58.488675 curies-0.6.0/src/curies/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      812 2023-08-05 12:42:27.000000 curies-0.6.0/src/curies/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      146 2023-02-21 22:19:21.000000 curies-0.6.0/src/curies/__main__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    45846 2023-08-05 12:42:27.000000 curies-0.6.0/src/curies/api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     5112 2023-08-05 12:42:27.000000 curies-0.6.0/src/curies/cli.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-08-05 13:07:58.493452 curies-0.6.0/src/curies/mapping_service/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4478 2023-04-13 07:57:38.000000 curies-0.6.0/src/curies/mapping_service/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8224 2023-05-05 11:46:12.000000 curies-0.6.0/src/curies/mapping_service/api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3343 2023-03-26 20:29:12.000000 curies-0.6.0/src/curies/mapping_service/rdflib_custom.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4637 2023-05-05 11:46:12.000000 curies-0.6.0/src/curies/mapping_service/utils.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-07-31 23:04:01.000000 curies-0.6.0/src/curies/py.typed
+-rw-r--r--   0 cthoyt     (501) staff       (20)     9669 2023-08-05 12:42:27.000000 curies-0.6.0/src/curies/resolver_service.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2095 2023-08-05 12:42:27.000000 curies-0.6.0/src/curies/sources.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      255 2023-08-05 13:07:57.000000 curies-0.6.0/src/curies/version.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-08-05 13:07:58.490926 curies-0.6.0/src/curies.egg-info/
+-rw-r--r--   0 cthoyt     (501) staff       (20)    11908 2023-08-05 13:07:58.000000 curies-0.6.0/src/curies.egg-info/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2138 2023-08-05 13:07:58.000000 curies-0.6.0/src/curies.egg-info/SOURCES.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-08-05 13:07:58.000000 curies-0.6.0/src/curies.egg-info/dependency_links.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-07-31 23:04:24.000000 curies-0.6.0/src/curies.egg-info/not-zip-safe
+-rw-r--r--   0 cthoyt     (501) staff       (20)      221 2023-08-05 13:07:58.000000 curies-0.6.0/src/curies.egg-info/requires.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        7 2023-08-05 13:07:58.000000 curies-0.6.0/src/curies.egg-info/top_level.txt
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-08-05 13:07:58.497602 curies-0.6.0/tests/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       56 2022-07-31 23:04:00.000000 curies-0.6.0/tests/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    19360 2023-08-05 12:42:27.000000 curies-0.6.0/tests/test_api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     5198 2023-04-13 10:20:39.000000 curies-0.6.0/tests/test_federated_sparql.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    13426 2023-04-13 07:57:38.000000 curies-0.6.0/tests/test_mapping_service.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3286 2023-08-05 12:42:27.000000 curies-0.6.0/tests/test_resolver_service.py
```

### Comparing `curies-0.5.7/LICENSE` & `curies-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `curies-0.5.7/PKG-INFO` & `curies-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curies
-Version: 0.5.7
+Version: 0.6.0
 Summary: Idiomatic conversion between URIs and compact URIs (CURIEs).
 Home-page: https://github.com/cthoyt/curies
 Download-URL: https://github.com/cthoyt/curies/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
@@ -26,15 +26,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: pandas
-Provides-Extra: bioregistry
 Provides-Extra: flask
 Provides-Extra: fastapi
 Provides-Extra: rdflib
 Provides-Extra: docs
 License-File: LICENSE
 
 <!--
@@ -250,14 +249,18 @@
 The most recent release can be installed from
 [PyPI](https://pypi.org/project/curies/) with:
 
 ```bash
 $ pip install curies
 ```
 
+This package currently supports both Pydantic v1 and v2. See the
+[Pydantic migration guide](https://docs.pydantic.dev/2.0/migration/)
+for updating your code.
+
 ## 👐 Contributing
 
 Contributions, whether filing an issue, making a pull request, or forking, are appreciated. See
 [CONTRIBUTING.md](https://github.com/cthoyt/curies/blob/master/.github/CONTRIBUTING.md) for more information on getting
 involved.
 
 ## 👋 Attribution
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: curies Version: 0.5.7 Summary: Idiomatic conversion
+Metadata-Version: 2.1 Name: curies Version: 0.6.0 Summary: Idiomatic conversion
 between URIs and compact URIs (CURIEs). Home-page: https://github.com/cthoyt/
 curies Download-URL: https://github.com/cthoyt/curies/releases Author: Charles
 Tapley Hoyt Author-email: cthoyt@gmail.com Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com License: MIT Project-URL: Bug Tracker,
 https://github.com/cthoyt/curies/issues Project-URL: Source Code, https://
 github.com/cthoyt/curies Keywords: snekpack,cookiecutter,semantic web,compact
 uniform resource identifiers,uniform resource identifiers,curies Classifier:
@@ -11,17 +11,16 @@
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Framework :: Pytest Classifier: Framework :: tox Classifier: Framework ::
 Sphinx Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
 Only Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-
-Extra: tests Provides-Extra: pandas Provides-Extra: bioregistry Provides-Extra:
-flask Provides-Extra: fastapi Provides-Extra: rdflib Provides-Extra: docs
-License-File: LICENSE
+Extra: tests Provides-Extra: pandas Provides-Extra: flask Provides-Extra:
+fastapi Provides-Extra: rdflib Provides-Extra: docs License-File: LICENSE
                              ****** curies ******
 [Tests] [PyPI] [PyPI_-_Python_Version] [PyPI_-_License] [Documentation_Status]
   [Codecov_status] [Cookiecutter_template_from_@cthoyt] [Code_style:_black]
                          [Contributor_Covenant] [DOI]
 Idiomatic conversion between URIs and compact URIs (CURIEs). ```python from
 curies import Converter converter = Converter.from_prefix_map({ "CHEBI": "http:
 //purl.obolibrary.org/obo/CHEBI_", "MONDO": "http://purl.obolibrary.org/obo/
@@ -87,15 +86,17 @@
 available programmatically, see the docs for more information. ##
 ð§âð¤âð§ Related Other packages that convert between CURIEs and URIs:
 - https://github.com/prefixcommons/prefixcommons-py (Python) - https://
 github.com/prefixcommons/curie-util (Java) - https://github.com/geneontology/
 curie-util-py (Python) - https://github.com/geneontology/curie-util-es5
 (Node.js) - https://github.com/endoli/curie.rs (Rust) ## ð Installation The
 most recent release can be installed from [PyPI](https://pypi.org/project/
-curies/) with: ```bash $ pip install curies ``` ## ð Contributing
+curies/) with: ```bash $ pip install curies ``` This package currently supports
+both Pydantic v1 and v2. See the [Pydantic migration guide](https://
+docs.pydantic.dev/2.0/migration/) for updating your code. ## ð Contributing
 Contributions, whether filing an issue, making a pull request, or forking, are
 appreciated. See [CONTRIBUTING.md](https://github.com/cthoyt/curies/blob/
 master/.github/CONTRIBUTING.md) for more information on getting involved. ##
 ð Attribution ### ð Acknowledgements This package heavily builds on the
 [trie](https://en.wikipedia.org/wiki/Trie) data structure implemented in
 [`pytrie`](https://github.com/gsakkis/pytrie). ### âï¸ License The code in
 this package is licensed under the MIT License. ### ðª Cookiecutter This
```

### Comparing `curies-0.5.7/README.md` & `curies-0.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -211,14 +211,18 @@
 The most recent release can be installed from
 [PyPI](https://pypi.org/project/curies/) with:
 
 ```bash
 $ pip install curies
 ```
 
+This package currently supports both Pydantic v1 and v2. See the
+[Pydantic migration guide](https://docs.pydantic.dev/2.0/migration/)
+for updating your code.
+
 ## 👐 Contributing
 
 Contributions, whether filing an issue, making a pull request, or forking, are appreciated. See
 [CONTRIBUTING.md](https://github.com/cthoyt/curies/blob/master/.github/CONTRIBUTING.md) for more information on getting
 involved.
 
 ## 👋 Attribution
```

#### html2text {}

```diff
@@ -67,15 +67,17 @@
 available programmatically, see the docs for more information. ##
 ð§âð¤âð§ Related Other packages that convert between CURIEs and URIs:
 - https://github.com/prefixcommons/prefixcommons-py (Python) - https://
 github.com/prefixcommons/curie-util (Java) - https://github.com/geneontology/
 curie-util-py (Python) - https://github.com/geneontology/curie-util-es5
 (Node.js) - https://github.com/endoli/curie.rs (Rust) ## ð Installation The
 most recent release can be installed from [PyPI](https://pypi.org/project/
-curies/) with: ```bash $ pip install curies ``` ## ð Contributing
+curies/) with: ```bash $ pip install curies ``` This package currently supports
+both Pydantic v1 and v2. See the [Pydantic migration guide](https://
+docs.pydantic.dev/2.0/migration/) for updating your code. ## ð Contributing
 Contributions, whether filing an issue, making a pull request, or forking, are
 appreciated. See [CONTRIBUTING.md](https://github.com/cthoyt/curies/blob/
 master/.github/CONTRIBUTING.md) for more information on getting involved. ##
 ð Attribution ### ð Acknowledgements This package heavily builds on the
 [trie](https://en.wikipedia.org/wiki/Trie) data structure implemented in
 [`pytrie`](https://github.com/gsakkis/pytrie). ### âï¸ License The code in
 this package is licensed under the MIT License. ### ðª Cookiecutter This
```

### Comparing `curies-0.5.7/docs/source/api/curies.Converter.rst` & `curies-0.6.0/docs/source/api/curies.Converter.rst`

 * *Files 24% similar despite different names*

```diff
@@ -9,18 +9,20 @@
    .. rubric:: Methods Summary
 
    .. autosummary::
 
       ~Converter.add_prefix
       ~Converter.add_record
       ~Converter.compress
+      ~Converter.compress_strict
       ~Converter.expand
       ~Converter.expand_all
       ~Converter.expand_pair
       ~Converter.expand_pair_all
+      ~Converter.expand_strict
       ~Converter.file_compress
       ~Converter.file_expand
       ~Converter.format_curie
       ~Converter.from_extended_prefix_map
       ~Converter.from_jsonld
       ~Converter.from_jsonld_github
       ~Converter.from_prefix_map
@@ -29,27 +31,32 @@
       ~Converter.from_reverse_prefix_map
       ~Converter.get_prefixes
       ~Converter.get_record
       ~Converter.parse_curie
       ~Converter.parse_uri
       ~Converter.pd_compress
       ~Converter.pd_expand
+      ~Converter.pd_standardize_curie
+      ~Converter.pd_standardize_prefix
+      ~Converter.pd_standardize_uri
       ~Converter.standardize_curie
       ~Converter.standardize_prefix
       ~Converter.standardize_uri
 
    .. rubric:: Methods Documentation
 
    .. automethod:: add_prefix
    .. automethod:: add_record
    .. automethod:: compress
+   .. automethod:: compress_strict
    .. automethod:: expand
    .. automethod:: expand_all
    .. automethod:: expand_pair
    .. automethod:: expand_pair_all
+   .. automethod:: expand_strict
    .. automethod:: file_compress
    .. automethod:: file_expand
    .. automethod:: format_curie
    .. automethod:: from_extended_prefix_map
    .. automethod:: from_jsonld
    .. automethod:: from_jsonld_github
    .. automethod:: from_prefix_map
@@ -58,10 +65,13 @@
    .. automethod:: from_reverse_prefix_map
    .. automethod:: get_prefixes
    .. automethod:: get_record
    .. automethod:: parse_curie
    .. automethod:: parse_uri
    .. automethod:: pd_compress
    .. automethod:: pd_expand
+   .. automethod:: pd_standardize_curie
+   .. automethod:: pd_standardize_prefix
+   .. automethod:: pd_standardize_uri
    .. automethod:: standardize_curie
    .. automethod:: standardize_prefix
    .. automethod:: standardize_uri
```

### Comparing `curies-0.5.7/docs/source/conf.py` & `curies-0.6.0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "curies"
 copyright = f"{date.today().year}, Charles Tapley Hoyt"
 author = "Charles Tapley Hoyt"
 
 # The full version, including alpha/beta/rc tags.
-release = "0.5.7"
+release = "0.6.0"
 
 # The short X.Y version.
 parsed_version = re.match(
     "(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?",
     release,
 )
 version = parsed_version.expand("\g<major>.\g<minor>.\g<patch>")
@@ -59,15 +59,14 @@
     "sphinx.ext.autosummary",
     "sphinx.ext.autodoc",
     "sphinx.ext.coverage",
     "sphinx.ext.intersphinx",
     "sphinx.ext.todo",
     "sphinx.ext.mathjax",
     "sphinx.ext.viewcode",
-    "sphinx_autodoc_typehints",
     "sphinx_automodapi.automodapi",
     "sphinx_automodapi.smart_resolver",
     # 'texext',
 ]
 
 
 # generate autosummary pages
```

### Comparing `curies-0.5.7/setup.cfg` & `curies-0.6.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = curies
-version = 0.5.7
+version = 0.6.0
 description = Idiomatic conversion between URIs and compact URIs (CURIEs).
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/cthoyt/curies
 download_url = https://github.com/cthoyt/curies/releases
 project_urls = 
 	Bug Tracker = https://github.com/cthoyt/curies/issues
@@ -38,15 +38,15 @@
 	compact uniform resource identifiers
 	uniform resource identifiers
 	curies
 
 [options]
 install_requires = 
 	pytrie
-	pydantic<2.0
+	pydantic
 	requests
 zip_safe = false
 include_package_data = True
 python_requires = >=3.8
 packages = find:
 package_dir = 
 	= src
@@ -56,31 +56,28 @@
 
 [options.extras_require]
 tests = 
 	pytest
 	coverage
 pandas = 
 	pandas
-bioregistry = 
-	bioregistry>=0.5.136
 flask = 
 	flask
 	defusedxml
 fastapi = 
 	fastapi
 	python-multipart
 	httpx
 	defusedxml
 	uvicorn
 rdflib = 
 	rdflib
 docs = 
-	sphinx<7.0
+	sphinx
 	sphinx-rtd-theme
-	sphinx-autodoc-typehints
 	sphinx_automodapi
 
 [doc8]
 max-line-length = 120
 
 [coverage:run]
 branch = True
```

### Comparing `curies-0.5.7/src/curies/__init__.py` & `curies-0.6.0/src/curies/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     get_bioregistry_converter,
     get_go_converter,
     get_monarch_converter,
     get_obo_converter,
     get_prefixcommons_converter,
 )
 from .version import get_version
-from .web import get_fastapi_app, get_fastapi_router, get_flask_app, get_flask_blueprint
 
 __all__ = [
     "Converter",
     "Record",
     "ReferenceTuple",
     "Reference",
     "DuplicateValueError",
@@ -34,13 +33,8 @@
     "get_version",
     # sources
     "get_obo_converter",
     "get_prefixcommons_converter",
     "get_monarch_converter",
     "get_go_converter",
     "get_bioregistry_converter",
-    # Web extras
-    "get_flask_blueprint",
-    "get_flask_app",
-    "get_fastapi_router",
-    "get_fastapi_app",
 ]
```

### Comparing `curies-0.5.7/src/curies/api.py` & `curies-0.6.0/src/curies/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,14 +302,37 @@
         'http://purl.obolibrary.org/obo/CHEBI_1'
 
         # Example with unparsable URI:
         >>> converter.compress("http://example.com/missing:0000000")
 
         # Example with missing prefix:
         >>> converter.expand("missing:0000000")
+
+    Incremental Converters
+    ----------------------
+    As suggested in `#13 <https://github.com/cthoyt/curies/issues/33>`_, new prefixes
+    can be added to an existing converter like in the following:
+
+    .. code-block::
+
+        import curies
+
+        converter = curies.get_obo_converter()
+        converter.add_prefix("hgnc", "https://bioregistry.io/hgnc:")
+
+    Similarly, an empty converter can be instantiated using an empty list
+    for the `records` argument and prefixes can be added one at a time
+    (note this currently does not allow for adding synonyms separately):
+
+    .. code-block::
+
+        import curies
+
+        converter = curies.Converter(records=[])
+        converter.add_prefix("hgnc", "https://bioregistry.io/hgnc:")
     """
 
     #: The expansion dictionary with prefixes as keys and priority URI prefixes as values
     prefix_map: Dict[str, str]
     #: The mapping from URI prefixes to prefixes
     reverse_prefix_map: Dict[str, str]
     #: A prefix trie for efficient parsing of URIs
@@ -620,15 +643,21 @@
         Example from a remote context file:
 
         >>> base = "https://raw.githubusercontent.com"
         >>> url = f"{base}/biopragmatics/bioregistry/main/exports/contexts/semweb.context.jsonld"
         >>> converter = Converter.from_jsonld(url)
         >>> "rdf" in converter.prefix_map
         """
-        return cls.from_prefix_map(_prepare(data)["@context"])
+        prefix_map = {}
+        for key, value in _prepare(data)["@context"].items():
+            if isinstance(value, str):
+                prefix_map[key] = value
+            elif isinstance(value, dict) and value.get("@prefix") is True:
+                prefix_map[key] = value["@id"]
+        return cls.from_prefix_map(prefix_map)
 
     @classmethod
     def from_jsonld_github(
         cls, owner: str, repo: str, *path: str, branch: str = "main"
     ) -> "Converter":
         """Construct a remote JSON-LD URL on GitHub then parse with :meth:`Converter.from_jsonld`.
```

### Comparing `curies-0.5.7/src/curies/cli.py` & `curies-0.6.0/src/curies/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 """
 
 import sys
 from typing import Callable, Mapping
 
 import click
 
-import curies
 from curies import Converter, sources
 
 __all__ = [
     "main",
 ]
 
 LOADERS = {
@@ -61,18 +60,20 @@
     if format is None:
         click.secho("--format is required with remote data", fg="red")
         return sys.exit(1)
     return LOADERS[format](location)
 
 
 def _get_resolver_app(converter: Converter, framework: str):
+    from curies import resolver_service
+
     if framework == "flask":
-        return curies.get_flask_app(converter)
+        return resolver_service.get_flask_app(converter)
     elif framework == "fastapi":
-        return curies.get_fastapi_app(converter)
+        return resolver_service.get_fastapi_app(converter)
     else:
         raise ValueError(f"Unhandled framework: {framework}")
 
 
 def _get_mapper_app(converter: Converter, framework: str):
     from curies import mapping_service
```

### Comparing `curies-0.5.7/src/curies/mapping_service/__init__.py` & `curies-0.6.0/src/curies/mapping_service/__init__.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.7/src/curies/mapping_service/api.py` & `curies-0.6.0/src/curies/mapping_service/api.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.7/src/curies/mapping_service/rdflib_custom.py` & `curies-0.6.0/src/curies/mapping_service/rdflib_custom.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.7/src/curies/mapping_service/utils.py` & `curies-0.6.0/src/curies/mapping_service/utils.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.7/src/curies/sources.py` & `curies-0.6.0/src/curies/sources.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,10 +56,11 @@
     """Get the latest Bioregistry context."""
     if not web:
         try:
             import bioregistry
         except ImportError:  # pragma: no cover
             pass
         else:
-            return Converter.from_extended_prefix_map(bioregistry.manager.get_curies_records())
+            epm = bioregistry.manager.get_curies_records()  # pragma: no cover
+            return Converter.from_extended_prefix_map(epm)  # pragma: no cover
     url = f"{BIOREGISTRY_CONTEXTS}/bioregistry.epm.json"
     return Converter.from_extended_prefix_map(url, **kwargs)
```

### Comparing `curies-0.5.7/src/curies/web.py` & `curies-0.6.0/src/curies/resolver_service.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.7/src/curies.egg-info/PKG-INFO` & `curies-0.6.0/src/curies.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curies
-Version: 0.5.7
+Version: 0.6.0
 Summary: Idiomatic conversion between URIs and compact URIs (CURIEs).
 Home-page: https://github.com/cthoyt/curies
 Download-URL: https://github.com/cthoyt/curies/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
@@ -26,15 +26,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: pandas
-Provides-Extra: bioregistry
 Provides-Extra: flask
 Provides-Extra: fastapi
 Provides-Extra: rdflib
 Provides-Extra: docs
 License-File: LICENSE
 
 <!--
@@ -250,14 +249,18 @@
 The most recent release can be installed from
 [PyPI](https://pypi.org/project/curies/) with:
 
 ```bash
 $ pip install curies
 ```
 
+This package currently supports both Pydantic v1 and v2. See the
+[Pydantic migration guide](https://docs.pydantic.dev/2.0/migration/)
+for updating your code.
+
 ## 👐 Contributing
 
 Contributions, whether filing an issue, making a pull request, or forking, are appreciated. See
 [CONTRIBUTING.md](https://github.com/cthoyt/curies/blob/master/.github/CONTRIBUTING.md) for more information on getting
 involved.
 
 ## 👋 Attribution
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: curies Version: 0.5.7 Summary: Idiomatic conversion
+Metadata-Version: 2.1 Name: curies Version: 0.6.0 Summary: Idiomatic conversion
 between URIs and compact URIs (CURIEs). Home-page: https://github.com/cthoyt/
 curies Download-URL: https://github.com/cthoyt/curies/releases Author: Charles
 Tapley Hoyt Author-email: cthoyt@gmail.com Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com License: MIT Project-URL: Bug Tracker,
 https://github.com/cthoyt/curies/issues Project-URL: Source Code, https://
 github.com/cthoyt/curies Keywords: snekpack,cookiecutter,semantic web,compact
 uniform resource identifiers,uniform resource identifiers,curies Classifier:
@@ -11,17 +11,16 @@
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Framework :: Pytest Classifier: Framework :: tox Classifier: Framework ::
 Sphinx Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
 Only Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-
-Extra: tests Provides-Extra: pandas Provides-Extra: bioregistry Provides-Extra:
-flask Provides-Extra: fastapi Provides-Extra: rdflib Provides-Extra: docs
-License-File: LICENSE
+Extra: tests Provides-Extra: pandas Provides-Extra: flask Provides-Extra:
+fastapi Provides-Extra: rdflib Provides-Extra: docs License-File: LICENSE
                              ****** curies ******
 [Tests] [PyPI] [PyPI_-_Python_Version] [PyPI_-_License] [Documentation_Status]
   [Codecov_status] [Cookiecutter_template_from_@cthoyt] [Code_style:_black]
                          [Contributor_Covenant] [DOI]
 Idiomatic conversion between URIs and compact URIs (CURIEs). ```python from
 curies import Converter converter = Converter.from_prefix_map({ "CHEBI": "http:
 //purl.obolibrary.org/obo/CHEBI_", "MONDO": "http://purl.obolibrary.org/obo/
@@ -87,15 +86,17 @@
 available programmatically, see the docs for more information. ##
 ð§âð¤âð§ Related Other packages that convert between CURIEs and URIs:
 - https://github.com/prefixcommons/prefixcommons-py (Python) - https://
 github.com/prefixcommons/curie-util (Java) - https://github.com/geneontology/
 curie-util-py (Python) - https://github.com/geneontology/curie-util-es5
 (Node.js) - https://github.com/endoli/curie.rs (Rust) ## ð Installation The
 most recent release can be installed from [PyPI](https://pypi.org/project/
-curies/) with: ```bash $ pip install curies ``` ## ð Contributing
+curies/) with: ```bash $ pip install curies ``` This package currently supports
+both Pydantic v1 and v2. See the [Pydantic migration guide](https://
+docs.pydantic.dev/2.0/migration/) for updating your code. ## ð Contributing
 Contributions, whether filing an issue, making a pull request, or forking, are
 appreciated. See [CONTRIBUTING.md](https://github.com/cthoyt/curies/blob/
 master/.github/CONTRIBUTING.md) for more information on getting involved. ##
 ð Attribution ### ð Acknowledgements This package heavily builds on the
 [trie](https://en.wikipedia.org/wiki/Trie) data structure implemented in
 [`pytrie`](https://github.com/gsakkis/pytrie). ### âï¸ License The code in
 this package is licensed under the MIT License. ### ðª Cookiecutter This
```

### Comparing `curies-0.5.7/src/curies.egg-info/SOURCES.txt` & `curies-0.6.0/src/curies.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,59 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
+docs/source/api.rst
+docs/source/cli.rst
 docs/source/conf.py
 docs/source/index.rst
+docs/source/mapping_service.rst
+docs/source/resolver_service.rst
+docs/source/struct.rst
 docs/source/api/curies.Converter.rst
 docs/source/api/curies.DuplicatePrefixes.rst
 docs/source/api/curies.DuplicateURIPrefixes.rst
 docs/source/api/curies.DuplicateValueError.rst
 docs/source/api/curies.Record.rst
+docs/source/api/curies.Reference.rst
+docs/source/api/curies.ReferenceTuple.rst
 docs/source/api/curies.chain.rst
 docs/source/api/curies.get_bioregistry_converter.rst
-docs/source/api/curies.get_fastapi_app.rst
-docs/source/api/curies.get_fastapi_router.rst
-docs/source/api/curies.get_flask_app.rst
-docs/source/api/curies.get_flask_blueprint.rst
 docs/source/api/curies.get_go_converter.rst
 docs/source/api/curies.get_monarch_converter.rst
 docs/source/api/curies.get_obo_converter.rst
 docs/source/api/curies.get_prefixcommons_converter.rst
 docs/source/api/curies.get_version.rst
 docs/source/api/curies.mapping_service.MappingServiceGraph.rst
 docs/source/api/curies.mapping_service.MappingServiceSPARQLProcessor.rst
 docs/source/api/curies.mapping_service.get_fastapi_mapping_app.rst
 docs/source/api/curies.mapping_service.get_fastapi_router.rst
 docs/source/api/curies.mapping_service.get_flask_mapping_app.rst
 docs/source/api/curies.mapping_service.get_flask_mapping_blueprint.rst
+docs/source/api/curies.resolver_service.get_fastapi_app.rst
+docs/source/api/curies.resolver_service.get_fastapi_router.rst
+docs/source/api/curies.resolver_service.get_flask_app.rst
+docs/source/api/curies.resolver_service.get_flask_blueprint.rst
 src/curies/__init__.py
 src/curies/__main__.py
 src/curies/api.py
 src/curies/cli.py
 src/curies/py.typed
+src/curies/resolver_service.py
 src/curies/sources.py
 src/curies/version.py
-src/curies/web.py
 src/curies.egg-info/PKG-INFO
 src/curies.egg-info/SOURCES.txt
 src/curies.egg-info/dependency_links.txt
 src/curies.egg-info/not-zip-safe
 src/curies.egg-info/requires.txt
 src/curies.egg-info/top_level.txt
 src/curies/mapping_service/__init__.py
 src/curies/mapping_service/api.py
 src/curies/mapping_service/rdflib_custom.py
 src/curies/mapping_service/utils.py
 tests/__init__.py
 tests/test_api.py
 tests/test_federated_sparql.py
 tests/test_mapping_service.py
-tests/test_web.py
+tests/test_resolver_service.py
```

### Comparing `curies-0.5.7/tests/test_api.py` & `curies-0.6.0/tests/test_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import tempfile
 import unittest
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 import pandas as pd
 import rdflib
-from bioregistry.export.prefix_maps import EXTENDED_PREFIX_MAP_PATH
 
 from curies.api import (
     CompressionError,
     Converter,
     DuplicatePrefixes,
     DuplicateURIPrefixes,
     ExpansionError,
@@ -141,14 +140,32 @@
             bioregistry_converter = get_bioregistry_converter(web=web)
             self.assert_bioregistry_converter(bioregistry_converter)
 
         c = Converter.from_reverse_prefix_map(f"{BIOREGISTRY_CONTEXTS}/bioregistry.rpm.json")
         self.assertIn("chebi", c.prefix_map)
         self.assertNotIn("CHEBI", c.prefix_map)
 
+    def test_jsonld(self):
+        """Test parsing JSON-LD context."""
+        context = {
+            "@context": {
+                "hello": "https://example.org/hello:",
+                "CHEBI": {
+                    "@prefix": True,
+                    "@id": "http://purl.obolibrary.org/CHEBI_",
+                },
+                "nope": {
+                    "nope": "nope",
+                },
+            },
+        }
+        converter = Converter.from_jsonld(context)
+        self.assertIn("hello", converter.prefix_map)
+        self.assertIn("CHEBI", converter.prefix_map)
+
     def test_from_github(self):
         """Test getting a JSON-LD map from GitHub."""
         with self.assertRaises(ValueError):
             # missing end .jsonld file
             Converter.from_jsonld_github("biopragmatics", "bioregistry")
 
         semweb_converter = Converter.from_jsonld_github(
@@ -187,24 +204,14 @@
         self.assertIn("chebi", converter.prefix_map)
         # Synonyms that are non-conflicting also get added
         self.assertIn("CHEBI", converter.prefix_map)
         chebi_uri = converter.prefix_map["chebi"]
         self.assertIn(chebi_uri, converter.reverse_prefix_map)
         self.assertEqual("chebi", converter.reverse_prefix_map[chebi_uri])
 
-    @unittest.skipUnless(
-        EXTENDED_PREFIX_MAP_PATH.is_file(),
-        reason="missing local, editable installation of the Bioregistry",
-    )
-    def test_bioregistry_editable(self):
-        """Test loading the bioregistry extended prefix map locally."""
-        records = json.loads(EXTENDED_PREFIX_MAP_PATH.read_text())
-        converter = Converter.from_extended_prefix_map(records)
-        self.assert_bioregistry_converter(converter)
-
     def test_load_path(self):
         """Test loading from paths."""
         with tempfile.TemporaryDirectory() as directory:
             path = Path(directory).joinpath("pm.json")
             with self.assertRaises(FileNotFoundError):
                 Converter.from_prefix_map(path)
             with self.assertRaises(FileNotFoundError):
```

### Comparing `curies-0.5.7/tests/test_federated_sparql.py` & `curies-0.6.0/tests/test_federated_sparql.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.7/tests/test_mapping_service.py` & `curies-0.6.0/tests/test_mapping_service.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.7/tests/test_web.py` & `curies-0.6.0/tests/test_resolver_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import unittest
 from typing import ClassVar
 
 from fastapi.testclient import TestClient
 
 from curies import Converter
-from curies.web import FAILURE_CODE, get_fastapi_app, get_flask_app
+from curies.resolver_service import FAILURE_CODE, get_fastapi_app, get_flask_app
 
 
 class ConverterMixin(unittest.TestCase):
     """A mixin that has a converter."""
 
     delimiter: ClassVar[str] = ":"
```

