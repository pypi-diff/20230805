# Comparing `tmp/psycopg-3.1.8.tar.gz` & `tmp/psycopg-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psycopg-3.1.8.tar", last modified: Mon Jan 16 22:56:49 2023, max compression
+gzip compressed data, was "psycopg-3.1.9.tar", last modified: Tue May  2 11:44:22 2023, max compression
```

## Comparing `psycopg-3.1.8.tar` & `psycopg-3.1.9.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 22:56:49.293366 psycopg-3.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-01-16 22:56:40.000000 psycopg-3.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-01-16 22:56:49.293366 psycopg-3.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-01-16 22:56:40.000000 psycopg-3.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 22:56:49.289366 psycopg-3.1.8/psycopg/
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/_adapters_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/_cmodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/_dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/_encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/_preparing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/_tpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    14440 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/_typeinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/_tz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/adapt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/client_cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)    33925 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    14212 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/connection_async.py
--rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/conninfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    29176 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/copy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 22:56:49.289366 psycopg-3.1.8/psycopg/crdb/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/crdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/crdb/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/crdb/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    30734 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/cursor_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/dbapi20.py
--rw-r--r--   0 runner    (1001) docker     (123)    40279 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 22:56:49.293366 psycopg-3.1.8/psycopg/pq/
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/pq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/pq/_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/pq/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    20061 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/pq/_pq_ctypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/pq/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/pq/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    35791 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/pq/pq_ctypes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/rows.py
--rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/server_cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15925 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 22:56:49.293366 psycopg-3.1.8/psycopg/types/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14647 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/types/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/types/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/types/composite.py
--rw-r--r--   0 runner    (1001) docker     (123)    24812 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/types/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/types/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/types/hstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/types/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/types/multirange.py
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/types/net.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/types/none.py
--rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/types/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)    20485 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/types/range.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/types/shapely.py
--rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/types/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/types/uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-01-16 22:56:40.000000 psycopg-3.1.8/psycopg/waiting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 22:56:49.289366 psycopg-3.1.8/psycopg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-01-16 22:56:49.000000 psycopg-3.1.8/psycopg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-01-16 22:56:49.000000 psycopg-3.1.8/psycopg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 22:56:49.000000 psycopg-3.1.8/psycopg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 22:56:49.000000 psycopg-3.1.8/psycopg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-01-16 22:56:49.000000 psycopg-3.1.8/psycopg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-16 22:56:49.000000 psycopg-3.1.8/psycopg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-01-16 22:56:40.000000 psycopg-3.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-01-16 22:56:49.293366 psycopg-3.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-01-16 22:56:40.000000 psycopg-3.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:44:22.052085 psycopg-3.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-02 11:44:12.000000 psycopg-3.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-02 11:44:22.052085 psycopg-3.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-02 11:44:12.000000 psycopg-3.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:44:22.048084 psycopg-3.1.9/psycopg/
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/_adapters_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/_cmodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/_dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/_preparing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/_tpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14726 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/_typeinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/_tz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/adapt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/client_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33949 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14051 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/connection_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/conninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29148 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/copy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:44:22.052085 psycopg-3.1.9/psycopg/crdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/crdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/crdb/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/crdb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30765 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/cursor_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/dbapi20.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40714 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:44:22.052085 psycopg-3.1.9/psycopg/pq/
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/pq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/pq/_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/pq/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20061 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/pq/_pq_ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/pq/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/pq/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35791 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/pq/pq_ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/server_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15925 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:44:22.052085 psycopg-3.1.9/psycopg/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14643 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/types/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/types/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/types/composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24788 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/types/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/types/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/types/hstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/types/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16390 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/types/multirange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/types/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/types/none.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13703 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/types/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20483 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/types/range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/types/shapely.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/types/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/types/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-05-02 11:44:12.000000 psycopg-3.1.9/psycopg/waiting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:44:22.048084 psycopg-3.1.9/psycopg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-02 11:44:22.000000 psycopg-3.1.9/psycopg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-02 11:44:22.000000 psycopg-3.1.9/psycopg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:44:22.000000 psycopg-3.1.9/psycopg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:44:21.000000 psycopg-3.1.9/psycopg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-02 11:44:22.000000 psycopg-3.1.9/psycopg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 11:44:22.000000 psycopg-3.1.9/psycopg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-02 11:44:12.000000 psycopg-3.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-02 11:44:22.056084 psycopg-3.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-02 11:44:12.000000 psycopg-3.1.9/setup.py
```

### Comparing `psycopg-3.1.8/LICENSE.txt` & `psycopg-3.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/PKG-INFO` & `psycopg-3.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psycopg
-Version: 3.1.8
+Version: 3.1.9
 Summary: PostgreSQL database adapter for Python
 Home-page: https://psycopg.org/psycopg3/
 Author: Daniele Varrazzo
 Author-email: daniele.varrazzo@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Homepage, https://psycopg.org/
 Project-URL: Documentation, https://psycopg.org/psycopg3/docs/
```

### Comparing `psycopg-3.1.8/README.rst` & `psycopg-3.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/__init__.py` & `psycopg-3.1.9/psycopg/__init__.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/_adapters_map.py` & `psycopg-3.1.9/psycopg/_adapters_map.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/_cmodule.py` & `psycopg-3.1.9/psycopg/_cmodule.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/_column.py` & `psycopg-3.1.9/psycopg/_column.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 class ColumnData(NamedTuple):
     ftype: int
     fmod: int
     fsize: int
 
 
 class Column(Sequence[Any]):
-
     __module__ = "psycopg"
 
     def __init__(self, cursor: "BaseCursor[Any, Any]", index: int):
         res = cursor.pgresult
         assert res
 
         fname = res.fname(index)
```

### Comparing `psycopg-3.1.8/psycopg/_compat.py` & `psycopg-3.1.9/psycopg/_compat.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/_dns.py` & `psycopg-3.1.9/psycopg/_dns.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/_encodings.py` & `psycopg-3.1.9/psycopg/_encodings.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     Raise LookupError if the Python encoding is unknown.
     """
     return pg_codecs[codecs.lookup(name).name]
 
 
 @cache
 def pg2pyenc(name: bytes) -> str:
-    """Convert a Python encoding name to PostgreSQL encoding name.
+    """Convert a PostgreSQL encoding name to Python encoding name.
 
     Raise NotSupportedError if the PostgreSQL encoding is not supported by
     Python.
     """
     try:
         return py_codecs[name.replace(b"-", b"").replace(b"_", b"").upper()]
     except KeyError:
```

### Comparing `psycopg-3.1.8/psycopg/_enums.py` & `psycopg-3.1.9/psycopg/_enums.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/_pipeline.py` & `psycopg-3.1.9/psycopg/_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 
 ACTIVE = pq.TransactionStatus.ACTIVE
 
 logger = logging.getLogger("psycopg")
 
 
 class BasePipeline:
-
     command_queue: Deque[PipelineCommand]
     result_queue: Deque[PendingResult]
     _is_supported: Optional[bool] = None
 
     def __init__(self, conn: "BaseConnection[Any]") -> None:
         self._conn = conn
         self.pgconn = conn.pgconn
@@ -216,15 +215,15 @@
     def sync(self) -> None:
         """Sync the pipeline, send any pending command and receive and process
         all available results.
         """
         try:
             with self._conn.lock:
                 self._conn.wait(self._sync_gen())
-        except e.Error as ex:
+        except e._NO_TRACEBACK as ex:
             raise ex.with_traceback(None)
 
     def __enter__(self: _Self) -> _Self:
         with self._conn.lock:
             self._conn.wait(self._enter_gen())
         return self
 
@@ -257,15 +256,15 @@
     def __init__(self, conn: "AsyncConnection[Any]") -> None:
         super().__init__(conn)
 
     async def sync(self) -> None:
         try:
             async with self._conn.lock:
                 await self._conn.wait(self._sync_gen())
-        except e.Error as ex:
+        except e._NO_TRACEBACK as ex:
             raise ex.with_traceback(None)
 
     async def __aenter__(self: _Self) -> _Self:
         async with self._conn.lock:
             await self._conn.wait(self._enter_gen())
         return self
```

### Comparing `psycopg-3.1.8/psycopg/_preparing.py` & `psycopg-3.1.9/psycopg/_preparing.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/_queries.py` & `psycopg-3.1.9/psycopg/_queries.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/_struct.py` & `psycopg-3.1.9/psycopg/_struct.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/_tpc.py` & `psycopg-3.1.9/psycopg/_tpc.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/_transform.py` & `psycopg-3.1.9/psycopg/_transform.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/_typeinfo.py` & `psycopg-3.1.9/psycopg/_typeinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from typing import Any, Dict, Iterator, Optional, overload
 from typing import Sequence, Tuple, Type, TypeVar, Union, TYPE_CHECKING
 from typing_extensions import TypeAlias
 
 from . import errors as e
 from .abc import AdaptContext, Query
 from .rows import dict_row
+from ._encodings import conn_encoding
 
 if TYPE_CHECKING:
     from .connection import BaseConnection, Connection
     from .connection_async import AsyncConnection
     from .sql import Identifier, SQL
 
 T = TypeVar("T", bound="TypeInfo")
