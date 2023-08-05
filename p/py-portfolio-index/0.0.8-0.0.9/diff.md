# Comparing `tmp/py-portfolio-index-0.0.8.tar.gz` & `tmp/py-portfolio-index-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-portfolio-index-0.0.8.tar", last modified: Sat Jun 24 19:17:41 2023, max compression
+gzip compressed data, was "py-portfolio-index-0.0.9.tar", last modified: Sun Jul  2 21:51:31 2023, max compression
```

## Comparing `py-portfolio-index-0.0.8.tar` & `py-portfolio-index-0.0.9.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:17:41.001037 py-portfolio-index-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-24 19:17:41.001037 py-portfolio-index-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:17:40.993037 py-portfolio-index-0.0.8/py_portfolio_index/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:17:40.993037 py-portfolio-index-0.0.8/py_portfolio_index/bin/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:17:40.997037 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22537 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/esgv_2020_q4.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/esgv_2021_q4.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/esgv_2022_q2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/esgv_2022_q3.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/esgv_2022_q4.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/esgv_2023_q1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/qcln_2020_q4.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/sp500_2023_q3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    55272 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/vtsmx_2020_q4.csv
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/yolo_gme_2023_q1.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:17:41.001037 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/coal.csv
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/cruises.csv
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/fake_meat.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/meat_poultry.csv
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/non_ethical_conduct.csv
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/oil.csv
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/renewable.csv
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/semiconductor.csv
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/space.csv
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/vice.csv
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:17:41.001037 py-portfolio-index-0.0.8/py_portfolio_index/portfolio_providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/portfolio_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/portfolio_providers/alpaca.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/portfolio_providers/alpaca_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/portfolio_providers/base_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/portfolio_providers/local_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/portfolio_providers/robinhood.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:17:40.993037 py-portfolio-index-0.0.8/py_portfolio_index.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-24 19:17:40.000000 py-portfolio-index-0.0.8/py_portfolio_index.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-24 19:17:40.000000 py-portfolio-index-0.0.8/py_portfolio_index.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 19:17:40.000000 py-portfolio-index-0.0.8/py_portfolio_index.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-24 19:17:40.000000 py-portfolio-index-0.0.8/py_portfolio_index.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-24 19:17:40.000000 py-portfolio-index-0.0.8/py_portfolio_index.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 19:17:41.001037 py-portfolio-index-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:51:31.603463 py-portfolio-index-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-02 21:51:31.603463 py-portfolio-index-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:51:31.595463 py-portfolio-index-0.0.9/py_portfolio_index/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:51:31.595463 py-portfolio-index-0.0.9/py_portfolio_index/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:51:31.599463 py-portfolio-index-0.0.9/py_portfolio_index/bin/indexes/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/indexes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22537 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/indexes/esgv_2020_q4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/indexes/esgv_2021_q4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/indexes/esgv_2022_q2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/indexes/esgv_2022_q3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/indexes/esgv_2022_q4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/indexes/esgv_2023_q1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/indexes/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/indexes/qcln_2020_q4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/indexes/sp500_2023_q3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    55272 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/indexes/vtsmx_2020_q4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/indexes/yolo_gme_2023_q3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/indexes/yolo_wf_2023_q1.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:51:31.599463 py-portfolio-index-0.0.9/py_portfolio_index/bin/lists/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/lists/coal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/lists/cruises.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/lists/fake_meat.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/lists/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/lists/meat_poultry.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/lists/non_ethical_conduct.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/lists/oil.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/lists/renewable.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/lists/semiconductor.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/lists/space.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/bin/lists/vice.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:51:31.603463 py-portfolio-index-0.0.9/py_portfolio_index/portfolio_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/portfolio_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/portfolio_providers/alpaca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/portfolio_providers/alpaca_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/portfolio_providers/base_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/portfolio_providers/local_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10851 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/portfolio_providers/robinhood.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/py_portfolio_index/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:51:31.595463 py-portfolio-index-0.0.9/py_portfolio_index.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-02 21:51:31.000000 py-portfolio-index-0.0.9/py_portfolio_index.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-02 21:51:31.000000 py-portfolio-index-0.0.9/py_portfolio_index.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 21:51:31.000000 py-portfolio-index-0.0.9/py_portfolio_index.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-02 21:51:31.000000 py-portfolio-index-0.0.9/py_portfolio_index.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-02 21:51:31.000000 py-portfolio-index-0.0.9/py_portfolio_index.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 21:51:31.603463 py-portfolio-index-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-02 21:51:17.000000 py-portfolio-index-0.0.9/setup.py
```

### Comparing `py-portfolio-index-0.0.8/LICENSE.txt` & `py-portfolio-index-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.8/PKG-INFO` & `py-portfolio-index-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-portfolio-index
-Version: 0.0.8
+Version: 0.0.9
 Summary: Build index portfolios.
 Home-page: 
 Author: 
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `py-portfolio-index-0.0.8/README.md` & `py-portfolio-index-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.8/py_portfolio_index/__init__.py` & `py-portfolio-index-0.0.9/py_portfolio_index/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from py_portfolio_index.bin import INDEXES, STOCK_LISTS
 from py_portfolio_index.constants import Logger
 from py_portfolio_index.enums import PurchaseStrategy, RoundingStrategy
 from py_portfolio_index.operators import compare_portfolios, generate_order_plan
 from py_portfolio_index.portfolio_providers.alpaca import AlpacaProviderLegacy
 from py_portfolio_index.portfolio_providers.robinhood import RobinhoodProvider
-from py_portfolio_index.portfolio_providers.alpaca_v2 import AlpacaProvider
+from py_portfolio_index.portfolio_providers.alpaca_v2 import (
+    AlpacaProvider,
+    PaperAlpacaProvider,
+)
 from py_portfolio_index.config import get_providers
 
 AVAILABLE_PROVIDERS = get_providers()
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 __all__ = [
     "INDEXES",
     "STOCK_LISTS",
     "Logger",
     "compare_portfolios",
     "generate_order_plan",
+    "PaperAlpacaProvider",
     "AlpacaProvider",
     "AlpacaProviderLegacy",
     "RobinhoodProvider",
     "PurchaseStrategy",
     "RoundingStrategy",
 ]
```

