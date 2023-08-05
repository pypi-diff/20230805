# Comparing `tmp/psycopg2-binary-2.9.5.tar.gz` & `tmp/psycopg2-binary-2.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psycopg2-binary-2.9.5.tar", last modified: Tue Oct 25 11:05:46 2022, max compression
+gzip compressed data, was "psycopg2-binary-2.9.6.tar", last modified: Sun Apr  2 15:59:22 2023, max compression
```

## Comparing `psycopg2-binary-2.9.5.tar` & `psycopg2-binary-2.9.6.tar`

### file list

```diff
@@ -1,192 +1,191 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 11:05:46.208019 psycopg2-binary-2.9.5/
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/INSTALL
--rw-r--r--   0 runner    (1001) docker     (121)     2238 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2542 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)    55157 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/NEWS
--rw-r--r--   0 runner    (1001) docker     (121)     4995 2022-10-25 11:05:46.208019 psycopg2-binary-2.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2815 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 11:05:46.188019 psycopg2-binary-2.9.5/doc/
--rw-r--r--   0 runner    (1001) docker     (121)     7637 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      628 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4178 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/SUCCESS
--rw-r--r--   0 runner    (1001) docker     (121)    39154 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/pep-0249.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1140 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 11:05:46.188019 psycopg2-binary-2.9.5/doc/src/
--rw-r--r--   0 runner    (1001) docker     (121)     3388 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/src/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 11:05:46.188019 psycopg2-binary-2.9.5/doc/src/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     1784 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/src/_static/psycopg.css
--rw-r--r--   0 runner    (1001) docker     (121)    22425 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/src/advanced.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8766 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/src/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)    34747 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/src/connection.rst
--rw-r--r--   0 runner    (1001) docker     (121)    24529 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/src/cursor.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2514 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/src/errorcodes.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3169 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/src/errors.rst
--rw-r--r--   0 runner    (1001) docker     (121)    33077 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/src/extensions.rst
--rw-r--r--   0 runner    (1001) docker     (121)    36950 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/src/extras.rst
--rw-r--r--   0 runner    (1001) docker     (121)    14989 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/src/faq.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1894 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/src/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11582 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/src/install.rst
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/src/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13348 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/src/module.rst
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/src/news.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1866 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/src/pool.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4702 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/src/sql.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 11:05:46.188019 psycopg2-binary-2.9.5/doc/src/tools/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 11:05:46.188019 psycopg2-binary-2.9.5/doc/src/tools/lib/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1338 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/src/tools/lib/dbapi_extension.py
--rw-r--r--   0 runner    (1001) docker     (121)      500 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/src/tools/lib/sql_role.py
--rw-r--r--   0 runner    (1001) docker     (121)     1828 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/src/tools/lib/ticket_role.py
--rw-r--r--   0 runner    (1001) docker     (121)     1520 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/src/tools/make_sqlstate_docs.py
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/src/tz.rst
--rw-r--r--   0 runner    (1001) docker     (121)    42328 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/doc/src/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 11:05:46.192019 psycopg2-binary-2.9.5/lib/
--rw-r--r--   0 runner    (1001) docker     (121)     4768 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2922 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/lib/_ipaddress.py
--rw-r--r--   0 runner    (1001) docker     (121)     7153 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/lib/_json.py
--rw-r--r--   0 runner    (1001) docker     (121)    18494 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/lib/_range.py
--rw-r--r--   0 runner    (1001) docker     (121)    14362 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/lib/errorcodes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1425 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/lib/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     6797 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/lib/extensions.py
--rw-r--r--   0 runner    (1001) docker     (121)    44215 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/lib/extras.py
--rw-r--r--   0 runner    (1001) docker     (121)     6316 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/lib/pool.py
--rw-r--r--   0 runner    (1001) docker     (121)    14779 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/lib/sql.py
--rw-r--r--   0 runner    (1001) docker     (121)     4870 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/lib/tz.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 11:05:46.200019 psycopg2-binary-2.9.5/psycopg/
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/_psycopg.vc9.amd64.manifest
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/_psycopg.vc9.x86.manifest
--rw-r--r--   0 runner    (1001) docker     (121)     4928 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/adapter_asis.c
--rw-r--r--   0 runner    (1001) docker     (121)     1428 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/adapter_asis.h
--rw-r--r--   0 runner    (1001) docker     (121)     7399 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/adapter_binary.c
--rw-r--r--   0 runner    (1001) docker     (121)     1425 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/adapter_binary.h
--rw-r--r--   0 runner    (1001) docker     (121)    13521 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/adapter_datetime.c
--rw-r--r--   0 runner    (1001) docker     (121)     4018 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/adapter_datetime.h
--rw-r--r--   0 runner    (1001) docker     (121)     9352 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/adapter_list.c
--rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/adapter_list.h
--rw-r--r--   0 runner    (1001) docker     (121)     4912 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/adapter_pboolean.c
--rw-r--r--   0 runner    (1001) docker     (121)     1455 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/adapter_pboolean.h
--rw-r--r--   0 runner    (1001) docker     (121)     6472 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/adapter_pdecimal.c
--rw-r--r--   0 runner    (1001) docker     (121)     1455 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/adapter_pdecimal.h
--rw-r--r--   0 runner    (1001) docker     (121)     5757 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/adapter_pfloat.c
--rw-r--r--   0 runner    (1001) docker     (121)     1441 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/adapter_pfloat.h
--rw-r--r--   0 runner    (1001) docker     (121)     5663 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/adapter_pint.c
--rw-r--r--   0 runner    (1001) docker     (121)     1435 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/adapter_pint.h
--rw-r--r--   0 runner    (1001) docker     (121)     8185 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/adapter_qstring.c
--rw-r--r--   0 runner    (1001) docker     (121)     1474 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/adapter_qstring.h
--rw-r--r--   0 runner    (1001) docker     (121)     1854 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/aix_support.c
--rw-r--r--   0 runner    (1001) docker     (121)     1677 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/aix_support.h
--rw-r--r--   0 runner    (1001) docker     (121)    11046 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/bytes_format.c
--rw-r--r--   0 runner    (1001) docker     (121)     1540 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/column.h
--rw-r--r--   0 runner    (1001) docker     (121)    12071 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/column_type.c
--rw-r--r--   0 runner    (1001) docker     (121)     6468 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/config.h
--rw-r--r--   0 runner    (1001) docker     (121)     8892 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/connection.h
--rw-r--r--   0 runner    (1001) docker     (121)    40966 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/connection_int.c
--rw-r--r--   0 runner    (1001) docker     (121)    43102 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/connection_type.c
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/conninfo.h
--rw-r--r--   0 runner    (1001) docker     (121)    17795 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/conninfo_type.c
--rw-r--r--   0 runner    (1001) docker     (121)     5501 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/cursor.h
--rw-r--r--   0 runner    (1001) docker     (121)     4808 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/cursor_int.c
--rw-r--r--   0 runner    (1001) docker     (121)    59927 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/cursor_type.c
--rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/diagnostics.h
--rw-r--r--   0 runner    (1001) docker     (121)     7095 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/diagnostics_type.c
--rw-r--r--   0 runner    (1001) docker     (121)     1646 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/error.h
--rw-r--r--   0 runner    (1001) docker     (121)    11429 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/error_type.c
--rw-r--r--   0 runner    (1001) docker     (121)     5995 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/green.c
--rw-r--r--   0 runner    (1001) docker     (121)     2781 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/green.h
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/libpq_support.c
--rw-r--r--   0 runner    (1001) docker     (121)     1908 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/libpq_support.h
--rw-r--r--   0 runner    (1001) docker     (121)     3719 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/lobject.h
--rw-r--r--   0 runner    (1001) docker     (121)    11996 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/lobject_int.c
--rw-r--r--   0 runner    (1001) docker     (121)    12549 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/lobject_type.c
--rw-r--r--   0 runner    (1001) docker     (121)     8137 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/microprotocols.c
--rw-r--r--   0 runner    (1001) docker     (121)     2247 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/microprotocols.h
--rw-r--r--   0 runner    (1001) docker     (121)     4853 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/microprotocols_proto.c
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/microprotocols_proto.h
--rw-r--r--   0 runner    (1001) docker     (121)     1348 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/notify.h
--rw-r--r--   0 runner    (1001) docker     (121)     9059 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/notify_type.c
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/pgtypes.h
--rw-r--r--   0 runner    (1001) docker     (121)    53540 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/pqpath.c
--rw-r--r--   0 runner    (1001) docker     (121)     3489 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/pqpath.h
--rw-r--r--   0 runner    (1001) docker     (121)     3113 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/psycopg.h
--rw-r--r--   0 runner    (1001) docker     (121)    31621 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/psycopgmodule.c
--rw-r--r--   0 runner    (1001) docker     (121)     3455 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/python.h
--rw-r--r--   0 runner    (1001) docker     (121)     1753 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/replication_connection.h
--rw-r--r--   0 runner    (1001) docker     (121)     6580 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/replication_connection_type.c
--rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/replication_cursor.h
--rw-r--r--   0 runner    (1001) docker     (121)    12012 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/replication_cursor_type.c
--rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/replication_message.h
--rw-r--r--   0 runner    (1001) docker     (121)     5606 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/replication_message_type.c
--rw-r--r--   0 runner    (1001) docker     (121)     1918 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/solaris_support.c
--rw-r--r--   0 runner    (1001) docker     (121)     1723 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/solaris_support.h
--rw-r--r--   0 runner    (1001) docker     (121)    11103 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/sqlstate_errors.h
--rw-r--r--   0 runner    (1001) docker     (121)    17651 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/typecast.c
--rw-r--r--   0 runner    (1001) docker     (121)     3172 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/typecast.h
--rw-r--r--   0 runner    (1001) docker     (121)     8944 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/typecast_array.c
--rw-r--r--   0 runner    (1001) docker     (121)     4146 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/typecast_basic.c
--rw-r--r--   0 runner    (1001) docker     (121)     8647 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/typecast_binary.c
--rw-r--r--   0 runner    (1001) docker     (121)     1533 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/typecast_binary.h
--rw-r--r--   0 runner    (1001) docker     (121)     4615 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/typecast_builtins.c
--rw-r--r--   0 runner    (1001) docker     (121)    14285 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/typecast_datetime.c
--rw-r--r--   0 runner    (1001) docker     (121)    11786 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/utils.c
--rw-r--r--   0 runner    (1001) docker     (121)     2336 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/utils.h
--rw-r--r--   0 runner    (1001) docker     (121)     2739 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/win32_support.c
--rw-r--r--   0 runner    (1001) docker     (121)     1804 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/win32_support.h
--rw-r--r--   0 runner    (1001) docker     (121)     1775 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/xid.h
--rw-r--r--   0 runner    (1001) docker     (121)    19411 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/psycopg/xid_type.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 11:05:46.200019 psycopg2-binary-2.9.5/psycopg2_binary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4995 2022-10-25 11:05:46.000000 psycopg2-binary-2.9.5/psycopg2_binary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4065 2022-10-25 11:05:46.000000 psycopg2-binary-2.9.5/psycopg2_binary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 11:05:46.000000 psycopg2-binary-2.9.5/psycopg2_binary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-25 11:05:46.000000 psycopg2-binary-2.9.5/psycopg2_binary.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 11:05:46.200019 psycopg2-binary-2.9.5/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 11:05:46.200019 psycopg2-binary-2.9.5/scripts/build/
--rwxr-xr-x   0 runner    (1001) docker     (121)    22465 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/scripts/build/appveyor.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3453 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/scripts/build/build_libpq.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     2552 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/scripts/build/build_macos.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     2686 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/scripts/build/build_macos_arm64.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     2446 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/scripts/build/build_manylinux2014.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     2457 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/scripts/build/build_manylinux_2_24.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     2157 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/scripts/build/build_musllinux_1_1.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      695 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/scripts/build/build_sdist.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     3310 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/scripts/build/download_packages_appveyor.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2876 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/scripts/build/download_packages_github.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1034 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/scripts/build/run_build_macos_arm64.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      960 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/scripts/build/strip_wheel.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     4608 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/scripts/make_errorcodes.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4246 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/scripts/make_errors.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3175 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/scripts/refcounter.py
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-10-25 11:05:46.208019 psycopg2-binary-2.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    20993 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 11:05:46.208019 psycopg2-binary-2.9.5/tests/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3601 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31821 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/dbapi20.py
--rw-r--r--   0 runner    (1001) docker     (121)     4137 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/dbapi20_tpc.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    17918 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/test_async.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1783 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/test_bugX000.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1766 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/test_bug_gc.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3725 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/test_cancel.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    69373 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/test_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12640 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/test_copy.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    26173 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/test_cursor.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    23357 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/test_dates.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2524 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/test_errcodes.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3216 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/test_errors.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    24065 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/test_extras_dictcursor.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10495 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/test_fast_executemany.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8396 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/test_green.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4326 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/test_ipaddress.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15473 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/test_lobject.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12365 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/test_module.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7899 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/test_notify.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2928 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/test_psycopg2_dbapi20.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8189 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/test_quote.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9058 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/test_replication.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15970 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/test_sql.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9432 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/test_transaction.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    17765 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/test_types_basic.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    60114 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/test_types_extras.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10515 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/test_with.py
--rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/testconfig.py
--rw-r--r--   0 runner    (1001) docker     (121)    16688 2022-10-25 11:05:45.000000 psycopg2-binary-2.9.5/tests/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:59:22.273957 psycopg2-binary-2.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    55397 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/NEWS
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-04-02 15:59:22.273957 psycopg2-binary-2.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:59:22.257957 psycopg2-binary-2.9.6/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/SUCCESS
+-rw-r--r--   0 runner    (1001) docker     (123)    39154 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/pep-0249.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:59:22.257957 psycopg2-binary-2.9.6/doc/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/src/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:59:22.257957 psycopg2-binary-2.9.6/doc/src/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/src/_static/psycopg.css
+-rw-r--r--   0 runner    (1001) docker     (123)    22425 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/src/advanced.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8766 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/src/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34747 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/src/connection.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    24529 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/src/cursor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/src/errorcodes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/src/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    33077 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/src/extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    36950 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/src/extras.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14989 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/src/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/src/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11582 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/src/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/src/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/src/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/src/news.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/src/pool.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/src/sql.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:59:22.257957 psycopg2-binary-2.9.6/doc/src/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:59:22.257957 psycopg2-binary-2.9.6/doc/src/tools/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1338 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/src/tools/lib/dbapi_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/src/tools/lib/sql_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/src/tools/lib/ticket_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/src/tools/make_sqlstate_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/src/tz.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    42328 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/doc/src/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:59:22.261957 psycopg2-binary-2.9.6/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/lib/_ipaddress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/lib/_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18494 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/lib/_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14362 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/lib/errorcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/lib/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/lib/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44215 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/lib/extras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/lib/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/lib/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/lib/tz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:59:22.269956 psycopg2-binary-2.9.6/psycopg/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/_psycopg.vc9.amd64.manifest
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/_psycopg.vc9.x86.manifest
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/adapter_asis.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/adapter_asis.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/adapter_binary.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/adapter_binary.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/adapter_datetime.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/adapter_datetime.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/adapter_list.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/adapter_list.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/adapter_pboolean.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/adapter_pboolean.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/adapter_pdecimal.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/adapter_pdecimal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/adapter_pfloat.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/adapter_pfloat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/adapter_pint.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/adapter_pint.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/adapter_qstring.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/adapter_qstring.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/aix_support.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/aix_support.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/bytes_format.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/column.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/column_type.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/config.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/connection.h
+-rw-r--r--   0 runner    (1001) docker     (123)    40966 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/connection_int.c
+-rw-r--r--   0 runner    (1001) docker     (123)    43102 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/connection_type.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/conninfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17795 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/conninfo_type.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/cursor.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/cursor_int.c
+-rw-r--r--   0 runner    (1001) docker     (123)    59927 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/cursor_type.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/diagnostics.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/diagnostics_type.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/error.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/error_type.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/green.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/green.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/libpq_support.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/libpq_support.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/lobject.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/lobject_int.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12549 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/lobject_type.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/microprotocols.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/microprotocols.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/microprotocols_proto.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/microprotocols_proto.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/notify.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/notify_type.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/pgtypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)    53540 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/pqpath.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/pqpath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/psycopg.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31621 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/psycopgmodule.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/python.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/replication_connection.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/replication_connection_type.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/replication_cursor.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12012 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/replication_cursor_type.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/replication_message.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/replication_message_type.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/solaris_support.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/solaris_support.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11103 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/sqlstate_errors.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17651 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/typecast.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/typecast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/typecast_array.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/typecast_basic.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/typecast_binary.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/typecast_binary.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/typecast_builtins.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14285 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/typecast_datetime.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/win32_support.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/win32_support.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/xid.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19411 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/psycopg/xid_type.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:59:22.269956 psycopg2-binary-2.9.6/psycopg2_binary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-04-02 15:59:22.000000 psycopg2-binary-2.9.6/psycopg2_binary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-04-02 15:59:22.000000 psycopg2-binary-2.9.6/psycopg2_binary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 15:59:22.000000 psycopg2-binary-2.9.6/psycopg2_binary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-02 15:59:22.000000 psycopg2-binary-2.9.6/psycopg2_binary.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:59:22.269956 psycopg2-binary-2.9.6/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:59:22.269956 psycopg2-binary-2.9.6/scripts/build/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22554 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/scripts/build/appveyor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4686 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/scripts/build/build_libpq.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2839 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/scripts/build/build_macos_arm64.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      677 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/scripts/build/build_sdist.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3310 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/scripts/build/download_packages_appveyor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2876 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/scripts/build/download_packages_github.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      938 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/scripts/build/print_so_versions.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1034 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/scripts/build/run_build_macos_arm64.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1221 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/scripts/build/strip_wheel.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1555 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/scripts/build/wheel_linux_before_all.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      822 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/scripts/build/wheel_macos_before_all.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4608 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/scripts/make_errorcodes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4246 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/scripts/make_errors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3175 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/scripts/refcounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-02 15:59:22.273957 psycopg2-binary-2.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    20993 2023-04-02 15:59:22.000000 psycopg2-binary-2.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:59:22.273957 psycopg2-binary-2.9.6/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3601 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31821 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/dbapi20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/dbapi20_tpc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17918 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/test_async.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1783 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/test_bugX000.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1766 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/test_bug_gc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3725 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/test_cancel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    69373 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/test_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12640 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/test_copy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26173 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/test_cursor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23357 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/test_dates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2524 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/test_errcodes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3216 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/test_errors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24065 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/test_extras_dictcursor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10495 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/test_fast_executemany.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8396 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/test_green.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4326 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/test_ipaddress.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15473 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/test_lobject.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12365 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/test_module.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7899 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/test_notify.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2928 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/test_psycopg2_dbapi20.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8189 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/test_quote.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9058 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/test_replication.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15970 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/test_sql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9432 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/test_transaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17765 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/test_types_basic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    60114 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/test_types_extras.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10515 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/test_with.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/testconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16688 2023-04-02 15:59:21.000000 psycopg2-binary-2.9.6/tests/testutils.py
```

### Comparing `psycopg2-binary-2.9.5/LICENSE` & `psycopg2-binary-2.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/Makefile` & `psycopg2-binary-2.9.6/Makefile`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/NEWS` & `psycopg2-binary-2.9.6/NEWS`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Current release
 ---------------
 