@@ -90,28 +91,32 @@
     @classmethod
     def _fetch(cls: Type[T], conn: "Connection[Any]", name: str) -> Optional[T]:
         # This might result in a nested transaction. What we want is to leave
         # the function with the connection in the state we found (either idle
         # or intrans)
         try:
             with conn.transaction():
+                if conn_encoding(conn) == "ascii":
+                    conn.execute("set local client_encoding to utf8")
                 with conn.cursor(row_factory=dict_row) as cur:
                     cur.execute(cls._get_info_query(conn), {"name": name})
                     recs = cur.fetchall()
         except e.UndefinedObject:
             return None
 
         return cls._from_records(name, recs)
 
     @classmethod
     async def _fetch_async(
         cls: Type[T], conn: "AsyncConnection[Any]", name: str
     ) -> Optional[T]:
         try:
             async with conn.transaction():
+                if conn_encoding(conn) == "ascii":
+                    await conn.execute("set local client_encoding to utf8")
                 async with conn.cursor(row_factory=dict_row) as cur:
                     await cur.execute(cls._get_info_query(conn), {"name": name})
                     recs = await cur.fetchall()
         except e.UndefinedObject:
             return None
 
         return cls._from_records(name, recs)
```

### Comparing `psycopg-3.1.8/psycopg/_tz.py` & `psycopg-3.1.9/psycopg/_tz.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/_wrappers.py` & `psycopg-3.1.9/psycopg/_wrappers.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/abc.py` & `psycopg-3.1.9/psycopg/abc.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,14 @@
 
         :param data: the data to convert.
         """
         ...
 
 
 class Transformer(Protocol):
-
     types: Optional[Tuple[int, ...]]
     formats: Optional[List[pq.Format]]
 
     def __init__(self, context: Optional[AdaptContext] = None):
         ...
 
     @classmethod
```

### Comparing `psycopg-3.1.8/psycopg/adapt.py` & `psycopg-3.1.9/psycopg/adapt.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/client_cursor.py` & `psycopg-3.1.9/psycopg/client_cursor.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/connection.py` & `psycopg-3.1.9/psycopg/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -720,15 +720,15 @@
         conninfo = make_conninfo(**params)
 
         try:
             rv = cls._wait_conn(
                 cls._connect_gen(conninfo, autocommit=autocommit),
                 timeout=params["connect_timeout"],
             )
-        except e.Error as ex:
+        except e._NO_TRACEBACK as ex:
             raise ex.with_traceback(None)
 
         if row_factory:
             rv.row_factory = row_factory
         if cursor_factory:
             rv.cursor_factory = cursor_factory
         if context:
@@ -871,15 +871,15 @@
         try:
             cur = self.cursor()
             if binary:
                 cur.format = BINARY
 
             return cur.execute(query, params, prepare=prepare)
 
-        except e.Error as ex:
+        except e._NO_TRACEBACK as ex:
             raise ex.with_traceback(None)
 
     def commit(self) -> None:
         """Commit any pending transaction to the database."""
         with self.lock:
             self.wait(self._commit_gen())
 
@@ -915,15 +915,15 @@
         """
         Yield `Notify` objects as soon as they are received from the database.
         """
         while True:
             with self.lock:
                 try:
                     ns = self.wait(notifies(self.pgconn))
-                except e.Error as ex:
+                except e._NO_TRACEBACK as ex:
                     raise ex.with_traceback(None)
             enc = pgconn_encoding(self.pgconn)
             for pgn in ns:
                 n = Notify(pgn.relname.decode(enc), pgn.extra.decode(enc), pgn.be_pid)
                 yield n
 
     @contextmanager
```

### Comparing `psycopg-3.1.8/psycopg/connection_async.py` & `psycopg-3.1.9/psycopg/connection_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,15 +103,14 @@
         autocommit: bool = False,
         prepare_threshold: Optional[int] = 5,
         context: Optional[AdaptContext] = None,
         row_factory: Optional[AsyncRowFactory[Row]] = None,
         cursor_factory: Optional[Type[AsyncCursor[Row]]] = None,
         **kwargs: Any,
     ) -> "AsyncConnection[Any]":
-
         if sys.platform == "win32":
             loop = asyncio.get_running_loop()
             if isinstance(loop, asyncio.ProactorEventLoop):
                 raise e.InterfaceError(
                     "Psycopg cannot use the 'ProactorEventLoop' to run in async"
                     " mode. Please use a compatible event loop, for instance by"
                     " setting 'asyncio.set_event_loop_policy"
@@ -122,15 +121,15 @@
         conninfo = make_conninfo(**params)
 
         try:
             rv = await cls._wait_conn(
                 cls._connect_gen(conninfo, autocommit=autocommit),
                 timeout=params["connect_timeout"],
             )
-        except e.Error as ex:
+        except e._NO_TRACEBACK as ex:
             raise ex.with_traceback(None)
 
         if row_factory:
             rv.row_factory = row_factory
         if cursor_factory:
             rv.cursor_factory = cursor_factory
         if context:
@@ -278,15 +277,15 @@
         try:
             cur = self.cursor()
             if binary:
                 cur.format = BINARY
 
             return await cur.execute(query, params, prepare=prepare)
 
-        except e.Error as ex:
+        except e._NO_TRACEBACK as ex:
             raise ex.with_traceback(None)
 
     async def commit(self) -> None:
         async with self.lock:
             await self.wait(self._commit_gen())
 
     async def rollback(self) -> None:
@@ -313,15 +312,15 @@
                 yield tx
 
     async def notifies(self) -> AsyncGenerator[Notify, None]:
         while True:
             async with self.lock:
                 try:
                     ns = await self.wait(notifies(self.pgconn))
-                except e.Error as ex:
+                except e._NO_TRACEBACK as ex:
                     raise ex.with_traceback(None)
             enc = pgconn_encoding(self.pgconn)
             for pgn in ns:
                 n = Notify(pgn.relname.decode(enc), pgn.extra.decode(enc), pgn.be_pid)
                 yield n
 
     @asynccontextmanager
@@ -343,21 +342,17 @@
                 async with self.lock:
                     assert pipeline is self._pipeline
                     self._pipeline = None
 
     async def wait(self, gen: PQGen[RV]) -> RV:
         try:
             return await waiting.wait_async(gen, self.pgconn.socket)
-        except KeyboardInterrupt:
-            # TODO: this doesn't seem to work as it does for sync connections
-            # see tests/test_concurrency_async.py::test_ctrl_c
-            # In the test, the code doesn't reach this branch.
-
+        except (asyncio.CancelledError, KeyboardInterrupt):
             # On Ctrl-C, try to cancel the query in the server, otherwise
-            # otherwise the connection will be stuck in ACTIVE state
+            # the connection will remain stuck in ACTIVE state.
             c = self.pgconn.get_cancel()
             c.cancel()
             try:
                 await waiting.wait_async(gen, self.pgconn.socket)
             except e.QueryCanceled:
                 pass  # as expected
             raise
```

### Comparing `psycopg-3.1.8/psycopg/conninfo.py` & `psycopg-3.1.9/psycopg/conninfo.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/copy.py` & `psycopg-3.1.9/psycopg/copy.py`

 * *Files 0% similar despite different names*

```diff
@@ -457,15 +457,15 @@
         in binary mode.
     """
 
     def __init__(self, file: IO[bytes]):
         self.file = file
 
     def write(self, data: Buffer) -> None:
-        self.file.write(data)  # type: ignore[arg-type]
+        self.file.write(data)
 
 
 class AsyncCopy(BaseCopy["AsyncConnection[Any]"]):
     """Manage an asynchronous :sql:`COPY` operation."""
 
     __module__ = "psycopg"
 
@@ -665,15 +665,14 @@
 
     @abstractmethod
     def end(self) -> Buffer:
         ...
 
 
 class TextFormatter(Formatter):
-
     format = TEXT
 
     def __init__(self, transformer: Transformer, encoding: str = "utf-8"):
         super().__init__(transformer)
         self._encoding = encoding
 
     def parse_row(self, data: Buffer) -> Optional[Tuple[Any, ...]]:
@@ -710,15 +709,14 @@
             # Assume, for simplicity, that the user is not passing stupid
             # things to the write function. If that's the case, things
             # will fail downstream.
             return data
 
 
 class BinaryFormatter(Formatter):
-
     format = BINARY
 
     def __init__(self, transformer: Transformer):
         super().__init__(transformer)
         self._signature_sent = False
 
     def parse_row(self, data: Buffer) -> Optional[Tuple[Any, ...]]:
```

### Comparing `psycopg-3.1.8/psycopg/crdb/_types.py` & `psycopg-3.1.9/psycopg/crdb/_types.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/crdb/connection.py` & `psycopg-3.1.9/psycopg/crdb/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 if TYPE_CHECKING:
     from ..pq.abc import PGconn
     from ..cursor import Cursor
     from ..cursor_async import AsyncCursor
 
 
 class _CrdbConnectionMixin:
-
     _adapters: Optional[AdaptersMap]
     pgconn: "PGconn"
 
     @classmethod
     def is_crdb(
         cls, conn: Union[Connection[Any], AsyncConnection[Any], "PGconn"]
     ) -> bool:
```

### Comparing `psycopg-3.1.8/psycopg/cursor.py` & `psycopg-3.1.9/psycopg/cursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -715,15 +715,15 @@
         Execute a query or command to the database.
         """
         try:
             with self._conn.lock:
                 self._conn.wait(
                     self._execute_gen(query, params, prepare=prepare, binary=binary)
                 )
-        except e.Error as ex:
+        except e._NO_TRACEBACK as ex:
             raise ex.with_traceback(None)
         return self
 
     def executemany(
         self,
         query: Query,
         params_seq: Iterable[Params],
@@ -750,15 +750,15 @@
                             self._executemany_gen_pipeline(query, params_seq, returning)
                         )
             else:
                 with self._conn.lock:
                     self._conn.wait(
                         self._executemany_gen_no_pipeline(query, params_seq, returning)
                     )
-        except e.Error as ex:
+        except e._NO_TRACEBACK as ex:
             raise ex.with_traceback(None)
 
     def stream(
         self,
         query: Query,
         params: Optional[Params] = None,
         *,
@@ -767,25 +767,24 @@
         """
         Iterate row-by-row on a result from the database.
         """
         if self._pgconn.pipeline_status:
             raise e.ProgrammingError("stream() cannot be used in pipeline mode")
 
         with self._conn.lock:
-
             try:
                 self._conn.wait(self._stream_send_gen(query, params, binary=binary))
                 first = True
                 while self._conn.wait(self._stream_fetchone_gen(first)):
                     # We know that, if we got a result, it has a single row.
                     rec: Row = self._tx.load_row(0, self._make_row)  # type: ignore
                     yield rec
                     first = False
 
-            except e.Error as ex:
+            except e._NO_TRACEBACK as ex:
                 raise ex.with_traceback(None)
 
             finally:
                 if self._pgconn.transaction_status == ACTIVE:
                     # Try to cancel the query, then consume the results
                     # already received.
                     self._conn.cancel()
@@ -895,15 +894,15 @@
         """
         try:
             with self._conn.lock:
                 self._conn.wait(self._start_copy_gen(statement, params))
 
             with Copy(self, writer=writer) as copy:
                 yield copy
-        except e.Error as ex:
+        except e._NO_TRACEBACK as ex:
             raise ex.with_traceback(None)
 
         # If a fresher result has been set on the cursor by the Copy object,
         # read its properties (especially rowcount).
         self._select_current_result(0)
 
     def _fetch_pipeline(self) -> None:
```

### Comparing `psycopg-3.1.8/psycopg/cursor_async.py` & `psycopg-3.1.9/psycopg/cursor_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         binary: Optional[bool] = None,
     ) -> _Self:
         try:
             async with self._conn.lock:
                 await self._conn.wait(
                     self._execute_gen(query, params, prepare=prepare, binary=binary)
                 )
-        except e.Error as ex:
+        except e._NO_TRACEBACK as ex:
             raise ex.with_traceback(None)
         return self
 
     async def executemany(
         self,
         query: Query,
         params_seq: Iterable[Params],
@@ -117,41 +117,40 @@
                         await self._conn.wait(
                             self._executemany_gen_pipeline(query, params_seq, returning)
                         )
             else:
                 await self._conn.wait(
                     self._executemany_gen_no_pipeline(query, params_seq, returning)
                 )
-        except e.Error as ex:
+        except e._NO_TRACEBACK as ex:
             raise ex.with_traceback(None)
 
     async def stream(
         self,
         query: Query,
         params: Optional[Params] = None,
         *,
         binary: Optional[bool] = None,
     ) -> AsyncIterator[Row]:
         if self._pgconn.pipeline_status:
             raise e.ProgrammingError("stream() cannot be used in pipeline mode")
 
         async with self._conn.lock:
-
             try:
                 await self._conn.wait(
                     self._stream_send_gen(query, params, binary=binary)
                 )
                 first = True
                 while await self._conn.wait(self._stream_fetchone_gen(first)):
                     # We know that, if we got a result, it has a single row.
                     rec: Row = self._tx.load_row(0, self._make_row)  # type: ignore
                     yield rec
                     first = False
 
-            except e.Error as ex:
+            except e._NO_TRACEBACK as ex:
                 raise ex.with_traceback(None)
 
             finally:
                 if self._pgconn.transaction_status == ACTIVE:
                     # Try to cancel the query, then consume the results
                     # already received.
                     self._conn.cancel()
@@ -231,15 +230,15 @@
         """
         try:
             async with self._conn.lock:
                 await self._conn.wait(self._start_copy_gen(statement, params))
 
             async with AsyncCopy(self, writer=writer) as copy:
                 yield copy
-        except e.Error as ex:
+        except e._NO_TRACEBACK as ex:
             raise ex.with_traceback(None)
 
         self._select_current_result(0)
 
     async def _fetch_pipeline(self) -> None:
         if (
             self._execmany_returning is not False
```

### Comparing `psycopg-3.1.8/psycopg/dbapi20.py` & `psycopg-3.1.9/psycopg/dbapi20.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/errors.py` & `psycopg-3.1.9/psycopg/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
           |__NotSupportedError
 """
 
 # Copyright (C) 2020 The Psycopg Team
 
 from typing import Any, Dict, Optional, Sequence, Tuple, Type, Union
 from typing_extensions import TypeAlias
+from asyncio import CancelledError
 
 from .pq.abc import PGconn, PGresult
 from .pq._enums import DiagnosticField
 from ._compat import TypeGuard
 
 ErrorInfo: TypeAlias = Union[None, PGresult, Dict[int, Optional[bytes]]]
 
@@ -1529,7 +1530,15 @@
 class IndexCorrupted(InternalError,
     code='XX002', name='INDEX_CORRUPTED'):
     pass
 
 
 # autogenerated: end
 # fmt: on
+
+# Don't show a complete traceback upon raising these exception.
+# Usually the traceback starts from internal functions (for instance in the
+# server communication callbacks) but, for the end user, it's more important
+# to get the high level information about where the exception was raised, for
+# instance in a certain `Cursor.execute()`.
+
+_NO_TRACEBACK = (Error, KeyboardInterrupt, CancelledError)
```

### Comparing `psycopg-3.1.8/psycopg/generators.py` & `psycopg-3.1.9/psycopg/generators.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/postgres.py` & `psycopg-3.1.9/psycopg/postgres.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,14 @@
 # A few oids used a bit everywhere
 INVALID_OID = 0
 TEXT_OID = types["text"].oid
 TEXT_ARRAY_OID = types["text"].array_oid
 
 
 def register_default_adapters(context: AdaptContext) -> None:
-
     from .types import array, bool, composite, datetime, enum, json, multirange
     from .types import net, none, numeric, range, string, uuid
 
     array.register_default_adapters(context)
     bool.register_default_adapters(context)
     composite.register_default_adapters(context)
     datetime.register_default_adapters(context)
```

### Comparing `psycopg-3.1.8/psycopg/pq/__init__.py` & `psycopg-3.1.9/psycopg/pq/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             from psycopg_binary import pq as module  # type: ignore
         except Exception as e:
             handle_error("binary", e)
 
     # Pure Python implementation, slow and requires the system libpq installed.
     if not module and (not impl or impl == "python"):
         try:
-            from . import pq_ctypes as module  # type: ignore[no-redef]
+            from . import pq_ctypes as module  # type: ignore[assignment]
         except Exception as e:
             handle_error("python", e)
 
     if module:
         __impl__ = module.__impl__
         version = module.version
         PGconn = module.PGconn
```

### Comparing `psycopg-3.1.8/psycopg/pq/_debug.py` & `psycopg-3.1.9/psycopg/pq/_debug.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     """Wrap a function in order to log its arguments and return value on call."""
 
     @wraps(f)
     def debugging_(*args: Any, **kwargs: Any) -> Any:
         reprs = []
         for arg in args:
             reprs.append(f"{arg!r}")
-        for (k, v) in kwargs.items():
+        for k, v in kwargs.items():
             reprs.append(f"{k}={v!r}")
 
         logger.info("PGconn.%s(%s)", f.__name__, ", ".join(reprs))
         rv = f(*args, **kwargs)
         # Display the return value only if the function is declared to return
         # something else than None.
         ra = inspect.signature(f).return_annotation
```

### Comparing `psycopg-3.1.8/psycopg/pq/_enums.py` & `psycopg-3.1.9/psycopg/pq/_enums.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/pq/_pq_ctypes.py` & `psycopg-3.1.9/psycopg/pq/_pq_ctypes.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/pq/abc.py` & `psycopg-3.1.9/psycopg/pq/abc.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     from .misc import PGnotify, ConninfoOption, PGresAttDesc
 
 # An object implementing the buffer protocol (ish)
 Buffer: TypeAlias = Union[bytes, bytearray, memoryview]
 
 
 class PGconn(Protocol):
-
     notice_handler: Optional[Callable[["PGresult"], None]]
     notify_handler: Optional[Callable[["PGnotify"], None]]
 
     @classmethod
     def connect(cls, conninfo: bytes) -> "PGconn":
         ...
```

### Comparing `psycopg-3.1.8/psycopg/pq/misc.py` & `psycopg-3.1.9/psycopg/pq/misc.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/pq/pq_ctypes.py` & `psycopg-3.1.9/psycopg/pq/pq_ctypes.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/rows.py` & `psycopg-3.1.9/psycopg/rows.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/server_cursor.py` & `psycopg-3.1.9/psycopg/server_cursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,14 @@
             sql.SQL(" ABSOLUTE" if mode == "absolute" else ""),
             sql.Literal(value),
             sql.Identifier(self._name),
         )
         yield from self._conn._exec_command(query)
 
     def _make_declare_statement(self, query: Query) -> sql.Composed:
-
         if isinstance(query, bytes):
             query = query.decode(self._encoding)
         if not isinstance(query, sql.Composable):
             query = sql.SQL(query)
 
         parts = [
             sql.SQL("DECLARE"),
@@ -287,15 +286,15 @@
             raise e.NotSupportedError(
                 "server-side cursors not supported in pipeline mode"
             )
 
         try:
             with self._conn.lock:
                 self._conn.wait(self._declare_gen(query, params, binary))
-        except e.Error as ex:
+        except e._NO_TRACEBACK as ex:
             raise ex.with_traceback(None)
 
         return self
 
     def executemany(
         self,
         query: Query,
@@ -423,15 +422,15 @@
             raise e.NotSupportedError(
                 "server-side cursors not supported in pipeline mode"
             )
 
         try:
             async with self._conn.lock:
                 await self._conn.wait(self._declare_gen(query, params, binary))
-        except e.Error as ex:
+        except e._NO_TRACEBACK as ex:
             raise ex.with_traceback(None)
 
         return self
 
     async def executemany(
         self,
         query: Query,
```

### Comparing `psycopg-3.1.8/psycopg/sql.py` & `psycopg-3.1.9/psycopg/sql.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/transaction.py` & `psycopg-3.1.9/psycopg/transaction.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/types/array.py` & `psycopg-3.1.9/psycopg/types/array.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,14 @@
             if info:
                 return info
 
         return self._tx.adapters.types["text"]
 
 
 class ListDumper(BaseListDumper):
-
     delimiter = b","
 
     def get_key(self, obj: List[Any], format: PyFormat) -> DumperKey:
         if self.oid:
             return self.cls
 
         item = self._find_list_element(obj, format)
@@ -210,15 +209,14 @@
         | ^null$          # or the word NULL
         """
         % delimiter
     )
 
 
 class ListBinaryDumper(BaseListDumper):
-
     format = pq.Format.BINARY
 
     def get_key(self, obj: List[Any], format: PyFormat) -> DumperKey:
         if self.oid:
             return self.cls
 
         item = self._find_list_element(obj, format)
@@ -290,25 +288,23 @@
 
         data[0] = _pack_head(len(dims), hasnull, sub_oid)
         data[1] = b"".join(_pack_dim(dim, 1) for dim in dims)
         return b"".join(data)
 
 
 class ArrayLoader(RecursiveLoader):
-
     delimiter = b","
     base_oid: int
 
     def load(self, data: Buffer) -> List[Any]:
         loader = self._tx.get_loader(self.base_oid, self.format)
         return _load_text(data, loader, self.delimiter)
 
 
 class ArrayBinaryLoader(RecursiveLoader):
-
     format = pq.Format.BINARY
 
     def load(self, data: Buffer) -> List[Any]:
         return _load_binary(data, self._tx)
 
 
 def register_array(info: TypeInfo, context: Optional[AdaptContext] = None) -> None:
```

### Comparing `psycopg-3.1.8/psycopg/types/bool.py` & `psycopg-3.1.9/psycopg/types/bool.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,40 +7,37 @@
 from .. import postgres
 from ..pq import Format
 from ..abc import AdaptContext
 from ..adapt import Buffer, Dumper, Loader
 
 
 class BoolDumper(Dumper):
-
     oid = postgres.types["bool"].oid
 
     def dump(self, obj: bool) -> bytes:
         return b"t" if obj else b"f"
 
     def quote(self, obj: bool) -> bytes:
         return b"true" if obj else b"false"
 
 
 class BoolBinaryDumper(Dumper):
-
     format = Format.BINARY
     oid = postgres.types["bool"].oid
 
     def dump(self, obj: bool) -> bytes:
         return b"\x01" if obj else b"\x00"
 
 
 class BoolLoader(Loader):
     def load(self, data: Buffer) -> bool:
         return data == b"t"
 
 
 class BoolBinaryLoader(Loader):
-
     format = Format.BINARY
 
     def load(self, data: Buffer) -> bool:
         return data != b"\x00"
 
 
 def register_default_adapters(context: AdaptContext) -> None:
```

### Comparing `psycopg-3.1.8/psycopg/types/composite.py` & `psycopg-3.1.9/psycopg/types/composite.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,41 +3,41 @@
 """
 
 # Copyright (C) 2020 The Psycopg Team
 
 import re
 import struct
 from collections import namedtuple
-from typing import Any, Callable, cast, Iterator, List, Optional
+from typing import Any, Callable, cast, Dict, Iterator, List, Optional
 from typing import Sequence, Tuple, Type
 
 from .. import pq
+from .. import abc
 from .. import postgres
-from ..abc import AdaptContext, Buffer
-from ..adapt import Transformer, PyFormat, RecursiveDumper, Loader
+from ..adapt import Transformer, PyFormat, RecursiveDumper, Loader, Dumper
 from .._struct import pack_len, unpack_len
 from ..postgres import TEXT_OID
 from .._typeinfo import CompositeInfo as CompositeInfo  # exported here
 from .._encodings import _as_python_identifier
 
 _struct_oidlen = struct.Struct("!Ii")
 _pack_oidlen = cast(Callable[[int, int], bytes], _struct_oidlen.pack)
 _unpack_oidlen = cast(
-    Callable[[Buffer, int], Tuple[int, int]], _struct_oidlen.unpack_from
+    Callable[[abc.Buffer, int], Tuple[int, int]], _struct_oidlen.unpack_from
 )
 
 
 class SequenceDumper(RecursiveDumper):
     def _dump_sequence(
         self, obj: Sequence[Any], start: bytes, end: bytes, sep: bytes
     ) -> bytes:
         if not obj:
             return start + end
 
-        parts: List[Buffer] = [start]
+        parts: List[abc.Buffer] = [start]
 
         for item in obj:
             if item is None:
                 parts.append(sep)
                 continue
 
             dumper = self._tx.get_dumper(item, PyFormat.from_pq(self.format))
@@ -55,33 +55,38 @@
         return b"".join(parts)
 
     _re_needs_quotes = re.compile(rb'[",\\\s()]')
     _re_esc = re.compile(rb"([\\\"])")
 
 
 class TupleDumper(SequenceDumper):
-
     # Should be this, but it doesn't work
     # oid = postgres_types["record"].oid
 
     def dump(self, obj: Tuple[Any, ...]) -> bytes:
         return self._dump_sequence(obj, b"(", b")", b",")
 
 
-class TupleBinaryDumper(RecursiveDumper):
-
+class TupleBinaryDumper(Dumper):
     format = pq.Format.BINARY
 
     # Subclasses must set an info
     info: CompositeInfo
 
-    def __init__(self, cls: type, context: Optional[AdaptContext] = None):
+    def __init__(self, cls: type, context: Optional[abc.AdaptContext] = None):
         super().__init__(cls, context)
-        nfields = len(self.info.field_types)
+
+        # Note: this class is not a RecursiveDumper because it would use the
+        # same Transformer of the context, which would confuse dump_sequence()
+        # in case the composite contains another composite. Make sure to use
+        # a separate Transformer instance instead.
+        self._tx = Transformer(context)
         self._tx.set_dumper_types(self.info.field_types, self.format)
+
+        nfields = len(self.info.field_types)
         self._formats = (PyFormat.from_pq(self.format),) * nfields
 
     def dump(self, obj: Tuple[Any, ...]) -> bytearray:
         out = bytearray(pack_len(len(obj)))
         adapted = self._tx.dump_sequence(obj, self._formats)
         for i in range(len(obj)):
             b = adapted[i]
@@ -92,19 +97,19 @@
             else:
                 out += _pack_oidlen(oid, -1)
 
         return out
 
 
 class BaseCompositeLoader(Loader):
-    def __init__(self, oid: int, context: Optional[AdaptContext] = None):
+    def __init__(self, oid: int, context: Optional[abc.AdaptContext] = None):
         super().__init__(oid, context)
         self._tx = Transformer(context)
 
-    def _parse_record(self, data: Buffer) -> Iterator[Optional[bytes]]:
+    def _parse_record(self, data: abc.Buffer) -> Iterator[Optional[bytes]]:
         """
         Split a non-empty representation of a composite type into components.
 
         Terminators shouldn't be used in `!data` (so that both record and range
         representations can be parsed).
         """
         for m in self._re_tokenize.finditer(data):
@@ -128,96 +133,93 @@
         """
     )
 
     _re_undouble = re.compile(rb'(["\\])\1')
 
 
 class RecordLoader(BaseCompositeLoader):
-    def load(self, data: Buffer) -> Tuple[Any, ...]:
+    def load(self, data: abc.Buffer) -> Tuple[Any, ...]:
         if data == b"()":
             return ()
 
         cast = self._tx.get_loader(TEXT_OID, self.format).load
         return tuple(
             cast(token) if token is not None else None
             for token in self._parse_record(data[1:-1])
         )
 
 
 class RecordBinaryLoader(Loader):
     format = pq.Format.BINARY
-    _types_set = False
 
-    def __init__(self, oid: int, context: Optional[AdaptContext] = None):
+    def __init__(self, oid: int, context: Optional[abc.AdaptContext] = None):
         super().__init__(oid, context)
-        self._tx = Transformer(context)
-
-    def load(self, data: Buffer) -> Tuple[Any, ...]:
-        if not self._types_set:
-            self._config_types(data)
-            self._types_set = True
-
-        return self._tx.load_sequence(
-            tuple(
-                data[offset : offset + length] if length != -1 else None
-                for _, offset, length in self._walk_record(data)
-            )
-        )
+        self._ctx = context
+        # Cache a transformer for each sequence of oid found.
+        # Usually there will be only one, but if there is more than one
+        # row in the same query (in different columns, or even in different
+        # records), oids might differ and we'd need separate transformers.
+        self._txs: Dict[Tuple[int, ...], abc.Transformer] = {}
 
-    def _walk_record(self, data: Buffer) -> Iterator[Tuple[int, int, int]]:
-        """
-        Yield a sequence of (oid, offset, length) for the content of the record
-        """
+    def load(self, data: abc.Buffer) -> Tuple[Any, ...]:
         nfields = unpack_len(data, 0)[0]
-        i = 4
+        offset = 4
+        oids = []
+        record = []
         for _ in range(nfields):
-            oid, length = _unpack_oidlen(data, i)
-            yield oid, i + 8, length
-            i += (8 + length) if length > 0 else 8
-
-    def _config_types(self, data: Buffer) -> None:
-        oids = [r[0] for r in self._walk_record(data)]
-        self._tx.set_loader_types(oids, self.format)
+            oid, length = _unpack_oidlen(data, offset)
+            offset += 8
+            record.append(data[offset : offset + length] if length != -1 else None)
+            oids.append(oid)
+            if length >= 0:
+                offset += length
+
+        key = tuple(oids)
+        try:
+            tx = self._txs[key]
+        except KeyError:
+            tx = self._txs[key] = Transformer(self._ctx)
+            tx.set_loader_types(oids, self.format)
 
+        return tx.load_sequence(tuple(record))
 
-class CompositeLoader(RecordLoader):
 
+class CompositeLoader(RecordLoader):
     factory: Callable[..., Any]
     fields_types: List[int]
     _types_set = False
 
-    def load(self, data: Buffer) -> Any:
+    def load(self, data: abc.Buffer) -> Any:
         if not self._types_set:
             self._config_types(data)
             self._types_set = True
 
         if data == b"()":
             return type(self).factory()
 
         return type(self).factory(
             *self._tx.load_sequence(tuple(self._parse_record(data[1:-1])))
         )
 
-    def _config_types(self, data: Buffer) -> None:
+    def _config_types(self, data: abc.Buffer) -> None:
         self._tx.set_loader_types(self.fields_types, self.format)
 
 
 class CompositeBinaryLoader(RecordBinaryLoader):
-
     format = pq.Format.BINARY
     factory: Callable[..., Any]
 
-    def load(self, data: Buffer) -> Any:
+    def load(self, data: abc.Buffer) -> Any:
         r = super().load(data)
         return type(self).factory(*r)
 
 
 def register_composite(
     info: CompositeInfo,
-    context: Optional[AdaptContext] = None,
+    context: Optional[abc.AdaptContext] = None,
     factory: Optional[Callable[..., Any]] = None,
 ) -> None:
     """Register the adapters to load and dump a composite type.
 
     :param info: The object with the information about the composite to register.
     :param context: The context where to register the adapters. If `!None`,
         register it globally.
@@ -279,12 +281,12 @@
         # Default to the text dumper because it is more flexible
         dumper = type(f"{info.name.title()}Dumper", (TupleDumper,), {"oid": info.oid})
         adapters.register_dumper(factory, dumper)
 
         info.python_type = factory
 
 
-def register_default_adapters(context: AdaptContext) -> None:
+def register_default_adapters(context: abc.AdaptContext) -> None:
     adapters = context.adapters
     adapters.register_dumper(tuple, TupleDumper)
     adapters.register_loader("record", RecordLoader)
     adapters.register_loader("record", RecordBinaryLoader)
```

### Comparing `psycopg-3.1.8/psycopg/types/datetime.py` & `psycopg-3.1.9/psycopg/types/datetime.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,25 +34,23 @@
 _pg_date_epoch_days = date(2000, 1, 1).toordinal()
 _pg_datetime_epoch = datetime(2000, 1, 1)
 _pg_datetimetz_epoch = datetime(2000, 1, 1, tzinfo=utc)
 _py_date_min_days = date.min.toordinal()
 
 
 class DateDumper(Dumper):
-
     oid = postgres.types["date"].oid
 
     def dump(self, obj: date) -> bytes:
         # NOTE: whatever the PostgreSQL DateStyle input format (DMY, MDY, YMD)
         # the YYYY-MM-DD is always understood correctly.
         return str(obj).encode()
 
 
 class DateBinaryDumper(Dumper):
-
     format = Format.BINARY
     oid = postgres.types["date"].oid
 
     def dump(self, obj: date) -> bytes:
         days = obj.toordinal() - _pg_date_epoch_days
         return pack_int4(days)
 
@@ -72,31 +70,28 @@
 
 class _BaseTimeTextDumper(_BaseTimeDumper):
     def dump(self, obj: time) -> bytes:
         return str(obj).encode()
 
 
 class TimeDumper(_BaseTimeTextDumper):
-
     oid = postgres.types["time"].oid
 
     def upgrade(self, obj: time, format: PyFormat) -> Dumper:
         if not obj.tzinfo:
             return self
         else:
             return TimeTzDumper(self.cls)
 
 
 class TimeTzDumper(_BaseTimeTextDumper):
-
     oid = postgres.types["timetz"].oid
 
 
 class TimeBinaryDumper(_BaseTimeDumper):
-
     format = Format.BINARY
     oid = postgres.types["time"].oid
 
     def dump(self, obj: time) -> bytes:
         us = obj.microsecond + 1_000_000 * (
             obj.second + 60 * (obj.minute + 60 * obj.hour)
         )
@@ -106,15 +101,14 @@
         if not obj.tzinfo:
             return self
         else:
             return TimeTzBinaryDumper(self.cls)
 
 
 class TimeTzBinaryDumper(_BaseTimeDumper):
-
     format = Format.BINARY
     oid = postgres.types["timetz"].oid
 
     def dump(self, obj: time) -> bytes:
         us = obj.microsecond + 1_000_000 * (
             obj.second + 60 * (obj.minute + 60 * obj.hour)
         )
@@ -140,31 +134,28 @@
     def dump(self, obj: datetime) -> bytes:
         # NOTE: whatever the PostgreSQL DateStyle input format (DMY, MDY, YMD)
         # the YYYY-MM-DD is always understood correctly.
         return str(obj).encode()
 
 
 class DatetimeDumper(_BaseDatetimeTextDumper):
-
     oid = postgres.types["timestamptz"].oid
 
     def upgrade(self, obj: datetime, format: PyFormat) -> Dumper:
         if obj.tzinfo:
             return self
         else:
             return DatetimeNoTzDumper(self.cls)
 
 
 class DatetimeNoTzDumper(_BaseDatetimeTextDumper):
-
     oid = postgres.types["timestamp"].oid
 
 
 class DatetimeBinaryDumper(_BaseDatetimeDumper):
-
     format = Format.BINARY
     oid = postgres.types["timestamptz"].oid
 
     def dump(self, obj: datetime) -> bytes:
         delta = obj - _pg_datetimetz_epoch
         micros = delta.microseconds + 1_000_000 * (86_400 * delta.days + delta.seconds)
         return pack_int8(micros)
@@ -173,26 +164,24 @@
         if obj.tzinfo:
             return self
         else:
             return DatetimeNoTzBinaryDumper(self.cls)
 
 
 class DatetimeNoTzBinaryDumper(_BaseDatetimeDumper):
-
     format = Format.BINARY
     oid = postgres.types["timestamp"].oid
 
     def dump(self, obj: datetime) -> bytes:
         delta = obj - _pg_datetime_epoch
         micros = delta.microseconds + 1_000_000 * (86_400 * delta.days + delta.seconds)
         return pack_int8(micros)
 
 
 class TimedeltaDumper(Dumper):
-
     oid = postgres.types["interval"].oid
 
     def __init__(self, cls: type, context: Optional[AdaptContext] = None):
         super().__init__(cls, context)
         if self.connection:
             if (
                 self.connection.pgconn.parameter_status(b"IntervalStyle")
@@ -212,25 +201,23 @@
             obj.days,
             obj.seconds,
             obj.microseconds,
         )
 
 
 class TimedeltaBinaryDumper(Dumper):
-
     format = Format.BINARY
     oid = postgres.types["interval"].oid
 
     def dump(self, obj: timedelta) -> bytes:
         micros = 1_000_000 * obj.seconds + obj.microseconds
         return _pack_interval(micros, obj.days, 0)
 
 
 class DateLoader(Loader):
-
     _ORDER_YMD = 0
     _ORDER_DMY = 1
     _ORDER_MDY = 2
 
     def __init__(self, oid: int, context: Optional[AdaptContext] = None):
         super().__init__(oid, context)
         ds = _get_datestyle(self.connection)
@@ -266,30 +253,28 @@
             elif s == "-infinity" or "BC" in s:
                 raise DataError(f"date too small (before year 1): {s!r}") from None
             else:
                 raise DataError(f"can't parse date {s!r}: {ex}") from None
 
 
 class DateBinaryLoader(Loader):
-
     format = Format.BINARY
 
     def load(self, data: Buffer) -> date:
         days = unpack_int4(data)[0] + _pg_date_epoch_days
         try:
             return date.fromordinal(days)
         except (ValueError, OverflowError):
             if days < _py_date_min_days:
                 raise DataError("date too small (before year 1)") from None
             else:
                 raise DataError("date too large (after year 10K)") from None
 
 
 class TimeLoader(Loader):
-
     _re_format = re.compile(rb"^(\d+):(\d+):(\d+)(?:\.(\d+))?")
 
     def load(self, data: Buffer) -> time:
         m = self._re_format.match(data)
         if not m:
             s = bytes(data).decode("utf8", "replace")
             raise DataError(f"can't parse time {s!r}")
@@ -308,30 +293,28 @@
             return time(int(ho), int(mi), int(se), us)
         except ValueError as e:
             s = bytes(data).decode("utf8", "replace")
             raise DataError(f"can't parse time {s!r}: {e}") from None
 
 
 class TimeBinaryLoader(Loader):
-
     format = Format.BINARY
 
     def load(self, data: Buffer) -> time:
         val = unpack_int8(data)[0]
         val, us = divmod(val, 1_000_000)
         val, s = divmod(val, 60)
         h, m = divmod(val, 60)
         try:
             return time(h, m, s, us)
         except ValueError:
             raise DataError(f"time not supported by Python: hour={h}") from None
 
 
 class TimetzLoader(Loader):
-
     _re_format = re.compile(
         rb"""(?ix)
         ^
         (\d+) : (\d+) : (\d+) (?: \. (\d+) )?       # Time and micros
         ([-+]) (\d+) (?: : (\d+) )? (?: : (\d+) )?  # Timezone
         $
         """
@@ -365,15 +348,14 @@
             return time(int(ho), int(mi), int(se), us, tz)
         except ValueError as e:
             s = bytes(data).decode("utf8", "replace")
             raise DataError(f"can't parse timetz {s!r}: {e}") from None
 
 
 class TimetzBinaryLoader(Loader):
-
     format = Format.BINARY
 
     def load(self, data: Buffer) -> time:
         val, off = _unpack_timetz(data)
 
         val, us = divmod(val, 1_000_000)
         val, s = divmod(val, 60)
@@ -382,15 +364,14 @@
         try:
             return time(h, m, s, us, timezone(timedelta(seconds=-off)))
         except ValueError:
             raise DataError(f"time not supported by Python: hour={h}") from None
 
 
 class TimestampLoader(Loader):
-
     _re_format = re.compile(
         rb"""(?ix)
         ^
         (\d+) [^a-z0-9] (\d+) [^a-z0-9] (\d+)   # Date
         (?: T | [^a-z0-9] )                     # Separator, including T
         (\d+) [^a-z0-9] (\d+) [^a-z0-9] (\d+)   # Time
         (?: \.(\d+) )?                          # Micros
@@ -468,30 +449,28 @@
         try:
             return datetime(int(ye), imo, int(da), int(ho), int(mi), int(se), us)
         except ValueError as ex:
             raise _get_timestamp_load_error(self.connection, data, ex) from None
 
 
 class TimestampBinaryLoader(Loader):
-
     format = Format.BINARY
 
     def load(self, data: Buffer) -> datetime:
         micros = unpack_int8(data)[0]
         try:
             return _pg_datetime_epoch + timedelta(microseconds=micros)
         except OverflowError:
             if micros <= 0:
                 raise DataError("timestamp too small (before year 1)") from None
             else:
                 raise DataError("timestamp too large (after year 10K)") from None
 
 
 class TimestamptzLoader(Loader):
-
     _re_format = re.compile(
         rb"""(?ix)
         ^
         (\d+) [^a-z0-9] (\d+) [^a-z0-9] (\d+)       # Date
         (?: T | [^a-z0-9] )                         # Separator, including T
         (\d+) [^a-z0-9] (\d+) [^a-z0-9] (\d+)       # Time
         (?: \.(\d+) )?                              # Micros
@@ -559,15 +538,14 @@
         ds = _get_datestyle(self.connection).decode("ascii")
         raise NotImplementedError(
             f"can't parse timestamptz with DateStyle {ds!r}: {s!r}"
         )
 
 
 class TimestamptzBinaryLoader(Loader):
-
     format = Format.BINARY
 
     def __init__(self, oid: int, context: Optional[AdaptContext] = None):
         super().__init__(oid, context)
         self._timezone = get_tzinfo(self.connection.pgconn if self.connection else None)
 
     def load(self, data: Buffer) -> datetime:
@@ -596,15 +574,14 @@
             if micros <= 0:
                 raise DataError("timestamp too small (before year 1)") from None
             else:
                 raise DataError("timestamp too large (after year 10K)") from None
 
 
 class IntervalLoader(Loader):
-
     _re_interval = re.compile(
         rb"""
         (?: ([-+]?\d+) \s+ years? \s* )?                # Years
         (?: ([-+]?\d+) \s+ mons? \s* )?                 # Months
         (?: ([-+]?\d+) \s+ days? \s* )?                 # Days
         (?: ([-+])? (\d+) : (\d+) : (\d+ (?:\.\d+)?)    # Time
         )?
@@ -656,15 +633,14 @@
         ).decode("utf8", "replace")
         raise NotImplementedError(
             f"can't parse interval with IntervalStyle {ints}: {s!r}"
         )
 
 
 class IntervalBinaryLoader(Loader):
-
     format = Format.BINARY
 
     def load(self, data: Buffer) -> timedelta:
         micros, days, months = _unpack_interval(data)
         if months > 0:
             years, months = divmod(months, 12)
             days = days + 30 * months + 365 * years
```

### Comparing `psycopg-3.1.8/psycopg/types/enum.py` & `psycopg-3.1.9/psycopg/types/enum.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/types/hstore.py` & `psycopg-3.1.9/psycopg/types/hstore.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 
         def add_token(s: str) -> None:
             tokens.append('"')
             tokens.append(_re_escape.sub(r"\\\1", s))
             tokens.append('"')
 
         for k, v in obj.items():
-
             if not isinstance(k, str):
                 raise e.DataError("hstore keys can only be strings")
             add_token(k)
 
             tokens.append("=>")
 
             if v is None:
```

### Comparing `psycopg-3.1.8/psycopg/types/json.py` & `psycopg-3.1.9/psycopg/types/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,56 +114,53 @@
 
 
 class Jsonb(_JsonWrapper):
     __slots__ = ()
 
 
 class _JsonDumper(Dumper):
-
     # The globally used JSON dumps() function. It can be changed globally (by
     # set_json_dumps) or by a subclass.
     _dumps: JsonDumpsFunction = json.dumps
 
     def __init__(self, cls: type, context: Optional[abc.AdaptContext] = None):
         super().__init__(cls, context)
         self.dumps = self.__class__._dumps
 
-    def dump(self, obj: _JsonWrapper) -> bytes:
-        dumps = obj.dumps or self.dumps
-        return dumps(obj.obj).encode()
+    def dump(self, obj: Any) -> bytes:
+        if isinstance(obj, _JsonWrapper):
+            dumps = obj.dumps or self.dumps
+            obj = obj.obj
+        else:
+            dumps = self.dumps
+        return dumps(obj).encode()
 
 
 class JsonDumper(_JsonDumper):
-
     oid = postgres.types["json"].oid
 
 
 class JsonBinaryDumper(_JsonDumper):
-
     format = Format.BINARY
     oid = postgres.types["json"].oid
 
 
 class JsonbDumper(_JsonDumper):
-
     oid = postgres.types["jsonb"].oid
 
 
 class JsonbBinaryDumper(_JsonDumper):
-
     format = Format.BINARY
     oid = postgres.types["jsonb"].oid
 
-    def dump(self, obj: _JsonWrapper) -> bytes:
-        dumps = obj.dumps or self.dumps
-        return b"\x01" + dumps(obj.obj).encode()
+    def dump(self, obj: Any) -> bytes:
+        return b"\x01" + super().dump(obj)
 
 
 class _JsonLoader(Loader):
-
     # The globally used JSON loads() function. It can be changed globally (by
     # set_json_loads) or by a subclass.
     _loads: JsonLoadsFunction = json.loads
 
     def __init__(self, oid: int, context: Optional[abc.AdaptContext] = None):
         super().__init__(oid, context)
         self.loads = self.__class__._loads
@@ -184,15 +181,14 @@
 
 
 class JsonBinaryLoader(_JsonLoader):
     format = Format.BINARY
 
 
 class JsonbBinaryLoader(_JsonLoader):
-
     format = Format.BINARY
 
     def load(self, data: Buffer) -> Any:
         if data and data[0] != 1:
             raise DataError("unknown jsonb binary format: {data[0]}")
         data = data[1:]
         if not isinstance(data, bytes):
```

### Comparing `psycopg-3.1.8/psycopg/types/multirange.py` & `psycopg-3.1.9/psycopg/types/multirange.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,14 @@
             out.append(dump_range_text(r, dump))
             out.append(b",")
         out[-1] = b"}"
         return b"".join(out)
 
 
 class MultirangeBinaryDumper(BaseMultirangeDumper):
-
     format = Format.BINARY
 
     def dump(self, obj: Multirange[Any]) -> Buffer:
         item = self._get_item(obj)
         if item is not None:
             dump = self._tx.get_dumper(item, self._adapt_format).dump
         else:
@@ -248,15 +247,14 @@
             data = dump_range_binary(r, dump)
             out.append(pack_len(len(data)))
             out.append(data)
         return b"".join(out)
 
 
 class BaseMultirangeLoader(RecursiveLoader, Generic[T]):
-
     subtype_oid: int
 
     def __init__(self, oid: int, context: Optional[AdaptContext] = None):
         super().__init__(oid, context)
         self._load = self._tx.get_loader(self.subtype_oid, format=self.format).load
 
 
@@ -303,15 +301,14 @@
 
 _SEP_INT = ord(",")
 _START_INT = ord("{")
 _END_INT = ord("}")
 
 
 class MultirangeBinaryLoader(BaseMultirangeLoader[T]):
-
     format = Format.BINARY
 
     def load(self, data: Buffer) -> Multirange[T]:
         nelems = unpack_len(data, 0)[0]
         pos = 4
         out = Multirange[T]()
         for i in range(nelems):
```

### Comparing `psycopg-3.1.8/psycopg/types/net.py` & `psycopg-3.1.9/psycopg/types/net.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,23 +46,21 @@
             from ipaddress import ip_address, ip_interface, ip_network
             from ipaddress import IPv4Address, IPv6Address
             from ipaddress import IPv4Interface, IPv6Interface
             from ipaddress import IPv4Network, IPv6Network
 
 
 class InterfaceDumper(Dumper):
-
     oid = postgres.types["inet"].oid
 
     def dump(self, obj: Interface) -> bytes:
         return str(obj).encode()
 
 
 class NetworkDumper(Dumper):
-
     oid = postgres.types["cidr"].oid
 
     def dump(self, obj: Network) -> bytes:
         return str(obj).encode()
 
 
 class _AIBinaryDumper(Dumper):
@@ -105,15 +103,14 @@
             prefixlen = obj.max_prefixlen
 
         head = bytes((family, prefixlen, 0, len(packed)))
         return head + packed
 
 
 class NetworkBinaryDumper(Dumper):
-
     format = Format.BINARY
     oid = postgres.types["cidr"].oid
 
     def dump(self, obj: Network) -> bytes:
         packed = obj.network_address.packed
         family = PGSQL_AF_INET if obj.version == 4 else PGSQL_AF_INET6
         head = bytes((family, obj.prefixlen, 1, len(packed)))
@@ -134,15 +131,14 @@
         if b"/" in data:
             return ip_interface(data.decode())
         else:
             return ip_address(data.decode())
 
 
 class InetBinaryLoader(_LazyIpaddressLoader):
-
     format = Format.BINARY
 
     def load(self, data: Buffer) -> Union[Address, Interface]:
         if isinstance(data, memoryview):
             data = bytes(data)
 
         prefix = data[1]
@@ -164,15 +160,14 @@
         if isinstance(data, memoryview):
             data = bytes(data)
 
         return ip_network(data.decode())
 
 
 class CidrBinaryLoader(_LazyIpaddressLoader):
-
     format = Format.BINARY
 
     def load(self, data: Buffer) -> Network:
         if isinstance(data, memoryview):
             data = bytes(data)
 
         prefix = data[1]
```

### Comparing `psycopg-3.1.8/psycopg/types/none.py` & `psycopg-3.1.9/psycopg/types/none.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/types/numeric.py` & `psycopg-3.1.9/psycopg/types/numeric.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 
     def quote(self, obj: Any) -> Buffer:
         value = self.dump(obj)
         return value if obj >= 0 else b" " + value
 
 
 class _SpecialValuesDumper(Dumper):
-
     _special: Dict[bytes, bytes] = {}
 
     def dump(self, obj: Any) -> bytes:
         return str(obj).encode()
 
     def quote(self, obj: Any) -> bytes:
         value = self.dump(obj)
@@ -61,47 +60,43 @@
         if value in self._special:
             return self._special[value]
 
         return value if obj >= 0 else b" " + value
 
 
 class FloatDumper(_SpecialValuesDumper):
-
     oid = postgres.types["float8"].oid
 
     _special = {
         b"inf": b"'Infinity'::float8",
         b"-inf": b"'-Infinity'::float8",
         b"nan": b"'NaN'::float8",
     }
 
 
 class Float4Dumper(FloatDumper):
     oid = postgres.types["float4"].oid
 
 
 class FloatBinaryDumper(Dumper):
-
     format = Format.BINARY
     oid = postgres.types["float8"].oid
 
     def dump(self, obj: float) -> bytes:
         return pack_float8(obj)
 
 
 class Float4BinaryDumper(FloatBinaryDumper):
-
     oid = postgres.types["float4"].oid
 
     def dump(self, obj: float) -> bytes:
         return pack_float4(obj)
 
 
 class DecimalDumper(_SpecialValuesDumper):
-
     oid = postgres.types["numeric"].oid
 
     def dump(self, obj: Decimal) -> bytes:
         if obj.is_nan():
             # cover NaN and sNaN
             return b"NaN"
         else:
@@ -159,60 +154,54 @@
             if -(2**63) <= obj < 2**63:
                 return self._int8_dumper
             else:
                 return self._int_numeric_dumper
 
 
 class Int2BinaryDumper(Int2Dumper):
-
     format = Format.BINARY
 
     def dump(self, obj: int) -> bytes:
         return pack_int2(obj)
 
 
 class Int4BinaryDumper(Int4Dumper):
-
     format = Format.BINARY
 
     def dump(self, obj: int) -> bytes:
         return pack_int4(obj)
 
 
 class Int8BinaryDumper(Int8Dumper):
-
     format = Format.BINARY
 
     def dump(self, obj: int) -> bytes:
         return pack_int8(obj)
 
 
 # Ratio between number of bits required to store a number and number of pg
 # decimal digits required.
 BIT_PER_PGDIGIT = log(2) / log(10_000)
 
 
 class IntNumericBinaryDumper(IntNumericDumper):
-
     format = Format.BINARY
 
     def dump(self, obj: int) -> Buffer:
         return dump_int_to_numeric_binary(obj)
 
 
 class OidBinaryDumper(OidDumper):
-
     format = Format.BINARY
 
     def dump(self, obj: int) -> bytes:
         return pack_uint4(obj)
 
 
 class IntBinaryDumper(IntDumper):
-
     format = Format.BINARY
 
     _int2_dumper = Int2BinaryDumper(Int2)
     _int4_dumper = Int4BinaryDumper(Int4)
     _int8_dumper = Int8BinaryDumper(Int8)
     _int_numeric_dumper = IntNumericBinaryDumper(IntNumeric)
 
@@ -220,61 +209,55 @@
 class IntLoader(Loader):
     def load(self, data: Buffer) -> int:
         # it supports bytes directly
         return int(data)
 
 
 class Int2BinaryLoader(Loader):
-
     format = Format.BINARY
 
     def load(self, data: Buffer) -> int:
         return unpack_int2(data)[0]
 
 
 class Int4BinaryLoader(Loader):
-
     format = Format.BINARY
 
     def load(self, data: Buffer) -> int:
         return unpack_int4(data)[0]
 
 
 class Int8BinaryLoader(Loader):
-
     format = Format.BINARY
 
     def load(self, data: Buffer) -> int:
         return unpack_int8(data)[0]
 
 
 class OidBinaryLoader(Loader):
-
     format = Format.BINARY
 
     def load(self, data: Buffer) -> int:
         return unpack_uint4(data)[0]
 
 
 class FloatLoader(Loader):
     def load(self, data: Buffer) -> float:
         # it supports bytes directly
         return float(data)
 
 
 class Float4BinaryLoader(Loader):
-
     format = Format.BINARY
 
     def load(self, data: Buffer) -> float:
         return unpack_float4(data)[0]
 
 
 class Float8BinaryLoader(Loader):
-
     format = Format.BINARY
 
     def load(self, data: Buffer) -> float:
         return unpack_float8(data)[0]
 
 
 class NumericLoader(Loader):
@@ -327,15 +310,14 @@
 _pack_numeric_head = cast(
     Callable[[int, int, int, int], bytes],
     struct.Struct("!HhHH").pack,
 )
 
 
 class NumericBinaryLoader(Loader):
-
     format = Format.BINARY
 
     def load(self, data: Buffer) -> Decimal:
         ndigits, weight, sign, dscale = _unpack_numeric_head(data)
         if sign == NUMERIC_POS or sign == NUMERIC_NEG:
             val = 0
             for i in range(8, len(data), 2):
@@ -357,15 +339,14 @@
 
 NUMERIC_NAN_BIN = _pack_numeric_head(0, 0, NUMERIC_NAN, 0)
 NUMERIC_PINF_BIN = _pack_numeric_head(0, 0, NUMERIC_PINF, 0)
 NUMERIC_NINF_BIN = _pack_numeric_head(0, 0, NUMERIC_NINF, 0)
 
 
 class DecimalBinaryDumper(Dumper):
-
     format = Format.BINARY
     oid = postgres.types["numeric"].oid
 
     def dump(self, obj: Decimal) -> Buffer:
         return dump_decimal_to_numeric_binary(obj)
 
 
@@ -374,30 +355,29 @@
         if isinstance(obj, int):
             return str(obj).encode()
         else:
             return super().dump(obj)
 
 
 class NumericBinaryDumper(Dumper):
-
     format = Format.BINARY
     oid = postgres.types["numeric"].oid
 
     def dump(self, obj: Union[Decimal, int]) -> Buffer:
         if isinstance(obj, int):
             return dump_int_to_numeric_binary(obj)
         else:
             return dump_decimal_to_numeric_binary(obj)
 
 
 def dump_decimal_to_numeric_binary(obj: Decimal) -> Union[bytearray, bytes]:
     sign, digits, exp = obj.as_tuple()
-    if exp == "n" or exp == "N":  # type: ignore[comparison-overlap]
+    if exp == "n" or exp == "N":
         return NUMERIC_NAN_BIN
-    elif exp == "F":  # type: ignore[comparison-overlap]
+    elif exp == "F":
         return NUMERIC_NINF_BIN if sign else NUMERIC_PINF_BIN
 
     # Weights of py digits into a pg digit according to their positions.
     # Starting with an index wi != 0 is equivalent to prepending 0's to
     # the digits tuple, but without really changing it.
     weights = (1000, 100, 10, 1)
     wi = 0
```

### Comparing `psycopg-3.1.8/psycopg/types/range.py` & `psycopg-3.1.9/psycopg/types/range.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,15 +354,14 @@
 
 
 _re_needs_quotes = re.compile(rb'[",\\\s()\[\]]')
 _re_esc = re.compile(rb"([\\\"])")
 
 
 class RangeBinaryDumper(BaseRangeDumper):
-
     format = Format.BINARY
 
     def dump(self, obj: Range[Any]) -> Buffer:
         item = self._get_item(obj)
         if item is not None:
             dump = self._tx.get_dumper(item, self._adapt_format).dump
         else:
@@ -475,15 +474,14 @@
     re.VERBOSE,
 )
 
 _re_undouble = re.compile(rb'(["\\])\1')
 
 
 class RangeBinaryLoader(BaseRangeLoader[T]):
-
     format = Format.BINARY
 
     def load(self, data: Buffer) -> Range[T]:
         return load_range_binary(data, self._load)
 
 
 def load_range_binary(data: Buffer, load: Callable[[Buffer], Any]) -> Range[Any]:
```

### Comparing `psycopg-3.1.8/psycopg/types/shapely.py` & `psycopg-3.1.9/psycopg/types/shapely.py`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/psycopg/types/string.py` & `psycopg-3.1.9/psycopg/types/string.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,25 +52,22 @@
             return obj.encode(self._encoding)
 
 
 # The next are concrete dumpers, each one specifying the oid they dump to.
 
 
 class StrBinaryDumper(_StrBinaryDumper):
-
     oid = postgres.types["text"].oid
 
 
 class StrBinaryDumperVarchar(_StrBinaryDumper):
-
     oid = postgres.types["varchar"].oid
 
 
 class StrBinaryDumperName(_StrBinaryDumper):
-
     oid = postgres.types["name"].oid
 
 
 class StrDumper(_StrDumper):
     """
     Dumper for strings in text format to the text oid.
 
@@ -80,20 +77,18 @@
     text oid is required, for instance with variadic functions.
     """
 
     oid = postgres.types["text"].oid
 
 
 class StrDumperVarchar(_StrDumper):
-
     oid = postgres.types["varchar"].oid
 
 
 class StrDumperName(_StrDumper):
-
     oid = postgres.types["name"].oid
 
 
 class StrDumperUnknown(_StrDumper):
     """
     Dumper for strings in text format to the unknown oid.
 
@@ -122,20 +117,18 @@
             # return bytes for SQL_ASCII db
             if not isinstance(data, bytes):
                 data = bytes(data)
             return data
 
 
 class TextBinaryLoader(TextLoader):
-
     format = Format.BINARY
 
 
 class BytesDumper(Dumper):
-
     oid = postgres.types["bytea"].oid
     _qprefix = b""
 
     def __init__(self, cls: type, context: Optional[AdaptContext] = None):
         super().__init__(cls, context)
         self._esc = Escaping(self.connection.pgconn if self.connection else None)
 
@@ -165,37 +158,34 @@
         rv: bytes = b" E'" + escaped + b"'"
         if self._esc.escape_bytea(b"\x00") == b"\\000":
             rv = rv.replace(b"\\", b"\\\\")
         return rv
 
 
 class BytesBinaryDumper(Dumper):
-
     format = Format.BINARY
     oid = postgres.types["bytea"].oid
 
     def dump(self, obj: Buffer) -> Buffer:
         return obj
 
 
 class ByteaLoader(Loader):
-
     _escaping: "EscapingProto"
 
     def __init__(self, oid: int, context: Optional[AdaptContext] = None):
         super().__init__(oid, context)
         if not hasattr(self.__class__, "_escaping"):
             self.__class__._escaping = Escaping()
 
     def load(self, data: Buffer) -> bytes:
         return self._escaping.unescape_bytea(data)
 
 
 class ByteaBinaryLoader(Loader):
-
     format = Format.BINARY
 
     def load(self, data: Buffer) -> Buffer:
         return data
 
 
 def register_default_adapters(context: AdaptContext) -> None:
```

### Comparing `psycopg-3.1.8/psycopg/types/uuid.py` & `psycopg-3.1.9/psycopg/types/uuid.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,23 +15,21 @@
     import uuid
 
 # Importing the uuid module is slow, so import it only on request.
 UUID: Callable[..., "uuid.UUID"] = None  # type: ignore[assignment]
 
 
 class UUIDDumper(Dumper):
-
     oid = postgres.types["uuid"].oid
 
     def dump(self, obj: "uuid.UUID") -> bytes:
         return obj.hex.encode()
 
 
 class UUIDBinaryDumper(UUIDDumper):
-
     format = Format.BINARY
 
     def dump(self, obj: "uuid.UUID") -> bytes:
         return obj.bytes
 
 
 class UUIDLoader(Loader):
@@ -44,15 +42,14 @@
     def load(self, data: Buffer) -> "uuid.UUID":
         if isinstance(data, memoryview):
             data = bytes(data)
         return UUID(data.decode())
 
 
 class UUIDBinaryLoader(UUIDLoader):
-
     format = Format.BINARY
 
     def load(self, data: Buffer) -> "uuid.UUID":
         if isinstance(data, memoryview):
             data = bytes(data)
         return UUID(bytes=data)
```

### Comparing `psycopg-3.1.8/psycopg/waiting.py` & `psycopg-3.1.9/psycopg/waiting.py`

 * *Files 7% similar despite different names*

```diff
@@ -314,18 +314,11 @@
     wait = wait_c
 
 elif selectors.DefaultSelector is getattr(selectors, "SelectSelector", None):
     # On Windows, SelectSelector should be the default.
     wait = wait_select
 
 elif selectors.DefaultSelector is getattr(selectors, "EpollSelector", None):
-    # NOTE: select seems more performing than epoll. It is admittedly unlikely
-    # that a platform has epoll but not select, so maybe we could kill
-    # wait_epoll altogether(). More testing to do.
-    wait = wait_select if hasattr(selectors, "SelectSelector") else wait_epoll
-
-elif selectors.DefaultSelector is getattr(selectors, "KqueueSelector", None):
-    # wait_select is faster than wait_selector, probably because of less overhead
-    wait = wait_select if hasattr(selectors, "SelectSelector") else wait_selector
+    wait = wait_epoll
 
 else:
     wait = wait_selector
```

### Comparing `psycopg-3.1.8/psycopg.egg-info/PKG-INFO` & `psycopg-3.1.9/psycopg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psycopg
-Version: 3.1.8
+Version: 3.1.9
 Summary: PostgreSQL database adapter for Python
 Home-page: https://psycopg.org/psycopg3/
 Author: Daniele Varrazzo
 Author-email: daniele.varrazzo@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Homepage, https://psycopg.org/
 Project-URL: Documentation, https://psycopg.org/psycopg3/docs/
```

### Comparing `psycopg-3.1.8/psycopg.egg-info/SOURCES.txt` & `psycopg-3.1.9/psycopg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psycopg-3.1.8/setup.cfg` & `psycopg-3.1.9/setup.cfg`

 * *Files identical despite different names*

