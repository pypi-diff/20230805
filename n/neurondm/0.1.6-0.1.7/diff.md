# Comparing `tmp/neurondm-0.1.6.tar.gz` & `tmp/neurondm-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurondm-0.1.6.tar", last modified: Wed Jul 19 03:43:16 2023, max compression
+gzip compressed data, was "neurondm-0.1.7.tar", last modified: Sat Aug  5 01:09:51 2023, max compression
```

## Comparing `neurondm-0.1.6.tar` & `neurondm-0.1.7.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-19 03:43:16.679680 neurondm-0.1.6/
--rw-r--r--   0 tom       (1000) tom       (1000)       35 2023-07-19 03:21:26.000000 neurondm-0.1.6/.coveragerc
--rw-r--r--   0 tom       (1000) tom       (1000)     1080 2023-07-19 03:21:26.000000 neurondm-0.1.6/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)     4080 2023-07-19 03:43:16.679680 neurondm-0.1.6/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     2885 2023-07-19 03:21:26.000000 neurondm-0.1.6/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-19 03:43:16.673681 neurondm-0.1.6/docs/
--rw-r--r--   0 tom       (1000) tom       (1000)    35150 2023-07-19 03:21:26.000000 neurondm-0.1.6/docs/NeuronLangExample.ipynb
--rw-r--r--   0 tom       (1000) tom       (1000)    11858 2023-07-19 03:21:26.000000 neurondm-0.1.6/docs/basic-model.org
--rw-r--r--   0 tom       (1000) tom       (1000)     8852 2023-07-19 03:21:26.000000 neurondm-0.1.6/docs/composer.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1618 2023-07-19 03:21:26.000000 neurondm-0.1.6/docs/neurons_notebook.md
--rw-r--r--   0 tom       (1000) tom       (1000)     9180 2023-07-19 03:21:26.000000 neurondm-0.1.6/docs/types.org
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-19 03:43:16.675680 neurondm-0.1.6/neurondm/
--rw-r--r--   0 tom       (1000) tom       (1000)       69 2023-07-19 03:22:19.000000 neurondm-0.1.6/neurondm/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      199 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/auth-config.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    68696 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/build.py
--rw-r--r--   0 tom       (1000) tom       (1000)   152101 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/core.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)     4459 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/example.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)     6333 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/indicators.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3843 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/lang.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-19 03:43:16.677681 neurondm-0.1.6/neurondm/models/
--rw-r--r--   0 tom       (1000) tom       (1000)      642 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/README.md
--rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/__init__.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    14860 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/allen_cell_types.py
--rw-r--r--   0 tom       (1000) tom       (1000)    12913 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/allen_type_specimen_mapping.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3853 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/apinat_npo.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10886 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/apinat_pops_more.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)     4389 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/basic_neurons.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)     3001 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/bolew.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    28861 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/cuts.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    35426 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/huang2017.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    20675 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/keast2020.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)     6991 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/ma2015.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1310 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/nerves.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6685 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/nlp.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4334 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/pcl.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)     4341 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/phenotype_direct.py
--rw-r--r--   0 tom       (1000) tom       (1000)     8922 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/orders.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    13633 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/phenotype_namespaces.py
--rw-r--r--   0 tom       (1000) tom       (1000)    29628 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/sheets.py
--rw-r--r--   0 tom       (1000) tom       (1000)    15634 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/simple.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-19 03:43:16.675680 neurondm-0.1.6/neurondm.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     4080 2023-07-19 03:43:16.000000 neurondm-0.1.6/neurondm.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     1364 2023-07-19 03:43:16.000000 neurondm-0.1.6/neurondm.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-07-19 03:43:16.000000 neurondm-0.1.6/neurondm.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)      168 2023-07-19 03:43:16.000000 neurondm-0.1.6/neurondm.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        9 2023-07-19 03:43:16.000000 neurondm-0.1.6/neurondm.egg-info/top_level.txt
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-19 03:43:16.678681 neurondm-0.1.6/resources/
--rw-r--r--   0 tom       (1000) tom       (1000)   104921 2023-07-19 03:43:15.000000 neurondm-0.1.6/resources/part-of-self.ttl
--rw-r--r--   0 tom       (1000) tom       (1000)    27641 2023-07-19 03:43:15.000000 neurondm-0.1.6/resources/phenotype-core.ttl
--rw-r--r--   0 tom       (1000) tom       (1000)    14792 2023-07-19 03:43:15.000000 neurondm-0.1.6/resources/phenotype-indicators.ttl
--rw-r--r--   0 tom       (1000) tom       (1000)    37820 2023-07-19 03:43:15.000000 neurondm-0.1.6/resources/phenotypes.ttl
--rw-r--r--   0 tom       (1000) tom       (1000)      166 2023-07-19 03:43:16.679680 neurondm-0.1.6/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)     4513 2023-07-19 03:21:26.000000 neurondm-0.1.6/setup.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-19 03:43:16.679680 neurondm-0.1.6/test/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2023-07-19 03:21:26.000000 neurondm-0.1.6/test/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1202 2023-07-19 03:21:26.000000 neurondm-0.1.6/test/common.py
--rw-r--r--   0 tom       (1000) tom       (1000)      407 2023-07-19 03:21:26.000000 neurondm-0.1.6/test/test_0_fix_sys_modules.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2403 2023-07-19 03:21:26.000000 neurondm-0.1.6/test/test_integration.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2316 2023-07-19 03:21:26.000000 neurondm-0.1.6/test/test_label.py
--rw-r--r--   0 tom       (1000) tom       (1000)      387 2023-07-19 03:21:26.000000 neurondm-0.1.6/test/test_load.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2023 2023-07-19 03:21:26.000000 neurondm-0.1.6/test/test_madness.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10400 2023-07-19 03:21:26.000000 neurondm-0.1.6/test/test_neurons.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3399 2023-07-19 03:21:26.000000 neurondm-0.1.6/test/test_simple.py
--rw-r--r--   0 tom       (1000) tom       (1000)      754 2023-07-19 03:21:26.000000 neurondm-0.1.6/test/test_triples.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-07-19 03:21:26.000000 neurondm-0.1.6/test/test_write.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-08-05 01:09:51.430831 neurondm-0.1.7/
+-rw-r--r--   0 tom       (1000) tom       (1000)       35 2023-08-05 01:06:38.000000 neurondm-0.1.7/.coveragerc
+-rw-r--r--   0 tom       (1000) tom       (1000)     1080 2023-08-05 01:06:38.000000 neurondm-0.1.7/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)     4080 2023-08-05 01:09:51.430831 neurondm-0.1.7/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     2885 2023-08-05 01:06:38.000000 neurondm-0.1.7/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-08-05 01:09:51.425831 neurondm-0.1.7/docs/
+-rw-r--r--   0 tom       (1000) tom       (1000)    35150 2023-08-05 01:06:38.000000 neurondm-0.1.7/docs/NeuronLangExample.ipynb
+-rw-r--r--   0 tom       (1000) tom       (1000)    11858 2023-08-05 01:06:38.000000 neurondm-0.1.7/docs/basic-model.org
+-rw-r--r--   0 tom       (1000) tom       (1000)     9380 2023-08-05 01:06:38.000000 neurondm-0.1.7/docs/composer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1618 2023-08-05 01:06:38.000000 neurondm-0.1.7/docs/neurons_notebook.md
+-rw-r--r--   0 tom       (1000) tom       (1000)     9180 2023-08-05 01:06:38.000000 neurondm-0.1.7/docs/types.org
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-08-05 01:09:51.426831 neurondm-0.1.7/neurondm/
+-rw-r--r--   0 tom       (1000) tom       (1000)       69 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      199 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/auth-config.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    68696 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/build.py
+-rw-r--r--   0 tom       (1000) tom       (1000)   152446 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/core.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     4459 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/example.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     6333 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/indicators.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3843 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/lang.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-08-05 01:09:51.428831 neurondm-0.1.7/neurondm/models/
+-rw-r--r--   0 tom       (1000) tom       (1000)      642 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/models/README.md
+-rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/models/__init__.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    14860 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/models/allen_cell_types.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    12913 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/models/allen_type_specimen_mapping.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3853 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/models/apinat_npo.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10886 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/models/apinat_pops_more.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     4389 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/models/basic_neurons.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     3001 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/models/bolew.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    28861 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/models/cuts.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    35426 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/models/huang2017.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    20675 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/models/keast2020.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     6991 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/models/ma2015.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1310 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/models/nerves.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     7593 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/models/nlp.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4334 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/models/pcl.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     4341 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/models/phenotype_direct.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    16091 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/orders.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    13633 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/phenotype_namespaces.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    29628 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/sheets.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    15634 2023-08-05 01:06:38.000000 neurondm-0.1.7/neurondm/simple.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-08-05 01:09:51.427831 neurondm-0.1.7/neurondm.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     4080 2023-08-05 01:09:51.000000 neurondm-0.1.7/neurondm.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     1364 2023-08-05 01:09:51.000000 neurondm-0.1.7/neurondm.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-08-05 01:09:51.000000 neurondm-0.1.7/neurondm.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)      168 2023-08-05 01:09:51.000000 neurondm-0.1.7/neurondm.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        9 2023-08-05 01:09:51.000000 neurondm-0.1.7/neurondm.egg-info/top_level.txt
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-08-05 01:09:51.429831 neurondm-0.1.7/resources/
+-rw-r--r--   0 tom       (1000) tom       (1000)   107828 2023-08-05 01:09:50.000000 neurondm-0.1.7/resources/part-of-self.ttl
+-rw-r--r--   0 tom       (1000) tom       (1000)    27641 2023-08-05 01:09:50.000000 neurondm-0.1.7/resources/phenotype-core.ttl
+-rw-r--r--   0 tom       (1000) tom       (1000)    14792 2023-08-05 01:09:50.000000 neurondm-0.1.7/resources/phenotype-indicators.ttl
+-rw-r--r--   0 tom       (1000) tom       (1000)    37820 2023-08-05 01:09:50.000000 neurondm-0.1.7/resources/phenotypes.ttl
+-rw-r--r--   0 tom       (1000) tom       (1000)      166 2023-08-05 01:09:51.430831 neurondm-0.1.7/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)     4513 2023-08-05 01:06:38.000000 neurondm-0.1.7/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-08-05 01:09:51.430831 neurondm-0.1.7/test/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2023-08-05 01:06:38.000000 neurondm-0.1.7/test/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1202 2023-08-05 01:06:38.000000 neurondm-0.1.7/test/common.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      407 2023-08-05 01:06:38.000000 neurondm-0.1.7/test/test_0_fix_sys_modules.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2403 2023-08-05 01:06:38.000000 neurondm-0.1.7/test/test_integration.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2316 2023-08-05 01:06:38.000000 neurondm-0.1.7/test/test_label.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      387 2023-08-05 01:06:38.000000 neurondm-0.1.7/test/test_load.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2023 2023-08-05 01:06:38.000000 neurondm-0.1.7/test/test_madness.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10400 2023-08-05 01:06:38.000000 neurondm-0.1.7/test/test_neurons.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3399 2023-08-05 01:06:38.000000 neurondm-0.1.7/test/test_simple.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      754 2023-08-05 01:06:38.000000 neurondm-0.1.7/test/test_triples.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-08-05 01:06:38.000000 neurondm-0.1.7/test/test_write.py
```

### Comparing `neurondm-0.1.6/LICENSE` & `neurondm-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/PKG-INFO` & `neurondm-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurondm
-Version: 0.1.6
+Version: 0.1.7
 Summary: A data model for neuron types.
 Home-page: https://github.com/tgbugs/pyontutils/tree/master/neurondm
 Author: Tom Gillespie
 Author-email: tgbugs@gmail.com
 License: MIT
 Keywords: neuron types NIF ontology neuroscience phenotype OWL rdf rdflib data model
 Classifier: Development Status :: 4 - Beta