+What's new in psycopg 2.9.6
+^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+- Package manylinux 2014 for aarch64 and ppc64le platforms, in order to
+  include libpq 15 in the binary package (:ticket:`#1396`).
+- Wheel package compiled against OpenSSL 1.1.1t.
+
+
 What's new in psycopg 2.9.5
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 - Add support for Python 3.11.
 - Add support for rowcount in MERGE statements in binary packages
   (:ticket:`#1497`).
 - Wheel package compiled against OpenSSL 1.1.1r and PostgreSQL 15 libpq.
```

### Comparing `psycopg2-binary-2.9.5/PKG-INFO` & `psycopg2-binary-2.9.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,93 +1,22 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: psycopg2-binary
-Version: 2.9.5
+Version: 2.9.6
 Summary: psycopg2 - Python-PostgreSQL Database Adapter
 Home-page: https://psycopg.org/
 Author: Federico Di Gregorio
 Author-email: fog@initd.org
 Maintainer: Daniele Varrazzo
 Maintainer-email: daniele.varrazzo@gmail.com
 License: LGPL with exceptions
 Project-URL: Homepage, https://psycopg.org/
 Project-URL: Documentation, https://www.psycopg.org/docs/
 Project-URL: Code, https://github.com/psycopg/psycopg2
 Project-URL: Issue Tracker, https://github.com/psycopg/psycopg2/issues
 Project-URL: Download, https://pypi.org/project/psycopg2/
