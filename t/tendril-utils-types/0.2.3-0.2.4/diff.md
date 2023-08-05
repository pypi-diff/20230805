# Comparing `tmp/tendril-utils-types-0.2.3.tar.gz` & `tmp/tendril-utils-types-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-utils-types-0.2.3.tar", last modified: Sat Aug  5 15:26:24 2023, max compression
+gzip compressed data, was "tendril-utils-types-0.2.4.tar", last modified: Sat Aug  5 20:50:13 2023, max compression
```

## Comparing `tendril-utils-types-0.2.3.tar` & `tendril-utils-types-0.2.4.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 15:26:24.000186 tendril-utils-types-0.2.3/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2120 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3555 2023-08-05 15:26:24.000186 tendril-utils-types-0.2.3/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2256 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 15:26:23.992188 tendril-utils-types-0.2.3/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 15:26:23.996187 tendril-utils-types-0.2.3/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 15:26:23.996187 tendril-utils-types-0.2.3/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 15:26:23.996187 tendril-utils-types-0.2.3/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      669 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       95 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/docs/api/tendril.config.types.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      178 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/docs/api/tendril.utils.types.cartesian.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      177 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/docs/api/tendril.utils.types.currency.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      196 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/docs/api/tendril.utils.types.electromagnetic.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      172 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/docs/api/tendril.utils.types.lengths.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      181 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/docs/api/tendril.utils.types.signalbase.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      190 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/docs/api/tendril.utils.types.thermodynamic.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      163 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/docs/api/tendril.utils.types.time.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      177 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/docs/api/tendril.utils.types.unitbase.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1078 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1672 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 15:26:23.996187 tendril-utils-types-0.2.3/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-08-05 15:26:24.004185 tendril-utils-types-0.2.3/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3293 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 15:26:23.992188 tendril-utils-types-0.2.3/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 15:26:23.996187 tendril-utils-types-0.2.3/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:08:45.000000 tendril-utils-types-0.2.3/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 15:26:23.996187 tendril-utils-types-0.2.3/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1055 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/src/tendril/config/types.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 15:26:23.996187 tendril-utils-types-0.2.3/src/tendril/utils/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:09:00.000000 tendril-utils-types-0.2.3/src/tendril/utils/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 15:26:24.000186 tendril-utils-types-0.2.3/src/tendril/utils/types/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5027 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/src/tendril/utils/types/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2804 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/src/tendril/utils/types/cartesian.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    16522 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/src/tendril/utils/types/currency.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3502 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/src/tendril/utils/types/electromagnetic.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2742 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/src/tendril/utils/types/lengths.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1069 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/src/tendril/utils/types/mass.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      283 2023-07-29 07:46:30.000000 tendril-utils-types-0.2.3/src/tendril/utils/types/memory.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     8689 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/src/tendril/utils/types/signalbase.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1475 2023-08-05 15:03:39.000000 tendril-utils-types-0.2.3/src/tendril/utils/types/thermodynamic.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7725 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/src/tendril/utils/types/time.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    19190 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/src/tendril/utils/types/unitbase.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 15:26:24.000186 tendril-utils-types-0.2.3/src/tendril_utils_types.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3555 2023-08-05 15:26:23.000000 tendril-utils-types-0.2.3/src/tendril_utils_types.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1711 2023-08-05 15:26:23.000000 tendril-utils-types-0.2.3/src/tendril_utils_types.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-08-05 15:26:23.000000 tendril-utils-types-0.2.3/src/tendril_utils_types.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      615 2023-08-05 15:26:23.000000 tendril-utils-types-0.2.3/src/tendril_utils_types.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-08-05 15:26:23.000000 tendril-utils-types-0.2.3/src/tendril_utils_types.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 15:26:24.000186 tendril-utils-types-0.2.3/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2562 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/tests/test_utils_types_cartesian.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4316 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/tests/test_utils_types_currency.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2305 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/tests/test_utils_types_thermodynamic.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4187 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/tests/test_utils_types_time.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5797 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/tests/test_utils_types_unitbase.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      831 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.3/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:50:13.312831 tendril-utils-types-0.2.4/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2120 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3555 2023-08-05 20:50:13.312831 tendril-utils-types-0.2.4/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2256 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:50:13.304832 tendril-utils-types-0.2.4/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:50:13.304832 tendril-utils-types-0.2.4/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:50:13.304832 tendril-utils-types-0.2.4/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:50:13.308832 tendril-utils-types-0.2.4/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      669 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       95 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/docs/api/tendril.config.types.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      178 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/docs/api/tendril.utils.types.cartesian.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      177 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/docs/api/tendril.utils.types.currency.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      196 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/docs/api/tendril.utils.types.electromagnetic.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      172 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/docs/api/tendril.utils.types.lengths.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      181 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/docs/api/tendril.utils.types.signalbase.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      190 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/docs/api/tendril.utils.types.thermodynamic.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      163 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/docs/api/tendril.utils.types.time.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      177 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/docs/api/tendril.utils.types.unitbase.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1078 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1672 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:50:13.308832 tendril-utils-types-0.2.4/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-08-05 20:50:13.312831 tendril-utils-types-0.2.4/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3293 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:50:13.300832 tendril-utils-types-0.2.4/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:50:13.308832 tendril-utils-types-0.2.4/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:08:45.000000 tendril-utils-types-0.2.4/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:50:13.308832 tendril-utils-types-0.2.4/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1055 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/src/tendril/config/types.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:50:13.308832 tendril-utils-types-0.2.4/src/tendril/utils/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:09:00.000000 tendril-utils-types-0.2.4/src/tendril/utils/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:50:13.308832 tendril-utils-types-0.2.4/src/tendril/utils/types/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5027 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/src/tendril/utils/types/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2804 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/src/tendril/utils/types/cartesian.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    16522 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/src/tendril/utils/types/currency.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3502 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/src/tendril/utils/types/electromagnetic.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2742 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/src/tendril/utils/types/lengths.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1069 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/src/tendril/utils/types/mass.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      283 2023-07-29 07:46:30.000000 tendril-utils-types-0.2.4/src/tendril/utils/types/memory.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     8689 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/src/tendril/utils/types/signalbase.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1475 2023-08-05 15:03:39.000000 tendril-utils-types-0.2.4/src/tendril/utils/types/thermodynamic.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7725 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/src/tendril/utils/types/time.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    19262 2023-08-05 18:03:30.000000 tendril-utils-types-0.2.4/src/tendril/utils/types/unitbase.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:50:13.312831 tendril-utils-types-0.2.4/src/tendril_utils_types.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3555 2023-08-05 20:50:13.000000 tendril-utils-types-0.2.4/src/tendril_utils_types.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1711 2023-08-05 20:50:13.000000 tendril-utils-types-0.2.4/src/tendril_utils_types.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-08-05 20:50:13.000000 tendril-utils-types-0.2.4/src/tendril_utils_types.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      615 2023-08-05 20:50:13.000000 tendril-utils-types-0.2.4/src/tendril_utils_types.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-08-05 20:50:13.000000 tendril-utils-types-0.2.4/src/tendril_utils_types.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-05 20:50:13.312831 tendril-utils-types-0.2.4/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2562 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/tests/test_utils_types_cartesian.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4316 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/tests/test_utils_types_currency.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2305 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/tests/test_utils_types_thermodynamic.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4187 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/tests/test_utils_types_time.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5797 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/tests/test_utils_types_unitbase.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      831 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.4/tox.ini
```

### Comparing `tendril-utils-types-0.2.3/.gitignore` & `tendril-utils-types-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/.readthedocs.yml` & `tendril-utils-types-0.2.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/.travis.yml` & `tendril-utils-types-0.2.4/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/LICENSE` & `tendril-utils-types-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/PKG-INFO` & `tendril-utils-types-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-utils-types
-Version: 0.2.3
+Version: 0.2.4
 Summary: Type classes for tendril
 Home-page: https://github.com/tendril-framework/tendril-utils-types
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-utils-types.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-utils-types/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-utils-types
```

### Comparing `tendril-utils-types-0.2.3/README.rst` & `tendril-utils-types-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/docs/Makefile` & `tendril-utils-types-0.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/docs/_static/custom.css` & `tendril-utils-types-0.2.4/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/docs/_static/favicon.ico` & `tendril-utils-types-0.2.4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/docs/_static/logo.png` & `tendril-utils-types-0.2.4/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/docs/_static/logo_packed.png` & `tendril-utils-types-0.2.4/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/docs/_templates/about.html` & `tendril-utils-types-0.2.4/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/docs/api/index.rst` & `tendril-utils-types-0.2.4/docs/api/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/docs/conf.py` & `tendril-utils-types-0.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/docs/index.rst` & `tendril-utils-types-0.2.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/docs/installation.rst` & `tendril-utils-types-0.2.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/setup.py` & `tendril-utils-types-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/src/tendril/config/__init__.py` & `tendril-utils-types-0.2.4/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/src/tendril/config/types.py` & `tendril-utils-types-0.2.4/src/tendril/config/types.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/src/tendril/utils/types/__init__.py` & `tendril-utils-types-0.2.4/src/tendril/utils/types/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/src/tendril/utils/types/cartesian.py` & `tendril-utils-types-0.2.4/src/tendril/utils/types/cartesian.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/src/tendril/utils/types/currency.py` & `tendril-utils-types-0.2.4/src/tendril/utils/types/currency.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/src/tendril/utils/types/electromagnetic.py` & `tendril-utils-types-0.2.4/src/tendril/utils/types/electromagnetic.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/src/tendril/utils/types/lengths.py` & `tendril-utils-types-0.2.4/src/tendril/utils/types/lengths.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/src/tendril/utils/types/mass.py` & `tendril-utils-types-0.2.4/src/tendril/utils/types/mass.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/src/tendril/utils/types/signalbase.py` & `tendril-utils-types-0.2.4/src/tendril/utils/types/signalbase.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/src/tendril/utils/types/thermodynamic.py` & `tendril-utils-types-0.2.4/src/tendril/utils/types/thermodynamic.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/src/tendril/utils/types/time.py` & `tendril-utils-types-0.2.4/src/tendril/utils/types/time.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/src/tendril/utils/types/unitbase.py` & `tendril-utils-types-0.2.4/src/tendril/utils/types/unitbase.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,14 +224,16 @@
     _has_bare_order = False
 
     _rorders = None
     _pluralize_ostr = False
     _separate_unit = False
 
     def __init__(self, value):