```

### Comparing `neurondm-0.1.6/README.md` & `neurondm-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/docs/NeuronLangExample.ipynb` & `neurondm-0.1.7/docs/NeuronLangExample.ipynb`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/docs/basic-model.org` & `neurondm-0.1.7/docs/basic-model.org`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/docs/composer.py` & `neurondm-0.1.7/docs/composer.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,14 +149,21 @@
         header = 'label', 'curie', 'iri', 'source'
         rows = (
             [header] +
             [(_.label, _.curie, _.iri, loc_src[_]) for _ in sorted(locations, key=key)])
         with open('/tmp/npo-nlp-apinat-location-summary.csv', 'wt') as f:
             csv.writer(f, lineterminator='\n').writerows(rows)
 
+        preds = sorted(set(e for n in neurons for e in n.edges))
+        header = ['id'] + [OntId(p).curie for p in preds]
+        _rows = [[n.id_, *[','.join(sorted([OntId(o).curie  for o in n.getObjects(p)])) for p in preds]] for n in neurons]
+        rows = [header] + _rows
+        with open('/tmp/npo-by-predicates.csv', 'wt') as f:
+            csv.writer(f, lineterminator='\n').writerows(rows)
+
     else:
         header = 'o', 'o_label', 'o_synonym'
         rows = (
             [header] +
             [(_.iri, _.label, syn) for _ in sorted(locations, key=key)
              for syn in _.synonyms])
         with open('/tmp/anatomical_entities.csv', 'wt') as f:
@@ -222,13 +229,16 @@
     fcs = [for_composer(n) for n in mvp_ingest]
     _fcne = [for_composer(n, cull=True) for n in mvp_ingest]  # exclude empties for easier manual review
 
     # example neuron
     n = mvp_ingest[0]
     fc = for_composer(n)
 
+    # example partial orders
+    view_partial_orders = [tuple(simplify_nested(simplify, n.partialOrder())) for n in neurons]
+
     if anatomical_entities:
         location_summary(neurons, _noloc_query_services, anatent_simple)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `neurondm-0.1.6/docs/neurons_notebook.md` & `neurondm-0.1.7/docs/neurons_notebook.md`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/docs/types.org` & `neurondm-0.1.7/docs/types.org`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/neurondm/build.py` & `neurondm-0.1.7/neurondm/build.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/neurondm/core.py` & `neurondm-0.1.7/neurondm/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -519,20 +519,33 @@
 
         sco = self(rdfs.subClassOf, depth=2, asTerm=True)
         uris = [t.URIRef for t in sco]
         if ilxtr.PhenotypeIndicator in uris:
             if uris[0] == ilxtr.PhenotypeIndicator:
                 return self
 
-            ind = sco[0]
-            # FIXME it being first is by accident of implementation only
-            log.debug(f'{sco} {self}')
-            assert ind.predicates['rdfs:subClassOf']
-            assert ilxtr.PhenotypeIndicator == rdflib.URIRef(ind.predicates['rdfs:subClassOf'][0].iri)
-            self._cache_ind[self] = ind
+            done = False
+            for ind in sco:
+                if ind.URIRef == ilxtr.PhenotypeIndicator:
+                    continue
+                elif ind.predicates and ind.predicates['rdfs:subClassOf']:
+                    for _sco in ind.predicates['rdfs:subClassOf']:
+                        if _sco.URIRef == ilxtr.PhenotypeIndicator:
+                            done = True
+                            self._cache_ind[self] = ind
+                            break
+
+                    if done:
+                        break
+
+                else:
+                    msg = f'missing predicates {ind}'
+                    log.debug(msg)
+
+            assert done
             return ind
         else:
             self._cache_ind[self] = self  # avoid repeated lookup cost which is quite high
             if (self.prefix in ('UBERON', 'PATO', 'FMA', 'ilxtr')):
                 pass
             else:
                 log.debug(f'No indicator for {self.curie} {self.label}')
```