-Description: Psycopg is the most popular PostgreSQL database adapter for the Python
-        programming language.  Its main features are the complete implementation of
-        the Python DB API 2.0 specification and the thread safety (several threads can
-        share the same connection).  It was designed for heavily multi-threaded
-        applications that create and destroy lots of cursors and make a large number
-        of concurrent "INSERT"s or "UPDATE"s.
-        
-        Psycopg 2 is mostly implemented in C as a libpq wrapper, resulting in being
-        both efficient and secure.  It features client-side and server-side cursors,
-        asynchronous communication and notifications, "COPY TO/COPY FROM" support.
-        Many Python types are supported out-of-the-box and adapted to matching
-        PostgreSQL data types; adaptation can be extended and customized thanks to a
-        flexible objects adaptation system.
-        
-        Psycopg 2 is both Unicode and Python 3 friendly.
-        
-        
-        Documentation
-        -------------
-        
-        Documentation is included in the ``doc`` directory and is `available online`__.
-        
-        .. __: https://www.psycopg.org/docs/
-        
-        For any other resource (source code repository, bug tracker, mailing list)
-        please check the `project homepage`__.
-        
-        .. __: https://psycopg.org/
-        
-        
-        Installation
-        ------------
-        
-        Building Psycopg requires a few prerequisites (a C compiler, some development
-        packages): please check the install_ and the faq_ documents in the ``doc`` dir
-        or online for the details.
-        
-        If prerequisites are met, you can install psycopg like any other Python
-        package, using ``pip`` to download it from PyPI_::
-        
-            $ pip install psycopg2
-        
-        or using ``setup.py`` if you have downloaded the source package locally::
-        
-            $ python setup.py build
-            $ sudo python setup.py install
-        
-        You can also obtain a stand-alone package, not requiring a compiler or
-        external libraries, by installing the `psycopg2-binary`_ package from PyPI::
-        
-            $ pip install psycopg2-binary
-        
-        The binary package is a practical choice for development and testing but in
-        production it is advised to use the package built from sources.
-        
-        .. _PyPI: https://pypi.org/project/psycopg2/
-        .. _psycopg2-binary: https://pypi.org/project/psycopg2-binary/
-        .. _install: https://www.psycopg.org/docs/install.html#install-from-source
-        .. _faq: https://www.psycopg.org/docs/faq.html#faq-compile
-        
-        :Linux/OSX: |gh-actions|
-        :Windows: |appveyor|
-        
-        .. |gh-actions| image:: https://github.com/psycopg/psycopg2/actions/workflows/tests.yml/badge.svg
-            :target: https://github.com/psycopg/psycopg2/actions/workflows/tests.yml
-            :alt: Linux and OSX build status
-        
-        .. |appveyor| image:: https://ci.appveyor.com/api/projects/status/github/psycopg/psycopg2?branch=master&svg=true
-            :target: https://ci.appveyor.com/project/psycopg/psycopg2/branch/master
-            :alt: Windows build status
-        
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -103,7 +32,81 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Requires-Python: >=3.6
+License-File: LICENSE
+
+Psycopg is the most popular PostgreSQL database adapter for the Python
+programming language.  Its main features are the complete implementation of
+the Python DB API 2.0 specification and the thread safety (several threads can
+share the same connection).  It was designed for heavily multi-threaded
+applications that create and destroy lots of cursors and make a large number
+of concurrent "INSERT"s or "UPDATE"s.
+
+Psycopg 2 is mostly implemented in C as a libpq wrapper, resulting in being
+both efficient and secure.  It features client-side and server-side cursors,
+asynchronous communication and notifications, "COPY TO/COPY FROM" support.
+Many Python types are supported out-of-the-box and adapted to matching
+PostgreSQL data types; adaptation can be extended and customized thanks to a
+flexible objects adaptation system.
+
+Psycopg 2 is both Unicode and Python 3 friendly.
+
+
+Documentation
+-------------
+
+Documentation is included in the ``doc`` directory and is `available online`__.
+
+.. __: https://www.psycopg.org/docs/
+
+For any other resource (source code repository, bug tracker, mailing list)
+please check the `project homepage`__.
+
+.. __: https://psycopg.org/
+
+
+Installation
+------------
+
+Building Psycopg requires a few prerequisites (a C compiler, some development
+packages): please check the install_ and the faq_ documents in the ``doc`` dir
+or online for the details.
+
+If prerequisites are met, you can install psycopg like any other Python
+package, using ``pip`` to download it from PyPI_::
+
+    $ pip install psycopg2
+
+or using ``setup.py`` if you have downloaded the source package locally::
+
+    $ python setup.py build
+    $ sudo python setup.py install
+
+You can also obtain a stand-alone package, not requiring a compiler or
+external libraries, by installing the `psycopg2-binary`_ package from PyPI::
+
+    $ pip install psycopg2-binary
+
+The binary package is a practical choice for development and testing but in
+production it is advised to use the package built from sources.
+
+.. _PyPI: https://pypi.org/project/psycopg2/
+.. _psycopg2-binary: https://pypi.org/project/psycopg2-binary/
+.. _install: https://www.psycopg.org/docs/install.html#install-from-source
+.. _faq: https://www.psycopg.org/docs/faq.html#faq-compile
+
+:Linux/OSX: |gh-actions|
+:Windows: |appveyor|
+
+.. |gh-actions| image:: https://github.com/psycopg/psycopg2/actions/workflows/tests.yml/badge.svg
+    :target: https://github.com/psycopg/psycopg2/actions/workflows/tests.yml
+    :alt: Linux and OSX build status
+
+.. |appveyor| image:: https://ci.appveyor.com/api/projects/status/github/psycopg/psycopg2?branch=master&svg=true
+    :target: https://ci.appveyor.com/project/psycopg/psycopg2/branch/master
+    :alt: Windows build status
+
+
```

### Comparing `psycopg2-binary-2.9.5/README.rst` & `psycopg2-binary-2.9.6/README.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/COPYING.LESSER` & `psycopg2-binary-2.9.6/doc/COPYING.LESSER`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 		   GNU LESSER GENERAL PUBLIC LICENSE
                        Version 3, 29 June 2007
 
- Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
 
 
   This version of the GNU Lesser General Public License incorporates
 the terms and conditions of version 3 of the GNU General Public
 License, supplemented by the additional permissions listed below.
```