### Comparing `py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/esgv_2020_q4.csv` & `py-portfolio-index-0.0.9/py_portfolio_index/bin/indexes/esgv_2020_q4.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/esgv_2021_q4.csv` & `py-portfolio-index-0.0.9/py_portfolio_index/bin/indexes/esgv_2021_q4.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/esgv_2022_q2.csv` & `py-portfolio-index-0.0.9/py_portfolio_index/bin/indexes/esgv_2022_q2.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/esgv_2022_q3.csv` & `py-portfolio-index-0.0.9/py_portfolio_index/bin/indexes/esgv_2022_q3.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/esgv_2022_q4.csv` & `py-portfolio-index-0.0.9/py_portfolio_index/bin/indexes/esgv_2022_q4.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/esgv_2023_q1.csv` & `py-portfolio-index-0.0.9/py_portfolio_index/bin/indexes/esgv_2023_q1.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/inventory.py` & `py-portfolio-index-0.0.9/py_portfolio_index/bin/indexes/inventory.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/qcln_2020_q4.csv` & `py-portfolio-index-0.0.9/py_portfolio_index/bin/indexes/qcln_2020_q4.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/sp500_2023_q3.csv` & `py-portfolio-index-0.0.9/py_portfolio_index/bin/indexes/sp500_2023_q3.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/vtsmx_2020_q4.csv` & `py-portfolio-index-0.0.9/py_portfolio_index/bin/indexes/vtsmx_2020_q4.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/inventory.py` & `py-portfolio-index-0.0.9/py_portfolio_index/bin/lists/inventory.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/oil.csv` & `py-portfolio-index-0.0.9/py_portfolio_index/bin/lists/oil.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.8/py_portfolio_index/config.py` & `py-portfolio-index-0.0.9/py_portfolio_index/config.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.8/py_portfolio_index/models.py` & `py-portfolio-index-0.0.9/py_portfolio_index/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from datetime import datetime, date
+from datetime import date
 from typing import List, Optional, Union, TYPE_CHECKING
 from pydantic import BaseModel, Field, validator