### Comparing `neurondm-0.1.6/neurondm/example.py` & `neurondm-0.1.7/neurondm/example.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/neurondm/indicators.py` & `neurondm-0.1.7/neurondm/indicators.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/neurondm/lang.py` & `neurondm-0.1.7/neurondm/lang.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/neurondm/models/README.md` & `neurondm-0.1.7/neurondm/models/README.md`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/neurondm/models/allen_cell_types.py` & `neurondm-0.1.7/neurondm/models/allen_cell_types.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/neurondm/models/allen_type_specimen_mapping.py` & `neurondm-0.1.7/neurondm/models/allen_type_specimen_mapping.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/neurondm/models/apinat_npo.py` & `neurondm-0.1.7/neurondm/models/apinat_npo.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/neurondm/models/apinat_pops_more.py` & `neurondm-0.1.7/neurondm/models/apinat_pops_more.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/neurondm/models/basic_neurons.py` & `neurondm-0.1.7/neurondm/models/basic_neurons.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/neurondm/models/bolew.py` & `neurondm-0.1.7/neurondm/models/bolew.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/neurondm/models/cuts.py` & `neurondm-0.1.7/neurondm/models/cuts.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/neurondm/models/huang2017.py` & `neurondm-0.1.7/neurondm/models/huang2017.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/neurondm/models/keast2020.py` & `neurondm-0.1.7/neurondm/models/keast2020.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/neurondm/models/ma2015.py` & `neurondm-0.1.7/neurondm/models/ma2015.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/neurondm/models/nerves.py` & `neurondm-0.1.7/neurondm/models/nerves.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/neurondm/models/nlp.py` & `neurondm-0.1.7/neurondm/models/nlp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 from collections import defaultdict
+from urllib.parse import quote as url_quote
 import rdflib
 from pyontutils.sheets import Sheet
 from pyontutils.namespaces import ilxtr, TEMP, rdfs, skos, owl, interlex_namespace
 from neurondm.core import Config, NeuronEBM, Phenotype, NegPhenotype, log, OntId, add_partial_orders
 from neurondm import orders
 
 