### Comparing `psycopg2-binary-2.9.5/doc/Makefile` & `psycopg2-binary-2.9.6/doc/Makefile`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/README.rst` & `psycopg2-binary-2.9.6/doc/README.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/SUCCESS` & `psycopg2-binary-2.9.6/doc/SUCCESS`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/pep-0249.txt` & `psycopg2-binary-2.9.6/doc/pep-0249.txt`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/requirements.txt` & `psycopg2-binary-2.9.6/doc/requirements.txt`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/src/Makefile` & `psycopg2-binary-2.9.6/doc/src/Makefile`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/src/_static/psycopg.css` & `psycopg2-binary-2.9.6/doc/src/_static/psycopg.css`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/src/advanced.rst` & `psycopg2-binary-2.9.6/doc/src/advanced.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/src/conf.py` & `psycopg2-binary-2.9.6/doc/src/conf.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/src/connection.rst` & `psycopg2-binary-2.9.6/doc/src/connection.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/src/cursor.rst` & `psycopg2-binary-2.9.6/doc/src/cursor.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/src/errorcodes.rst` & `psycopg2-binary-2.9.6/doc/src/errorcodes.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/src/errors.rst` & `psycopg2-binary-2.9.6/doc/src/errors.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/src/extensions.rst` & `psycopg2-binary-2.9.6/doc/src/extensions.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/src/extras.rst` & `psycopg2-binary-2.9.6/doc/src/extras.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/src/faq.rst` & `psycopg2-binary-2.9.6/doc/src/faq.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/src/index.rst` & `psycopg2-binary-2.9.6/doc/src/index.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/src/install.rst` & `psycopg2-binary-2.9.6/doc/src/install.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/src/module.rst` & `psycopg2-binary-2.9.6/doc/src/module.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/src/pool.rst` & `psycopg2-binary-2.9.6/doc/src/pool.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/src/sql.rst` & `psycopg2-binary-2.9.6/doc/src/sql.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/src/tools/lib/dbapi_extension.py` & `psycopg2-binary-2.9.6/doc/src/tools/lib/dbapi_extension.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/src/tools/lib/ticket_role.py` & `psycopg2-binary-2.9.6/doc/src/tools/lib/ticket_role.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/src/tools/make_sqlstate_docs.py` & `psycopg2-binary-2.9.6/doc/src/tools/make_sqlstate_docs.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/src/tz.rst` & `psycopg2-binary-2.9.6/doc/src/tz.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/doc/src/usage.rst` & `psycopg2-binary-2.9.6/doc/src/usage.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/lib/__init__.py` & `psycopg2-binary-2.9.6/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/lib/_ipaddress.py` & `psycopg2-binary-2.9.6/lib/_ipaddress.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/lib/_json.py` & `psycopg2-binary-2.9.6/lib/_json.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/lib/_range.py` & `psycopg2-binary-2.9.6/lib/_range.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/lib/errorcodes.py` & `psycopg2-binary-2.9.6/lib/errorcodes.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/lib/errors.py` & `psycopg2-binary-2.9.6/lib/errors.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/lib/extensions.py` & `psycopg2-binary-2.9.6/lib/extensions.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/lib/extras.py` & `psycopg2-binary-2.9.6/lib/extras.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/lib/pool.py` & `psycopg2-binary-2.9.6/lib/pool.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/lib/sql.py` & `psycopg2-binary-2.9.6/lib/sql.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/lib/tz.py` & `psycopg2-binary-2.9.6/lib/tz.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/_psycopg.vc9.amd64.manifest` & `psycopg2-binary-2.9.6/psycopg/_psycopg.vc9.amd64.manifest`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/_psycopg.vc9.x86.manifest` & `psycopg2-binary-2.9.6/psycopg/_psycopg.vc9.x86.manifest`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/adapter_asis.c` & `psycopg2-binary-2.9.6/psycopg/adapter_asis.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/adapter_asis.h` & `psycopg2-binary-2.9.6/psycopg/adapter_asis.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/adapter_binary.c` & `psycopg2-binary-2.9.6/psycopg/adapter_binary.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/adapter_binary.h` & `psycopg2-binary-2.9.6/psycopg/adapter_binary.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/adapter_datetime.c` & `psycopg2-binary-2.9.6/psycopg/adapter_datetime.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/adapter_datetime.h` & `psycopg2-binary-2.9.6/psycopg/adapter_datetime.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/adapter_list.c` & `psycopg2-binary-2.9.6/psycopg/adapter_list.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/adapter_list.h` & `psycopg2-binary-2.9.6/psycopg/adapter_list.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/adapter_pboolean.c` & `psycopg2-binary-2.9.6/psycopg/adapter_pboolean.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/adapter_pboolean.h` & `psycopg2-binary-2.9.6/psycopg/adapter_pboolean.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/adapter_pdecimal.c` & `psycopg2-binary-2.9.6/psycopg/adapter_pdecimal.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/adapter_pdecimal.h` & `psycopg2-binary-2.9.6/psycopg/adapter_pdecimal.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/adapter_pfloat.c` & `psycopg2-binary-2.9.6/psycopg/adapter_pfloat.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/adapter_pfloat.h` & `psycopg2-binary-2.9.6/psycopg/adapter_pfloat.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/adapter_pint.c` & `psycopg2-binary-2.9.6/psycopg/adapter_pint.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/adapter_pint.h` & `psycopg2-binary-2.9.6/psycopg/adapter_pint.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/adapter_qstring.c` & `psycopg2-binary-2.9.6/psycopg/adapter_qstring.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/adapter_qstring.h` & `psycopg2-binary-2.9.6/psycopg/adapter_qstring.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/aix_support.c` & `psycopg2-binary-2.9.6/psycopg/aix_support.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/aix_support.h` & `psycopg2-binary-2.9.6/psycopg/aix_support.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/bytes_format.c` & `psycopg2-binary-2.9.6/psycopg/bytes_format.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/column.h` & `psycopg2-binary-2.9.6/psycopg/column.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/column_type.c` & `psycopg2-binary-2.9.6/psycopg/column_type.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/config.h` & `psycopg2-binary-2.9.6/psycopg/config.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/connection.h` & `psycopg2-binary-2.9.6/psycopg/connection.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/connection_int.c` & `psycopg2-binary-2.9.6/psycopg/connection_int.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/connection_type.c` & `psycopg2-binary-2.9.6/psycopg/connection_type.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/conninfo.h` & `psycopg2-binary-2.9.6/psycopg/conninfo.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/conninfo_type.c` & `psycopg2-binary-2.9.6/psycopg/conninfo_type.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/cursor.h` & `psycopg2-binary-2.9.6/psycopg/cursor.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/cursor_int.c` & `psycopg2-binary-2.9.6/psycopg/cursor_int.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/cursor_type.c` & `psycopg2-binary-2.9.6/psycopg/cursor_type.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/diagnostics.h` & `psycopg2-binary-2.9.6/psycopg/diagnostics.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/diagnostics_type.c` & `psycopg2-binary-2.9.6/psycopg/diagnostics_type.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/error.h` & `psycopg2-binary-2.9.6/psycopg/error.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/error_type.c` & `psycopg2-binary-2.9.6/psycopg/error_type.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/green.c` & `psycopg2-binary-2.9.6/psycopg/green.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/green.h` & `psycopg2-binary-2.9.6/psycopg/green.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/libpq_support.c` & `psycopg2-binary-2.9.6/psycopg/libpq_support.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/libpq_support.h` & `psycopg2-binary-2.9.6/psycopg/libpq_support.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/lobject.h` & `psycopg2-binary-2.9.6/psycopg/lobject.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/lobject_int.c` & `psycopg2-binary-2.9.6/psycopg/lobject_int.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/lobject_type.c` & `psycopg2-binary-2.9.6/psycopg/lobject_type.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/microprotocols.c` & `psycopg2-binary-2.9.6/psycopg/microprotocols.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/microprotocols.h` & `psycopg2-binary-2.9.6/psycopg/microprotocols.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/microprotocols_proto.c` & `psycopg2-binary-2.9.6/psycopg/microprotocols_proto.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/microprotocols_proto.h` & `psycopg2-binary-2.9.6/psycopg/microprotocols_proto.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/notify.h` & `psycopg2-binary-2.9.6/psycopg/notify.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/notify_type.c` & `psycopg2-binary-2.9.6/psycopg/notify_type.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/pgtypes.h` & `psycopg2-binary-2.9.6/psycopg/pgtypes.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/pqpath.c` & `psycopg2-binary-2.9.6/psycopg/pqpath.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/pqpath.h` & `psycopg2-binary-2.9.6/psycopg/pqpath.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/psycopg.h` & `psycopg2-binary-2.9.6/psycopg/psycopg.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/psycopgmodule.c` & `psycopg2-binary-2.9.6/psycopg/psycopgmodule.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/python.h` & `psycopg2-binary-2.9.6/psycopg/python.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/replication_connection.h` & `psycopg2-binary-2.9.6/psycopg/replication_connection.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/replication_connection_type.c` & `psycopg2-binary-2.9.6/psycopg/replication_connection_type.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/replication_cursor.h` & `psycopg2-binary-2.9.6/psycopg/replication_cursor.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/replication_cursor_type.c` & `psycopg2-binary-2.9.6/psycopg/replication_cursor_type.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/replication_message.h` & `psycopg2-binary-2.9.6/psycopg/replication_message.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/replication_message_type.c` & `psycopg2-binary-2.9.6/psycopg/replication_message_type.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/solaris_support.c` & `psycopg2-binary-2.9.6/psycopg/solaris_support.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/solaris_support.h` & `psycopg2-binary-2.9.6/psycopg/solaris_support.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/sqlstate_errors.h` & `psycopg2-binary-2.9.6/psycopg/sqlstate_errors.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/typecast.c` & `psycopg2-binary-2.9.6/psycopg/typecast.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/typecast.h` & `psycopg2-binary-2.9.6/psycopg/typecast.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/typecast_array.c` & `psycopg2-binary-2.9.6/psycopg/typecast_array.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/typecast_basic.c` & `psycopg2-binary-2.9.6/psycopg/typecast_basic.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/typecast_binary.c` & `psycopg2-binary-2.9.6/psycopg/typecast_binary.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/typecast_binary.h` & `psycopg2-binary-2.9.6/psycopg/typecast_binary.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/typecast_builtins.c` & `psycopg2-binary-2.9.6/psycopg/typecast_builtins.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/typecast_datetime.c` & `psycopg2-binary-2.9.6/psycopg/typecast_datetime.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/utils.c` & `psycopg2-binary-2.9.6/psycopg/utils.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/utils.h` & `psycopg2-binary-2.9.6/psycopg/utils.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/win32_support.c` & `psycopg2-binary-2.9.6/psycopg/win32_support.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/win32_support.h` & `psycopg2-binary-2.9.6/psycopg/win32_support.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/xid.h` & `psycopg2-binary-2.9.6/psycopg/xid.h`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg/xid_type.c` & `psycopg2-binary-2.9.6/psycopg/xid_type.c`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/psycopg2_binary.egg-info/PKG-INFO` & `psycopg2-binary-2.9.6/psycopg2_binary.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,93 +1,22 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: psycopg2-binary
-Version: 2.9.5
+Version: 2.9.6
 Summary: psycopg2 - Python-PostgreSQL Database Adapter
 Home-page: https://psycopg.org/
 Author: Federico Di Gregorio
 Author-email: fog@initd.org
 Maintainer: Daniele Varrazzo
 Maintainer-email: daniele.varrazzo@gmail.com
 License: LGPL with exceptions
 Project-URL: Homepage, https://psycopg.org/
 Project-URL: Documentation, https://www.psycopg.org/docs/
 Project-URL: Code, https://github.com/psycopg/psycopg2
 Project-URL: Issue Tracker, https://github.com/psycopg/psycopg2/issues
 Project-URL: Download, https://pypi.org/project/psycopg2/