-from pandas import DataFrame
 from py_portfolio_index.enums import Currency
 from py_portfolio_index.constants import Logger
 from py_portfolio_index.exceptions import PriceFetchError
 from decimal import Decimal
 from enum import Enum
 
 if TYPE_CHECKING:
@@ -14,18 +13,18 @@
 
 class Money(BaseModel):
     value: Union[Decimal, int, float, "Money"]
     currency: Currency = Currency.USD
 
     @property
     def decimal(self) -> Decimal:
-        return self.value #type: ignore
-    
+        return self.value  # type: ignore
+
     @validator("value", pre=True)
-    def coerce_to_decimal(cls, v)-> Decimal:
+    def coerce_to_decimal(cls, v) -> Decimal:
         if isinstance(v, (int, float)):
             return Decimal(v)
         elif isinstance(v, Money):
             # TODO convert this
             return v.decimal
         elif isinstance(v, Decimal):
             return v
@@ -127,22 +126,22 @@
         for item in self.holdings:
             item.weight = item.weight * scaling_factor
 
     def exclude(self, exclusion_list: List[str]):
         reweighted = []
         excluded = Decimal(0.0)
         for ticker in exclusion_list:
-            reweighted.append(ticker)
             for item in self.holdings:
                 if item.ticker == ticker:
+                    reweighted.append(ticker)
                     excluded += item.weight
                     item.weight = Decimal(0.0)
 
         self.holdings = [
-            item for item in self.holdings if item.ticker not in reweighted
+            item for item in self.holdings if item.ticker not in exclusion_list
         ]
         self._reweight_portfolio()
         Logger.info(
             f"Set the following stocks to weight 0 {reweighted}. Total value excluded {excluded}."
         )
         return self
 
@@ -166,57 +165,63 @@
                     found = True
             if not found:
                 reweighted.append(ticker)
                 total_value += cmin_weight
                 self.holdings.append(
                     IdealPortfolioElement(ticker=ticker, weight=cmin_weight)
                 )
-            
+
         self._reweight_portfolio()
         Logger.info(
             f"modified the following by weight {cweight} {reweighted}. Total value modified {total_value}."
         )
         return self
 
-    def reweight_to_present(self, provider: "BaseProvider"):
+    def reweight_to_present(self, provider: "BaseProvider") -> dict:
+        output = {}
         imaginary_base = Decimal(1_000_000)
         values = {}
+        if provider.SUPPORTS_BATCH_HISTORY:
+            tickers = [item.ticker for item in self.holdings]
+            historic_prices = provider.get_instrument_prices(tickers, self.source_date)
+            today_prices = provider.get_instrument_prices(tickers, None)
+        else:
+            historic_prices = {}
+            today_prices = {}
+            for item in self.holdings:
+                try:
+                    historic_prices[item.ticker] = provider.get_instrument_price(
+                        item.ticker, self.source_date
+                    )
+                    today_prices[item.ticker] = provider.get_instrument_price(
+                        item.ticker
+                    )
+                except PriceFetchError:
+                    historic_prices[item.ticker] = None
+                    today_prices[item.ticker] = None
         for item in self.holdings:
-            try:
-                source_price = provider.get_instrument_price(
-                    item.ticker, self.source_date
-                )
-            except PriceFetchError:
-                source_price = provider.get_instrument_price(item.ticker)
-            today_price = provider.get_instrument_price(item.ticker)
+            source_price = historic_prices.get(item.ticker, None)
+            today_price = today_prices.get(item.ticker, None)
             if not source_price or not today_price:
                 # if we couldn't get a historical price
                 # keep the value the same
                 values[item.ticker] = imaginary_base * item.weight
                 continue
             source_shares = imaginary_base * item.weight / source_price
-
-            today_value = today_price * source_shares
-            values[item.ticker] = today_value
+            stock_value_today = today_price * source_shares
+            values[item.ticker] = stock_value_today
         today_value = Decimal(sum(values.values()))
 
         for item in self.holdings:
             new_weight = values[item.ticker] / today_value