@@ -16,22 +17,32 @@
     name = 'off-nlp-1'
 
 
 class NLP2(Sheet):
     name = 'off-nlp-2'
 
 
+class NLPSemVes(Sheet):
+    name = 'off-nlp-il-semves'
+
+
+class NLPProst(Sheet):
+    name = 'off-nlp-il-prostate'
+
+
 def nlp_ns(name):
     return rdflib.Namespace(interlex_namespace(f'tgbugs/uris/readable/sparc-nlp/{name}/'))
 
 
 snames = {
     'MM Set 1': (NLP1, nlp_ns('mmset1')),
     'MM Set 2 Cranial Nerves': (NLP1, nlp_ns('mmset2cn')),
     'MM Set 4': (NLP2, nlp_ns('mmset4')),
+    'Seminal Vesicles': (NLPSemVes, nlp_ns('semves')),
+    'Prostate': (NLPProst, nlp_ns('prostate')),
 }
 
 
 sheet_classes = [
     type(f'{base.__name__}{sname.replace(" ", "_")}',
          (base,), dict(sheet_name=sname))
     for sname, (base, ns) in snames.items()]
@@ -82,39 +93,51 @@
              ]
 
     to_add = []
 
     def vl(meth):
         return rdflib.Literal(meth().value)
 
-    def asdf(s, p, rm):
+    def asdf(s, p, rm, split=False, rdf_type=rdflib.Literal):
         v = vl(rm)
         if v:
             # XXX watch out for non-homogenous subject types
             # (e.g. OntId vs rdflib.URIRef)