-Description: Psycopg is the most popular PostgreSQL database adapter for the Python
-        programming language.  Its main features are the complete implementation of
-        the Python DB API 2.0 specification and the thread safety (several threads can
-        share the same connection).  It was designed for heavily multi-threaded
-        applications that create and destroy lots of cursors and make a large number
-        of concurrent "INSERT"s or "UPDATE"s.
-        
-        Psycopg 2 is mostly implemented in C as a libpq wrapper, resulting in being
-        both efficient and secure.  It features client-side and server-side cursors,
-        asynchronous communication and notifications, "COPY TO/COPY FROM" support.
-        Many Python types are supported out-of-the-box and adapted to matching
-        PostgreSQL data types; adaptation can be extended and customized thanks to a
-        flexible objects adaptation system.
-        
-        Psycopg 2 is both Unicode and Python 3 friendly.
-        
-        
-        Documentation
-        -------------
-        
-        Documentation is included in the ``doc`` directory and is `available online`__.
-        
-        .. __: https://www.psycopg.org/docs/
-        
-        For any other resource (source code repository, bug tracker, mailing list)
-        please check the `project homepage`__.
-        
-        .. __: https://psycopg.org/
-        
-        
-        Installation
-        ------------
-        
-        Building Psycopg requires a few prerequisites (a C compiler, some development
-        packages): please check the install_ and the faq_ documents in the ``doc`` dir
-        or online for the details.
-        
-        If prerequisites are met, you can install psycopg like any other Python
-        package, using ``pip`` to download it from PyPI_::
-        
-            $ pip install psycopg2
-        
-        or using ``setup.py`` if you have downloaded the source package locally::
-        
-            $ python setup.py build
-            $ sudo python setup.py install
-        
-        You can also obtain a stand-alone package, not requiring a compiler or
-        external libraries, by installing the `psycopg2-binary`_ package from PyPI::
-        
-            $ pip install psycopg2-binary
-        
-        The binary package is a practical choice for development and testing but in
-        production it is advised to use the package built from sources.
-        
-        .. _PyPI: https://pypi.org/project/psycopg2/
-        .. _psycopg2-binary: https://pypi.org/project/psycopg2-binary/
-        .. _install: https://www.psycopg.org/docs/install.html#install-from-source
-        .. _faq: https://www.psycopg.org/docs/faq.html#faq-compile
-        
-        :Linux/OSX: |gh-actions|
-        :Windows: |appveyor|
-        
-        .. |gh-actions| image:: https://github.com/psycopg/psycopg2/actions/workflows/tests.yml/badge.svg
-            :target: https://github.com/psycopg/psycopg2/actions/workflows/tests.yml
-            :alt: Linux and OSX build status
-        
-        .. |appveyor| image:: https://ci.appveyor.com/api/projects/status/github/psycopg/psycopg2?branch=master&svg=true
-            :target: https://ci.appveyor.com/project/psycopg/psycopg2/branch/master
-            :alt: Windows build status
-        
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -103,7 +32,81 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Requires-Python: >=3.6
+License-File: LICENSE
+
+Psycopg is the most popular PostgreSQL database adapter for the Python
+programming language.  Its main features are the complete implementation of
+the Python DB API 2.0 specification and the thread safety (several threads can
+share the same connection).  It was designed for heavily multi-threaded
+applications that create and destroy lots of cursors and make a large number
+of concurrent "INSERT"s or "UPDATE"s.
+
+Psycopg 2 is mostly implemented in C as a libpq wrapper, resulting in being
+both efficient and secure.  It features client-side and server-side cursors,
+asynchronous communication and notifications, "COPY TO/COPY FROM" support.
+Many Python types are supported out-of-the-box and adapted to matching
+PostgreSQL data types; adaptation can be extended and customized thanks to a
+flexible objects adaptation system.
+
+Psycopg 2 is both Unicode and Python 3 friendly.
+
+
+Documentation
+-------------
+
+Documentation is included in the ``doc`` directory and is `available online`__.
+
+.. __: https://www.psycopg.org/docs/
+
+For any other resource (source code repository, bug tracker, mailing list)
+please check the `project homepage`__.
+
+.. __: https://psycopg.org/
+
+
+Installation
+------------
+
+Building Psycopg requires a few prerequisites (a C compiler, some development
+packages): please check the install_ and the faq_ documents in the ``doc`` dir
+or online for the details.
+
+If prerequisites are met, you can install psycopg like any other Python
+package, using ``pip`` to download it from PyPI_::
+
+    $ pip install psycopg2
+
+or using ``setup.py`` if you have downloaded the source package locally::
+
+    $ python setup.py build
+    $ sudo python setup.py install
+
+You can also obtain a stand-alone package, not requiring a compiler or
+external libraries, by installing the `psycopg2-binary`_ package from PyPI::
+
+    $ pip install psycopg2-binary
+
+The binary package is a practical choice for development and testing but in
+production it is advised to use the package built from sources.
+
+.. _PyPI: https://pypi.org/project/psycopg2/
+.. _psycopg2-binary: https://pypi.org/project/psycopg2-binary/
+.. _install: https://www.psycopg.org/docs/install.html#install-from-source
+.. _faq: https://www.psycopg.org/docs/faq.html#faq-compile
+
+:Linux/OSX: |gh-actions|
+:Windows: |appveyor|
+
+.. |gh-actions| image:: https://github.com/psycopg/psycopg2/actions/workflows/tests.yml/badge.svg
+    :target: https://github.com/psycopg/psycopg2/actions/workflows/tests.yml
+    :alt: Linux and OSX build status
+
+.. |appveyor| image:: https://ci.appveyor.com/api/projects/status/github/psycopg/psycopg2?branch=master&svg=true
+    :target: https://ci.appveyor.com/project/psycopg/psycopg2/branch/master
+    :alt: Windows build status
+
+
```

### Comparing `psycopg2-binary-2.9.5/psycopg2_binary.egg-info/SOURCES.txt` & `psycopg2-binary-2.9.6/psycopg2_binary.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -133,24 +133,23 @@
 psycopg2_binary.egg-info/dependency_links.txt
 psycopg2_binary.egg-info/top_level.txt
 scripts/make_errorcodes.py
 scripts/make_errors.py
 scripts/refcounter.py
 scripts/build/appveyor.py
 scripts/build/build_libpq.sh