+        if isinstance(value, bytes):
+            value = value.decode()
         if not self._orders:
             doidx = self._ostrs.index(self._dostr)
             self._orders = [(ostr, (3 * (idx - doidx)))
                             for idx, ostr in enumerate(self._ostrs)]
             self._order_type = 0
         elif not self._ostrs:
             self._ostrs = [order[0] for order in self._orders]
```

### Comparing `tendril-utils-types-0.2.3/src/tendril_utils_types.egg-info/PKG-INFO` & `tendril-utils-types-0.2.4/src/tendril_utils_types.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-utils-types
-Version: 0.2.3
+Version: 0.2.4
 Summary: Type classes for tendril
 Home-page: https://github.com/tendril-framework/tendril-utils-types
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-utils-types.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-utils-types/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-utils-types
```

### Comparing `tendril-utils-types-0.2.3/src/tendril_utils_types.egg-info/SOURCES.txt` & `tendril-utils-types-0.2.4/src/tendril_utils_types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/src/tendril_utils_types.egg-info/requires.txt` & `tendril-utils-types-0.2.4/src/tendril_utils_types.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/tests/coveralls.py` & `tendril-utils-types-0.2.4/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/tests/test_utils_types_cartesian.py` & `tendril-utils-types-0.2.4/tests/test_utils_types_cartesian.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/tests/test_utils_types_currency.py` & `tendril-utils-types-0.2.4/tests/test_utils_types_currency.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/tests/test_utils_types_thermodynamic.py` & `tendril-utils-types-0.2.4/tests/test_utils_types_thermodynamic.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/tests/test_utils_types_time.py` & `tendril-utils-types-0.2.4/tests/test_utils_types_time.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/tests/test_utils_types_unitbase.py` & `tendril-utils-types-0.2.4/tests/test_utils_types_unitbase.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.3/tox.ini` & `tendril-utils-types-0.2.4/tox.ini`

 * *Files identical despite different names*