-            to_add.append((s.u, p, v))
+            if split:
+                for _v in v.split(split):
+                    to_add.append((s.u, p, rdf_type(_v.strip())))
+            else:
+                to_add.append((s.u, p, v))
+
+    def lcc(uri_or_curie):
+        if '<' in uri_or_curie:
+            # see pyontutils.utils_extra check_value
+            return rdflib.URIRef(url_quote(uri_or_curie, ':/;()'))
+        else:
+            return OntId(uri_or_curie).u
 
     dd = defaultdict(list)
     ec = {}
     for cl in cs:
         _, nlpns = snames[cl.sheet_name]
         for r in cl.rows():
             if (r.row_index > 0 and
                 r.id().value and
                 r.proposed_action().value.lower() != "don't add"):
                 # extra trips
                 #print(repr(r.id()))
                 s = OntId(nlpns[r.id().value])
                 #print(s)
                 asdf(s, ilxtr.sentenceNumber, r.sentence_number)
-                asdf(s, ilxtr.curatorNote, r.different_from_existing)
+                if hasattr(r, 'different_from_existing'):
+                    asdf(s, ilxtr.curatorNote, r.different_from_existing)
                 asdf(s, ilxtr.curatorNote, r.curation_notes)
                 asdf(s, ilxtr.reviewNote, r.review_notes)
                 asdf(s, ilxtr.reference, r.reference_pubmed_id__doi_or_text)
-                asdf(s, ilxtr.literatureCitation, r.literature_citation)
+                asdf(s, ilxtr.literatureCitation, r.literature_citation, split=',', rdf_type=lcc)
                 asdf(s, rdfs.label, r.neuron_population_label_a_to_b_via_c)
                 if hasattr(r, 'alert_explanation'):
                     asdf(s, ilxtr.alertNote, r.alert_explanation)
 
                 if hasattr(r, 'explicit_complement') and r.explicit_complement().value:
                     p = map_predicates(r.relationship().value)
                     o = OntId(r.explicit_complement().value)
@@ -173,14 +196,16 @@
         if False and eff(n):
             n._sigh()  # XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX FIXME figure out why this is not getting called internally
             sigh.append(n)
 
         nrns.append(n)
 
     Phenotype.in_graph.bind('mmset4', snames['MM Set 4'][-1])  # XXX FIXME UGH
+    Phenotype.in_graph.bind('semves', snames['Seminal Vesicles'][-1])
+    Phenotype.in_graph.bind('prostate', snames['Prostate'][-1])
     config.write()
     labels = (
         #ilxtr.genLabel,
         ilxtr.localLabel, ilxtr.simpleLabel,
         ilxtr.simpleLocalLabel, rdfs.label, skos.prefLabel)
     to_remove = [t for t in config._written_graph if t[1] in labels]
     [config._written_graph.remove(t) for t in to_remove]
```

### Comparing `neurondm-0.1.6/neurondm/models/pcl.py` & `neurondm-0.1.7/neurondm/models/pcl.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/neurondm/models/phenotype_direct.py` & `neurondm-0.1.7/neurondm/models/phenotype_direct.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/neurondm/phenotype_namespaces.py` & `neurondm-0.1.7/neurondm/phenotype_namespaces.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/neurondm/sheets.py` & `neurondm-0.1.7/neurondm/sheets.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/neurondm/simple.py` & `neurondm-0.1.7/neurondm/simple.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/neurondm.egg-info/PKG-INFO` & `neurondm-0.1.7/neurondm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurondm
-Version: 0.1.6
+Version: 0.1.7
 Summary: A data model for neuron types.
 Home-page: https://github.com/tgbugs/pyontutils/tree/master/neurondm
 Author: Tom Gillespie
 Author-email: tgbugs@gmail.com
 License: MIT
 Keywords: neuron types NIF ontology neuroscience phenotype OWL rdf rdflib data model
 Classifier: Development Status :: 4 - Beta
```

### Comparing `neurondm-0.1.6/neurondm.egg-info/SOURCES.txt` & `neurondm-0.1.7/neurondm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/resources/part-of-self.ttl` & `neurondm-0.1.7/resources/part-of-self.ttl`

 * *Files 1% similar despite different names*

```diff
@@ -481,14 +481,18 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0793336 ] .
 
 ILX:0793357 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0793357 ] .
 
+ILX:0793358 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793358 ] .
+
 ILX:0793359 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0793359 ] .
 
 ILX:0793360 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0793360 ] .