-scripts/build/build_macos.sh
 scripts/build/build_macos_arm64.sh
-scripts/build/build_manylinux2014.sh
-scripts/build/build_manylinux_2_24.sh
-scripts/build/build_musllinux_1_1.sh
 scripts/build/build_sdist.sh
 scripts/build/download_packages_appveyor.py
 scripts/build/download_packages_github.py
+scripts/build/print_so_versions.sh
 scripts/build/run_build_macos_arm64.sh
 scripts/build/strip_wheel.sh
+scripts/build/wheel_linux_before_all.sh
+scripts/build/wheel_macos_before_all.sh
 tests/__init__.py
 tests/dbapi20.py
 tests/dbapi20_tpc.py
 tests/test_async.py
 tests/test_bugX000.py
 tests/test_bug_gc.py
 tests/test_cancel.py
```

### Comparing `psycopg2-binary-2.9.5/scripts/build/appveyor.py` & `psycopg2-binary-2.9.6/scripts/build/appveyor.py`

 * *Files 1% similar despite different names*

```diff
@@ -651,17 +651,20 @@
 class Options:
     """
     An object exposing the script configuration from env vars and command line.
     """
 
     @property
     def py_ver(self):
-        """The Python version to build as 2 digits string."""
+        """The Python version to build as 2 digits string.
+
+        For large values of 2, occasionally.
+        """
         rv = os.environ['PY_VER']