+            ratio = round(((new_weight - item.weight) / item.weight) * 100, 2)
+            output[item.ticker] = ratio
             item.weight = new_weight
         self._reweight_portfolio()
-
-    def produce_tear_sheet_from_date(self, datetime: datetime):
-        raise NotImplementedError
-        import pyfolio
-
-        columns = ["date"] + [item.ticker for item in self.holdings]
-        values = [datetime] + [item.value for item in self.holdings]
-        df = DataFrame([values], columns=columns)
-        df.set_index(keys=["date"], drop=True)
-        pyfolio.create_simple_tear_sheet(positions=df, live_start_date=datetime)
+        return output
 
 
 class RealPortfolioElement(IdealPortfolioElement):
     ticker: str
     units: Decimal
     value: Money
     weight: Decimal = Decimal(0.0)
```

### Comparing `py-portfolio-index-0.0.8/py_portfolio_index/operators.py` & `py-portfolio-index-0.0.9/py_portfolio_index/operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from py_portfolio_index.enums import PurchaseStrategy, RoundingStrategy
 from py_portfolio_index.models import Money, OrderElement, OrderPlan, OrderType
 from .models import IdealPortfolio, RealPortfolio
 
 MIN_ORDER_SIZE = 2
 MIN_ORDER_MONEY = Money(value=MIN_ORDER_SIZE)
 
+
 @dataclass
 class ComparisonResult:
     ticker: str
     model: Decimal
     comparison: Decimal
     actual: Money
 
@@ -185,16 +186,16 @@
                 target_value * diffvalue.comparison - target_value * diffvalue.model
             )
             if buy_order == PurchaseStrategy.PEANUT_BUTTER:
                 sell_target = sell_target * scaling_factor
             # if not fractional_shares:
             #     price = real.get_instrument_price(key)
             #     qty = round_with_strategy(target/price, rounding_strategy)
-            #     target = 
-            sell_target = max(sell_target, MIN_ORDER_MONEY )
+            #     target =
+            sell_target = max(sell_target, MIN_ORDER_MONEY)
             to_sell.append(
                 OrderElement(
                     ticker=key, value=sell_target, order_type=OrderType.SELL, qty=None
                 )
             )
             #     target_value * diffvalue.comparison - target_value * diffvalue.model
             # )
@@ -216,15 +217,15 @@
             if buy_order == PurchaseStrategy.PEANUT_BUTTER:
                 if buy_target > 0.0:
                     max_value: Decimal = max(
                         Decimal(float(buy_target.value)) * scaling_factor.decimal,
                         Decimal(1.0),
                     )
                     buy_target = Money(value=max_value)
-            buy_target = max(buy_target, min_order_value )
+            buy_target = max(buy_target, min_order_value)
             to_purchase.append(
                 OrderElement(
                     ticker=key, value=buy_target, qty=None, order_type=OrderType.BUY
                 )
             )
             purchase_power = purchase_power - buy_target
```

### Comparing `py-portfolio-index-0.0.8/py_portfolio_index/portfolio_providers/alpaca.py` & `py-portfolio-index-0.0.9/py_portfolio_index/portfolio_providers/alpaca.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.8/py_portfolio_index/portfolio_providers/base_portfolio.py` & `py-portfolio-index-0.0.9/py_portfolio_index/portfolio_providers/base_portfolio.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,40 @@
 from math import floor, ceil
-from typing import Dict, Union, Optional, Set
+from typing import Dict, Union, Optional, Set, List
 from decimal import Decimal
 from datetime import date
 
 from py_portfolio_index.common import print_money, print_per, round_up_to_place
 from py_portfolio_index.constants import Logger
 from py_portfolio_index.enums import RoundingStrategy
 from py_portfolio_index.exceptions import PriceFetchError
 from py_portfolio_index.models import Money, OrderPlan
 from functools import lru_cache
+from py_portfolio_index.models import RealPortfolio
 
 
 class BaseProvider(object):
     MIN_ORDER_VALUE = Money(value=1)
     MAX_ORDER_DECIMALS = 2