@@ -829,14 +833,46 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0793833 ] .
 
 ILX:0793834 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0793834 ] .
 
+ILX:0793877 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793877 ] .
+
+ILX:0793878 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793878 ] .
+
+ILX:0793879 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793879 ] .
+
+ILX:0793880 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793880 ] .
+
+ILX:0793881 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793881 ] .
+
+ILX:0793882 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793882 ] .
+
+ILX:0793883 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793883 ] .
+
+ILX:0793884 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793884 ] .
+
 MBA:33 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom MBA:33 ] .
 
 MBA:41 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom MBA:41 ] .
@@ -1181,14 +1217,18 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0000396 ] .
 
 UBERON:0000411 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0000411 ] .
 
+UBERON:0000428 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0000428 ] .
+
 UBERON:0000468 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0000468 ] .
 
 UBERON:0000929 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0000929 ] .
@@ -1217,14 +1257,18 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0000988 ] .
 
 UBERON:0000992 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0000992 ] .
 
+UBERON:0000998 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0000998 ] .
+
 UBERON:0001043 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0001043 ] .
 
 UBERON:0001051 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0001051 ] .
@@ -1609,14 +1653,18 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0002009 ] .
 
 UBERON:0002012 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0002012 ] .
 
+UBERON:0002013 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0002013 ] .
+
 UBERON:0002014 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0002014 ] .
 
 UBERON:0002019 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0002019 ] .
@@ -2225,18 +2273,26 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0004133 ] .
 
 UBERON:0004186 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0004186 ] .
 
+UBERON:0004243 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0004243 ] .
+
 UBERON:0004641 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0004641 ] .
 
+UBERON:0004665 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0004665 ] .
+
 UBERON:0004676 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0004676 ] .
 
 UBERON:0004679 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0004679 ] .
@@ -2249,14 +2305,18 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0004713 ] .
 
 UBERON:0004789 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0004789 ] .
 
+UBERON:0004805 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0004805 ] .
+
 UBERON:0004917 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0004917 ] .
 
 UBERON:0004982 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0004982 ] .
@@ -2417,14 +2477,26 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0006459 ] .
 
 UBERON:0006460 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0006460 ] .
 
+UBERON:0006461 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0006461 ] .
+
+UBERON:0006462 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0006462 ] .
+
+UBERON:0006463 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0006463 ] .
+
 UBERON:0006465 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0006465 ] .
 
 UBERON:0006466 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0006466 ] .
@@ -2733,14 +2805,22 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0011327 ] .
 
 UBERON:0011390 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0011390 ] .
 
+UBERON:0011926 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0011926 ] .
+
+UBERON:0011929 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0011929 ] .
+
 UBERON:0012170 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0012170 ] .
 
 UBERON:0012171 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0012171 ] .
@@ -3005,14 +3085,18 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0035642 ] .
 
 UBERON:0035647 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0035647 ] .
 
+UBERON:0035770 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0035770 ] .
+
 UBERON:0035772 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0035772 ] .
 
 UBERON:0035971 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0035971 ] .
```

### Comparing `neurondm-0.1.6/resources/phenotype-core.ttl` & `neurondm-0.1.7/resources/phenotype-core.ttl`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/resources/phenotype-indicators.ttl` & `neurondm-0.1.7/resources/phenotype-indicators.ttl`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/resources/phenotypes.ttl` & `neurondm-0.1.7/resources/phenotypes.ttl`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/setup.py` & `neurondm-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/test/common.py` & `neurondm-0.1.7/test/common.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/test/test_integration.py` & `neurondm-0.1.7/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/test/test_label.py` & `neurondm-0.1.7/test/test_label.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/test/test_madness.py` & `neurondm-0.1.7/test/test_madness.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/test/test_neurons.py` & `neurondm-0.1.7/test/test_neurons.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/test/test_simple.py` & `neurondm-0.1.7/test/test_simple.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/test/test_triples.py` & `neurondm-0.1.7/test/test_triples.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.6/test/test_write.py` & `neurondm-0.1.7/test/test_write.py`

 * *Files identical despite different names*