-        assert rv in ('36', '37', '38', '39', '310'), rv
+        assert rv in ('36', '37', '38', '39', '310', '311'), rv
         return rv
 
     @property
     def py_arch(self):
         """The Python architecture to build, 32 or 64."""
         rv = os.environ['PY_ARCH']
         assert rv in ('32', '64'), rv
@@ -740,14 +743,15 @@
         # Py 3.9 = VS Ver. 16.0 (VS 2019)
         vsvers = {
             '36': '14.0',
             '37': '14.0',
             '38': '14.0',
             '39': '16.0',
             '310': '16.0',
+            '311': '16.0',
         }
         return vsvers[self.py_ver]
 
     @property
     def clone_dir(self):
         """The directory where the repository is cloned."""
         return Path(r"C:\Project")
```

### Comparing `psycopg2-binary-2.9.5/scripts/build/build_macos_arm64.sh` & `psycopg2-binary-2.9.6/scripts/build/build_macos_arm64.sh`

 * *Files 12% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 #
 # The script cannot be run as sudo (installing brew fails), but requires sudo,
 # so it can pretty much only be executed by a sudo user as it is.
 
 set -euo pipefail
 set -x
 
-python_versions="3.8.10 3.9.13 3.10.5 3.11"
-postgres_version=15
+python_versions="3.8.10 3.9.13 3.10.5 3.11.0"
+pg_version=15
 
 # Move to the root of the project
 dir="$( cd "$( dirname "${BASH_SOURCE[0]}" )" && pwd )"
 cd "${dir}/../../"
 
 # Add /usr/local/bin to the path. It seems it's not, in non-interactive sessions
 if ! (echo $PATH | grep -q '/usr/local/bin'); then
@@ -31,25 +31,34 @@
         # xcode-select --install
         NONINTERACTIVE=1 /bin/bash -c "$(curl -fsSL \
             https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
     )
     eval "$(/opt/homebrew/bin/brew shellenv)"
 fi
 
+export PGDATA=/opt/homebrew/var/postgresql@${pg_version}
+
 # Install PostgreSQL, if necessary
 command -v pg_config > /dev/null || (
-    brew install postgresql@${postgres_version}
-    # Currently not working
-    # brew services start postgresql@${postgres_version}
-    pg_ctl \
-        -D /opt/homebrew/var/postgresql@${postgres_version} \
-        -l /opt/homebrew/var/log/postgresql@${postgres_version}.log \
-        start
+    brew install postgresql@${pg_version}
 )
 
+# After PostgreSQL 15, the bin path is not in the path.
+export PATH=$(ls -d1 /opt/homebrew/Cellar/postgresql@${pg_version}/*/bin):$PATH
+
+# Make sure the server is running
+
+# Currently not working
+# brew services start postgresql@${pg_version}
+
+if ! pg_ctl status; then
+    pg_ctl -l /opt/homebrew/var/log/postgresql@${pg_version}.log start
+fi
+
+
 # Install the Python versions we want to build
 for ver3 in $python_versions; do
     ver2=$(echo $ver3 | sed 's/\([^\.]*\)\(\.[^\.]*\)\(.*\)/\1\2/')
     command -v python${ver2} > /dev/null || (
         (cd /tmp &&
             curl -fsSl -O \
                 https://www.python.org/ftp/python/${ver3}/python-${ver3}-macos11.pkg)
@@ -64,15 +73,15 @@
 
 source .venv/bin/activate
 pip install cibuildwheel
 
 # Build the binary packages
 export CIBW_PLATFORM=macos
 export CIBW_ARCHS=arm64
-export CIBW_BUILD='cp{38,39,310}-*'
+export CIBW_BUILD='cp{38,39,310,311}-*'
 export CIBW_TEST_COMMAND='python -c "import tests; tests.unittest.main(defaultTest=\"tests.test_suite\")"'
 
 export PSYCOPG2_TESTDB=postgres
 export PYTHONPATH=$(pwd)
 
 # For some reason, cibuildwheel tests says that psycopg2 is already installed,
 # refuses to install, then promptly fails import. So, please, seriously,
```