-    
+    SUPPORTS_BATCH_HISTORY = 0
+
     def _get_instrument_price(self, ticker: str, at_day: Optional[date] = None):
         raise NotImplementedError
 
+    def get_holdings(self) -> RealPortfolio:
+        raise NotImplementedError
+
+    def get_instrument_prices(
+        self, tickers: List[str], at_day: Optional[date] = None
+    ) -> Dict[str, Optional[Decimal]]:
+        output = {}
+        for ticker in tickers:
+            output[ticker] = self.get_instrument_price(ticker, at_day=at_day)
+        return output
+
     @lru_cache(maxsize=None)
     def get_instrument_price(
         self, ticker: str, at_day: Optional[date] = None
     ) -> Optional[Decimal]:
         try:
             return self._get_instrument_price(ticker, at_day)
         except NotImplementedError as e:
@@ -128,15 +141,15 @@
         )
 
     def purchase_order_plan(
         self,
         plan: OrderPlan,
         skip_errored_stocks=False,
         ignore_unsettled: bool = True,
-        plan_only:bool = False
+        plan_only: bool = False,
     ):
         if ignore_unsettled:
             unsettled = self.get_unsettled_instruments()
         else:
             unsettled = set()
         for item in plan.to_buy:
             if item.ticker in unsettled:
@@ -156,15 +169,17 @@
                     price: Money = Money(value=raw_price)
                     Logger.info(f"got price of {price} for {item.ticker}")
                 except Exception as e:
                     if not skip_errored_stocks:
                         raise e
                     else:
                         continue
-                units = round_up_to_place((item.value/price).value, self.MAX_ORDER_DECIMALS)
+                units = round_up_to_place(
+                    (item.value / price).value, self.MAX_ORDER_DECIMALS
+                )
             else:
                 raise ValueError("Order element must have qty or value")
             try:
                 if not plan_only:
                     self.buy_instrument(item.ticker, units)
                     Logger.info(f"Bought {units} of {item.ticker}")
                 else:
```

### Comparing `py-portfolio-index-0.0.8/py_portfolio_index/portfolio_providers/local_dict.py` & `py-portfolio-index-0.0.9/py_portfolio_index/portfolio_providers/local_dict.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.8/py_portfolio_index.egg-info/PKG-INFO` & `py-portfolio-index-0.0.9/py_portfolio_index.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-portfolio-index
-Version: 0.0.8
+Version: 0.0.9
 Summary: Build index portfolios.
 Home-page: 
 Author: 
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `py-portfolio-index-0.0.8/py_portfolio_index.egg-info/SOURCES.txt` & `py-portfolio-index-0.0.9/py_portfolio_index.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 py_portfolio_index/bin/indexes/esgv_2022_q3.csv
 py_portfolio_index/bin/indexes/esgv_2022_q4.csv
 py_portfolio_index/bin/indexes/esgv_2023_q1.csv
 py_portfolio_index/bin/indexes/inventory.py
 py_portfolio_index/bin/indexes/qcln_2020_q4.csv
 py_portfolio_index/bin/indexes/sp500_2023_q3.csv
 py_portfolio_index/bin/indexes/vtsmx_2020_q4.csv
-py_portfolio_index/bin/indexes/yolo_gme_2023_q1.csv
+py_portfolio_index/bin/indexes/yolo_gme_2023_q3.csv
+py_portfolio_index/bin/indexes/yolo_wf_2023_q1.csv
 py_portfolio_index/bin/lists/__init__.py
 py_portfolio_index/bin/lists/coal.csv
 py_portfolio_index/bin/lists/cruises.csv
 py_portfolio_index/bin/lists/fake_meat.csv
 py_portfolio_index/bin/lists/inventory.py
 py_portfolio_index/bin/lists/meat_poultry.csv
 py_portfolio_index/bin/lists/non_ethical_conduct.csv
```

### Comparing `py-portfolio-index-0.0.8/setup.py` & `py-portfolio-index-0.0.9/setup.py`

 * *Files identical despite different names*