### Comparing `psycopg2-binary-2.9.5/scripts/build/build_sdist.sh` & `psycopg2-binary-2.9.6/scripts/build/build_sdist.sh`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 dir="$( cd "$( dirname "${BASH_SOURCE[0]}" )" && pwd )"
 prjdir="$( cd "${dir}/../.." && pwd )"
 
 # Find psycopg version
 version=$(grep -e ^PSYCOPG_VERSION setup.py | sed "s/.*'\(.*\)'/\1/")
 # A gratuitous comment to fix broken vim syntax file: '")
-distdir="${prjdir}/dist/psycopg2-$version"
+distdir="${prjdir}/dist"
 
 # Replace the package name
 if [[ "${PACKAGE_NAME:-}" ]]; then
     sed -i "s/^setup(name=\"psycopg2\"/setup(name=\"${PACKAGE_NAME}\"/" \
         "${prjdir}/setup.py"
 fi
```

### Comparing `psycopg2-binary-2.9.5/scripts/build/download_packages_appveyor.py` & `psycopg2-binary-2.9.6/scripts/build/download_packages_appveyor.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/scripts/build/download_packages_github.py` & `psycopg2-binary-2.9.6/scripts/build/download_packages_github.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/scripts/build/run_build_macos_arm64.sh` & `psycopg2-binary-2.9.6/scripts/build/run_build_macos_arm64.sh`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/scripts/build/strip_wheel.sh` & `psycopg2-binary-2.9.6/scripts/build/strip_wheel.sh`

 * *Files 16% similar despite different names*

```diff
@@ -10,32 +10,40 @@
 #
 # System libraries are already pretty stripped. _psycopg2.so goes around
 # 1.6M -> 300K (python 3.8, x86_64)
 #
 # This script is designed to run on a wheel archive before auditwheel.
 
 set -euo pipefail
-set -x
+# set -x
+
+source /etc/os-release
+dir="$( cd "$( dirname "${BASH_SOURCE[0]}" )" && pwd )"
 
 wheel=$(realpath "$1")
 shift
 
-# python or python3?
-if which python > /dev/null; then
-    py=python
-else
-    py=python3
-fi
-
 tmpdir=$(mktemp -d)
 trap "rm -r ${tmpdir}" EXIT
 
 cd "${tmpdir}"
-$py -m zipfile -e "${wheel}" .
+python -m zipfile -e "${wheel}" .
+
+echo "
+Libs before:"
+# Busybox doesn't have "find -ls"
+find . -name \*.so | xargs ls -l
+
+# On Debian, print the package versions libraries come from
+echo "
+Dependencies versions of '_psycopg.so' library:"
+"${dir}/print_so_versions.sh" "$(find . -name \*_psycopg\*.so)"
+
+find . -name \*.so -exec strip "$@" {} \;
 
-find . -name *.so -ls -exec strip "$@" {} \;
-# Display the size after strip
-find . -name *.so -ls
+echo "
+Libs after:"
+find . -name \*.so | xargs ls -l
 
-$py -m zipfile -c "${wheel}" *
+python -m zipfile -c ${wheel} *
 
 cd -
```

### Comparing `psycopg2-binary-2.9.5/scripts/make_errorcodes.py` & `psycopg2-binary-2.9.6/scripts/make_errorcodes.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/scripts/make_errors.py` & `psycopg2-binary-2.9.6/scripts/make_errors.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/scripts/refcounter.py` & `psycopg2-binary-2.9.6/scripts/refcounter.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/setup.py` & `psycopg2-binary-2.9.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     import configparser
 except ImportError:
     import ConfigParser as configparser
 
 # Take a look at https://www.python.org/dev/peps/pep-0440/
 # for a consistent versioning pattern.
 
-PSYCOPG_VERSION = '2.9.5'
+PSYCOPG_VERSION = '2.9.6'
 
 
 # note: if you are changing the list of supported Python version please fix
 # the docs in install.rst and the /features/ page on the website.
 classifiers = """\
 Development Status :: 5 - Production/Stable
 Intended Audience :: Developers
```

### Comparing `psycopg2-binary-2.9.5/tests/__init__.py` & `psycopg2-binary-2.9.6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/dbapi20.py` & `psycopg2-binary-2.9.6/tests/dbapi20.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/dbapi20_tpc.py` & `psycopg2-binary-2.9.6/tests/dbapi20_tpc.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/test_async.py` & `psycopg2-binary-2.9.6/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/test_bugX000.py` & `psycopg2-binary-2.9.6/tests/test_bugX000.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/test_bug_gc.py` & `psycopg2-binary-2.9.6/tests/test_bug_gc.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/test_cancel.py` & `psycopg2-binary-2.9.6/tests/test_cancel.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/test_connection.py` & `psycopg2-binary-2.9.6/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/test_copy.py` & `psycopg2-binary-2.9.6/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/test_cursor.py` & `psycopg2-binary-2.9.6/tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/test_dates.py` & `psycopg2-binary-2.9.6/tests/test_dates.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/test_errcodes.py` & `psycopg2-binary-2.9.6/tests/test_errcodes.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/test_errors.py` & `psycopg2-binary-2.9.6/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/test_extras_dictcursor.py` & `psycopg2-binary-2.9.6/tests/test_extras_dictcursor.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/test_fast_executemany.py` & `psycopg2-binary-2.9.6/tests/test_fast_executemany.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/test_green.py` & `psycopg2-binary-2.9.6/tests/test_green.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/test_ipaddress.py` & `psycopg2-binary-2.9.6/tests/test_ipaddress.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/test_lobject.py` & `psycopg2-binary-2.9.6/tests/test_lobject.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/test_module.py` & `psycopg2-binary-2.9.6/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/test_notify.py` & `psycopg2-binary-2.9.6/tests/test_notify.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/test_psycopg2_dbapi20.py` & `psycopg2-binary-2.9.6/tests/test_psycopg2_dbapi20.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/test_quote.py` & `psycopg2-binary-2.9.6/tests/test_quote.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/test_replication.py` & `psycopg2-binary-2.9.6/tests/test_replication.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/test_sql.py` & `psycopg2-binary-2.9.6/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/test_transaction.py` & `psycopg2-binary-2.9.6/tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/test_types_basic.py` & `psycopg2-binary-2.9.6/tests/test_types_basic.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/test_types_extras.py` & `psycopg2-binary-2.9.6/tests/test_types_extras.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/test_with.py` & `psycopg2-binary-2.9.6/tests/test_with.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/testconfig.py` & `psycopg2-binary-2.9.6/tests/testconfig.py`

 * *Files identical despite different names*

### Comparing `psycopg2-binary-2.9.5/tests/testutils.py` & `psycopg2-binary-2.9.6/tests/testutils.py`

 * *Files identical despite different names*

