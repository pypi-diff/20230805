# Comparing `tmp/pglast-5.2.tar.gz` & `tmp/pglast-5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pglast-5.2.tar", last modified: Sat May 20 07:30:25 2023, max compression
+gzip compressed data, was "pglast-5.3.tar", last modified: Sat Aug  5 06:55:40 2023, max compression
```

## Comparing `pglast-5.2.tar` & `pglast-5.3.tar`

### file list

```diff
@@ -1,904 +1,906 @@
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.194373 pglast-5.2/
--rw-rw-r--   0 lele      (1000) lele      (1000)    23485 2023-05-20 07:30:08.000000 pglast-5.2/CHANGES.rst
--rw-rw-r--   0 lele      (1000) lele      (1000)      843 2022-12-01 07:04:43.000000 pglast-5.2/MANIFEST.in
--rw-rw-r--   0 lele      (1000) lele      (1000)     4716 2023-01-11 20:10:25.000000 pglast-5.2/Makefile
--rw-rw-r--   0 lele      (1000) lele      (1000)     2763 2022-12-01 07:04:43.000000 pglast-5.2/Makefile.release
--rw-rw-r--   0 lele      (1000) lele      (1000)     1328 2022-12-01 07:04:43.000000 pglast-5.2/Makefile.virtualenv
--rw-rw-r--   0 lele      (1000) lele      (1000)    26923 2023-05-20 07:30:25.194373 pglast-5.2/PKG-INFO
--rw-r--r--   0 lele      (1000) lele      (1000)     2426 2023-02-19 16:04:29.000000 pglast-5.2/README.rst
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.070376 pglast-5.2/docs/
--rw-rw-r--   0 lele      (1000) lele      (1000)      607 2022-12-01 07:04:43.000000 pglast-5.2/docs/Makefile
--rw-rw-r--   0 lele      (1000) lele      (1000)      625 2022-12-01 07:04:43.000000 pglast-5.2/docs/api.rst
--rw-r--r--   0 lele      (1000) lele      (1000)   148863 2023-05-19 08:03:11.000000 pglast-5.2/docs/ast.rst
--rw-rw-r--   0 lele      (1000) lele      (1000)    23485 2023-05-20 07:30:08.000000 pglast-5.2/docs/changes.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     5216 2022-12-13 12:49:31.000000 pglast-5.2/docs/conf.py
--rw-r--r--   0 lele      (1000) lele      (1000)    42541 2023-05-19 08:03:41.000000 pglast-5.2/docs/ddl.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     6702 2022-12-19 18:34:08.000000 pglast-5.2/docs/development.rst
--rw-rw-r--   0 lele      (1000) lele      (1000)    23171 2023-05-19 08:03:41.000000 pglast-5.2/docs/dml.rst
--rw-rw-r--   0 lele      (1000) lele      (1000)     1049 2022-12-01 07:04:43.000000 pglast-5.2/docs/enums.rst
--rw-rw-r--   0 lele      (1000) lele      (1000)     1194 2022-12-13 12:47:14.000000 pglast-5.2/docs/index.rst
--rw-rw-r--   0 lele      (1000) lele      (1000)      540 2022-12-01 07:04:43.000000 pglast-5.2/docs/installation.rst
--rw-rw-r--   0 lele      (1000) lele      (1000)     1926 2022-12-01 07:04:43.000000 pglast-5.2/docs/introduction.rst
--rw-rw-r--   0 lele      (1000) lele      (1000)      756 2022-12-01 07:04:43.000000 pglast-5.2/docs/keywords.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     2216 2023-05-19 08:03:09.000000 pglast-5.2/docs/lockdefs.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     1642 2023-05-19 08:03:10.000000 pglast-5.2/docs/lockoptions.rst
--rw-r--r--   0 lele      (1000) lele      (1000)    17012 2023-05-19 08:03:10.000000 pglast-5.2/docs/nodes.rst
--rw-r--r--   0 lele      (1000) lele      (1000)    26350 2023-05-19 08:03:10.000000 pglast-5.2/docs/parsenodes.rst
--rw-rw-r--   0 lele      (1000) lele      (1000)     3922 2022-12-01 07:04:43.000000 pglast-5.2/docs/parser.rst
--rw-r--r--   0 lele      (1000) lele      (1000)      925 2023-05-19 08:03:10.000000 pglast-5.2/docs/pg_am.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     1207 2023-05-19 08:03:10.000000 pglast-5.2/docs/pg_attribute.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     3421 2023-05-19 08:03:10.000000 pglast-5.2/docs/pg_class.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     2139 2023-05-19 08:03:10.000000 pglast-5.2/docs/pg_trigger.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     5204 2023-05-19 08:03:10.000000 pglast-5.2/docs/primnodes.rst
--rw-rw-r--   0 lele      (1000) lele      (1000)      963 2022-12-01 07:04:43.000000 pglast-5.2/docs/printers.rst
--rw-rw-r--   0 lele      (1000) lele      (1000)      990 2022-12-01 07:04:43.000000 pglast-5.2/docs/sfuncs.rst
--rw-rw-r--   0 lele      (1000) lele      (1000)      666 2022-12-01 07:04:43.000000 pglast-5.2/docs/stream.rst
--rw-rw-r--   0 lele      (1000) lele      (1000)    15486 2022-12-04 09:48:04.000000 pglast-5.2/docs/usage.rst
--rw-rw-r--   0 lele      (1000) lele      (1000)      580 2022-12-01 07:04:43.000000 pglast-5.2/docs/visitors.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     1483 2023-05-19 08:03:11.000000 pglast-5.2/docs/xml.rst
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.070376 pglast-5.2/libpg_query/
--rw-rw-r--   0 lele      (1000) lele      (1000)     1561 2023-02-10 08:11:28.000000 pglast-5.2/libpg_query/LICENSE
--rw-rw-r--   0 lele      (1000) lele      (1000)    13474 2023-05-19 08:02:43.000000 pglast-5.2/libpg_query/Makefile
--rw-rw-r--   0 lele      (1000) lele      (1000)     3462 2023-01-11 21:06:42.000000 pglast-5.2/libpg_query/pg_query.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.074376 pglast-5.2/libpg_query/protobuf/
--rw-rw-r--   0 lele      (1000) lele      (1000)  1257968 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/protobuf/pg_query.pb-c.c
--rw-rw-r--   0 lele      (1000) lele      (1000)   474315 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/protobuf/pg_query.pb-c.h
--rw-rw-r--   0 lele      (1000) lele      (1000)   106559 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/protobuf/pg_query.proto
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.078376 pglast-5.2/libpg_query/src/
--rw-rw-r--   0 lele      (1000) lele      (1000)     2214 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/src/pg_query.c
--rw-rw-r--   0 lele      (1000) lele      (1000)   306664 2023-05-17 06:20:05.000000 pglast-5.2/libpg_query/src/pg_query_deparse.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    73716 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/pg_query_enum_defs.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    10960 2023-01-11 21:06:42.000000 pglast-5.2/libpg_query/src/pg_query_fingerprint.c
--rw-rw-r--   0 lele      (1000) lele      (1000)      257 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/src/pg_query_fingerprint.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    32338 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/pg_query_fingerprint_conds.c
--rw-rw-r--   0 lele      (1000) lele      (1000)   455292 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/pg_query_fingerprint_defs.c
--rw-rw-r--   0 lele      (1000) lele      (1000)      525 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/src/pg_query_internal.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1264 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/src/pg_query_json_helper.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    21956 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/src/pg_query_json_plpgsql.c
--rw-rw-r--   0 lele      (1000) lele      (1000)      162 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/src/pg_query_json_plpgsql.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    20362 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/src/pg_query_normalize.c
--rw-rw-r--   0 lele      (1000) lele      (1000)      243 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/src/pg_query_outfuncs.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    32991 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/pg_query_outfuncs_conds.c
--rw-rw-r--   0 lele      (1000) lele      (1000)   117512 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/pg_query_outfuncs_defs.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     8655 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/pg_query_outfuncs_json.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     8308 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/pg_query_outfuncs_protobuf.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     3668 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/src/pg_query_parse.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    13406 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/src/pg_query_parse_plpgsql.c
--rw-rw-r--   0 lele      (1000) lele      (1000)      201 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/src/pg_query_readfuncs.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    25246 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/pg_query_readfuncs_conds.c
--rw-rw-r--   0 lele      (1000) lele      (1000)   123173 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/pg_query_readfuncs_defs.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     5641 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/pg_query_readfuncs_protobuf.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     4748 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/src/pg_query_scan.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     5998 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/src/pg_query_split.c
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.090375 pglast-5.2/libpg_query/src/postgres/
--rw-rw-r--   0 lele      (1000) lele      (1000)        0 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/src/postgres/guc-file.c
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.094375 pglast-5.2/libpg_query/src/postgres/include/
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.098375 pglast-5.2/libpg_query/src/postgres/include/access/
--rw-rw-r--   0 lele      (1000) lele      (1000)     9967 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/amapi.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1656 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/attmap.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1547 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/attnum.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1780 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/clog.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2263 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/commit_ts.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2443 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/detoast.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     9090 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/genam.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2203 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/gin.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3276 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/htup.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    29211 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/htup_details.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     5347 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/itup.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2641 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/parallel.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1080 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/printtup.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      977 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/relation.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     6829 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/relscan.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1400 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/rmgr.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3434 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/rmgrlist.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1470 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/sdir.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     6444 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/skey.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3075 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/stratnum.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      853 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/sysattr.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      932 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/table.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    76360 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/tableam.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2738 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/toast_compression.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    12618 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/transam.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1624 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/tupconvert.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     5304 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/tupdesc.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     7547 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/tupmacs.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2226 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/twophase.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    17876 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/xact.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    11150 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/xlog.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    12298 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/xlog_internal.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3022 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/xlogdefs.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1515 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/xlogprefetcher.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    15433 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/xlogreader.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     8744 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/xlogrecord.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     5330 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/access/xlogrecovery.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    45563 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/c.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.106375 pglast-5.2/libpg_query/src/postgres/include/catalog/
--rw-rw-r--   0 lele      (1000) lele      (1000)     1295 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/catalog.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2591 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/catversion.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     9705 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/dependency.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     6472 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/genbki.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     6577 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/index.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1824 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/indexing.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     7383 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/namespace.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     9202 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/objectaccess.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3208 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/objectaddress.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     6006 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_aggregate.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2817 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_aggregate_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1594 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_am.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1154 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_am_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     7827 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_attribute.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1982 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_attribute_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2335 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_authid.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1763 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_authid_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     7973 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_class.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     4725 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_class_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2948 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_collation.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1598 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_collation_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     9801 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_constraint.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2392 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_constraint_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     9099 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_control.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2476 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_conversion.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1134 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_conversion_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2807 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_depend.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      991 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_depend_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1915 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_event_trigger.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1084 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_event_trigger_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3545 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_index.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1827 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_index_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2056 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_language.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1168 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_language_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1941 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_namespace.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1005 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_namespace_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3242 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_opclass.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1544 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_opclass_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3202 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_operator.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     4976 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_operator_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1893 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_opfamily.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1437 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_opfamily_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1924 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_parameter_acl.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      997 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_parameter_acl_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2814 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_partitioned_table.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1162 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_partitioned_table_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     6659 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_proc.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3381 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_proc_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     4916 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_publication.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1148 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_publication_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2093 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_replication_origin.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1021 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_replication_origin_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    12527 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_statistic.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     9160 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_statistic_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2990 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_statistic_ext.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1347 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_statistic_ext_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1542 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_transform.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      954 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_transform_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     6313 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_trigger.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     4237 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_trigger_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1526 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_ts_config.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      954 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_ts_config_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1681 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_ts_dict.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      991 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_ts_dict_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1750 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_ts_parser.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1067 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_ts_parser_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1583 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_ts_template.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      985 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_ts_template_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    14425 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_type.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     9672 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/pg_type_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1752 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/catalog/storage.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.110375 pglast-5.2/libpg_query/src/postgres/include/commands/
--rw-rw-r--   0 lele      (1000) lele      (1000)     1592 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/commands/async.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1419 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/commands/dbcommands.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     6863 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/commands/defrem.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3343 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/commands/event_trigger.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     4972 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/commands/explain.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2201 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/commands/prepare.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2067 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/commands/tablespace.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    10160 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/commands/trigger.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1329 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/commands/user.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    13483 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/commands/vacuum.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1773 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/commands/variable.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.110375 pglast-5.2/libpg_query/src/postgres/include/common/
--rw-rw-r--   0 lele      (1000) lele      (1000)     1716 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/common/file_perm.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2558 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/common/hashfn.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      942 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/common/ip.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      845 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/common/keywords.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1482 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/common/kwlookup.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2132 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/common/pg_prng.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2622 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/common/relpath.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1541 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/common/string.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     6132 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/common/unicode_combining_table.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2569 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/common/unicode_east_asian_fw_table.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.110375 pglast-5.2/libpg_query/src/postgres/include/datatype/
--rw-rw-r--   0 lele      (1000) lele      (1000)     8640 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/datatype/timestamp.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.110375 pglast-5.2/libpg_query/src/postgres/include/executor/
--rw-rw-r--   0 lele      (1000) lele      (1000)     2393 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/executor/execdesc.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    25464 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/executor/executor.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1828 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/executor/functions.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     4975 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/executor/instrument.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     7898 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/executor/spi.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2850 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/executor/tablefunc.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    17334 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/executor/tuptable.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    34850 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/fmgr.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    12948 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/funcapi.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3972 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/getaddrinfo.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.110375 pglast-5.2/libpg_query/src/postgres/include/jit/
--rw-rw-r--   0 lele      (1000) lele      (1000)     2820 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/jit/jit.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    16679 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/kwlist_d.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.110375 pglast-5.2/libpg_query/src/postgres/include/lib/
--rw-rw-r--   0 lele      (1000) lele      (1000)     4429 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/lib/dshash.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    21457 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/lib/ilist.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3505 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/lib/pairingheap.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    33200 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/lib/simplehash.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    13087 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/lib/sort_template.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     5803 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/lib/stringinfo.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.114375 pglast-5.2/libpg_query/src/postgres/include/libpq/
--rw-rw-r--   0 lele      (1000) lele      (1000)      981 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/libpq/auth.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1527 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/libpq/crypt.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     4099 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/libpq/hba.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    10842 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/libpq/libpq-be.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     4549 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/libpq/libpq.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     6136 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/libpq/pqcomm.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     5968 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/libpq/pqformat.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1236 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/libpq/pqsignal.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.114375 pglast-5.2/libpg_query/src/postgres/include/mb/
--rw-rw-r--   0 lele      (1000) lele      (1000)    28560 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/mb/pg_wchar.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      667 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/mb/stringinfo_mb.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    17867 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/miscadmin.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.114375 pglast-5.2/libpg_query/src/postgres/include/nodes/
--rw-rw-r--   0 lele      (1000) lele      (1000)     4414 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/nodes/bitmapset.h
--rw-rw-r--   0 lele      (1000) lele      (1000)   100579 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/nodes/execnodes.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     5629 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/nodes/extensible.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1884 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/nodes/lockoptions.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3528 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/nodes/makefuncs.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     4030 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/nodes/memnodes.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     5109 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/nodes/nodeFuncs.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    21378 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/nodes/nodes.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     6697 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/nodes/params.h
--rw-rw-r--   0 lele      (1000) lele      (1000)   131739 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/nodes/parsenodes.h
--rw-rw-r--   0 lele      (1000) lele      (1000)   115826 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/nodes/pathnodes.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    21912 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/nodes/pg_list.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    50560 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/nodes/plannodes.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    66016 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/nodes/primnodes.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1077 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/nodes/print.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2732 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/nodes/tidbitmap.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2118 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/nodes/value.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.118375 pglast-5.2/libpg_query/src/postgres/include/optimizer/
--rw-rw-r--   0 lele      (1000) lele      (1000)     9691 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/optimizer/cost.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2278 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/optimizer/geqo.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1118 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/optimizer/geqo_gene.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     7094 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/optimizer/optimizer.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    10023 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/optimizer/paths.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     4515 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/optimizer/planmain.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.118375 pglast-5.2/libpg_query/src/postgres/include/parser/
--rw-rw-r--   0 lele      (1000) lele      (1000)     2449 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/parser/analyze.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    23149 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/parser/gram.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2284 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/parser/gramparse.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    29432 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/parser/kwlist.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2008 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/parser/parse_agg.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3713 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/parser/parse_coerce.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      722 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/parser/parse_expr.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2505 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/parser/parse_func.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    15245 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/parser/parse_node.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2406 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/parser/parse_oper.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     5100 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/parser/parse_relation.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2196 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/parser/parse_type.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2082 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/parser/parser.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1473 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/parser/parsetree.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     5471 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/parser/scanner.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      777 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/parser/scansup.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.118375 pglast-5.2/libpg_query/src/postgres/include/partitioning/
--rw-rw-r--   0 lele      (1000) lele      (1000)      680 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/partitioning/partdefs.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    32407 2023-02-10 08:11:28.000000 pglast-5.2/libpg_query/src/postgres/include/pg_config.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      323 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/src/postgres/include/pg_config_ext.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    15372 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/pg_config_manual.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      158 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/src/postgres/include/pg_config_os.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1719 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/pg_getopt.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      320 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/pg_trace.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    21897 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/pgstat.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2843 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/pgtime.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     8945 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/pl_gram.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1592 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/pl_reserved_kwlist.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2074 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/pl_reserved_kwlist_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3800 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/pl_unreserved_kwlist.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     4126 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/pl_unreserved_kwlist_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    17168 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/plerrcodes.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    37657 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/plpgsql.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.118375 pglast-5.2/libpg_query/src/postgres/include/port/
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.122375 pglast-5.2/libpg_query/src/postgres/include/port/atomics/
--rw-rw-r--   0 lele      (1000) lele      (1000)      966 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/port/atomics/arch-arm.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     7081 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/port/atomics/arch-ppc.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     7357 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/port/atomics/arch-x86.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     5653 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/port/atomics/fallback.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     8837 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/port/atomics/generic-gcc.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    11081 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/port/atomics/generic.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    15634 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/port/atomics.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     6827 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/port/pg_bitutils.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     4268 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/port/pg_bswap.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3277 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/port/pg_crc32c.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    17459 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/port.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.122375 pglast-5.2/libpg_query/src/postgres/include/portability/
--rw-rw-r--   0 lele      (1000) lele      (1000)     7053 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/portability/instr_time.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    24207 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/postgres.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2239 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/src/postgres/include/postgres_ext.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.122375 pglast-5.2/libpg_query/src/postgres/include/postmaster/
--rw-rw-r--   0 lele      (1000) lele      (1000)     2689 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/postmaster/autovacuum.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      627 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/postmaster/auxprocess.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     6134 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/postmaster/bgworker.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2185 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/postmaster/bgworker_internals.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1370 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/postmaster/bgwriter.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      451 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/postmaster/fork_process.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1008 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/postmaster/interrupt.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2327 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/postmaster/pgarch.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2837 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/postmaster/postmaster.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1192 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/postmaster/startup.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3177 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/postmaster/syslogger.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      571 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/postmaster/walwriter.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.122375 pglast-5.2/libpg_query/src/postgres/include/regex/
--rw-rw-r--   0 lele      (1000) lele      (1000)     7559 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/regex/regex.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.122375 pglast-5.2/libpg_query/src/postgres/include/replication/
--rw-rw-r--   0 lele      (1000) lele      (1000)      870 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/replication/logicallauncher.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     9613 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/replication/logicalproto.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      515 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/replication/logicalworker.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2435 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/replication/origin.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    21080 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/replication/reorderbuffer.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     7741 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/replication/slot.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3602 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/replication/syncrep.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    15207 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/replication/walreceiver.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1979 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/replication/walsender.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.122375 pglast-5.2/libpg_query/src/postgres/include/rewrite/
--rw-rw-r--   0 lele      (1000) lele      (1000)     1056 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/rewrite/prs2lock.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1168 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/rewrite/rewriteHandler.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3100 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/rewrite/rewriteManip.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      782 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/rewrite/rewriteSupport.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.130375 pglast-5.2/libpg_query/src/postgres/include/storage/
--rw-rw-r--   0 lele      (1000) lele      (1000)     1130 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/backendid.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3100 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/block.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1086 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/buf.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    10127 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/bufmgr.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    16310 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/bufpage.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2971 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/condition_variable.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2102 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/dsm.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2212 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/dsm_impl.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     7635 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/fd.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1166 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/fileset.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2920 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/ipc.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      473 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/item.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     4428 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/itemid.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     5709 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/itemptr.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3665 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/large_object.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     7135 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/latch.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     4644 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/lmgr.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    24824 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/lock.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2060 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/lockdefs.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     7350 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/lwlock.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2640 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/src/postgres/include/storage/lwlocknames.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1562 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/off.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2191 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/pg_sema.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2905 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/pg_shmem.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3435 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/pmsignal.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3228 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/predicate.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    18569 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/proc.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     4009 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/procarray.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1592 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/proclist_types.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2351 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/procsignal.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3903 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/relfilenode.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    31291 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/s_lock.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1036 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/sharedfileset.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2753 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/shm_mq.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2255 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/shm_toc.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2850 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/shmem.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     5639 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/sinval.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1623 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/sinvaladt.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     4467 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/smgr.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2491 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/spin.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3879 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/standby.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2318 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/standbydefs.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2031 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/storage/sync.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.130375 pglast-5.2/libpg_query/src/postgres/include/tcop/
--rw-rw-r--   0 lele      (1000) lele      (1000)     1459 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/tcop/cmdtag.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    14664 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/tcop/cmdtaglist.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2088 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/tcop/deparse_utility.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     6160 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/tcop/dest.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      514 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/tcop/fastpath.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1372 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/tcop/pquery.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3682 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/tcop/tcopprot.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3994 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/tcop/utility.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.130375 pglast-5.2/libpg_query/src/postgres/include/tsearch/
--rw-rw-r--   0 lele      (1000) lele      (1000)     2125 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/tsearch/ts_cache.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.138374 pglast-5.2/libpg_query/src/postgres/include/utils/
--rw-rw-r--   0 lele      (1000) lele      (1000)    14055 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/acl.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1451 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/aclchk_internal.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    17915 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/array.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1215 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/backend_progress.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     9374 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/backend_status.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     4407 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/builtins.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      637 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/bytea.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     8613 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/catcache.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3246 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/date.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    10712 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/datetime.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2380 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/datum.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     4859 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/dsa.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      523 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/dynahash.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    17600 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/elog.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    22334 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/errcodes.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     7075 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/expandeddatum.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     9635 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/expandedrecord.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     8439 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/float.h
--rw-rw-r--   0 lele      (1000) lele      (1000)   104816 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/fmgroids.h
--rw-rw-r--   0 lele      (1000) lele      (1000)   136097 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/fmgrprotos.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1501 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/fmgrtab.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    18082 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/guc.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     8318 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/guc_tables.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     5963 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/hsearch.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1929 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/inval.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     9013 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/lsyscache.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2196 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/memdebug.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     8057 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/memutils.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3068 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/numeric.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     5915 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/palloc.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2362 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/partcache.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3887 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/pg_locale.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      840 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/pg_lsn.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    22060 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/pgstat_internal.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2113 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/pidfile.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    10830 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/plancache.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    10507 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/portal.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     7568 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/src/postgres/include/utils/probes.h
--rw-rw-r--   0 lele      (1000) lele      (1000)      602 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/ps_status.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2810 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/queryenvironment.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2257 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/queryjumble.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1519 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/regproc.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    24885 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/rel.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     4799 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/relcache.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2258 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/reltrigger.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2831 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/resowner.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1784 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/rls.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1705 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/ruleutils.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1907 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/sharedtuplestore.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     6976 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/snapmgr.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     8021 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/snapshot.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    13622 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/sortsupport.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     6579 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/syscache.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2829 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/timeout.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     4415 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/timestamp.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    12855 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/tuplesort.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3366 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/tuplestore.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     7622 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/typcache.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1159 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/tzparser.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1541 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/varlena.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     8603 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/wait_event.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2786 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/include/utils/xml.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    33659 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_catalog_namespace.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     4143 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_catalog_pg_proc.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     2740 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_commands_define.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    11639 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_nodes_bitmapset.c
--rw-rw-r--   0 lele      (1000) lele      (1000)   135144 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_nodes_copyfuncs.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    98014 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_nodes_equalfuncs.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     2473 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_nodes_extensible.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    27163 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_nodes_list.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     8618 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_nodes_makefuncs.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    42760 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_nodes_nodeFuncs.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     1449 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_nodes_value.c
--rw-rw-r--   0 lele      (1000) lele      (1000)  2518588 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_parser_gram.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    13800 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_parser_parser.c
--rw-rw-r--   0 lele      (1000) lele      (1000)   339600 2023-02-10 08:11:28.000000 pglast-5.2/libpg_query/src/postgres/src_backend_parser_scan.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     3825 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_parser_scansup.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    61905 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_postmaster_postmaster.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     6035 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_storage_ipc_ipc.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     9856 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_storage_lmgr_s_lock.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    20772 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_tcop_postgres.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     2914 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_utils_activity_pgstat_database.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    11164 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_utils_adt_datum.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     2596 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_utils_adt_expandeddatum.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     4679 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_utils_adt_format_type.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    57648 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_utils_adt_ruleutils.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     2111 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_utils_error_assert.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    51006 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_utils_error_elog.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    15343 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_utils_fmgr_fmgr.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    35477 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_utils_hash_dynahash.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     3289 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_utils_init_globals.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    22803 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_utils_mb_mbutils.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    50256 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_utils_misc_guc.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    48567 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_utils_mmgr_aset.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    32000 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_backend_utils_mmgr_mcxt.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     3541 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_common_encnames.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    12002 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_common_hashfn.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     1195 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_common_keywords.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    16965 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_common_kwlist_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2568 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_common_kwlookup.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     3294 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_common_pg_prng.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     4533 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_common_psprintf.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     2402 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_common_string.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     8700 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_common_stringinfo.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    48699 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_common_wchar.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    31225 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_pl_plpgsql_src_pl_comp.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    18660 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_pl_plpgsql_src_pl_funcs.c
--rw-rw-r--   0 lele      (1000) lele      (1000)   202852 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_pl_plpgsql_src_pl_gram.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     2018 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_pl_plpgsql_src_pl_handler.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     2384 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_pl_plpgsql_src_pl_reserved_kwlist_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    18612 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_pl_plpgsql_src_pl_scanner.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     4444 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_pl_plpgsql_src_pl_unreserved_kwlist_d.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     5403 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_port_pg_bitutils.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     2189 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_port_pgsleep.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     2315 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_port_pgstrcasecmp.c
--rw-rw-r--   0 lele      (1000) lele      (1000)      613 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/src/postgres/src_port_qsort.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    34914 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_port_snprintf.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     6965 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_port_strerror.c
--rw-rw-r--   0 lele      (1000) lele      (1000)     1012 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/src/postgres/src_port_strnlen.c
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.138374 pglast-5.2/libpg_query/srcdata/
--rw-rw-r--   0 lele      (1000) lele      (1000)     1206 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/srcdata/all_known_enums.json
--rw-rw-r--   0 lele      (1000) lele      (1000)   162108 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/srcdata/enum_defs.json
--rw-rw-r--   0 lele      (1000) lele      (1000)     8261 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/srcdata/nodetypes.json
--rw-rw-r--   0 lele      (1000) lele      (1000)   320269 2022-12-02 06:45:28.000000 pglast-5.2/libpg_query/srcdata/struct_defs.json
--rw-rw-r--   0 lele      (1000) lele      (1000)     8193 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/srcdata/typedefs.json
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.062376 pglast-5.2/libpg_query/test/
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.062376 pglast-5.2/libpg_query/test/sql/
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.170374 pglast-5.2/libpg_query/test/sql/postgres_regress/
--rw-rw-r--   0 lele      (1000) lele      (1000)     4097 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/advisory_lock.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    40418 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/aggregates.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    28361 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/alter_generic.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     3397 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/alter_operator.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)   114445 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/alter_table.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     4261 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/amutils.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    27257 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/arrays.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      767 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/async.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     7764 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/bit.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1365 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/bitmapops.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     5501 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/boolean.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     8011 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/box.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    18088 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/brin.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    11310 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/brin_bloom.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    14944 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/brin_multi.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     7779 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/btree_index.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     6236 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/case.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1776 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/char.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1364 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/circle.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    12412 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/cluster.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    29968 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/collate.icu.utf8.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    15125 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/collate.linux.utf8.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    11513 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/collate.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     2830 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/combocid.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1041 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/comments.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     5590 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/compression.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    17298 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/constraints.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    13138 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/conversion.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     6930 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/copy.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    10255 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/copy2.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     3911 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/copydml.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     2211 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/copyselect.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     8327 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/create_aggregate.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     8808 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/create_am.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1596 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/create_cast.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1148 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/create_function_c.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    13412 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/create_function_sql.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    47027 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/create_index.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    17028 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/create_index_spgist.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     6144 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/create_misc.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     5909 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/create_operator.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     5188 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/create_procedure.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     5440 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/create_role.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    29569 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/create_table.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     9072 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/create_table_like.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     7984 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/create_type.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    24891 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/create_view.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    11512 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/date.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     2944 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/dbsize.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      671 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/delete.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     3630 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/dependency.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    22942 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/domain.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     8931 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/drop_if_exists.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1367 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/drop_operator.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     9514 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/enum.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     8888 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/equivclass.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     6103 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/errors.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    16330 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/event_trigger.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     4623 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/explain.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     6396 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/expressions.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    16417 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/fast_default.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    11349 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/float4.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    15968 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/float8.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    35554 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/foreign_data.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    76770 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/foreign_key.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     5389 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/functional_deps.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    20127 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/generated.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    14606 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/geometry.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     5655 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/gin.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     6371 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/gist.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    21315 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/groupingsets.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    10372 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/guc.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    13559 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/hash_func.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     6398 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/hash_index.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     3126 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/hash_part.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    24856 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/horology.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    12882 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/identity.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    12501 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/incremental_sort.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    10174 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/index_including.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     3872 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/index_including_gist.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    37633 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/indexing.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     3339 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/indirect_toast.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    10374 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/inet.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      995 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/infinite_recurse.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    43363 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/inherit.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      364 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/init_privs.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    25563 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/insert.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    28212 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/insert_conflict.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     2785 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/int2.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     4534 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/int4.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     9303 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/int8.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    22509 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/interval.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    68118 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/join.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    20252 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/join_hash.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    35738 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/json.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     3504 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/json_encoding.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    70496 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/jsonb.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    36554 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/jsonb_jsonpath.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     6558 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/jsonpath.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     2488 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/jsonpath_encoding.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     8668 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/largeobject.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     6077 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/limit.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1343 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/line.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     6597 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/lock.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      778 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/lseg.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1847 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/macaddr.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     4288 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/macaddr8.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    12345 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/matview.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     5234 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/memoize.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    35511 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/merge.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     6827 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/misc.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     6914 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/misc_functions.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     2371 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/misc_sanity.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     3825 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/money.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    41427 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/multirangetypes.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1886 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/mvcc.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     3399 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/name.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1409 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/namespace.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    58045 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/numeric.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)   304889 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/numeric_big.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     2304 2023-02-10 08:11:28.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/numerology.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    13166 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/object_address.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1236 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/oid.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1559 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/oidjoins.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    53611 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/opr_sanity.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    17532 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/partition_aggregate.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     5619 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/partition_info.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    64684 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/partition_join.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    52394 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/partition_prune.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     5027 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/password.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1012 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/path.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1796 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/pg_lsn.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     5878 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/plancache.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)   121705 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/plpgsql.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     3215 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/point.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     5251 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/polygon.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    38472 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/polymorphism.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    14468 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/portals.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1375 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/portals_p2.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     2234 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/prepare.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     4020 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/prepared_xacts.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    62670 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/privileges.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    37432 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/psql.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     3686 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/psql_crosstab.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    48460 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/publication.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1142 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/random.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    33410 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/rangefuncs.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    25404 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/rangetypes.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     6035 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/regex.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     3356 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/regproc.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     2575 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/reindex_catalog.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     5476 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/reloptions.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     4772 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/replica_identity.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     3901 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/returning.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     9159 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/roleattributes.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    73108 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/rowsecurity.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    16638 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/rowtypes.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    42539 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/rules.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1986 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/sanity_check.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1576 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/security_label.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     8129 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/select.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     4508 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/select_distinct.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      587 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/select_distinct_on.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1749 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/select_having.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     5500 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/select_implicit.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     4880 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/select_into.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    15079 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/select_parallel.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     5379 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/select_views.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    12228 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/sequence.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     3672 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/spgist.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    16648 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/stats.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    74163 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/stats_ext.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    30800 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/strings.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     9508 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/subscription.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    26655 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/subselect.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     2983 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/sysviews.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     4268 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/tablesample.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    20103 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/tablespace.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     8124 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/temp.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     6387 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/test_setup.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     4136 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/text.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     2031 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/tid.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     3247 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/tidrangescan.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     3627 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/tidscan.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     2710 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/time.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    14175 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/timestamp.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    25820 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/timestamptz.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     3533 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/timetz.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    16701 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/transactions.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    96332 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/triggers.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     9834 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/truncate.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     9307 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/tsdicts.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    35645 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/tsearch.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     7917 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/tsrf.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    14061 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/tstypes.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    10455 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/tuplesort.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     3185 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/txid.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    21411 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/type_sanity.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1758 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/typed_table.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1247 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/unicode.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    17131 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/union.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    60351 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/updatable_views.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    26663 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/update.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     3188 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/uuid.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    11384 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/vacuum.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     2184 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/vacuum_parallel.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1258 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/varchar.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    59955 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/window.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    41225 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/with.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1434 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/write_parallel.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     4790 2022-12-01 07:07:45.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/xid.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    28479 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/xml.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     2989 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/test/sql/postgres_regress/xmlmap.sql
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.062376 pglast-5.2/libpg_query/vendor/
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.170374 pglast-5.2/libpg_query/vendor/protobuf-c/
--rw-rw-r--   0 lele      (1000) lele      (1000)    96734 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/vendor/protobuf-c/protobuf-c.c
--rw-rw-r--   0 lele      (1000) lele      (1000)    33674 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/vendor/protobuf-c/protobuf-c.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.174374 pglast-5.2/libpg_query/vendor/xxhash/
--rw-rw-r--   0 lele      (1000) lele      (1000)     1854 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/vendor/xxhash/xxhash.c
--rw-rw-r--   0 lele      (1000) lele      (1000)   204232 2022-12-01 07:05:49.000000 pglast-5.2/libpg_query/vendor/xxhash/xxhash.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.178374 pglast-5.2/pglast/
--rw-r--r--   0 lele      (1000) lele      (1000)     4576 2023-05-20 07:30:24.000000 pglast-5.2/pglast/__init__.py
--rw-rw-r--   0 lele      (1000) lele      (1000)     4551 2022-12-01 07:04:43.000000 pglast-5.2/pglast/__main__.py
--rw-r--r--   0 lele      (1000) lele      (1000)   180264 2023-05-19 08:03:11.000000 pglast-5.2/pglast/ast.py
--rw-r--r--   0 lele      (1000) lele      (1000)   155182 2023-05-19 08:03:11.000000 pglast-5.2/pglast/ast.pyx
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.178374 pglast-5.2/pglast/enums/
--rw-rw-r--   0 lele      (1000) lele      (1000)      741 2022-12-01 07:04:43.000000 pglast-5.2/pglast/enums/__init__.py
--rw-r--r--   0 lele      (1000) lele      (1000)      690 2023-05-19 08:03:09.000000 pglast-5.2/pglast/enums/lockdefs.py
--rw-r--r--   0 lele      (1000) lele      (1000)      890 2023-05-19 08:03:10.000000 pglast-5.2/pglast/enums/lockoptions.py
--rw-r--r--   0 lele      (1000) lele      (1000)    14455 2023-05-19 08:03:10.000000 pglast-5.2/pglast/enums/nodes.py
--rw-r--r--   0 lele      (1000) lele      (1000)    12252 2023-05-19 08:03:10.000000 pglast-5.2/pglast/enums/parsenodes.py
--rw-r--r--   0 lele      (1000) lele      (1000)      521 2023-05-19 08:03:10.000000 pglast-5.2/pglast/enums/pg_am.py
--rw-r--r--   0 lele      (1000) lele      (1000)      592 2023-05-19 08:03:10.000000 pglast-5.2/pglast/enums/pg_attribute.py
--rw-r--r--   0 lele      (1000) lele      (1000)      960 2023-05-19 08:03:10.000000 pglast-5.2/pglast/enums/pg_class.py
--rw-r--r--   0 lele      (1000) lele      (1000)      748 2023-05-19 08:03:10.000000 pglast-5.2/pglast/enums/pg_trigger.py
--rw-r--r--   0 lele      (1000) lele      (1000)     2696 2023-05-19 08:03:10.000000 pglast-5.2/pglast/enums/primnodes.py
--rw-r--r--   0 lele      (1000) lele      (1000)      846 2023-05-19 08:03:11.000000 pglast-5.2/pglast/enums/xml.py
--rw-rw-r--   0 lele      (1000) lele      (1000)      333 2022-12-01 07:04:43.000000 pglast-5.2/pglast/error.py
--rw-rw-r--   0 lele      (1000) lele      (1000)     6786 2023-05-19 08:03:41.000000 pglast-5.2/pglast/keywords.py
--rw-rw-r--   0 lele      (1000) lele      (1000)  3000439 2023-05-19 08:03:16.000000 pglast-5.2/pglast/parser.c
--rw-r--r--   0 lele      (1000) lele      (1000)    15555 2023-05-19 08:03:11.000000 pglast-5.2/pglast/parser.pyx
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.178374 pglast-5.2/pglast/printers/
--rw-r--r--   0 lele      (1000) lele      (1000)     6280 2022-12-04 09:39:06.000000 pglast-5.2/pglast/printers/__init__.py
--rw-rw-r--   0 lele      (1000) lele      (1000)   112907 2023-04-27 06:18:51.000000 pglast-5.2/pglast/printers/ddl.py
--rw-rw-r--   0 lele      (1000) lele      (1000)    65995 2023-02-28 06:47:01.000000 pglast-5.2/pglast/printers/dml.py
--rw-r--r--   0 lele      (1000) lele      (1000)     5173 2022-12-04 09:39:06.000000 pglast-5.2/pglast/printers/sfuncs.py
--rw-r--r--   0 lele      (1000) lele      (1000)    27863 2022-12-04 11:55:32.000000 pglast-5.2/pglast/stream.py
--rw-r--r--   0 lele      (1000) lele      (1000)    58201 2023-05-19 08:03:11.000000 pglast-5.2/pglast/structs.pxd
--rw-r--r--   0 lele      (1000) lele      (1000)    17561 2022-12-04 09:52:17.000000 pglast-5.2/pglast/visitors.py
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.178374 pglast-5.2/pglast.egg-info/
--rw-rw-r--   0 lele      (1000) lele      (1000)    26923 2023-05-20 07:30:24.000000 pglast-5.2/pglast.egg-info/PKG-INFO
--rw-rw-r--   0 lele      (1000) lele      (1000)    41162 2023-05-20 07:30:25.000000 pglast-5.2/pglast.egg-info/SOURCES.txt
--rw-rw-r--   0 lele      (1000) lele      (1000)        1 2023-05-20 07:30:24.000000 pglast-5.2/pglast.egg-info/dependency_links.txt
--rw-rw-r--   0 lele      (1000) lele      (1000)       46 2023-05-20 07:30:24.000000 pglast-5.2/pglast.egg-info/entry_points.txt
--rw-rw-r--   0 lele      (1000) lele      (1000)       82 2023-05-20 07:30:24.000000 pglast-5.2/pglast.egg-info/requires.txt
--rw-rw-r--   0 lele      (1000) lele      (1000)        7 2023-05-20 07:30:24.000000 pglast-5.2/pglast.egg-info/top_level.txt
--rw-r--r--   0 lele      (1000) lele      (1000)      357 2023-03-29 06:30:40.000000 pglast-5.2/requirements-test.txt
--rw-r--r--   0 lele      (1000) lele      (1000)      457 2023-03-29 06:30:40.000000 pglast-5.2/requirements.txt
--rw-rw-r--   0 lele      (1000) lele      (1000)      318 2023-05-20 07:30:25.194373 pglast-5.2/setup.cfg
--rw-rw-r--   0 lele      (1000) lele      (1000)     3061 2022-12-01 07:04:43.000000 pglast-5.2/setup.py
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.182374 pglast-5.2/tests/
--rw-r--r--   0 lele      (1000) lele      (1000)     3871 2023-02-11 09:52:17.000000 pglast-5.2/tests/test_ast.py
--rw-r--r--   0 lele      (1000) lele      (1000)     8014 2022-12-04 10:22:40.000000 pglast-5.2/tests/test_cli.py
--rw-r--r--   0 lele      (1000) lele      (1000)     6110 2022-12-04 10:26:19.000000 pglast-5.2/tests/test_parser.py
--rw-rw-r--   0 lele      (1000) lele      (1000)     3531 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers.py
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.066376 pglast-5.2/tests/test_printers_prettification/
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.186373 pglast-5.2/tests/test_printers_prettification/ddl/
--rw-rw-r--   0 lele      (1000) lele      (1000)      384 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/ddl/alter_default_privileges.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1060 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/ddl/alter_subscription.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      103 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/ddl/alter_text_search.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      548 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/ddl/comment.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      752 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/ddl/create_aggregate.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      480 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/ddl/create_database.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      449 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/ddl/create_domain.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      647 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/ddl/create_event_trigger.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      267 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/ddl/create_extension.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      993 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/ddl/create_foreign_data_wrapper.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1262 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/ddl/create_foreign_table.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     2089 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/ddl/create_function.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      235 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/ddl/create_index.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      298 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/ddl/create_language.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      900 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/ddl/create_rule.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      300 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/ddl/create_schema.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      184 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/ddl/create_sequence.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     2049 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/ddl/create_table.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      306 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/ddl/create_transform.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     2483 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/ddl/create_trigger.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)       34 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/ddl/create_type.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      121 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/ddl/create_view.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      348 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/ddl/grant.sql
--rw-r--r--   0 lele      (1000) lele      (1000)      800 2022-12-19 09:20:50.000000 pglast-5.2/tests/test_printers_prettification/ddl/issue110.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)       97 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/ddl/notify.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)       20 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/ddl/show.sql
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.186373 pglast-5.2/tests/test_printers_prettification/dml/
--rw-r--r--   0 lele      (1000) lele      (1000)      523 2022-12-04 11:06:47.000000 pglast-5.2/tests/test_printers_prettification/dml/copy.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      907 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/dml/insert.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)    11464 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/dml/select.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      216 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/dml/truncate.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      638 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification/dml/update.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     2717 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_prettification.py
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.066376 pglast-5.2/tests/test_printers_roundtrip/
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.190373 pglast-5.2/tests/test_printers_roundtrip/ddl/
--rw-rw-r--   0 lele      (1000) lele      (1000)      123 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/alter_database.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      240 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/alter_default_privileges.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)       52 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/alter_domain.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      183 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/alter_extension.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)       42 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/alter_fdw.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      192 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/alter_function.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      136 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/alter_owner.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      124 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/alter_policy.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      415 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/alter_rename.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      194 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/alter_role.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)       74 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/alter_sequence.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)       30 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/alter_server.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)       99 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/alter_set_schema.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      210 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/alter_subscription.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     2054 2022-12-04 10:36:47.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/alter_table.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      259 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/alter_text_search.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      233 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/alter_type.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)       48 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/analyze.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)       53 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/cluster.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     2849 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/comment.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      138 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/create_access_method.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1226 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/create_aggregate.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      447 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/create_cast.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      352 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/create_collation.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      129 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/create_conversion.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      274 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/create_database.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      155 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/create_fdw.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      811 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/create_function.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      667 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/create_index.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      602 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/create_operator.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1095 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/create_operator_class.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      274 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/create_policy.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)       69 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/create_role.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      243 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/create_schema.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      387 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/create_sequence.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     7017 2023-04-27 06:15:47.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/create_table.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      874 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/create_trigger.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)       89 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/create_type.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      144 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/create_view.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)       60 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/discard.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)       41 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/do.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1902 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/drop.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      298 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/grant.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)       85 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/lock_table.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)       90 2022-12-04 16:30:03.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/reindex.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)       97 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/revoke.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)       52 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/security_label.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      169 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/ddl/vacuum.sql
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.194373 pglast-5.2/tests/test_printers_roundtrip/dml/
--rw-r--r--   0 lele      (1000) lele      (1000)      418 2022-12-04 11:29:45.000000 pglast-5.2/tests/test_printers_roundtrip/dml/copy.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)       70 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/dml/cursor.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      552 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/dml/delete.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1537 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/dml/insert.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)       29 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/dml/reset.sql
--rw-r--r--   0 lele      (1000) lele      (1000)    14276 2023-02-11 11:00:01.000000 pglast-5.2/tests/test_printers_roundtrip/dml/select.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      642 2023-02-28 06:31:27.000000 pglast-5.2/tests/test_printers_roundtrip/dml/set.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)      404 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/dml/transaction.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     1078 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip/dml/update.sql
--rw-rw-r--   0 lele      (1000) lele      (1000)     5300 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_printers_roundtrip.py
--rw-rw-r--   0 lele      (1000) lele      (1000)     4014 2022-12-01 07:04:43.000000 pglast-5.2/tests/test_stream.py
--rw-r--r--   0 lele      (1000) lele      (1000)    10262 2022-12-04 09:39:06.000000 pglast-5.2/tests/test_visitors.py
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-05-20 07:30:25.194373 pglast-5.2/tools/
--rw-rw-r--   0 lele      (1000) lele      (1000)    32699 2023-02-28 06:40:06.000000 pglast-5.2/tools/extract_ast.py
--rw-rw-r--   0 lele      (1000) lele      (1000)     9613 2022-12-01 07:04:43.000000 pglast-5.2/tools/extract_enums.py
--rw-rw-r--   0 lele      (1000) lele      (1000)     2566 2022-12-01 07:04:43.000000 pglast-5.2/tools/extract_keywords.py
--rw-r--r--   0 lele      (1000) lele      (1000)     5846 2022-12-19 18:19:58.000000 pglast-5.2/tools/extract_printers_doc.py
--rw-r--r--   0 lele      (1000) lele      (1000)        3 2023-05-20 07:29:52.000000 pglast-5.2/version.txt
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.640143 pglast-5.3/
+-rw-rw-r--   0 lele      (1000) lele      (1000)    23628 2023-08-05 06:54:59.000000 pglast-5.3/CHANGES.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)      843 2022-12-01 07:04:43.000000 pglast-5.3/MANIFEST.in
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4716 2023-01-11 20:10:25.000000 pglast-5.3/Makefile
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2763 2022-12-01 07:04:43.000000 pglast-5.3/Makefile.release
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1328 2022-12-01 07:04:43.000000 pglast-5.3/Makefile.virtualenv
+-rw-rw-r--   0 lele      (1000) lele      (1000)    27066 2023-08-05 06:55:40.640143 pglast-5.3/PKG-INFO
+-rw-r--r--   0 lele      (1000) lele      (1000)     2426 2023-02-19 16:04:29.000000 pglast-5.3/README.rst
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.516145 pglast-5.3/docs/
+-rw-rw-r--   0 lele      (1000) lele      (1000)      607 2022-12-01 07:04:43.000000 pglast-5.3/docs/Makefile
+-rw-rw-r--   0 lele      (1000) lele      (1000)      625 2022-12-01 07:04:43.000000 pglast-5.3/docs/api.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)   148863 2023-08-05 06:32:29.000000 pglast-5.3/docs/ast.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)    23628 2023-08-05 06:54:59.000000 pglast-5.3/docs/changes.rst
+-rw-r--r--   0 lele      (1000) lele      (1000)     5216 2022-12-13 12:49:31.000000 pglast-5.3/docs/conf.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)    42541 2023-08-05 06:32:58.000000 pglast-5.3/docs/ddl.rst
+-rw-r--r--   0 lele      (1000) lele      (1000)     6702 2022-12-19 18:34:08.000000 pglast-5.3/docs/development.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)    23171 2023-08-05 06:32:58.000000 pglast-5.3/docs/dml.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1049 2022-12-01 07:04:43.000000 pglast-5.3/docs/enums.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1194 2022-12-13 12:47:14.000000 pglast-5.3/docs/index.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)      540 2022-12-01 07:04:43.000000 pglast-5.3/docs/installation.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1926 2022-12-01 07:04:43.000000 pglast-5.3/docs/introduction.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)      756 2022-12-01 07:04:43.000000 pglast-5.3/docs/keywords.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2216 2023-08-05 06:32:27.000000 pglast-5.3/docs/lockdefs.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1642 2023-08-05 06:32:27.000000 pglast-5.3/docs/lockoptions.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)    17012 2023-08-05 06:32:28.000000 pglast-5.3/docs/nodes.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)    26350 2023-08-05 06:32:28.000000 pglast-5.3/docs/parsenodes.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3922 2022-12-01 07:04:43.000000 pglast-5.3/docs/parser.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)      925 2023-08-05 06:32:28.000000 pglast-5.3/docs/pg_am.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1207 2023-08-05 06:32:28.000000 pglast-5.3/docs/pg_attribute.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3421 2023-08-05 06:32:28.000000 pglast-5.3/docs/pg_class.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2139 2023-08-05 06:32:28.000000 pglast-5.3/docs/pg_trigger.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5204 2023-08-05 06:32:28.000000 pglast-5.3/docs/primnodes.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)      963 2022-12-01 07:04:43.000000 pglast-5.3/docs/printers.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)      990 2022-12-01 07:04:43.000000 pglast-5.3/docs/sfuncs.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)      666 2022-12-01 07:04:43.000000 pglast-5.3/docs/stream.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)    15486 2022-12-04 09:48:04.000000 pglast-5.3/docs/usage.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)      580 2022-12-01 07:04:43.000000 pglast-5.3/docs/visitors.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1483 2023-08-05 06:32:29.000000 pglast-5.3/docs/xml.rst
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.516145 pglast-5.3/libpg_query/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1561 2023-02-10 08:11:28.000000 pglast-5.3/libpg_query/LICENSE
+-rw-rw-r--   0 lele      (1000) lele      (1000)    13627 2023-08-05 06:31:44.000000 pglast-5.3/libpg_query/Makefile
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3462 2023-01-11 21:06:42.000000 pglast-5.3/libpg_query/pg_query.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.520145 pglast-5.3/libpg_query/protobuf/
+-rw-rw-r--   0 lele      (1000) lele      (1000)  1257968 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/protobuf/pg_query.pb-c.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)   474315 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/protobuf/pg_query.pb-c.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)   106559 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/protobuf/pg_query.proto
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.524145 pglast-5.3/libpg_query/src/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2214 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/src/pg_query.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1406 2023-07-10 05:20:35.000000 pglast-5.3/libpg_query/src/pg_query_deparse.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    73716 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/pg_query_enum_defs.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    10960 2023-01-11 21:06:42.000000 pglast-5.3/libpg_query/src/pg_query_fingerprint.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)      257 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/src/pg_query_fingerprint.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    32338 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/pg_query_fingerprint_conds.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)   455292 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/pg_query_fingerprint_defs.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)      525 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/src/pg_query_internal.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1264 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/src/pg_query_json_helper.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    21956 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/src/pg_query_json_plpgsql.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)      162 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/src/pg_query_json_plpgsql.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    20362 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/src/pg_query_normalize.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)      243 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/src/pg_query_outfuncs.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    32991 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/pg_query_outfuncs_conds.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)   117512 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/pg_query_outfuncs_defs.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8655 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/pg_query_outfuncs_json.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8308 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/pg_query_outfuncs_protobuf.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3668 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/src/pg_query_parse.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    13406 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/src/pg_query_parse_plpgsql.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)      201 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/src/pg_query_readfuncs.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    25246 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/pg_query_readfuncs_conds.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)   123173 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/pg_query_readfuncs_defs.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5641 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/pg_query_readfuncs_protobuf.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4748 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/src/pg_query_scan.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5998 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/src/pg_query_split.c
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.536144 pglast-5.3/libpg_query/src/postgres/
+-rw-rw-r--   0 lele      (1000) lele      (1000)        0 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/src/postgres/guc-file.c
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.540144 pglast-5.3/libpg_query/src/postgres/include/
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.544144 pglast-5.3/libpg_query/src/postgres/include/access/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9967 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/amapi.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1656 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/attmap.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1547 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/attnum.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1780 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/clog.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2263 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/commit_ts.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2443 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/detoast.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9090 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/genam.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2203 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/gin.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3276 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/htup.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    29211 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/htup_details.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5347 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/itup.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2641 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/parallel.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1080 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/printtup.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      977 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/relation.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6829 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/relscan.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1400 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/rmgr.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3434 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/rmgrlist.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1470 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/sdir.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6444 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/skey.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3075 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/stratnum.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      853 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/sysattr.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      932 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/table.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    76360 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/tableam.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2738 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/toast_compression.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    12618 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/transam.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1624 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/tupconvert.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5304 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/tupdesc.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     7547 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/tupmacs.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2226 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/twophase.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    17876 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/xact.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    11150 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/xlog.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    12298 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/xlog_internal.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3022 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/xlogdefs.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1515 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/xlogprefetcher.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    15433 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/xlogreader.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8744 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/xlogrecord.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5330 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/access/xlogrecovery.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    45563 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/c.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.552144 pglast-5.3/libpg_query/src/postgres/include/catalog/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1295 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/catalog.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2591 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/catversion.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9705 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/dependency.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6472 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/genbki.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6577 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/index.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1824 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/indexing.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     7383 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/namespace.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9202 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/objectaccess.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3208 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/objectaddress.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6006 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_aggregate.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2817 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_aggregate_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1594 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_am.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1154 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_am_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     7827 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_attribute.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1982 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_attribute_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2335 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_authid.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1763 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_authid_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     7973 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_class.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4725 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_class_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2948 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_collation.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1598 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_collation_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9801 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_constraint.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2392 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_constraint_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9099 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_control.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2476 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_conversion.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1134 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_conversion_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2807 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_depend.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      991 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_depend_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1915 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_event_trigger.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1084 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_event_trigger_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3545 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_index.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1827 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_index_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2056 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_language.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1168 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_language_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1941 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_namespace.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1005 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_namespace_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3242 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_opclass.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1544 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_opclass_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3202 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_operator.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4976 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_operator_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1893 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_opfamily.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1437 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_opfamily_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1924 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_parameter_acl.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      997 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_parameter_acl_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2814 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_partitioned_table.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1162 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_partitioned_table_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6659 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_proc.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3381 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_proc_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4916 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_publication.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1148 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_publication_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2093 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_replication_origin.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1021 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_replication_origin_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    12527 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_statistic.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9160 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_statistic_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2990 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_statistic_ext.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1347 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_statistic_ext_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1542 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_transform.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      954 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_transform_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6313 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_trigger.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4237 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_trigger_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1526 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_ts_config.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      954 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_ts_config_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1681 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_ts_dict.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      991 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_ts_dict_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1750 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_ts_parser.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1067 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_ts_parser_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1583 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_ts_template.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      985 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_ts_template_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    14425 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_type.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9672 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/pg_type_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1752 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/catalog/storage.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.556144 pglast-5.3/libpg_query/src/postgres/include/commands/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1592 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/commands/async.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1419 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/commands/dbcommands.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6863 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/commands/defrem.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3343 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/commands/event_trigger.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4972 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/commands/explain.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2201 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/commands/prepare.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2067 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/commands/tablespace.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    10160 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/commands/trigger.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1329 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/commands/user.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    13483 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/commands/vacuum.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1773 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/commands/variable.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.556144 pglast-5.3/libpg_query/src/postgres/include/common/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1716 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/common/file_perm.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2558 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/common/hashfn.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      942 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/common/ip.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      845 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/common/keywords.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1482 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/common/kwlookup.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2132 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/common/pg_prng.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2622 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/common/relpath.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1541 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/common/string.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6132 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/common/unicode_combining_table.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2569 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/common/unicode_east_asian_fw_table.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.556144 pglast-5.3/libpg_query/src/postgres/include/datatype/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8640 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/datatype/timestamp.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.556144 pglast-5.3/libpg_query/src/postgres/include/executor/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2393 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/executor/execdesc.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    25464 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/executor/executor.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1828 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/executor/functions.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4975 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/executor/instrument.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     7898 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/executor/spi.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2850 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/executor/tablefunc.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    17334 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/executor/tuptable.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    34850 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/fmgr.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    12948 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/funcapi.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3972 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/getaddrinfo.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.556144 pglast-5.3/libpg_query/src/postgres/include/jit/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2820 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/jit/jit.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    16679 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/kwlist_d.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.556144 pglast-5.3/libpg_query/src/postgres/include/lib/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4429 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/lib/dshash.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    21457 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/lib/ilist.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3505 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/lib/pairingheap.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    33200 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/lib/simplehash.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    13087 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/lib/sort_template.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5803 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/lib/stringinfo.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.560144 pglast-5.3/libpg_query/src/postgres/include/libpq/
+-rw-rw-r--   0 lele      (1000) lele      (1000)      981 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/libpq/auth.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1527 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/libpq/crypt.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4099 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/libpq/hba.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    10842 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/libpq/libpq-be.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4549 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/libpq/libpq.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6136 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/libpq/pqcomm.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5968 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/libpq/pqformat.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1236 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/libpq/pqsignal.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.560144 pglast-5.3/libpg_query/src/postgres/include/mb/
+-rw-rw-r--   0 lele      (1000) lele      (1000)    28560 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/mb/pg_wchar.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      667 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/mb/stringinfo_mb.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    17867 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/miscadmin.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.560144 pglast-5.3/libpg_query/src/postgres/include/nodes/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4414 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/nodes/bitmapset.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)   100579 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/nodes/execnodes.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5629 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/nodes/extensible.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1884 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/nodes/lockoptions.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3528 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/nodes/makefuncs.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4030 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/nodes/memnodes.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5109 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/nodes/nodeFuncs.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    21378 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/nodes/nodes.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6697 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/nodes/params.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)   131739 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/nodes/parsenodes.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)   115826 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/nodes/pathnodes.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    21912 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/nodes/pg_list.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    50560 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/nodes/plannodes.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    66016 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/nodes/primnodes.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1077 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/nodes/print.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2732 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/nodes/tidbitmap.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2118 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/nodes/value.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.564144 pglast-5.3/libpg_query/src/postgres/include/optimizer/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9691 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/optimizer/cost.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2278 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/optimizer/geqo.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1118 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/optimizer/geqo_gene.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     7094 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/optimizer/optimizer.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    10023 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/optimizer/paths.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4515 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/optimizer/planmain.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.564144 pglast-5.3/libpg_query/src/postgres/include/parser/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2449 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/parser/analyze.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    23149 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/parser/gram.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2284 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/parser/gramparse.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    29432 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/parser/kwlist.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2008 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/parser/parse_agg.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3713 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/parser/parse_coerce.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      722 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/parser/parse_expr.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2505 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/parser/parse_func.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    15245 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/parser/parse_node.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2406 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/parser/parse_oper.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5100 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/parser/parse_relation.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2196 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/parser/parse_type.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2082 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/parser/parser.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1473 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/parser/parsetree.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5471 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/parser/scanner.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      777 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/parser/scansup.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.564144 pglast-5.3/libpg_query/src/postgres/include/partitioning/
+-rw-rw-r--   0 lele      (1000) lele      (1000)      680 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/partitioning/partdefs.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    32515 2023-08-05 06:31:44.000000 pglast-5.3/libpg_query/src/postgres/include/pg_config.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      323 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/src/postgres/include/pg_config_ext.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    15372 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/pg_config_manual.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      158 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/src/postgres/include/pg_config_os.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1719 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/pg_getopt.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      320 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/pg_trace.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    21897 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/pgstat.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2843 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/pgtime.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8945 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/pl_gram.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1592 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/pl_reserved_kwlist.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2074 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/pl_reserved_kwlist_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3800 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/pl_unreserved_kwlist.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4126 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/pl_unreserved_kwlist_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    17168 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/plerrcodes.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    37657 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/plpgsql.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.564144 pglast-5.3/libpg_query/src/postgres/include/port/
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.568144 pglast-5.3/libpg_query/src/postgres/include/port/atomics/
+-rw-rw-r--   0 lele      (1000) lele      (1000)      966 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/port/atomics/arch-arm.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     7081 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/port/atomics/arch-ppc.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     7357 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/port/atomics/arch-x86.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5653 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/port/atomics/fallback.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8837 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/port/atomics/generic-gcc.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    11081 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/port/atomics/generic.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    15634 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/port/atomics.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6827 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/port/pg_bitutils.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4268 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/port/pg_bswap.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3277 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/port/pg_crc32c.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    17459 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/port.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.568144 pglast-5.3/libpg_query/src/postgres/include/portability/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     7053 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/portability/instr_time.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    24207 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/postgres.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2239 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/src/postgres/include/postgres_ext.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.568144 pglast-5.3/libpg_query/src/postgres/include/postmaster/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2689 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/postmaster/autovacuum.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      627 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/postmaster/auxprocess.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6134 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/postmaster/bgworker.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2185 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/postmaster/bgworker_internals.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1370 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/postmaster/bgwriter.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      451 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/postmaster/fork_process.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1008 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/postmaster/interrupt.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2327 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/postmaster/pgarch.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2837 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/postmaster/postmaster.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1192 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/postmaster/startup.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3177 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/postmaster/syslogger.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      571 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/postmaster/walwriter.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.568144 pglast-5.3/libpg_query/src/postgres/include/regex/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     7559 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/regex/regex.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.568144 pglast-5.3/libpg_query/src/postgres/include/replication/
+-rw-rw-r--   0 lele      (1000) lele      (1000)      870 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/replication/logicallauncher.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9613 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/replication/logicalproto.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      515 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/replication/logicalworker.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2435 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/replication/origin.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    21080 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/replication/reorderbuffer.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     7741 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/replication/slot.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3602 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/replication/syncrep.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    15207 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/replication/walreceiver.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1979 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/replication/walsender.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.568144 pglast-5.3/libpg_query/src/postgres/include/rewrite/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1056 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/rewrite/prs2lock.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1168 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/rewrite/rewriteHandler.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3100 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/rewrite/rewriteManip.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      782 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/rewrite/rewriteSupport.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.576144 pglast-5.3/libpg_query/src/postgres/include/storage/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1130 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/backendid.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3100 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/block.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1086 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/buf.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    10127 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/bufmgr.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    16310 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/bufpage.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2971 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/condition_variable.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2102 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/dsm.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2212 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/dsm_impl.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     7635 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/fd.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1166 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/fileset.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2920 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/ipc.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      473 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/item.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4428 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/itemid.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5709 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/itemptr.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3665 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/large_object.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     7135 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/latch.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4644 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/lmgr.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    24824 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/lock.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2060 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/lockdefs.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     7350 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/lwlock.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2640 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/src/postgres/include/storage/lwlocknames.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1562 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/off.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2191 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/pg_sema.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2905 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/pg_shmem.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3435 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/pmsignal.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3228 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/predicate.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    18569 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/proc.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4009 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/procarray.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1592 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/proclist_types.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2351 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/procsignal.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3903 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/relfilenode.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    31291 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/s_lock.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1036 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/sharedfileset.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2753 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/shm_mq.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2255 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/shm_toc.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2850 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/shmem.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5639 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/sinval.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1623 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/sinvaladt.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4467 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/smgr.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2491 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/spin.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3879 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/standby.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2318 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/standbydefs.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2031 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/storage/sync.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.576144 pglast-5.3/libpg_query/src/postgres/include/tcop/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1459 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/tcop/cmdtag.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    14664 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/tcop/cmdtaglist.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2088 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/tcop/deparse_utility.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6160 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/tcop/dest.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      514 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/tcop/fastpath.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1372 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/tcop/pquery.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3682 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/tcop/tcopprot.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3994 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/tcop/utility.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.576144 pglast-5.3/libpg_query/src/postgres/include/tsearch/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2125 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/tsearch/ts_cache.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.584144 pglast-5.3/libpg_query/src/postgres/include/utils/
+-rw-rw-r--   0 lele      (1000) lele      (1000)    14055 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/acl.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1451 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/aclchk_internal.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    17915 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/array.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1215 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/backend_progress.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9374 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/backend_status.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4407 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/builtins.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      637 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/bytea.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8613 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/catcache.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3246 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/date.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    10712 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/datetime.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2380 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/datum.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4859 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/dsa.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      523 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/dynahash.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    17600 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/elog.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    22334 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/errcodes.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     7075 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/expandeddatum.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9635 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/expandedrecord.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8439 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/float.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)   104816 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/fmgroids.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)   136097 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/fmgrprotos.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1501 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/fmgrtab.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    18082 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/guc.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8318 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/guc_tables.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5963 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/hsearch.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1929 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/inval.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9013 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/lsyscache.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2196 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/memdebug.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8057 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/memutils.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3068 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/numeric.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5915 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/palloc.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2362 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/partcache.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3887 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/pg_locale.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      840 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/pg_lsn.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    22060 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/pgstat_internal.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2113 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/pidfile.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    10830 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/plancache.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    10507 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/portal.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     7568 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/src/postgres/include/utils/probes.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)      602 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/ps_status.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2810 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/queryenvironment.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2257 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/queryjumble.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1519 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/regproc.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    24885 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/rel.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4799 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/relcache.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2258 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/reltrigger.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2831 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/resowner.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1784 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/rls.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1705 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/ruleutils.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1907 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/sharedtuplestore.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6976 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/snapmgr.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8021 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/snapshot.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    13622 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/sortsupport.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6579 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/syscache.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2829 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/timeout.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4415 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/timestamp.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    12855 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/tuplesort.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3366 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/tuplestore.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     7622 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/typcache.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1159 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/tzparser.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1541 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/varlena.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8603 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/wait_event.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2786 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/include/utils/xml.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    33659 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_catalog_namespace.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4143 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_catalog_pg_proc.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2740 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_commands_define.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    11639 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_nodes_bitmapset.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)   135144 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_nodes_copyfuncs.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    98014 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_nodes_equalfuncs.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2473 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_nodes_extensible.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    27163 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_nodes_list.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8618 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_nodes_makefuncs.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    42760 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_nodes_nodeFuncs.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1449 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_nodes_value.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)  2518588 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_parser_gram.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    13800 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_parser_parser.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)   339600 2023-02-10 08:11:28.000000 pglast-5.3/libpg_query/src/postgres/src_backend_parser_scan.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3825 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_parser_scansup.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    61905 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_postmaster_postmaster.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6035 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_storage_ipc_ipc.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9856 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_storage_lmgr_s_lock.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    20772 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_tcop_postgres.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2914 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_utils_activity_pgstat_database.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    11164 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_utils_adt_datum.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2596 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_utils_adt_expandeddatum.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4679 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_utils_adt_format_type.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    57648 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_utils_adt_ruleutils.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2111 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_utils_error_assert.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    51006 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_utils_error_elog.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    15343 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_utils_fmgr_fmgr.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    35477 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_utils_hash_dynahash.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3289 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_utils_init_globals.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    22803 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_utils_mb_mbutils.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    50256 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_utils_misc_guc.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    48567 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_utils_mmgr_aset.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    32000 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_backend_utils_mmgr_mcxt.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3541 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_common_encnames.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    12002 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_common_hashfn.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1195 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_common_keywords.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    16965 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_common_kwlist_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2568 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_common_kwlookup.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3294 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_common_pg_prng.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4533 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_common_psprintf.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2402 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_common_string.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8700 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_common_stringinfo.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    48699 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_common_wchar.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    31225 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_pl_plpgsql_src_pl_comp.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    18660 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_pl_plpgsql_src_pl_funcs.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)   202852 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_pl_plpgsql_src_pl_gram.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2018 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_pl_plpgsql_src_pl_handler.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2384 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_pl_plpgsql_src_pl_reserved_kwlist_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    18612 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_pl_plpgsql_src_pl_scanner.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4444 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_pl_plpgsql_src_pl_unreserved_kwlist_d.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5403 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_port_pg_bitutils.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2189 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_port_pgsleep.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2315 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_port_pgstrcasecmp.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)      613 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/src/postgres/src_port_qsort.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    34914 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_port_snprintf.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6965 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_port_strerror.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1012 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/src/postgres/src_port_strnlen.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)   306030 2023-08-05 06:31:44.000000 pglast-5.3/libpg_query/src/postgres_deparse.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)      185 2023-07-10 05:20:35.000000 pglast-5.3/libpg_query/src/postgres_deparse.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.588144 pglast-5.3/libpg_query/srcdata/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1206 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/srcdata/all_known_enums.json
+-rw-rw-r--   0 lele      (1000) lele      (1000)   162108 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/srcdata/enum_defs.json
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8261 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/srcdata/nodetypes.json
+-rw-rw-r--   0 lele      (1000) lele      (1000)   320269 2022-12-02 06:45:28.000000 pglast-5.3/libpg_query/srcdata/struct_defs.json
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8193 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/srcdata/typedefs.json
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.508145 pglast-5.3/libpg_query/test/
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.508145 pglast-5.3/libpg_query/test/sql/
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.620144 pglast-5.3/libpg_query/test/sql/postgres_regress/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4097 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/advisory_lock.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    40418 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/aggregates.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    28361 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/alter_generic.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3397 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/alter_operator.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)   114445 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/alter_table.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4261 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/amutils.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    27257 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/arrays.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      767 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/async.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     7764 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/bit.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1365 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/bitmapops.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5501 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/boolean.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8011 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/box.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    18088 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/brin.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    11310 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/brin_bloom.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    14944 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/brin_multi.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     7779 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/btree_index.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6236 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/case.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1776 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/char.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1364 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/circle.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    12412 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/cluster.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    29968 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/collate.icu.utf8.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    15125 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/collate.linux.utf8.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    11513 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/collate.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2830 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/combocid.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1041 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/comments.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5590 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/compression.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    17298 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/constraints.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    13138 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/conversion.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6930 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/copy.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    10255 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/copy2.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3911 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/copydml.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2211 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/copyselect.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8327 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/create_aggregate.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8808 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/create_am.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1596 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/create_cast.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1148 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/create_function_c.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    13412 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/create_function_sql.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    47027 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/create_index.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    17028 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/create_index_spgist.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6144 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/create_misc.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5909 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/create_operator.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5188 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/create_procedure.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5440 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/create_role.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    29569 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/create_table.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9072 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/create_table_like.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     7984 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/create_type.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    24891 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/create_view.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    11512 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/date.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2944 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/dbsize.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      671 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/delete.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3630 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/dependency.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    22942 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/domain.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8931 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/drop_if_exists.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1367 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/drop_operator.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9514 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/enum.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8888 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/equivclass.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6103 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/errors.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    16330 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/event_trigger.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4623 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/explain.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6396 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/expressions.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    16417 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/fast_default.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    11349 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/float4.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    15968 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/float8.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    35554 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/foreign_data.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    76770 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/foreign_key.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5389 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/functional_deps.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    20127 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/generated.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    14606 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/geometry.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5655 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/gin.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6371 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/gist.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    21315 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/groupingsets.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    10372 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/guc.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    13559 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/hash_func.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6398 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/hash_index.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3126 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/hash_part.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    24856 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/horology.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    12882 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/identity.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    12501 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/incremental_sort.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    10174 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/index_including.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3872 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/index_including_gist.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    37633 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/indexing.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3339 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/indirect_toast.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    10374 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/inet.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      995 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/infinite_recurse.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    43363 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/inherit.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      364 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/init_privs.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    25563 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/insert.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    28212 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/insert_conflict.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2785 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/int2.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4534 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/int4.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9303 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/int8.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    22509 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/interval.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    68118 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/join.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    20252 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/join_hash.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    35738 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/json.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3504 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/json_encoding.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    70496 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/jsonb.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    36554 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/jsonb_jsonpath.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6558 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/jsonpath.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2488 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/jsonpath_encoding.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8668 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/largeobject.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6077 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/limit.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1343 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/line.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6597 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/lock.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      778 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/lseg.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1847 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/macaddr.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4288 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/macaddr8.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    12345 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/matview.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5234 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/memoize.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    35511 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/merge.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6827 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/misc.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6914 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/misc_functions.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2371 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/misc_sanity.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3825 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/money.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    41427 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/multirangetypes.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1886 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/mvcc.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3399 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/name.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1409 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/namespace.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    58045 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/numeric.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)   304889 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/numeric_big.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2304 2023-02-10 08:11:28.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/numerology.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    13166 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/object_address.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1236 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/oid.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1559 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/oidjoins.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    53611 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/opr_sanity.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    17532 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/partition_aggregate.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5619 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/partition_info.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    64684 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/partition_join.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    52394 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/partition_prune.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5027 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/password.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1012 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/path.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1796 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/pg_lsn.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5878 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/plancache.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)   121705 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/plpgsql.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3215 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/point.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5251 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/polygon.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    38472 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/polymorphism.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    14468 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/portals.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1375 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/portals_p2.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2234 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/prepare.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4020 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/prepared_xacts.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    62670 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/privileges.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    37432 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/psql.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3686 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/psql_crosstab.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    48460 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/publication.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1142 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/random.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    33410 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/rangefuncs.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    25404 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/rangetypes.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6035 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/regex.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3356 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/regproc.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2575 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/reindex_catalog.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5476 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/reloptions.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4772 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/replica_identity.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3901 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/returning.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9159 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/roleattributes.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    73108 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/rowsecurity.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    16638 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/rowtypes.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    42539 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/rules.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1986 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/sanity_check.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1576 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/security_label.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8129 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/select.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4508 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/select_distinct.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      587 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/select_distinct_on.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1749 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/select_having.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5500 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/select_implicit.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4880 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/select_into.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    15079 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/select_parallel.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5379 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/select_views.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    12228 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/sequence.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3672 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/spgist.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    16648 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/stats.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    74163 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/stats_ext.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    30800 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/strings.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9508 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/subscription.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    26655 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/subselect.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2983 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/sysviews.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4268 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/tablesample.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    20103 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/tablespace.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8124 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/temp.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6387 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/test_setup.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4136 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/text.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2031 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/tid.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3247 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/tidrangescan.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3627 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/tidscan.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2710 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/time.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    14175 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/timestamp.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    25820 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/timestamptz.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3533 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/timetz.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    16701 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/transactions.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    96332 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/triggers.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9834 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/truncate.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9307 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/tsdicts.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    35645 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/tsearch.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     7917 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/tsrf.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    14061 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/tstypes.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    10455 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/tuplesort.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3185 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/txid.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    21411 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/type_sanity.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1758 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/typed_table.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1247 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/unicode.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    17131 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/union.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    60351 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/updatable_views.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    26663 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/update.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3188 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/uuid.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    11384 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/vacuum.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2184 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/vacuum_parallel.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1258 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/varchar.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    59955 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/window.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    41225 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/with.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1434 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/write_parallel.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4790 2022-12-01 07:07:45.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/xid.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    28479 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/xml.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2989 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/test/sql/postgres_regress/xmlmap.sql
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.508145 pglast-5.3/libpg_query/vendor/
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.620144 pglast-5.3/libpg_query/vendor/protobuf-c/
+-rw-rw-r--   0 lele      (1000) lele      (1000)    96734 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/vendor/protobuf-c/protobuf-c.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)    33674 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/vendor/protobuf-c/protobuf-c.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.620144 pglast-5.3/libpg_query/vendor/xxhash/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1854 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/vendor/xxhash/xxhash.c
+-rw-rw-r--   0 lele      (1000) lele      (1000)   204232 2022-12-01 07:05:49.000000 pglast-5.3/libpg_query/vendor/xxhash/xxhash.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.624143 pglast-5.3/pglast/
+-rw-r--r--   0 lele      (1000) lele      (1000)     4576 2023-08-05 06:55:13.000000 pglast-5.3/pglast/__init__.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4551 2022-12-01 07:04:43.000000 pglast-5.3/pglast/__main__.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)   180264 2023-08-05 06:32:29.000000 pglast-5.3/pglast/ast.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)   155182 2023-08-05 06:32:29.000000 pglast-5.3/pglast/ast.pyx
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.628143 pglast-5.3/pglast/enums/
+-rw-rw-r--   0 lele      (1000) lele      (1000)      741 2022-12-01 07:04:43.000000 pglast-5.3/pglast/enums/__init__.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)      690 2023-08-05 06:32:27.000000 pglast-5.3/pglast/enums/lockdefs.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)      890 2023-08-05 06:32:27.000000 pglast-5.3/pglast/enums/lockoptions.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)    14455 2023-08-05 06:32:28.000000 pglast-5.3/pglast/enums/nodes.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)    12252 2023-08-05 06:32:28.000000 pglast-5.3/pglast/enums/parsenodes.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)      521 2023-08-05 06:32:28.000000 pglast-5.3/pglast/enums/pg_am.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)      592 2023-08-05 06:32:28.000000 pglast-5.3/pglast/enums/pg_attribute.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)      960 2023-08-05 06:32:28.000000 pglast-5.3/pglast/enums/pg_class.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)      748 2023-08-05 06:32:28.000000 pglast-5.3/pglast/enums/pg_trigger.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2696 2023-08-05 06:32:28.000000 pglast-5.3/pglast/enums/primnodes.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)      846 2023-08-05 06:32:29.000000 pglast-5.3/pglast/enums/xml.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)      333 2022-12-01 07:04:43.000000 pglast-5.3/pglast/error.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6786 2023-08-05 06:32:58.000000 pglast-5.3/pglast/keywords.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)  3021198 2023-08-05 06:32:33.000000 pglast-5.3/pglast/parser.c
+-rw-r--r--   0 lele      (1000) lele      (1000)    15555 2023-08-05 06:32:29.000000 pglast-5.3/pglast/parser.pyx
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.628143 pglast-5.3/pglast/printers/
+-rw-r--r--   0 lele      (1000) lele      (1000)     6280 2022-12-04 09:39:06.000000 pglast-5.3/pglast/printers/__init__.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)   112907 2023-04-27 06:18:51.000000 pglast-5.3/pglast/printers/ddl.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)    65995 2023-02-28 06:47:01.000000 pglast-5.3/pglast/printers/dml.py
+-rw-r--r--   0 lele      (1000) lele      (1000)     5173 2022-12-04 09:39:06.000000 pglast-5.3/pglast/printers/sfuncs.py
+-rw-r--r--   0 lele      (1000) lele      (1000)    27863 2022-12-04 11:55:32.000000 pglast-5.3/pglast/stream.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)    58201 2023-08-05 06:32:29.000000 pglast-5.3/pglast/structs.pxd
+-rw-r--r--   0 lele      (1000) lele      (1000)    17561 2022-12-04 09:52:17.000000 pglast-5.3/pglast/visitors.py
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.624143 pglast-5.3/pglast.egg-info/
+-rw-rw-r--   0 lele      (1000) lele      (1000)    27066 2023-08-05 06:55:40.000000 pglast-5.3/pglast.egg-info/PKG-INFO
+-rw-rw-r--   0 lele      (1000) lele      (1000)    41232 2023-08-05 06:55:40.000000 pglast-5.3/pglast.egg-info/SOURCES.txt
+-rw-rw-r--   0 lele      (1000) lele      (1000)        1 2023-08-05 06:55:40.000000 pglast-5.3/pglast.egg-info/dependency_links.txt
+-rw-rw-r--   0 lele      (1000) lele      (1000)       46 2023-08-05 06:55:40.000000 pglast-5.3/pglast.egg-info/entry_points.txt
+-rw-rw-r--   0 lele      (1000) lele      (1000)       82 2023-08-05 06:55:40.000000 pglast-5.3/pglast.egg-info/requires.txt
+-rw-rw-r--   0 lele      (1000) lele      (1000)        7 2023-08-05 06:55:40.000000 pglast-5.3/pglast.egg-info/top_level.txt
+-rw-r--r--   0 lele      (1000) lele      (1000)      357 2023-07-10 05:49:44.000000 pglast-5.3/requirements-test.txt
+-rw-r--r--   0 lele      (1000) lele      (1000)      455 2023-07-20 06:03:07.000000 pglast-5.3/requirements.txt
+-rw-rw-r--   0 lele      (1000) lele      (1000)      318 2023-08-05 06:55:40.640143 pglast-5.3/setup.cfg
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3061 2022-12-01 07:04:43.000000 pglast-5.3/setup.py
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.628143 pglast-5.3/tests/
+-rw-r--r--   0 lele      (1000) lele      (1000)     3871 2023-02-11 09:52:17.000000 pglast-5.3/tests/test_ast.py
+-rw-r--r--   0 lele      (1000) lele      (1000)     8014 2022-12-04 10:22:40.000000 pglast-5.3/tests/test_cli.py
+-rw-r--r--   0 lele      (1000) lele      (1000)     6110 2022-12-04 10:26:19.000000 pglast-5.3/tests/test_parser.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3531 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers.py
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.512145 pglast-5.3/tests/test_printers_prettification/
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.632143 pglast-5.3/tests/test_printers_prettification/ddl/
+-rw-rw-r--   0 lele      (1000) lele      (1000)      384 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/ddl/alter_default_privileges.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1060 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/ddl/alter_subscription.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      103 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/ddl/alter_text_search.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      548 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/ddl/comment.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      752 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/ddl/create_aggregate.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      480 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/ddl/create_database.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      449 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/ddl/create_domain.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      647 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/ddl/create_event_trigger.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      267 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/ddl/create_extension.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      993 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/ddl/create_foreign_data_wrapper.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1262 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/ddl/create_foreign_table.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2089 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/ddl/create_function.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      235 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/ddl/create_index.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      298 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/ddl/create_language.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      900 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/ddl/create_rule.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      300 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/ddl/create_schema.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      184 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/ddl/create_sequence.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2049 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/ddl/create_table.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      306 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/ddl/create_transform.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2483 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/ddl/create_trigger.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)       34 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/ddl/create_type.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      121 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/ddl/create_view.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      348 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/ddl/grant.sql
+-rw-r--r--   0 lele      (1000) lele      (1000)      800 2022-12-19 09:20:50.000000 pglast-5.3/tests/test_printers_prettification/ddl/issue110.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)       97 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/ddl/notify.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)       20 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/ddl/show.sql
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.632143 pglast-5.3/tests/test_printers_prettification/dml/
+-rw-r--r--   0 lele      (1000) lele      (1000)      523 2022-12-04 11:06:47.000000 pglast-5.3/tests/test_printers_prettification/dml/copy.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      907 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/dml/insert.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)    11464 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/dml/select.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      216 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/dml/truncate.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      638 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification/dml/update.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2717 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_prettification.py
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.512145 pglast-5.3/tests/test_printers_roundtrip/
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.640143 pglast-5.3/tests/test_printers_roundtrip/ddl/
+-rw-rw-r--   0 lele      (1000) lele      (1000)      123 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/alter_database.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      240 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/alter_default_privileges.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)       52 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/alter_domain.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      183 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/alter_extension.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)       42 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/alter_fdw.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      192 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/alter_function.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      136 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/alter_owner.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      124 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/alter_policy.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      415 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/alter_rename.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      194 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/alter_role.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)       74 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/alter_sequence.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)       30 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/alter_server.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)       99 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/alter_set_schema.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      210 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/alter_subscription.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2054 2022-12-04 10:36:47.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/alter_table.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      259 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/alter_text_search.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      233 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/alter_type.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)       48 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/analyze.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)       53 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/cluster.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2849 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/comment.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      138 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/create_access_method.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1226 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/create_aggregate.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      447 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/create_cast.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      352 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/create_collation.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      129 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/create_conversion.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      274 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/create_database.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      155 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/create_fdw.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      811 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/create_function.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      667 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/create_index.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      602 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/create_operator.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1095 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/create_operator_class.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      274 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/create_policy.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)       69 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/create_role.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      243 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/create_schema.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      387 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/create_sequence.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     7017 2023-04-27 06:15:47.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/create_table.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      874 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/create_trigger.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)       89 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/create_type.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      144 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/create_view.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)       60 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/discard.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)       41 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/do.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1902 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/drop.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      298 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/grant.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)       85 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/lock_table.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)       90 2022-12-04 16:30:03.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/reindex.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)       97 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/revoke.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)       52 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/security_label.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      169 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/ddl/vacuum.sql
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.640143 pglast-5.3/tests/test_printers_roundtrip/dml/
+-rw-r--r--   0 lele      (1000) lele      (1000)      418 2022-12-04 11:29:45.000000 pglast-5.3/tests/test_printers_roundtrip/dml/copy.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)       70 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/dml/cursor.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      552 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/dml/delete.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1537 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/dml/insert.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)       29 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/dml/reset.sql
+-rw-r--r--   0 lele      (1000) lele      (1000)    14276 2023-02-11 11:00:01.000000 pglast-5.3/tests/test_printers_roundtrip/dml/select.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      642 2023-02-28 06:31:27.000000 pglast-5.3/tests/test_printers_roundtrip/dml/set.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)      404 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/dml/transaction.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1078 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip/dml/update.sql
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5300 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_printers_roundtrip.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4014 2022-12-01 07:04:43.000000 pglast-5.3/tests/test_stream.py
+-rw-r--r--   0 lele      (1000) lele      (1000)    10262 2022-12-04 09:39:06.000000 pglast-5.3/tests/test_visitors.py
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2023-08-05 06:55:40.640143 pglast-5.3/tools/
+-rw-rw-r--   0 lele      (1000) lele      (1000)    32699 2023-02-28 06:40:06.000000 pglast-5.3/tools/extract_ast.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9613 2022-12-01 07:04:43.000000 pglast-5.3/tools/extract_enums.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2566 2022-12-01 07:04:43.000000 pglast-5.3/tools/extract_keywords.py
+-rw-r--r--   0 lele      (1000) lele      (1000)     5846 2022-12-19 18:19:58.000000 pglast-5.3/tools/extract_printers_doc.py
+-rw-r--r--   0 lele      (1000) lele      (1000)        3 2023-08-05 06:54:33.000000 pglast-5.3/version.txt
```

### Comparing `pglast-5.2/CHANGES.rst` & `pglast-5.3/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,22 @@
 
 Changes
 -------
 
 Version 5
 #########
 
+5.3 (2023-08-05)
+~~~~~~~~~~~~~~~~
+
+- Update libpg_query to `15-4.2.3`__
+
+  __ https://github.com/pganalyze/libpg_query/releases/tag/15-4.2.3
+
+
 5.2 (2023-05-20)
 ~~~~~~~~~~~~~~~~
 
 - Update libpg_query to `15-4.2.1`__
 
   __ https://github.com/pganalyze/libpg_query/releases/tag/15-4.2.1
```

### Comparing `pglast-5.2/MANIFEST.in` & `pglast-5.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pglast-5.2/Makefile` & `pglast-5.3/Makefile`

 * *Files identical despite different names*

### Comparing `pglast-5.2/Makefile.release` & `pglast-5.3/Makefile.release`

 * *Files identical despite different names*

### Comparing `pglast-5.2/Makefile.virtualenv` & `pglast-5.3/Makefile.virtualenv`

 * *Files identical despite different names*

### Comparing `pglast-5.2/PKG-INFO` & `pglast-5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pglast
-Version: 5.2
+Version: 5.3
 Summary: PostgreSQL Languages AST and statements prettifier
 Home-page: https://github.com/lelit/pglast
 Author: Lele Gaifax
 Author-email: lele@metapensiero.it
 License: GPLv3+
 Keywords: postgresql parser sql prettifier
 Classifier: Development Status :: 5 - Production/Stable
@@ -111,14 +111,22 @@
 
 Changes
 -------
 
 Version 5
 #########
 
+5.3 (2023-08-05)
+~~~~~~~~~~~~~~~~
+
+- Update libpg_query to `15-4.2.3`__
+
+  __ https://github.com/pganalyze/libpg_query/releases/tag/15-4.2.3
+
+
 5.2 (2023-05-20)
 ~~~~~~~~~~~~~~~~
 
 - Update libpg_query to `15-4.2.1`__
 
   __ https://github.com/pganalyze/libpg_query/releases/tag/15-4.2.1
```

### Comparing `pglast-5.2/README.rst` & `pglast-5.3/README.rst`

 * *Files identical despite different names*

### Comparing `pglast-5.2/docs/Makefile` & `pglast-5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pglast-5.2/docs/api.rst` & `pglast-5.3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pglast-5.2/docs/ast.rst` & `pglast-5.3/docs/ast.rst`

 * *Files 4% similar despite different names*

```diff
@@ -10,56 +10,56 @@
 ===================================================================
  :mod:`pglast.ast` --- Python classes representing PG parser nodes
 ===================================================================
 
 The module implements a set of *data* classes, one for each ``C`` structure defined in several
 PostgreSQL headers, primarily those in the `include/nodes/`__ directory.
 
-__ https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes
+__ https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes
 
 The :class:`pglast.ast.Node` is an abstract class that implements the common behaviour of all
 the concrete classes. In particular any node can be :meth:`compared <pglast.ast.Node.__eq__>`
 with another instance, is able to :meth:`serialize <pglast.ast.Node.__call__>` itself and can
 be :meth:`altered <pglast.ast.Node.__setattr__>`.
 
 .. module:: pglast.ast
 
 .. autoclass:: Node
    :special-members: __repr__, __eq__, __call__, __setattr__
 
 
 .. class:: A_ArrayExpr(elements=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L444>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L444>`__ parser node.
 
    .. attribute:: elements
       :type: tuple
 
       Array element expressions
 
    .. attribute:: location
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: A_Const(isnull=None, val=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L301>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L301>`__ parser node.
 
    .. attribute:: isnull
       :type: bool
 
    .. attribute:: val
       :type: ValUnion
 
 
 .. class:: A_Expr(kind=None, name=None, lexpr=None, rexpr=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L288>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L288>`__ parser node.
 
    .. attribute:: kind
       :type: A_Expr_Kind
 
    .. attribute:: name
       :type: tuple
 
@@ -79,15 +79,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: A_Indices(is_slice=None, lidx=None, uidx=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L411>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L411>`__ parser node.
 
    .. attribute:: is_slice
       :type: bool
 
       True if slice (i.e., colon present)
 
    .. attribute:: lidx
@@ -99,50 +99,50 @@
       :type: Node
 
       Subscript, or slice upper bound if any
 
 
 .. class:: A_Indirection(arg=None, indirection=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L434>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L434>`__ parser node.
 
    .. attribute:: arg
       :type: Node
 
       The thing being selected from
 
    .. attribute:: indirection
       :type: tuple
 
       Subscripts and/or field names and/or *
 
 
 .. class:: A_Star()
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L400>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L400>`__ parser node.
 
 
 .. class:: AccessPriv(priv_name=None, cols=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2134>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2134>`__ parser node.
 
    .. attribute:: priv_name
       :type: str
 
       String name of privilege
 
    .. attribute:: cols
       :type: tuple
 
       List of String
 
 
 .. class:: Aggref(aggargtypes=None, aggdirectargs=None, args=None, aggorder=None, aggdistinct=None, aggfilter=None, aggstar=None, aggvariadic=None, aggkind=None, agglevelsup=None, aggsplit=None, aggno=None, aggtransno=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L320>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L320>`__ parser node.
 
    .. attribute:: aggargtypes
       :type: tuple
 
       Type Oids of direct and aggregated args
 
    .. attribute:: aggdirectargs
@@ -210,91 +210,91 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: Alias(aliasname=None, colnames=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L39>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L39>`__ parser node.
 
    .. attribute:: aliasname
       :type: str
 
       Aliased rel name (never qualified)
 
    .. attribute:: colnames
       :type: tuple
 
       Optional list of column aliases
 
 
 .. class:: AlterCollationStmt(collname=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2041>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2041>`__ parser node.
 
    .. attribute:: collname
       :type: tuple
 
 
 .. class:: AlterDatabaseRefreshCollStmt(dbname=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3371>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3371>`__ parser node.
 
    .. attribute:: dbname
       :type: str
 
 
 .. class:: AlterDatabaseSetStmt(dbname=None, setstmt=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3377>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3377>`__ parser node.
 
    .. attribute:: dbname
       :type: str
 
       Database name
 
    .. attribute:: setstmt
       :type: VariableSetStmt*
 
       SET or RESET subcommand
 
 
 .. class:: AlterDatabaseStmt(dbname=None, options=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3364>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3364>`__ parser node.
 
    .. attribute:: dbname
       :type: str
 
       Name of database to alter
 
    .. attribute:: options
       :type: tuple
 
       List of DefElem nodes
 
 
 .. class:: AlterDefaultPrivilegesStmt(options=None, action=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2165>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2165>`__ parser node.
 
    .. attribute:: options
       :type: tuple
 
       List of DefElem
 
    .. attribute:: action
       :type: GrantStmt*
 
       GRANT/REVOKE action (with objects=NIL)
 
 
 .. class:: AlterDomainStmt(subtype=None, typeName=None, name=None, def_=None, behavior=None, missing_ok=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2055>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2055>`__ parser node.
 
    .. attribute:: subtype
       :type: str
 
       * T = alter column default
       * N = alter column drop not null
       * O = alter column set not null
@@ -325,15 +325,15 @@
       :type: bool
 
       Skip error if missing?
 
 
 .. class:: AlterEnumStmt(typeName=None, oldVal=None, newVal=None, newValNeighbor=None, newValIsAfter=None, skipIfNewValExists=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3306>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3306>`__ parser node.
 
    .. attribute:: typeName
       :type: tuple
 
       Qualified name (list of String)
 
    .. attribute:: oldVal
@@ -360,15 +360,15 @@
       :type: bool
 
       No error if new already exists?
 
 
 .. class:: AlterEventTrigStmt(trigname=None, tgenabled=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2643>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2643>`__ parser node.
 
    .. attribute:: trigname
       :type: str
 
       TRIGGER's name
 
    .. attribute:: tgenabled
@@ -376,15 +376,15 @@
 
       Trigger's firing configuration WRT
       session_replication_role
 
 
 .. class:: AlterExtensionContentsStmt(extname=None, action=None, objtype=None, object=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2436>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2436>`__ parser node.
 
    .. attribute:: extname
       :type: str
 
       Extension's name
 
    .. attribute:: action
@@ -401,28 +401,28 @@
       :type: Node
 
       Qualified name of the object
 
 
 .. class:: AlterExtensionStmt(extname=None, options=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2429>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2429>`__ parser node.
 
    .. attribute:: extname
       :type: str
 
    .. attribute:: options
       :type: tuple
 
       List of DefElem nodes
 
 
 .. class:: AlterFdwStmt(fdwname=None, func_options=None, options=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2458>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2458>`__ parser node.
 
    .. attribute:: fdwname
       :type: str
 
       Foreign-data wrapper name
 
    .. attribute:: func_options
@@ -434,15 +434,15 @@
       :type: tuple
 
       Generic options to FDW
 
 
 .. class:: AlterForeignServerStmt(servername=None, version=None, options=None, has_version=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2482>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2482>`__ parser node.
 
    .. attribute:: servername
       :type: str
 
       Server name
 
    .. attribute:: version
@@ -459,15 +459,15 @@
       :type: bool
 
       Version specified
 
 
 .. class:: AlterFunctionStmt(objtype=None, func=None, actions=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3061>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3061>`__ parser node.
 
    .. attribute:: objtype
       :type: ObjectType
 
    .. attribute:: func
       :type: ObjectWithArgs*
 
@@ -477,15 +477,15 @@
       :type: tuple
 
       List of DefElem
 
 
 .. class:: AlterObjectDependsStmt(objectType=None, relation=None, object=None, extname=None, remove=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3135>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3135>`__ parser node.
 
    .. attribute:: objectType
       :type: ObjectType
 
       OBJECT_FUNCTION, OBJECT_TRIGGER, etc
 
    .. attribute:: relation
@@ -507,15 +507,15 @@
       :type: bool
 
       Set true to remove dep rather than add
 
 
 .. class:: AlterObjectSchemaStmt(objectType=None, relation=None, object=None, newschema=None, missing_ok=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3149>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3149>`__ parser node.
 
    .. attribute:: objectType
       :type: ObjectType
 
       OBJECT_TABLE, OBJECT_TYPE, etc
 
    .. attribute:: relation
@@ -537,15 +537,15 @@
       :type: bool
 
       Skip error if missing?
 
 
 .. class:: AlterOpFamilyStmt(opfamilyname=None, amname=None, isDrop=None, items=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2813>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2813>`__ parser node.
 
    .. attribute:: opfamilyname
       :type: tuple
 
       Qualified name (list of String)
 
    .. attribute:: amname
@@ -562,30 +562,30 @@
       :type: tuple
 
       List of CreateOpClassItem nodes
 
 
 .. class:: AlterOperatorStmt(opername=None, options=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3176>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3176>`__ parser node.
 
    .. attribute:: opername
       :type: ObjectWithArgs*
 
       Operator name and argument types
 
    .. attribute:: options
       :type: tuple
 
       List of DefElem nodes
 
 
 .. class:: AlterOwnerStmt(objectType=None, relation=None, object=None, newowner=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3163>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3163>`__ parser node.
 
    .. attribute:: objectType
       :type: ObjectType
 
       OBJECT_TABLE, OBJECT_TYPE, etc
 
    .. attribute:: relation
@@ -602,15 +602,15 @@
       :type: RoleSpec*
 
       The new owner
 
 
 .. class:: AlterPolicyStmt(policy_name=None, table=None, roles=None, qual=None, with_check=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2576>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2576>`__ parser node.
 
    .. attribute:: policy_name
       :type: str
 
       Policy's name
 
    .. attribute:: table
@@ -632,15 +632,15 @@
       :type: Node
 
       The policy's WITH CHECK condition.
 
 
 .. class:: AlterPublicationStmt(pubname=None, options=None, pubobjects=None, for_all_tables=None, action=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3755>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3755>`__ parser node.
 
    .. attribute:: pubname
       :type: str
 
       Name of the publication
 
    .. attribute:: options
@@ -663,15 +663,15 @@
 
       What action to perform with the given
       objects
 
 
 .. class:: AlterRoleSetStmt(role=None, database=None, setstmt=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2698>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2698>`__ parser node.
 
    .. attribute:: role
       :type: RoleSpec*
 
       Role
 
    .. attribute:: database
@@ -683,15 +683,15 @@
       :type: VariableSetStmt*
 
       SET or RESET subcommand
 
 
 .. class:: AlterRoleStmt(role=None, options=None, action=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2690>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2690>`__ parser node.
 
    .. attribute:: role
       :type: RoleSpec*
 
       Role
 
    .. attribute:: options
@@ -703,15 +703,15 @@
       :type: int
 
       +1 = add members, -1 = drop members
 
 
 .. class:: AlterSeqStmt(sequence=None, options=None, for_identity=None, missing_ok=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2728>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2728>`__ parser node.
 
    .. attribute:: sequence
       :type: RangeVar*
 
       The sequence to alter
 
    .. attribute:: options
@@ -724,15 +724,15 @@
       :type: bool
 
       Skip error if a role is missing?
 
 
 .. class:: AlterStatsStmt(defnames=None, stxstattarget=None, missing_ok=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3016>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3016>`__ parser node.
 
    .. attribute:: defnames
       :type: tuple
 
       Qualified name (list of String)
 
    .. attribute:: stxstattarget
@@ -744,15 +744,15 @@
       :type: bool
 
       Skip error if statistics object is missing
 
 
 .. class:: AlterSubscriptionStmt(kind=None, subname=None, conninfo=None, publication=None, options=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3794>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3794>`__ parser node.
 
    .. attribute:: kind
       :type: AlterSubscriptionType
 
       ALTER_SUBSCRIPTION_OPTIONS, etc
 
    .. attribute:: subname
@@ -774,25 +774,25 @@
       :type: tuple
 
       List of DefElem nodes
 
 
 .. class:: AlterSystemStmt(setstmt=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3400>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3400>`__ parser node.
 
    .. attribute:: setstmt
       :type: VariableSetStmt*
 
       SET subcommand
 
 
 .. class:: AlterTSConfigurationStmt(kind=None, cfgname=None, tokentype=None, dicts=None, override=None, replace=None, missing_ok=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3693>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3693>`__ parser node.
 
    .. attribute:: kind
       :type: AlterTSConfigType
 
       ALTER_TSCONFIG_ADD_MAPPING, etc
 
    .. attribute:: cfgname
@@ -824,30 +824,30 @@
       :type: bool
 
       For DROP - skip error if missing?
 
 
 .. class:: AlterTSDictionaryStmt(dictname=None, options=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3674>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3674>`__ parser node.
 
    .. attribute:: dictname
       :type: tuple
 
       Qualified name (list of String)
 
    .. attribute:: options
       :type: tuple
 
       List of DefElem nodes
 
 
 .. class:: AlterTableCmd(subtype=None, name=None, num=None, newowner=None, def_=None, behavior=None, missing_ok=None, recurse=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2020>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2020>`__ parser node.
 
    .. attribute:: subtype
       :type: AlterTableType
 
       Type of table alteration to apply
 
    .. attribute:: name
@@ -885,15 +885,15 @@
       :type: bool
 
       Exec-time recursion
 
 
 .. class:: AlterTableMoveAllStmt(orig_tablespacename=None, objtype=None, roles=None, new_tablespacename=None, nowait=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2405>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2405>`__ parser node.
 
    .. attribute:: orig_tablespacename
       :type: str
 
    .. attribute:: objtype
       :type: ObjectType
 
@@ -909,29 +909,29 @@
 
    .. attribute:: nowait
       :type: bool
 
 
 .. class:: AlterTableSpaceOptionsStmt(tablespacename=None, options=None, isReset=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2397>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2397>`__ parser node.
 
    .. attribute:: tablespacename
       :type: str
 
    .. attribute:: options
       :type: tuple
 
    .. attribute:: isReset
       :type: bool
 
 
 .. class:: AlterTableStmt(relation=None, cmds=None, objtype=None, missing_ok=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1929>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1929>`__ parser node.
 
    .. attribute:: relation
       :type: RangeVar*
 
       Table to work on
 
    .. attribute:: cmds
@@ -948,30 +948,30 @@
       :type: bool
 
       Skip error if table missing
 
 
 .. class:: AlterTypeStmt(typeName=None, options=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3187>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3187>`__ parser node.
 
    .. attribute:: typeName
       :type: tuple
 
       Type name (possibly qualified)
 
    .. attribute:: options
       :type: tuple
 
       List of DefElem nodes
 
 
 .. class:: AlterUserMappingStmt(user=None, servername=None, options=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2517>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2517>`__ parser node.
 
    .. attribute:: user
       :type: RoleSpec*
 
       User role
 
    .. attribute:: servername
@@ -983,25 +983,25 @@
       :type: tuple
 
       Generic options to server
 
 
 .. class:: AlternativeSubPlan(subplans=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L790>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L790>`__ parser node.
 
    .. attribute:: subplans
       :type: tuple
 
       SubPlan(s) with equivalent results
 
 
 .. class:: ArrayCoerceExpr(arg=None, elemexpr=None, resulttypmod=None, coerceformat=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L901>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L901>`__ parser node.
 
    .. attribute:: arg
       :type: Expr*
 
       Input expression (yields an array)
 
    .. attribute:: elemexpr
@@ -1023,15 +1023,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: ArrayExpr(elements=None, multidims=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1031>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1031>`__ parser node.
 
    .. attribute:: elements
       :type: tuple
 
       The array elements or sub-arrays
 
    .. attribute:: multidims
@@ -1043,23 +1043,23 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: BitString(bsval=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/value.h#L63>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/value.h#L63>`__ parser node.
 
    .. attribute:: bsval
       :type: str
 
 
 .. class:: BoolExpr(boolop=None, args=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L622>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L622>`__ parser node.
 
    .. attribute:: boolop
       :type: BoolExprType
 
    .. attribute:: args
       :type: tuple
 
@@ -1069,23 +1069,23 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: Boolean(boolval=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/value.h#L51>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/value.h#L51>`__ parser node.
 
    .. attribute:: boolval
       :type: bool
 
 
 .. class:: BooleanTest(arg=None, booltesttype=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1283>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1283>`__ parser node.
 
    .. attribute:: arg
       :type: Expr*
 
       Input expression
 
    .. attribute:: booltesttype
@@ -1097,15 +1097,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: CTECycleClause(cycle_col_list=None, cycle_mark_column=None, cycle_mark_value=None, cycle_mark_default=None, cycle_path_column=None, location=None, cycle_mark_typmod=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1505>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1505>`__ parser node.
 
    .. attribute:: cycle_col_list
       :type: tuple
 
    .. attribute:: cycle_mark_column
       :type: str
 
@@ -1123,15 +1123,15 @@
 
    .. attribute:: cycle_mark_typmod
       :type: int
 
 
 .. class:: CTESearchClause(search_col_list=None, search_breadth_first=None, search_seq_column=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1496>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1496>`__ parser node.
 
    .. attribute:: search_col_list
       :type: tuple
 
    .. attribute:: search_breadth_first
       :type: bool
 
@@ -1140,23 +1140,23 @@
 
    .. attribute:: location
       :type: int
 
 
 .. class:: CallContext(atomic=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3107>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3107>`__ parser node.
 
    .. attribute:: atomic
       :type: bool
 
 
 .. class:: CallStmt(funccall=None, funcexpr=None, outargs=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3099>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3099>`__ parser node.
 
    .. attribute:: funccall
       :type: FuncCall*
 
       From the parser
 
    .. attribute:: funcexpr
@@ -1168,15 +1168,15 @@
       :type: tuple
 
       Transformed output-argument expressions
 
 
 .. class:: CaseExpr(arg=None, args=None, defresult=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L973>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L973>`__ parser node.
 
    .. attribute:: arg
       :type: Expr*
 
       Implicit equality comparison argument
 
    .. attribute:: args
@@ -1193,25 +1193,25 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: CaseTestExpr(typeMod=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1015>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1015>`__ parser node.
 
    .. attribute:: typeMod
       :type: int32
 
       Typemod for substituted value
 
 
 .. class:: CaseWhen(expr=None, result=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L987>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L987>`__ parser node.
 
    .. attribute:: expr
       :type: Expr*
 
       Condition expression
 
    .. attribute:: result
@@ -1223,30 +1223,30 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: CheckPointStmt()
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3502>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3502>`__ parser node.
 
 
 .. class:: ClosePortalStmt(portalname=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2906>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2906>`__ parser node.
 
    .. attribute:: portalname
       :type: str
 
       Name of the portal (cursor)
 
 
 .. class:: ClusterStmt(relation=None, indexname=None, params=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3410>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3410>`__ parser node.
 
    .. attribute:: relation
       :type: RangeVar*
 
       Relation being indexed, or NULL if all
 
    .. attribute:: indexname
@@ -1258,30 +1258,30 @@
       :type: tuple
 
       List of DefElem nodes
 
 
 .. class:: CoalesceExpr(args=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1125>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1125>`__ parser node.
 
    .. attribute:: args
       :type: tuple
 
       The arguments
 
    .. attribute:: location
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: CoerceToDomain(arg=None, resulttypmod=None, coercionformat=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1300>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1300>`__ parser node.
 
    .. attribute:: arg
       :type: Expr*
 
       Input expression
 
    .. attribute:: resulttypmod
@@ -1298,30 +1298,30 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: CoerceToDomainValue(typeMod=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1320>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1320>`__ parser node.
 
    .. attribute:: typeMod
       :type: int32
 
       Typemod for substituted value
 
    .. attribute:: location
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: CoerceViaIO(arg=None, coerceformat=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L877>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L877>`__ parser node.
 
    .. attribute:: arg
       :type: Expr*
 
       Input expression
 
    .. attribute:: coerceformat
@@ -1333,15 +1333,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: CollateClause(arg=None, collname=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L336>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L336>`__ parser node.
 
    .. attribute:: arg
       :type: Node
 
       Input expression
 
    .. attribute:: collname
@@ -1353,30 +1353,30 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: CollateExpr(arg=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L943>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L943>`__ parser node.
 
    .. attribute:: arg
       :type: Expr*
 
       Input expression
 
    .. attribute:: location
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: ColumnDef(colname=None, typeName=None, compression=None, inhcount=None, is_local=None, is_not_null=None, is_from_type=None, storage=None, raw_default=None, cooked_default=None, identity=None, identitySequence=None, generated=None, collClause=None, constraints=None, fdwoptions=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L675>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L675>`__ parser node.
 
    .. attribute:: colname
       :type: str
 
       Name of column
 
    .. attribute:: typeName
@@ -1459,30 +1459,30 @@
       :type: int
 
       Parse location, or -1 if none/unknown
 
 
 .. class:: ColumnRef(fields=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L250>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L250>`__ parser node.
 
    .. attribute:: fields
       :type: tuple
 
       Field names (String nodes) or A_Star
 
    .. attribute:: location
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: CommentStmt(objtype=None, object=None, comment=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2853>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2853>`__ parser node.
 
    .. attribute:: objtype
       :type: ObjectType
 
       Object's type
 
    .. attribute:: object
@@ -1494,15 +1494,15 @@
       :type: str
 
       Comment to insert, or NULL to remove
 
 
 .. class:: CommonTableExpr(ctename=None, aliascolnames=None, ctematerialized=None, ctequery=None, search_clause=None, cycle_clause=None, location=None, cterecursive=None, cterefcount=None, ctecolnames=None, ctecoltypes=None, ctecoltypmods=None, ctecolcollations=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1521>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1521>`__ parser node.
 
    .. attribute:: ctename
       :type: str
 
       Query name (never qualified)
 
    .. attribute:: aliascolnames
@@ -1561,30 +1561,30 @@
       :type: tuple
 
       OID list of column collation OIDs
 
 
 .. class:: CompositeTypeStmt(typevar=None, coldeflist=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3273>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3273>`__ parser node.
 
    .. attribute:: typevar
       :type: RangeVar*
 
       The composite type to be created
 
    .. attribute:: coldeflist
       :type: tuple
 
       List of ColumnDef nodes
 
 
 .. class:: Constraint(contype=None, conname=None, deferrable=None, initdeferred=None, location=None, is_no_inherit=None, raw_expr=None, cooked_expr=None, generated_when=None, nulls_not_distinct=None, keys=None, including=None, exclusions=None, options=None, indexname=None, indexspace=None, reset_default_tblspc=None, access_method=None, where_clause=None, pktable=None, fk_attrs=None, pk_attrs=None, fk_matchtype=None, fk_upd_action=None, fk_del_action=None, fk_del_set_cols=None, old_conpfeqop=None, skip_validation=None, initially_valid=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2322>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2322>`__ parser node.
 
    .. attribute:: contype
       :type: ConstrType
 
    .. attribute:: conname
       :type: str
 
@@ -1727,28 +1727,28 @@
       :type: bool
 
       Mark the new constraint as valid?
 
 
 .. class:: ConstraintsSetStmt(constraints=None, deferred=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3542>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3542>`__ parser node.
 
    .. attribute:: constraints
       :type: tuple
 
       List of names as RangeVars
 
    .. attribute:: deferred
       :type: bool
 
 
 .. class:: ConvertRowtypeExpr(arg=None, convertformat=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L926>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L926>`__ parser node.
 
    .. attribute:: arg
       :type: Expr*
 
       Input expression
 
    .. attribute:: convertformat
@@ -1760,15 +1760,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: CopyStmt(relation=None, query=None, attlist=None, is_from=None, is_program=None, filename=None, options=None, whereClause=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2180>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2180>`__ parser node.
 
    .. attribute:: relation
       :type: RangeVar*
 
       The relation to copy
 
    .. attribute:: query
@@ -1807,15 +1807,15 @@
       :type: Node
 
       WHERE condition (or NULL)
 
 
 .. class:: CreateAmStmt(amname=None, handler_name=None, amtype=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2590>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2590>`__ parser node.
 
    .. attribute:: amname
       :type: str
 
       Access method name
 
    .. attribute:: handler_name
@@ -1827,15 +1827,15 @@
       :type: str
 
       Type of access method
 
 
 .. class:: CreateCastStmt(sourcetype=None, targettype=None, func=None, context=None, inout=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3590>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3590>`__ parser node.
 
    .. attribute:: sourcetype
       :type: TypeName*
 
    .. attribute:: targettype
       :type: TypeName*
 
@@ -1847,15 +1847,15 @@
 
    .. attribute:: inout
       :type: bool
 
 
 .. class:: CreateConversionStmt(conversion_name=None, for_encoding_name=None, to_encoding_name=None, func_name=None, def_=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3576>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3576>`__ parser node.
 
    .. attribute:: conversion_name
       :type: tuple
 
       Name of the conversion
 
    .. attribute:: for_encoding_name
@@ -1877,15 +1877,15 @@
       :type: bool
 
       Is this a default conversion?
 
 
 .. class:: CreateDomainStmt(domainname=None, typeName=None, collClause=None, constraints=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2757>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2757>`__ parser node.
 
    .. attribute:: domainname
       :type: tuple
 
       Qualified name (list of String)
 
    .. attribute:: typeName
@@ -1902,30 +1902,30 @@
       :type: tuple
 
       Constraints (list of Constraint nodes)
 
 
 .. class:: CreateEnumStmt(typeName=None, vals=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3284>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3284>`__ parser node.
 
    .. attribute:: typeName
       :type: tuple
 
       Qualified name (list of String)
 
    .. attribute:: vals
       :type: tuple
 
       Enum values (list of String)
 
 
 .. class:: CreateEventTrigStmt(trigname=None, eventname=None, whenclause=None, funcname=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2630>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2630>`__ parser node.
 
    .. attribute:: trigname
       :type: str
 
       TRIGGER's name
 
    .. attribute:: eventname
@@ -1942,15 +1942,15 @@
       :type: tuple
 
       Qual. name of function to call
 
 
 .. class:: CreateExtensionStmt(extname=None, if_not_exists=None, options=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2420>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2420>`__ parser node.
 
    .. attribute:: extname
       :type: str
 
    .. attribute:: if_not_exists
       :type: bool
 
@@ -1960,15 +1960,15 @@
       :type: tuple
 
       List of DefElem nodes
 
 
 .. class:: CreateFdwStmt(fdwname=None, func_options=None, options=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2450>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2450>`__ parser node.
 
    .. attribute:: fdwname
       :type: str
 
       Foreign-data wrapper name
 
    .. attribute:: func_options
@@ -1980,15 +1980,15 @@
       :type: tuple
 
       Generic options to FDW
 
 
 .. class:: CreateForeignServerStmt(servername=None, servertype=None, version=None, fdwname=None, if_not_exists=None, options=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2471>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2471>`__ parser node.
 
    .. attribute:: servername
       :type: str
 
       Server name
 
    .. attribute:: servertype
@@ -2015,29 +2015,29 @@
       :type: tuple
 
       Generic options to server
 
 
 .. class:: CreateForeignTableStmt(base=None, servername=None, options=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2496>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2496>`__ parser node.
 
    .. attribute:: base
       :type: CreateStmt
 
    .. attribute:: servername
       :type: str
 
    .. attribute:: options
       :type: tuple
 
 
 .. class:: CreateFunctionStmt(is_procedure=None, replace=None, funcname=None, parameters=None, returnType=None, options=None, sql_body=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3028>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3028>`__ parser node.
 
    .. attribute:: is_procedure
       :type: bool
 
       It's really CREATE PROCEDURE
 
    .. attribute:: replace
@@ -2067,15 +2067,15 @@
 
    .. attribute:: sql_body
       :type: Node
 
 
 .. class:: CreateOpClassItem(itemtype=None, name=None, number=None, order_family=None, class_args=None, storedtype=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2785>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2785>`__ parser node.
 
    .. attribute:: itemtype
       :type: int
 
       See codes above
 
    .. attribute:: name
@@ -2103,15 +2103,15 @@
       :type: TypeName*
 
       Datatype stored in index
 
 
 .. class:: CreateOpClassStmt(opclassname=None, opfamilyname=None, amname=None, datatype=None, items=None, isDefault=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2770>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2770>`__ parser node.
 
    .. attribute:: opclassname
       :type: tuple
 
       Qualified name (list of String)
 
    .. attribute:: opfamilyname
@@ -2138,30 +2138,30 @@
       :type: bool
 
       Should be marked as default for type?
 
 
 .. class:: CreateOpFamilyStmt(opfamilyname=None, amname=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2802>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2802>`__ parser node.
 
    .. attribute:: opfamilyname
       :type: tuple
 
       Qualified name (list of String)
 
    .. attribute:: amname
       :type: str
 
       Name of index AM opfamily is for
 
 
 .. class:: CreatePLangStmt(replace=None, plname=None, plhandler=None, plinline=None, plvalidator=None, pltrusted=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2655>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2655>`__ parser node.
 
    .. attribute:: replace
       :type: bool
 
       T => replace if already exists
 
    .. attribute:: plname
@@ -2188,15 +2188,15 @@
       :type: bool
 
       PL is trusted
 
 
 .. class:: CreatePolicyStmt(policy_name=None, table=None, cmd_name=None, permissive=None, roles=None, qual=None, with_check=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2560>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2560>`__ parser node.
 
    .. attribute:: policy_name
       :type: str
 
       Policy's name
 
    .. attribute:: table
@@ -2228,15 +2228,15 @@
       :type: Node
 
       The policy's WITH CHECK condition.
 
 
 .. class:: CreatePublicationStmt(pubname=None, options=None, pubobjects=None, for_all_tables=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3739>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3739>`__ parser node.
 
    .. attribute:: pubname
       :type: str
 
       Name of the publication
 
    .. attribute:: options
@@ -2253,30 +2253,30 @@
       :type: bool
 
       Special publication for all tables in db
 
 
 .. class:: CreateRangeStmt(typeName=None, params=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3295>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3295>`__ parser node.
 
    .. attribute:: typeName
       :type: tuple
 
       Qualified name (list of String)
 
    .. attribute:: params
       :type: tuple
 
       Range parameters (list of DefElem)
 
 
 .. class:: CreateRoleStmt(stmt_type=None, role=None, options=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2682>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2682>`__ parser node.
 
    .. attribute:: stmt_type
       :type: RoleStmtType
 
       ROLE/USER/GROUP
 
    .. attribute:: role
@@ -2288,15 +2288,15 @@
       :type: tuple
 
       List of DefElem nodes
 
 
 .. class:: CreateSchemaStmt(schemaname=None, authrole=None, schemaElts=None, if_not_exists=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1910>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1910>`__ parser node.
 
    .. attribute:: schemaname
       :type: str
 
       The name of the schema to create
 
    .. attribute:: authrole
@@ -2313,15 +2313,15 @@
       :type: bool
 
       Just do nothing if schema already exists?
 
 
 .. class:: CreateSeqStmt(sequence=None, options=None, for_identity=None, if_not_exists=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2718>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2718>`__ parser node.
 
    .. attribute:: sequence
       :type: RangeVar*
 
       The sequence to create
 
    .. attribute:: options
@@ -2334,15 +2334,15 @@
       :type: bool
 
       Just do nothing if it already exists?
 
 
 .. class:: CreateStatsStmt(defnames=None, stat_types=None, exprs=None, relations=None, stxcomment=None, transformed=None, if_not_exists=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2985>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2985>`__ parser node.
 
    .. attribute:: defnames
       :type: tuple
 
       Qualified name (list of String)
 
    .. attribute:: stat_types
@@ -2374,15 +2374,15 @@
       :type: bool
 
       Do nothing if stats name already exists
 
 
 .. class:: CreateStmt(relation=None, tableElts=None, inhRelations=None, partbound=None, partspec=None, ofTypename=None, constraints=None, options=None, oncommit=None, tablespacename=None, accessMethod=None, if_not_exists=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2242>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2242>`__ parser node.
 
    .. attribute:: relation
       :type: RangeVar*
 
       Relation to create
 
    .. attribute:: tableElts
@@ -2440,15 +2440,15 @@
       :type: bool
 
       Just do nothing if it already exists?
 
 
 .. class:: CreateSubscriptionStmt(subname=None, conninfo=None, publication=None, options=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3773>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3773>`__ parser node.
 
    .. attribute:: subname
       :type: str
 
       Name of the subscription
 
    .. attribute:: conninfo
@@ -2465,15 +2465,15 @@
       :type: tuple
 
       List of DefElem nodes
 
 
 .. class:: CreateTableAsStmt(query=None, into=None, objtype=None, is_select_into=None, if_not_exists=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3476>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3476>`__ parser node.
 
    .. attribute:: query
       :type: Node
 
       The query (see comments above)
 
    .. attribute:: into
@@ -2495,15 +2495,15 @@
       :type: bool
 
       Just do nothing if it already exists?
 
 
 .. class:: CreateTableSpaceStmt(tablespacename=None, owner=None, location=None, options=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2381>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2381>`__ parser node.
 
    .. attribute:: tablespacename
       :type: str
 
    .. attribute:: owner
       :type: RoleSpec*
 
@@ -2512,15 +2512,15 @@
 
    .. attribute:: options
       :type: tuple
 
 
 .. class:: CreateTransformStmt(replace=None, type_name=None, lang=None, fromsql=None, tosql=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3604>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3604>`__ parser node.
 
    .. attribute:: replace
       :type: bool
 
    .. attribute:: type_name
       :type: TypeName*
 
@@ -2532,15 +2532,15 @@
 
    .. attribute:: tosql
       :type: ObjectWithArgs*
 
 
 .. class:: CreateTrigStmt(replace=None, isconstraint=None, trigname=None, relation=None, funcname=None, args=None, row=None, timing=None, events=None, columns=None, whenClause=None, transitionRels=None, deferrable=None, initdeferred=None, constrrel=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2602>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2602>`__ parser node.
 
    .. attribute:: replace
       :type: bool
 
       Replace trigger if already exists
 
    .. attribute:: isconstraint
@@ -2612,15 +2612,15 @@
       :type: RangeVar*
 
       Opposite relation, if RI trigger
 
 
 .. class:: CreateUserMappingStmt(user=None, servername=None, if_not_exists=None, options=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2508>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2508>`__ parser node.
 
    .. attribute:: user
       :type: RoleSpec*
 
       User role
 
    .. attribute:: servername
@@ -2637,30 +2637,30 @@
       :type: tuple
 
       Generic options to server
 
 
 .. class:: CreatedbStmt(dbname=None, options=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3353>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3353>`__ parser node.
 
    .. attribute:: dbname
       :type: str
 
       Name of database to create
 
    .. attribute:: options
       :type: tuple
 
       List of DefElem nodes
 
 
 .. class:: CurrentOfExpr(cvarno=None, cursor_name=None, cursor_param=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1358>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1358>`__ parser node.
 
    .. attribute:: cvarno
       :type: Index
 
       RT index of target relation
 
    .. attribute:: cursor_name
@@ -2672,25 +2672,25 @@
       :type: int
 
       Refcursor parameter number, or 0
 
 
 .. class:: DeallocateStmt(name=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3644>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3644>`__ parser node.
 
    .. attribute:: name
       :type: str
 
       The name of the plan to remove
 
 
 .. class:: DeclareCursorStmt(portalname=None, options=None, query=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2894>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2894>`__ parser node.
 
    .. attribute:: portalname
       :type: str
 
       Name of the portal (cursor)
 
    .. attribute:: options
@@ -2702,15 +2702,15 @@
       :type: Node
 
       The query (see comments above)
 
 
 .. class:: DefElem(defnamespace=None, defname=None, arg=None, defaction=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L762>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L762>`__ parser node.
 
    .. attribute:: defnamespace
       :type: str
 
       NULL if unqualified name
 
    .. attribute:: defname
@@ -2731,15 +2731,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: DefineStmt(kind=None, oldstyle=None, defnames=None, args=None, definition=None, if_not_exists=None, replace=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2741>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2741>`__ parser node.
 
    .. attribute:: kind
       :type: ObjectType
 
       Aggregate, operator, type
 
    .. attribute:: oldstyle
@@ -2771,15 +2771,15 @@
       :type: bool
 
       Replace if already exists?
 
 
 .. class:: DeleteStmt(relation=None, usingClause=None, whereClause=None, returningList=None, withClause=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1650>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1650>`__ parser node.
 
    .. attribute:: relation
       :type: RangeVar*
 
       Relation to delete from
 
    .. attribute:: usingClause
@@ -2801,59 +2801,59 @@
       :type: WithClause*
 
       WITH clause
 
 
 .. class:: DiscardStmt(target=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3520>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3520>`__ parser node.
 
    .. attribute:: target
       :type: DiscardMode
 
 
 .. class:: DoStmt(args=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3075>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3075>`__ parser node.
 
    .. attribute:: args
       :type: tuple
 
       List of DefElem nodes
 
 
 .. class:: DropOwnedStmt(roles=None, behavior=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3654>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3654>`__ parser node.
 
    .. attribute:: roles
       :type: tuple
 
    .. attribute:: behavior
       :type: DropBehavior
 
 
 .. class:: DropRoleStmt(roles=None, missing_ok=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2706>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2706>`__ parser node.
 
    .. attribute:: roles
       :type: tuple
 
       List of roles to remove
 
    .. attribute:: missing_ok
       :type: bool
 
       Skip error if a role is missing?
 
 
 .. class:: DropStmt(objects=None, removeType=None, behavior=None, missing_ok=None, concurrent=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2827>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2827>`__ parser node.
 
    .. attribute:: objects
       :type: tuple
 
       List of names
 
    .. attribute:: removeType
@@ -2875,15 +2875,15 @@
       :type: bool
 
       Drop index concurrently?
 
 
 .. class:: DropSubscriptionStmt(subname=None, missing_ok=None, behavior=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3804>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3804>`__ parser node.
 
    .. attribute:: subname
       :type: str
 
       Name of the subscription
 
    .. attribute:: missing_ok
@@ -2895,28 +2895,28 @@
       :type: DropBehavior
 
       RESTRICT or CASCADE behavior
 
 
 .. class:: DropTableSpaceStmt(tablespacename=None, missing_ok=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2390>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2390>`__ parser node.
 
    .. attribute:: tablespacename
       :type: str
 
    .. attribute:: missing_ok
       :type: bool
 
       Skip error if missing?
 
 
 .. class:: DropUserMappingStmt(user=None, servername=None, missing_ok=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2525>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2525>`__ parser node.
 
    .. attribute:: user
       :type: RoleSpec*
 
       User role
 
    .. attribute:: servername
@@ -2928,15 +2928,15 @@
       :type: bool
 
       Ignore missing mappings
 
 
 .. class:: DropdbStmt(dbname=None, missing_ok=None, options=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3388>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3388>`__ parser node.
 
    .. attribute:: dbname
       :type: str
 
       Database to drop
 
    .. attribute:: missing_ok
@@ -2948,45 +2948,45 @@
       :type: tuple
 
       Currently only FORCE is supported
 
 
 .. class:: ExecuteStmt(name=None, params=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3632>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3632>`__ parser node.
 
    .. attribute:: name
       :type: str
 
       The name of the plan to execute
 
    .. attribute:: params
       :type: tuple
 
       Values to assign to parameters
 
 
 .. class:: ExplainStmt(query=None, options=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3456>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3456>`__ parser node.
 
    .. attribute:: query
       :type: Node
 
       The query (see comments above)
 
    .. attribute:: options
       :type: tuple
 
       List of DefElem nodes
 
 
 .. class:: FetchStmt(direction=None, howMany=None, portalname=None, ismove=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2929>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2929>`__ parser node.
 
    .. attribute:: direction
       :type: FetchDirection
 
    .. attribute:: howMany
       :type: long
 
@@ -3001,15 +3001,15 @@
       :type: bool
 
       True if MOVE
 
 
 .. class:: FieldSelect(arg=None, fieldnum=None, resulttypmod=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L805>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L805>`__ parser node.
 
    .. attribute:: arg
       :type: Expr*
 
       Input expression
 
    .. attribute:: fieldnum
@@ -3021,15 +3021,15 @@
       :type: int32
 
       Output typmod (usually -1)
 
 
 .. class:: FieldStore(arg=None, newvals=None, fieldnums=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L834>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L834>`__ parser node.
 
    .. attribute:: arg
       :type: Expr*
 
       Input tuple value
 
    .. attribute:: newvals
@@ -3041,38 +3041,38 @@
       :type: tuple
 
       Integer list of field attnums
 
 
 .. class:: Float(fval=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/value.h#L45>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/value.h#L45>`__ parser node.
 
    .. attribute:: fval
       :type: str
 
 
 .. class:: FromExpr(fromlist=None, quals=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1559>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1559>`__ parser node.
 
    .. attribute:: fromlist
       :type: tuple
 
       List of join subtrees
 
    .. attribute:: quals
       :type: Node
 
       Qualifiers on join, if any
 
 
 .. class:: FuncCall(funcname=None, args=None, agg_order=None, agg_filter=None, over=None, agg_within_group=None, agg_star=None, agg_distinct=None, func_variadic=None, funcformat=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L378>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L378>`__ parser node.
 
    .. attribute:: funcname
       :type: tuple
 
       Qualified name of function
 
    .. attribute:: args
@@ -3124,15 +3124,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: FuncExpr(funcretset=None, funcvariadic=None, funcformat=None, args=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L492>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L492>`__ parser node.
 
    .. attribute:: funcretset
       :type: bool
 
       True if function returns set
 
    .. attribute:: funcvariadic
@@ -3155,15 +3155,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: FunctionParameter(name=None, argType=None, mode=None, defexpr=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3052>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3052>`__ parser node.
 
    .. attribute:: name
       :type: str
 
       Parameter name, or NULL if not given
 
    .. attribute:: argType
@@ -3180,15 +3180,15 @@
       :type: Node
 
       Raw default expr, or NULL if not given
 
 
 .. class:: GrantRoleStmt(granted_roles=None, grantee_roles=None, is_grant=None, admin_opt=None, grantor=None, behavior=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2150>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2150>`__ parser node.
 
    .. attribute:: granted_roles
       :type: tuple
 
       List of roles to be granted/revoked
 
    .. attribute:: grantee_roles
@@ -3215,15 +3215,15 @@
       :type: DropBehavior
 
       Drop behavior (for REVOKE)
 
 
 .. class:: GrantStmt(is_grant=None, targtype=None, objtype=None, objects=None, privileges=None, grantees=None, grant_option=None, grantor=None, behavior=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2085>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2085>`__ parser node.
 
    .. attribute:: is_grant
       :type: bool
 
       True = GRANT, false = REVOKE
 
    .. attribute:: targtype
@@ -3264,15 +3264,15 @@
       :type: DropBehavior
 
       Drop behavior (for REVOKE)
 
 
 .. class:: GroupingFunc(args=None, refs=None, cols=None, agglevelsup=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L369>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L369>`__ parser node.
 
    .. attribute:: args
       :type: tuple
 
       Arguments, not evaluated but kept for
       benefit of EXPLAIN etc.
 
@@ -3295,29 +3295,29 @@
       :type: int
 
       Token location
 
 
 .. class:: GroupingSet(kind=None, content=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1372>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1372>`__ parser node.
 
    .. attribute:: kind
       :type: GroupingSetKind
 
    .. attribute:: content
       :type: tuple
 
    .. attribute:: location
       :type: int
 
 
 .. class:: ImportForeignSchemaStmt(server_name=None, remote_schema=None, local_schema=None, list_type=None, table_list=None, options=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2545>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2545>`__ parser node.
 
    .. attribute:: server_name
       :type: str
 
       FDW server name
 
    .. attribute:: remote_schema
@@ -3344,15 +3344,15 @@
       :type: tuple
 
       List of options to pass to FDW
 
 
 .. class:: IndexElem(name=None, expr=None, indexcolname=None, collation=None, opclass=None, opclassopts=None, ordering=None, nulls_ordering=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L731>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L731>`__ parser node.
 
    .. attribute:: name
       :type: str
 
       Name of attribute to index, or NULL
 
    .. attribute:: expr
@@ -3389,15 +3389,15 @@
       :type: SortByNulls
 
       FIRST/LAST/default
 
 
 .. class:: IndexStmt(idxname=None, relation=None, accessMethod=None, tableSpace=None, indexParams=None, indexIncludingParams=None, options=None, whereClause=None, excludeOpNames=None, idxcomment=None, oldCreateSubid=None, oldFirstRelfilenodeSubid=None, unique=None, nulls_not_distinct=None, primary=None, isconstraint=None, deferrable=None, initdeferred=None, transformed=None, concurrent=None, if_not_exists=None, reset_default_tblspc=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2949>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2949>`__ parser node.
 
    .. attribute:: idxname
       :type: str
 
       Name of new index, or NULL for default
 
    .. attribute:: relation
@@ -3507,15 +3507,15 @@
 
       Reset default_tablespace prior to
       executing
 
 
 .. class:: InferClause(indexElems=None, whereClause=None, conname=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1459>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1459>`__ parser node.
 
    .. attribute:: indexElems
       :type: tuple
 
       IndexElems to infer unique index
 
    .. attribute:: whereClause
@@ -3532,25 +3532,25 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: InferenceElem(expr=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1387>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1387>`__ parser node.
 
    .. attribute:: expr
       :type: Node
 
       Expression to infer from, or NULL
 
 
 .. class:: InlineCodeBlock(source_text=None, langIsTrusted=None, atomic=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3081>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3081>`__ parser node.
 
    .. attribute:: source_text
       :type: str
 
       Source text of anonymous code block
 
    .. attribute:: langIsTrusted
@@ -3562,15 +3562,15 @@
       :type: bool
 
       Atomic execution context
 
 
 .. class:: InsertStmt(relation=None, cols=None, selectStmt=None, onConflictClause=None, returningList=None, withClause=None, override=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1634>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1634>`__ parser node.
 
    .. attribute:: relation
       :type: RangeVar*
 
       Relation to insert into
 
    .. attribute:: cols
@@ -3602,23 +3602,23 @@
       :type: OverridingKind
 
       OVERRIDING clause
 
 
 .. class:: Integer(ival=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/value.h#L28>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/value.h#L28>`__ parser node.
 
    .. attribute:: ival
       :type: long
 
 
 .. class:: IntoClause(rel=None, colNames=None, accessMethod=None, options=None, onCommit=None, tableSpaceName=None, viewQuery=None, skipData=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L108>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L108>`__ parser node.
 
    .. attribute:: rel
       :type: RangeVar*
 
       Target relation name
 
    .. attribute:: colNames
@@ -3655,15 +3655,15 @@
       :type: bool
 
       True for WITH NO DATA
 
 
 .. class:: JoinExpr(jointype=None, isNatural=None, larg=None, rarg=None, usingClause=None, join_using_alias=None, quals=None, alias=None, rtindex=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1536>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1536>`__ parser node.
 
    .. attribute:: jointype
       :type: JoinType
 
       Type of join
 
    .. attribute:: isNatural
@@ -3705,35 +3705,35 @@
       :type: int
 
       RT index assigned for join, or 0
 
 
 .. class:: ListenStmt(conditionname=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3225>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3225>`__ parser node.
 
    .. attribute:: conditionname
       :type: str
 
       Condition name to listen on
 
 
 .. class:: LoadStmt(filename=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3343>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3343>`__ parser node.
 
    .. attribute:: filename
       :type: str
 
       File to load
 
 
 .. class:: LockStmt(relations=None, mode=None, nowait=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3530>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3530>`__ parser node.
 
    .. attribute:: relations
       :type: tuple
 
       Relations to lock
 
    .. attribute:: mode
@@ -3745,15 +3745,15 @@
       :type: bool
 
       No wait mode
 
 
 .. class:: LockingClause(lockedRels=None, strength=None, waitPolicy=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L782>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L782>`__ parser node.
 
    .. attribute:: lockedRels
       :type: tuple
 
       FOR [KEY] UPDATE/SHARE relations
 
    .. attribute:: strength
@@ -3763,15 +3763,15 @@
       :type: LockWaitPolicy
 
       NOWAIT and SKIP LOCKED
 
 
 .. class:: MergeAction(matched=None, commandType=None, override=None, qual=None, targetList=None, updateColnos=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1571>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1571>`__ parser node.
 
    .. attribute:: matched
       :type: bool
 
       True=MATCHED, false=NOT MATCHED
 
    .. attribute:: commandType
@@ -3798,15 +3798,15 @@
       :type: tuple
 
       Target attribute numbers of an UPDATE
 
 
 .. class:: MergeStmt(relation=None, sourceRelation=None, joinCondition=None, mergeWhenClauses=None, withClause=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1679>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1679>`__ parser node.
 
    .. attribute:: relation
       :type: RangeVar*
 
       Target relation to merge into
 
    .. attribute:: sourceRelation
@@ -3828,15 +3828,15 @@
       :type: WithClause*
 
       WITH clause
 
 
 .. class:: MergeWhenClause(matched=None, commandType=None, override=None, condition=None, targetList=None, values=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1555>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1555>`__ parser node.
 
    .. attribute:: matched
       :type: bool
 
       True=MATCHED, false=NOT MATCHED
 
    .. attribute:: commandType
@@ -3863,15 +3863,15 @@
       :type: tuple
 
       VALUES to INSERT, or NULL
 
 
 .. class:: MinMaxExpr(op=None, args=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1143>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1143>`__ parser node.
 
    .. attribute:: op
       :type: MinMaxOp
 
       Function to execute
 
    .. attribute:: args
@@ -3883,15 +3883,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: MultiAssignRef(source=None, colno=None, ncolumns=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L487>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L487>`__ parser node.
 
    .. attribute:: source
       :type: Node
 
       The row-valued expression
 
    .. attribute:: colno
@@ -3903,15 +3903,15 @@
       :type: int
 
       Number of targets in the construct
 
 
 .. class:: NamedArgExpr(arg=None, name=None, argnumber=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L521>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L521>`__ parser node.
 
    .. attribute:: arg
       :type: Expr*
 
       The argument expression
 
    .. attribute:: name
@@ -3928,30 +3928,30 @@
       :type: int
 
       Argument name location, or -1 if unknown
 
 
 .. class:: NotifyStmt(conditionname=None, payload=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3214>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3214>`__ parser node.
 
    .. attribute:: conditionname
       :type: str
 
       Condition name to notify
 
    .. attribute:: payload
       :type: str
 
       The payload string, or NULL if none
 
 
 .. class:: NullTest(arg=None, nulltesttype=None, argisrow=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1260>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1260>`__ parser node.
 
    .. attribute:: arg
       :type: Expr*
 
       Input expression
 
    .. attribute:: nulltesttype
@@ -3968,15 +3968,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: ObjectWithArgs(objname=None, objargs=None, objfuncargs=None, args_unspecified=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2118>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2118>`__ parser node.
 
    .. attribute:: objname
       :type: tuple
 
       Qualified name of function/operator
 
    .. attribute:: objargs
@@ -3993,15 +3993,15 @@
       :type: bool
 
       Argument list was omitted?
 
 
 .. class:: OnConflictClause(action=None, infer=None, targetList=None, whereClause=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1474>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1474>`__ parser node.
 
    .. attribute:: action
       :type: OnConflictAction
 
       DO NOTHING or UPDATE?
 
    .. attribute:: infer
@@ -4023,15 +4023,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: OnConflictExpr(action=None, arbiterElems=None, arbiterWhere=None, onConflictSet=None, onConflictWhere=None, exclRelIndex=None, exclRelTlist=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1575>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1575>`__ parser node.
 
    .. attribute:: action
       :type: OnConflictAction
 
       DO NOTHING or UPDATE?
 
    .. attribute:: arbiterElems
@@ -4064,15 +4064,15 @@
       :type: tuple
 
       Tlist of the EXCLUDED pseudo relation
 
 
 .. class:: OpExpr(opretset=None, args=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L539>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L539>`__ parser node.
 
    .. attribute:: opretset
       :type: bool
 
       True if operator returns set
 
    .. attribute:: args
@@ -4084,15 +4084,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: PLAssignStmt(name=None, indirection=None, nnames=None, val=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1814>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1814>`__ parser node.
 
    .. attribute:: name
       :type: str
 
       Initial column name
 
    .. attribute:: indirection
@@ -4114,15 +4114,15 @@
       :type: int
 
       Name's token location, or -1 if unknown
 
 
 .. class:: Param(paramkind=None, paramid=None, paramtypmod=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L264>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L264>`__ parser node.
 
    .. attribute:: paramkind
       :type: ParamKind
 
       Kind of parameter. See above
 
    .. attribute:: paramid
@@ -4139,30 +4139,30 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: ParamRef(number=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L260>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L260>`__ parser node.
 
    .. attribute:: number
       :type: int
 
       The number of the parameter
 
    .. attribute:: location
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: PartitionBoundSpec(strategy=None, is_default=None, modulus=None, remainder=None, listdatums=None, lowerdatums=None, upperdatums=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L845>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L845>`__ parser node.
 
    .. attribute:: strategy
       :type: str
 
       See PARTITION_STRATEGY codes above
 
    .. attribute:: is_default
@@ -4195,15 +4195,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: PartitionCmd(name=None, bound=None, concurrent=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L892>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L892>`__ parser node.
 
    .. attribute:: name
       :type: RangeVar*
 
       Name of partition to attach/detach
 
    .. attribute:: bound
@@ -4213,15 +4213,15 @@
 
    .. attribute:: concurrent
       :type: bool
 
 
 .. class:: PartitionElem(name=None, expr=None, collation=None, opclass=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L810>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L810>`__ parser node.
 
    .. attribute:: name
       :type: str
 
       Name of column to partition on, or NULL
 
    .. attribute:: expr
@@ -4243,15 +4243,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: PartitionRangeDatum(kind=None, value=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L878>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L878>`__ parser node.
 
    .. attribute:: kind
       :type: PartitionRangeDatumKind
 
    .. attribute:: value
       :type: Node
 
@@ -4262,15 +4262,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: PartitionSpec(strategy=None, partParams=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L825>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L825>`__ parser node.
 
    .. attribute:: strategy
       :type: str
 
       Partitioning strategy ('hash', 'list' or
       'range')
 
@@ -4283,15 +4283,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: PrepareStmt(name=None, argtypes=None, query=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3618>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3618>`__ parser node.
 
    .. attribute:: name
       :type: str
 
       Name of plan, arbitrary
 
    .. attribute:: argtypes
@@ -4303,15 +4303,15 @@
       :type: Node
 
       The query itself (as a raw parsetree)
 
 
 .. class:: PublicationObjSpec(pubobjtype=None, name=None, pubtable=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3730>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3730>`__ parser node.
 
    .. attribute:: pubobjtype
       :type: PublicationObjSpecType
 
       Type of this publication object
 
    .. attribute:: name
@@ -4324,15 +4324,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: PublicationTable(relation=None, whereClause=None, columns=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3710>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3710>`__ parser node.
 
    .. attribute:: relation
       :type: RangeVar*
 
       Relation to be published
 
    .. attribute:: whereClause
@@ -4344,15 +4344,15 @@
       :type: tuple
 
       List of columns in a publication table
 
 
 .. class:: Query(commandType=None, querySource=None, queryId=None, canSetTag=None, utilityStmt=None, resultRelation=None, hasAggs=None, hasWindowFuncs=None, hasTargetSRFs=None, hasSubLinks=None, hasDistinctOn=None, hasRecursive=None, hasModifyingCTE=None, hasForUpdate=None, hasRowSecurity=None, isReturn=None, cteList=None, rtable=None, jointree=None, mergeActionList=None, mergeUseOuterJoin=None, targetList=None, override=None, onConflict=None, returningList=None, groupClause=None, groupDistinct=None, groupingSets=None, havingQual=None, windowClause=None, distinctClause=None, sortClause=None, limitOffset=None, limitCount=None, limitOption=None, rowMarks=None, setOperations=None, constraintDeps=None, withCheckOptions=None, stmt_location=None, stmt_len=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L118>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L118>`__ parser node.
 
    .. attribute:: commandType
       :type: CmdType
 
       Select|insert|update|delete|merge|utility
 
    .. attribute:: querySource
@@ -4559,15 +4559,15 @@
       :type: int
 
       Length in bytes; 0 means "rest of string"
 
 
 .. class:: RangeFunction(lateral=None, ordinality=None, is_rowsfrom=None, functions=None, alias=None, coldeflist=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L592>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L592>`__ parser node.
 
    .. attribute:: lateral
       :type: bool
 
       Does it have LATERAL prefix?
 
    .. attribute:: ordinality
@@ -4595,15 +4595,15 @@
 
       List of ColumnDef nodes to describe result
       of function returning RECORD
 
 
 .. class:: RangeSubselect(lateral=None, subquery=None, alias=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L570>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L570>`__ parser node.
 
    .. attribute:: lateral
       :type: bool
 
       Does it have LATERAL prefix?
 
    .. attribute:: subquery
@@ -4615,15 +4615,15 @@
       :type: Alias*
 
       Table alias & optional column aliases
 
 
 .. class:: RangeTableFunc(lateral=None, docexpr=None, rowexpr=None, namespaces=None, columns=None, alias=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L607>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L607>`__ parser node.
 
    .. attribute:: lateral
       :type: bool
 
       Does it have LATERAL prefix?
 
    .. attribute:: docexpr
@@ -4655,15 +4655,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: RangeTableFuncCol(colname=None, typeName=None, for_ordinality=None, is_not_null=None, colexpr=None, coldefexpr=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L625>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L625>`__ parser node.
 
    .. attribute:: colname
       :type: str
 
       Name of generated column
 
    .. attribute:: typeName
@@ -4695,15 +4695,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: RangeTableSample(relation=None, method=None, args=None, repeatable=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L647>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L647>`__ parser node.
 
    .. attribute:: relation
       :type: Node
 
       Relation to be sampled
 
    .. attribute:: method
@@ -4725,15 +4725,15 @@
       :type: int
 
       Method name location, or -1 if unknown
 
 
 .. class:: RangeTblEntry(rtekind=None, relkind=None, rellockmode=None, tablesample=None, subquery=None, security_barrier=None, jointype=None, joinmergedcols=None, joinaliasvars=None, joinleftcols=None, joinrightcols=None, join_using_alias=None, functions=None, funcordinality=None, tablefunc=None, values_lists=None, ctename=None, ctelevelsup=None, self_reference=None, coltypes=None, coltypmods=None, colcollations=None, enrname=None, enrtuples=None, alias=None, eref=None, lateral=None, inh=None, inFromCl=None, requiredPerms=None, selectedCols=None, insertedCols=None, updatedCols=None, extraUpdatedCols=None, securityQuals=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1012>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1012>`__ parser node.
 
    .. attribute:: rtekind
       :type: RTEKind
 
    .. attribute:: relkind
       :type: str
 
@@ -4899,15 +4899,15 @@
       :type: tuple
 
       Security barrier quals to apply, if any
 
 
 .. class:: RangeTblFunction(funcexpr=None, funccolcount=None, funccolnames=None, funccoltypes=None, funccoltypmods=None, funccolcollations=None, funcparams=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1191>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1191>`__ parser node.
 
    .. attribute:: funcexpr
       :type: Node
 
       Expression tree for func call
 
    .. attribute:: funccolcount
@@ -4939,23 +4939,23 @@
       :type: Bitmapset*
 
       PARAM_EXEC Param IDs affecting this func
 
 
 .. class:: RangeTblRef(rtindex=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1502>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1502>`__ parser node.
 
    .. attribute:: rtindex
       :type: int
 
 
 .. class:: RangeVar(catalogname=None, schemaname=None, relname=None, inh=None, relpersistence=None, alias=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L63>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L63>`__ parser node.
 
    .. attribute:: catalogname
       :type: str
 
       The catalog (database) name, or NULL
 
    .. attribute:: schemaname
@@ -4988,15 +4988,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: RawStmt(stmt=None, stmt_location=None, stmt_len=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1614>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1614>`__ parser node.
 
    .. attribute:: stmt
       :type: Node
 
       Raw parse tree
 
    .. attribute:: stmt_location
@@ -5008,26 +5008,26 @@
       :type: int
 
       Length in bytes; 0 means "rest of string"
 
 
 .. class:: ReassignOwnedStmt(roles=None, newrole=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3664>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3664>`__ parser node.
 
    .. attribute:: roles
       :type: tuple
 
    .. attribute:: newrole
       :type: RoleSpec*
 
 
 .. class:: RefreshMatViewStmt(concurrent=None, skipData=None, relation=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3490>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3490>`__ parser node.
 
    .. attribute:: concurrent
       :type: bool
 
       Allow concurrent access?
 
    .. attribute:: skipData
@@ -5039,15 +5039,15 @@
       :type: RangeVar*
 
       Relation to insert into
 
 
 .. class:: ReindexStmt(kind=None, relation=None, name=None, params=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3562>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3562>`__ parser node.
 
    .. attribute:: kind
       :type: ReindexObjectType
 
       REINDEX_OBJECT_INDEX, REINDEX_OBJECT_TABLE,
       etc.
 
@@ -5065,15 +5065,15 @@
       :type: tuple
 
       List of DefElem nodes
 
 
 .. class:: RelabelType(arg=None, resulttypmod=None, relabelformat=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L857>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L857>`__ parser node.
 
    .. attribute:: arg
       :type: Expr*
 
       Input expression
 
    .. attribute:: resulttypmod
@@ -5090,15 +5090,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: RenameStmt(renameType=None, relationType=None, relation=None, object=None, subname=None, newname=None, behavior=None, missing_ok=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3117>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3117>`__ parser node.
 
    .. attribute:: renameType
       :type: ObjectType
 
       OBJECT_TABLE, OBJECT_COLUMN, etc
 
    .. attribute:: relationType
@@ -5136,26 +5136,26 @@
       :type: bool
 
       Skip error if missing?
 
 
 .. class:: ReplicaIdentityStmt(identity_type=None, name=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2013>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2013>`__ parser node.
 
    .. attribute:: identity_type
       :type: str
 
    .. attribute:: name
       :type: str
 
 
 .. class:: ResTarget(name=None, indirection=None, val=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L469>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L469>`__ parser node.
 
    .. attribute:: name
       :type: str
 
       Column name or NULL
 
    .. attribute:: indirection
@@ -5172,23 +5172,23 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: ReturnStmt(returnval=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1800>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1800>`__ parser node.
 
    .. attribute:: returnval
       :type: Node
 
 
 .. class:: RoleSpec(roletype=None, rolename=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L356>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L356>`__ parser node.
 
    .. attribute:: roletype
       :type: RoleSpecType
 
       Type of this rolespec
 
    .. attribute:: rolename
@@ -5200,15 +5200,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: RowCompareExpr(rctype=None, opnos=None, opfamilies=None, inputcollids=None, largs=None, rargs=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1111>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1111>`__ parser node.
 
    .. attribute:: rctype
       :type: RowCompareType
 
       LT LE GE or GT, never EQ or NE
 
    .. attribute:: opnos
@@ -5235,15 +5235,15 @@
       :type: tuple
 
       The right-hand input arguments
 
 
 .. class:: RowExpr(args=None, row_format=None, colnames=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1063>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1063>`__ parser node.
 
    .. attribute:: args
       :type: tuple
 
       The fields
 
    .. attribute:: row_format
@@ -5260,15 +5260,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: RowMarkClause(rti=None, strength=None, waitPolicy=None, pushedDown=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1429>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1429>`__ parser node.
 
    .. attribute:: rti
       :type: Index
 
       Range table index of target relation
 
    .. attribute:: strength
@@ -5283,15 +5283,15 @@
       :type: bool
 
       Pushed down from higher query level?
 
 
 .. class:: RuleStmt(relation=None, rulename=None, whereClause=None, event=None, instead=None, actions=None, replace=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3198>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3198>`__ parser node.
 
    .. attribute:: relation
       :type: RangeVar*
 
       Relation the rule is for
 
    .. attribute:: rulename
@@ -5323,15 +5323,15 @@
       :type: bool
 
       OR REPLACE
 
 
 .. class:: SQLValueFunction(op=None, typmod=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1184>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1184>`__ parser node.
 
    .. attribute:: op
       :type: SQLValueFunctionOp
 
       Which function this is
 
    .. attribute:: typmod
@@ -5341,15 +5341,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: ScalarArrayOpExpr(useOr=None, args=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L596>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L596>`__ parser node.
 
    .. attribute:: useOr
       :type: bool
 
       True for ANY, false for ALL
 
    .. attribute:: args
@@ -5361,15 +5361,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: SecLabelStmt(objtype=None, object=None, provider=None, label=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2865>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2865>`__ parser node.
 
    .. attribute:: objtype
       :type: ObjectType
 
       Object's type
 
    .. attribute:: object
@@ -5386,15 +5386,15 @@
       :type: str
 
       New security label to be assigned
 
 
 .. class:: SelectStmt(distinctClause=None, intoClause=None, targetList=None, fromClause=None, whereClause=None, groupClause=None, groupDistinct=None, havingClause=None, windowClause=None, valuesLists=None, sortClause=None, limitOffset=None, limitCount=None, limitOption=None, lockingClause=None, withClause=None, op=None, all=None, larg=None, rarg=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1710>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1710>`__ parser node.
 
    .. attribute:: distinctClause
       :type: tuple
 
       NULL, list of DISTINCT ON exprs, or
       lcons(NIL,NIL) for all (SELECT DISTINCT)
 
@@ -5492,15 +5492,15 @@
       :type: SelectStmt*
 
       Right child
 
 
 .. class:: SetOperationStmt(op=None, all=None, larg=None, rarg=None, colTypes=None, colTypmods=None, colCollations=None, groupClauses=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1779>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1779>`__ parser node.
 
    .. attribute:: op
       :type: SetOperation
 
       Type of set op
 
    .. attribute:: all
@@ -5537,30 +5537,30 @@
       :type: tuple
 
       A list of SortGroupClause's
 
 
 .. class:: SetToDefault(typeMod=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1336>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1336>`__ parser node.
 
    .. attribute:: typeMod
       :type: int32
 
       Typemod for substituted value
 
    .. attribute:: location
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: SortBy(node=None, sortby_dir=None, sortby_nulls=None, useOp=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L498>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L498>`__ parser node.
 
    .. attribute:: node
       :type: Node
 
       Expression to sort on
 
    .. attribute:: sortby_dir
@@ -5582,15 +5582,15 @@
       :type: int
 
       Operator location, or -1 if none/unknown
 
 
 .. class:: SortGroupClause(tleSortGroupRef=None, nulls_first=None, hashable=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1303>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1303>`__ parser node.
 
    .. attribute:: tleSortGroupRef
       :type: Index
 
       Reference into targetlist
 
    .. attribute:: nulls_first
@@ -5602,38 +5602,38 @@
       :type: bool
 
       Can eqop be implemented by hashing?
 
 
 .. class:: StatsElem(name=None, expr=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3004>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3004>`__ parser node.
 
    .. attribute:: name
       :type: str
 
       Name of attribute to index, or NULL
 
    .. attribute:: expr
       :type: Node
 
       Expression to index, or NULL
 
 
 .. class:: String(sval=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/value.h#L57>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/value.h#L57>`__ parser node.
 
    .. attribute:: sval
       :type: str
 
 
 .. class:: SubLink(subLinkType=None, subLinkId=None, testexpr=None, operName=None, subselect=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L694>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L694>`__ parser node.
 
    .. attribute:: subLinkType
       :type: SubLinkType
 
    .. attribute:: subLinkId
       :type: int
 
@@ -5658,15 +5658,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: SubPlan(subLinkType=None, testexpr=None, paramIds=None, plan_id=None, plan_name=None, firstColTypmod=None, useHashTable=None, unknownEqFalse=None, parallel_safe=None, setParam=None, parParam=None, args=None, startup_cost=None, per_call_cost=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L743>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L743>`__ parser node.
 
    .. attribute:: subLinkType
       :type: SubLinkType
 
    .. attribute:: testexpr
       :type: Node
 
@@ -5735,15 +5735,15 @@
       :type: Cost
 
       Cost for each subplan evaluation
 
 
 .. class:: SubscriptingRef(reftypmod=None, refupperindexpr=None, reflowerindexpr=None, refexpr=None, refassgnexpr=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L436>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L436>`__ parser node.
 
    .. attribute:: reftypmod
       :type: int32
 
       Typmod of the result
 
    .. attribute:: refupperindexpr
@@ -5770,15 +5770,15 @@
 
       Expression for the source value, or NULL if
       fetch
 
 
 .. class:: TableFunc(ns_uris=None, ns_names=None, docexpr=None, rowexpr=None, colnames=None, coltypes=None, coltypmods=None, colcollations=None, colexprs=None, coldefexprs=None, notnulls=None, ordinalitycol=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L82>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L82>`__ parser node.
 
    .. attribute:: ns_uris
       :type: tuple
 
       List of namespace URI expressions
 
    .. attribute:: ns_names
@@ -5840,43 +5840,43 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: TableLikeClause(relation=None, options=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L702>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L702>`__ parser node.
 
    .. attribute:: relation
       :type: RangeVar*
 
    .. attribute:: options
       :type: bits32
 
       OR of TableLikeOption flags
 
 
 .. class:: TableSampleClause(args=None, repeatable=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1211>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1211>`__ parser node.
 
    .. attribute:: args
       :type: tuple
 
       Tablesample argument expression(s)
 
    .. attribute:: repeatable
       :type: Expr*
 
       REPEATABLE expression, or NULL if none
 
 
 .. class:: TargetEntry(expr=None, resno=None, resname=None, ressortgroupref=None, resorigcol=None, resjunk=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1450>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1450>`__ parser node.
 
    .. attribute:: expr
       :type: Expr*
 
       Expression to evaluate
 
    .. attribute:: resno
@@ -5905,15 +5905,15 @@
 
       Set to true to eliminate the attribute from
       final target list
 
 
 .. class:: TransactionStmt(kind=None, options=None, savepoint_name=None, gid=None, chain=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3259>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3259>`__ parser node.
 
    .. attribute:: kind
       :type: TransactionStmtKind
 
    .. attribute:: options
       :type: tuple
 
@@ -5933,29 +5933,29 @@
       :type: bool
 
       AND CHAIN option
 
 
 .. class:: TriggerTransition(name=None, isNew=None, isTable=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1590>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1590>`__ parser node.
 
    .. attribute:: name
       :type: str
 
    .. attribute:: isNew
       :type: bool
 
    .. attribute:: isTable
       :type: bool
 
 
 .. class:: TruncateStmt(relations=None, restart_seqs=None, behavior=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2841>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2841>`__ parser node.
 
    .. attribute:: relations
       :type: tuple
 
       Relations (RangeVars) to be truncated
 
    .. attribute:: restart_seqs
@@ -5967,15 +5967,15 @@
       :type: DropBehavior
 
       RESTRICT or CASCADE behavior
 
 
 .. class:: TypeCast(arg=None, typeName=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L325>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L325>`__ parser node.
 
    .. attribute:: arg
       :type: Node
 
       The expression being casted
 
    .. attribute:: typeName
@@ -5987,15 +5987,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: TypeName(names=None, setof=None, pct_type=None, typmods=None, typemod=None, arrayBounds=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L224>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L224>`__ parser node.
 
    .. attribute:: names
       :type: tuple
 
       Qualified name (list of String nodes)
 
    .. attribute:: setof
@@ -6027,25 +6027,25 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: UnlistenStmt(conditionname=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3235>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3235>`__ parser node.
 
    .. attribute:: conditionname
       :type: str
 
       Name to unlisten on, or NULL for all
 
 
 .. class:: UpdateStmt(relation=None, targetList=None, whereClause=None, fromClause=None, returningList=None, withClause=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1664>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1664>`__ parser node.
 
    .. attribute:: relation
       :type: RangeVar*
 
       Relation to update
 
    .. attribute:: targetList
@@ -6072,30 +6072,30 @@
       :type: WithClause*
 
       WITH clause
 
 
 .. class:: VacuumRelation(relation=None, va_cols=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3440>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3440>`__ parser node.
 
    .. attribute:: relation
       :type: RangeVar*
 
       Table name to process, or NULL
 
    .. attribute:: va_cols
       :type: tuple
 
       List of column names, or NIL for all
 
 
 .. class:: VacuumStmt(options=None, rels=None, is_vacuumcmd=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3425>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3425>`__ parser node.
 
    .. attribute:: options
       :type: tuple
 
       List of DefElem nodes
 
    .. attribute:: rels
@@ -6107,15 +6107,15 @@
       :type: bool
 
       True for VACUUM, false for ANALYZE
 
 
 .. class:: Var(varno=None, varattno=None, vartypmod=None, varlevelsup=None, varnosyn=None, varattnosyn=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L186>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L186>`__ parser node.
 
    .. attribute:: varno
       :type: int
 
       Index of this var's relation in the range
       table, or INNER_VAR/OUTER_VAR/etc
 
@@ -6151,15 +6151,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: VariableSetStmt(kind=None, name=None, args=None, is_local=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2212>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2212>`__ parser node.
 
    .. attribute:: kind
       :type: VariableSetKind
 
    .. attribute:: name
       :type: str
 
@@ -6174,23 +6174,23 @@
       :type: bool
 
       SET LOCAL?
 
 
 .. class:: VariableShowStmt(name=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2225>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2225>`__ parser node.
 
    .. attribute:: name
       :type: str
 
 
 .. class:: ViewStmt(view=None, aliases=None, query=None, replace=None, options=None, withCheckOption=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3328>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3328>`__ parser node.
 
    .. attribute:: view
       :type: RangeVar*
 
       The view to be created
 
    .. attribute:: aliases
@@ -6217,15 +6217,15 @@
       :type: ViewCheckOption
 
       WITH CHECK OPTION
 
 
 .. class:: WindowClause(name=None, refname=None, partitionClause=None, orderClause=None, frameOptions=None, startOffset=None, endOffset=None, runCondition=None, inRangeAsc=None, inRangeNullsFirst=None, winref=None, copiedOrder=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1397>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1397>`__ parser node.
 
    .. attribute:: name
       :type: str
 
       Window name (NULL in an OVER clause)
 
    .. attribute:: refname
@@ -6282,15 +6282,15 @@
       :type: bool
 
       Did we copy orderClause from refname?
 
 
 .. class:: WindowDef(name=None, refname=None, partitionClause=None, orderClause=None, frameOptions=None, startOffset=None, endOffset=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L516>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L516>`__ parser node.
 
    .. attribute:: name
       :type: str
 
       Window's own name
 
    .. attribute:: refname
@@ -6327,15 +6327,15 @@
       :type: int
 
       Parse location, or -1 if none/unknown
 
 
 .. class:: WindowFunc(args=None, aggfilter=None, winref=None, winstar=None, winagg=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L383>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L383>`__ parser node.
 
    .. attribute:: args
       :type: tuple
 
       Arguments to the window function
 
    .. attribute:: aggfilter
@@ -6362,15 +6362,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: WithCheckOption(kind=None, relname=None, polname=None, qual=None, cascaded=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1235>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1235>`__ parser node.
 
    .. attribute:: kind
       :type: WCOKind
 
       Kind of WCO
 
    .. attribute:: relname
@@ -6392,15 +6392,15 @@
       :type: bool
 
       True for a cascaded WCO on a view
 
 
 .. class:: WithClause(ctes=None, recursive=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1445>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1445>`__ parser node.
 
    .. attribute:: ctes
       :type: tuple
 
       List of CommonTableExprs
 
    .. attribute:: recursive
@@ -6412,15 +6412,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: XmlExpr(op=None, name=None, named_args=None, arg_names=None, args=None, xmloption=None, typmod=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1222>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1222>`__ parser node.
 
    .. attribute:: op
       :type: XmlExprOp
 
       Xml function ID
 
    .. attribute:: name
@@ -6455,15 +6455,15 @@
       :type: int
 
       Token location, or -1 if unknown
 
 
 .. class:: XmlSerialize(xmloption=None, expr=None, typeName=None, location=None)
 
-   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L793>`__ parser node.
+   Wrapper for the `homonymous <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L793>`__ parser node.
 
    .. attribute:: xmloption
       :type: XmlOptionType
 
       DOCUMENT or CONTENT
 
    .. attribute:: expr
```

### Comparing `pglast-5.2/docs/changes.rst` & `pglast-5.3/docs/changes.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,22 @@
 
 Changes
 -------
 
 Version 5
 #########
 
+5.3 (2023-08-05)
+~~~~~~~~~~~~~~~~
+
+- Update libpg_query to `15-4.2.3`__
+
+  __ https://github.com/pganalyze/libpg_query/releases/tag/15-4.2.3
+
+
 5.2 (2023-05-20)
 ~~~~~~~~~~~~~~~~
 
 - Update libpg_query to `15-4.2.1`__
 
   __ https://github.com/pganalyze/libpg_query/releases/tag/15-4.2.1
```

### Comparing `pglast-5.2/docs/conf.py` & `pglast-5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pglast-5.2/docs/ddl.rst` & `pglast-5.3/docs/ddl.rst`

 * *Files 21% similar despite different names*

```diff
@@ -12,144 +12,144 @@
 .. module:: pglast.printers.ddl
    :synopsis: DDL printer functions
 
 .. index:: AccessPriv
 
 .. function:: access_priv(node, output)
 
-   Pretty print a `node` of type `AccessPriv <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2134>`__ to the `output` stream.
+   Pretty print a `node` of type `AccessPriv <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2134>`__ to the `output` stream.
 
 .. index:: AlterCollationStmt
 
 .. function:: alter_collation_stmt(node, output)
 
-   Pretty print a `node` of type `AlterCollationStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2041>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterCollationStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2041>`__ to the `output` stream.
 
 .. index:: AlterDatabaseStmt
 
 .. function:: alter_database_stmt(node, output)
 
-   Pretty print a `node` of type `AlterDatabaseStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3364>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterDatabaseStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3364>`__ to the `output` stream.
 
 .. index:: AlterDatabaseSetStmt
 
 .. function:: alter_database_set_stmt(node, output)
 
-   Pretty print a `node` of type `AlterDatabaseSetStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3377>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterDatabaseSetStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3377>`__ to the `output` stream.
 
 .. index:: AlterExtensionStmt
 
 .. function:: alter_extension_stmt(node, output)
 
-   Pretty print a `node` of type `AlterExtensionStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2429>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterExtensionStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2429>`__ to the `output` stream.
 
 .. index::
    pair: AlterExtensionStmt;DefElem
 
 .. function:: alter_extension_stmt_def_elem(node, output)
 
-   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `AlterExtensionStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2429>`__, to the `output` stream.
+   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `AlterExtensionStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2429>`__, to the `output` stream.
 
 .. index:: AlterExtensionContentsStmt
 
 .. function:: alter_extension_contents_stmt(node, output)
 
-   Pretty print a `node` of type `AlterExtensionContentsStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2436>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterExtensionContentsStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2436>`__ to the `output` stream.
 
 .. index:: AlterEnumStmt
 
 .. function:: alter_enum_stmt(node, output)
 
-   Pretty print a `node` of type `AlterEnumStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3306>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterEnumStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3306>`__ to the `output` stream.
 
 .. index:: AlterDefaultPrivilegesStmt
 
 .. function:: alter_default_privileges_stmt(node, output)
 
-   Pretty print a `node` of type `AlterDefaultPrivilegesStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2165>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterDefaultPrivilegesStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2165>`__ to the `output` stream.
 
 .. index:: AlterFunctionStmt
 
 .. function:: alter_function_stmt(node, output)
 
-   Pretty print a `node` of type `AlterFunctionStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3061>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterFunctionStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3061>`__ to the `output` stream.
 
 .. index:: AlterObjectSchemaStmt
 
 .. function:: alter_object_schema_stmt(node, output)
 
-   Pretty print a `node` of type `AlterObjectSchemaStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3149>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterObjectSchemaStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3149>`__ to the `output` stream.
 
 .. index:: AlterOperatorStmt
 
 .. function:: alter_operator_stmt(node, output)
 
-   Pretty print a `node` of type `AlterOperatorStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3176>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterOperatorStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3176>`__ to the `output` stream.
 
 .. index::
    pair: AlterOperatorStmt;DefElem
 
 .. function:: alter_operator_stmt_def_elem(node, output)
 
-   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `AlterOperatorStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3176>`__, to the `output` stream.
+   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `AlterOperatorStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3176>`__, to the `output` stream.
 
 .. index:: AlterOpFamilyStmt
 
 .. function:: alter_op_family_stmt(node, output)
 
-   Pretty print a `node` of type `AlterOpFamilyStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2813>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterOpFamilyStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2813>`__ to the `output` stream.
 
 .. index:: AlterOwnerStmt
 
 .. function:: alter_owner_stmt(node, output)
 
-   Pretty print a `node` of type `AlterOwnerStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3163>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterOwnerStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3163>`__ to the `output` stream.
 
 .. index:: AlterPolicyStmt
 
 .. function:: alter_policy_stmt(node, output)
 
-   Pretty print a `node` of type `AlterPolicyStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2576>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterPolicyStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2576>`__ to the `output` stream.
 
 .. index:: AlterRoleStmt
 
 .. function:: alter_role_stmt(node, output)
 
-   Pretty print a `node` of type `AlterRoleStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2690>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterRoleStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2690>`__ to the `output` stream.
 
 .. index:: AlterSeqStmt
 
 .. function:: alter_seq_stmt(node, output)
 
-   Pretty print a `node` of type `AlterSeqStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2728>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterSeqStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2728>`__ to the `output` stream.
 
 .. index:: AlterTableSpaceOptionsStmt
 
 .. function:: alter_tablespace_options_stmt(node, output)
 
-   Pretty print a `node` of type `AlterTableSpaceOptionsStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2397>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterTableSpaceOptionsStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2397>`__ to the `output` stream.
 
 .. index:: AlterTableStmt
 
 .. function:: alter_table_stmt(node, output)
 
-   Pretty print a `node` of type `AlterTableStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1929>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterTableStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1929>`__ to the `output` stream.
 
 .. index::
    pair: AlterTableStmt;RangeVar
 
 .. function:: range_var(node, output)
 
-   Pretty print a `node` of type `RangeVar <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L63>`__, when it is inside a `AlterTableStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1929>`__, to the `output` stream.
+   Pretty print a `node` of type `RangeVar <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L63>`__, when it is inside a `AlterTableStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1929>`__, to the `output` stream.
 
 .. index:: AlterTableCmd
 
 .. function:: alter_table_cmd(node, output)
 
-   Pretty print a `node` of type `AlterTableCmd <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2020>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterTableCmd <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2020>`__ to the `output` stream.
 
 .. index::
    pair: AlterTableCmd;DefElem
 
 .. index::
    pair: CreatePublicationStmt;DefElem
 
@@ -160,758 +160,758 @@
    pair: IndexStmt;DefElem
 
 .. index::
    pair: IntoClause;DefElem
 
 .. function:: alter_table_cmd_def_elem(node, output)
 
-   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `AlterTableCmd <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2020>`__ or a `CreatePublicationStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3739>`__ or a `CreateStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2242>`__ or a `IndexStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2949>`__ or a `IntoClause <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L108>`__, to the `output` stream.
+   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `AlterTableCmd <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2020>`__ or a `CreatePublicationStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3739>`__ or a `CreateStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2242>`__ or a `IndexStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2949>`__ or a `IntoClause <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L108>`__, to the `output` stream.
 
 .. index:: AlterTableMoveAllStmt
 
 .. function:: alter_table_move_all_stmt(node, output)
 
-   Pretty print a `node` of type `AlterTableMoveAllStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2405>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterTableMoveAllStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2405>`__ to the `output` stream.
 
 .. index:: AlterTSConfigurationStmt
 
 .. function:: alter_ts_configuration_stmt(node, output)
 
-   Pretty print a `node` of type `AlterTSConfigurationStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3693>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterTSConfigurationStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3693>`__ to the `output` stream.
 
 .. index:: AlterTSDictionaryStmt
 
 .. function:: alter_ts_dictionary_stmt(node, output)
 
-   Pretty print a `node` of type `AlterTSDictionaryStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3674>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterTSDictionaryStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3674>`__ to the `output` stream.
 
 .. index:: AlterStatsStmt
 
 .. function:: alter_stats_stmt(node, output)
 
-   Pretty print a `node` of type `AlterStatsStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3016>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterStatsStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3016>`__ to the `output` stream.
 
 .. index:: AlterSubscriptionStmt
 
 .. function:: alter_subscription_stmt(node, output)
 
-   Pretty print a `node` of type `AlterSubscriptionStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3794>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterSubscriptionStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3794>`__ to the `output` stream.
 
 .. index:: AlterPublicationStmt
 
 .. function:: alter_publication_stmt(node, output)
 
-   Pretty print a `node` of type `AlterPublicationStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3755>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterPublicationStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3755>`__ to the `output` stream.
 
 .. index:: AlterFdwStmt
 
 .. function:: alter_fdw_stmt(node, output)
 
-   Pretty print a `node` of type `AlterFdwStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2458>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterFdwStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2458>`__ to the `output` stream.
 
 .. index::
    pair: AlterFdwStmt;DefElem
 
 .. function:: alter_fdw_stmt_def_elem(node, output)
 
-   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `AlterFdwStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2458>`__, to the `output` stream.
+   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `AlterFdwStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2458>`__, to the `output` stream.
 
 .. index:: AlterForeignServerStmt
 
 .. function:: alter_foreign_server_stmt(node, output)
 
-   Pretty print a `node` of type `AlterForeignServerStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2482>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterForeignServerStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2482>`__ to the `output` stream.
 
 .. index:: AlterUserMappingStmt
 
 .. function:: alter_user_mapping_stmt(node, output)
 
-   Pretty print a `node` of type `AlterUserMappingStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2517>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterUserMappingStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2517>`__ to the `output` stream.
 
 .. index:: AlterRoleSetStmt
 
 .. function:: alter_role_set_stmt(node, output)
 
-   Pretty print a `node` of type `AlterRoleSetStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2698>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterRoleSetStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2698>`__ to the `output` stream.
 
 .. index:: AlterDomainStmt
 
 .. function:: alter_domain_stmt(node, output)
 
-   Pretty print a `node` of type `AlterDomainStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2055>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterDomainStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2055>`__ to the `output` stream.
 
 .. index:: AlterEventTrigStmt
 
 .. function:: alter_event_trig_stmt(node, output)
 
-   Pretty print a `node` of type `AlterEventTrigStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2643>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterEventTrigStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2643>`__ to the `output` stream.
 
 .. index:: AlterTypeStmt
 
 .. function:: alter_type_stmt(node, output)
 
-   Pretty print a `node` of type `AlterTypeStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3187>`__ to the `output` stream.
+   Pretty print a `node` of type `AlterTypeStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3187>`__ to the `output` stream.
 
 .. index:: CheckPointStmt
 
 .. function:: check_point_stmt(node, output)
 
-   Pretty print a `node` of type `CheckPointStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3502>`__ to the `output` stream.
+   Pretty print a `node` of type `CheckPointStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3502>`__ to the `output` stream.
 
 .. index:: ClusterStmt
 
 .. function:: cluster_stmt(node, output)
 
-   Pretty print a `node` of type `ClusterStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3410>`__ to the `output` stream.
+   Pretty print a `node` of type `ClusterStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3410>`__ to the `output` stream.
 
 .. index:: ColumnDef
 
 .. function:: column_def(node, output)
 
-   Pretty print a `node` of type `ColumnDef <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L675>`__ to the `output` stream.
+   Pretty print a `node` of type `ColumnDef <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L675>`__ to the `output` stream.
 
 .. index:: CommentStmt
 
 .. function:: comment_stmt(node, output)
 
-   Pretty print a `node` of type `CommentStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2853>`__ to the `output` stream.
+   Pretty print a `node` of type `CommentStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2853>`__ to the `output` stream.
 
 .. index:: CompositeTypeStmt
 
 .. function:: composite_type_stmt(node, output)
 
-   Pretty print a `node` of type `CompositeTypeStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3273>`__ to the `output` stream.
+   Pretty print a `node` of type `CompositeTypeStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3273>`__ to the `output` stream.
 
 .. index::
    pair: CompositeTypeStmt;RangeVar
 
 .. function:: composite_type_stmt_range_var(node, output)
 
-   Pretty print a `node` of type `RangeVar <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L63>`__, when it is inside a `CompositeTypeStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3273>`__, to the `output` stream.
+   Pretty print a `node` of type `RangeVar <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L63>`__, when it is inside a `CompositeTypeStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3273>`__, to the `output` stream.
 
 .. index:: Constraint
 
 .. function:: constraint(node, output)
 
-   Pretty print a `node` of type `Constraint <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2322>`__ to the `output` stream.
+   Pretty print a `node` of type `Constraint <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2322>`__ to the `output` stream.
 
 .. index:: CreateAmStmt
 
 .. function:: create_am_stmt(node, output)
 
-   Pretty print a `node` of type `CreateAmStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2590>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateAmStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2590>`__ to the `output` stream.
 
 .. index:: CreatedbStmt
 
 .. function:: create_db_stmt(node, output)
 
-   Pretty print a `node` of type `CreatedbStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3353>`__ to the `output` stream.
+   Pretty print a `node` of type `CreatedbStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3353>`__ to the `output` stream.
 
 .. index::
    pair: CreatedbStmt;DefElem
 
 .. function:: create_db_stmt_def_elem(node, output)
 
-   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `CreatedbStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3353>`__, to the `output` stream.
+   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `CreatedbStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3353>`__, to the `output` stream.
 
 .. index:: CreateCastStmt
 
 .. function:: create_cast_stmt(node, output)
 
-   Pretty print a `node` of type `CreateCastStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3590>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateCastStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3590>`__ to the `output` stream.
 
 .. index:: CreateConversionStmt
 
 .. function:: create_conversion_stmt(node, output)
 
-   Pretty print a `node` of type `CreateConversionStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3576>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateConversionStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3576>`__ to the `output` stream.
 
 .. index:: CreateDomainStmt
 
 .. function:: create_domain_stmt(node, output)
 
-   Pretty print a `node` of type `CreateDomainStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2757>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateDomainStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2757>`__ to the `output` stream.
 
 .. index:: CreateEnumStmt
 
 .. function:: create_enum_stmt(node, output)
 
-   Pretty print a `node` of type `CreateEnumStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3284>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateEnumStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3284>`__ to the `output` stream.
 
 .. index:: CreateEventTrigStmt
 
 .. function:: create_event_trig_stmt(node, output)
 
-   Pretty print a `node` of type `CreateEventTrigStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2630>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateEventTrigStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2630>`__ to the `output` stream.
 
 .. index::
    pair: CreateEventTrigStmt;DefElem
 
 .. function:: create_event_trig_stmt_def_elem(node, output)
 
-   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `CreateEventTrigStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2630>`__, to the `output` stream.
+   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `CreateEventTrigStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2630>`__, to the `output` stream.
 
 .. index:: CreateExtensionStmt
 
 .. function:: create_extension_stmt(node, output)
 
-   Pretty print a `node` of type `CreateExtensionStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2420>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateExtensionStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2420>`__ to the `output` stream.
 
 .. index::
    pair: CreateExtensionStmt;DefElem
 
 .. function:: create_extension_stmt_def_elem(node, output)
 
-   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `CreateExtensionStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2420>`__, to the `output` stream.
+   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `CreateExtensionStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2420>`__, to the `output` stream.
 
 .. index:: CreateFdwStmt
 
 .. function:: create_fdw_stmt(node, output)
 
-   Pretty print a `node` of type `CreateFdwStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2450>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateFdwStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2450>`__ to the `output` stream.
 
 .. index::
    pair: ColumnDef;DefElem
 
 .. index::
    pair: CreateUserMappingStmt;DefElem
 
 .. index::
    pair: CreateFdwStmt;DefElem
 
 .. function:: create_fdw_stmt_def_elem(node, output)
 
-   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `ColumnDef <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L675>`__ or a `CreateUserMappingStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2508>`__ or a `CreateFdwStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2450>`__, to the `output` stream.
+   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `ColumnDef <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L675>`__ or a `CreateUserMappingStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2508>`__ or a `CreateFdwStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2450>`__, to the `output` stream.
 
 .. index:: CreateForeignServerStmt
 
 .. function:: create_foreign_server_stmt(node, output)
 
-   Pretty print a `node` of type `CreateForeignServerStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2471>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateForeignServerStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2471>`__ to the `output` stream.
 
 .. index:: CreateForeignTableStmt
 
 .. function:: create_foreign_table_stmt(node, output)
 
-   Pretty print a `node` of type `CreateForeignTableStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2496>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateForeignTableStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2496>`__ to the `output` stream.
 
 .. index::
    pair: CreateForeignTableStmt;DefElem
 
 .. index::
    pair: CreateForeignServerStmt;DefElem
 
 .. function:: create_foreign_table_stmt_def_elem(node, output)
 
-   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `CreateForeignTableStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2496>`__ or a `CreateForeignServerStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2471>`__, to the `output` stream.
+   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `CreateForeignTableStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2496>`__ or a `CreateForeignServerStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2471>`__, to the `output` stream.
 
 .. index:: CreateFunctionStmt
 
 .. function:: create_function_stmt(node, output)
 
-   Pretty print a `node` of type `CreateFunctionStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3028>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateFunctionStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3028>`__ to the `output` stream.
 
 .. index::
    pair: AlterFunctionStmt;DefElem
 
 .. index::
    pair: CreateFunctionStmt;DefElem
 
 .. index::
    pair: DoStmt;DefElem
 
 .. function:: create_function_option(node, output)
 
-   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `AlterFunctionStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3061>`__ or a `CreateFunctionStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3028>`__ or a `DoStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3075>`__, to the `output` stream.
+   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `AlterFunctionStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3061>`__ or a `CreateFunctionStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3028>`__ or a `DoStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3075>`__, to the `output` stream.
 
 .. index:: CreateOpClassStmt
 
 .. function:: create_opclass_stmt(node, output)
 
-   Pretty print a `node` of type `CreateOpClassStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2770>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateOpClassStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2770>`__ to the `output` stream.
 
 .. index:: CreateOpClassItem
 
 .. function:: create_opclass_item(node, output)
 
-   Pretty print a `node` of type `CreateOpClassItem <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2785>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateOpClassItem <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2785>`__ to the `output` stream.
 
 .. index:: CreateOpFamilyStmt
 
 .. function:: create_op_family_stmt(node, output)
 
-   Pretty print a `node` of type `CreateOpFamilyStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2802>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateOpFamilyStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2802>`__ to the `output` stream.
 
 .. index:: CreatePLangStmt
 
 .. function:: create_plang_stmt(node, output)
 
-   Pretty print a `node` of type `CreatePLangStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2655>`__ to the `output` stream.
+   Pretty print a `node` of type `CreatePLangStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2655>`__ to the `output` stream.
 
 .. index:: CreatePolicyStmt
 
 .. function:: create_policy_stmt(node, output)
 
-   Pretty print a `node` of type `CreatePolicyStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2560>`__ to the `output` stream.
+   Pretty print a `node` of type `CreatePolicyStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2560>`__ to the `output` stream.
 
 .. index:: CreatePublicationStmt
 
 .. function:: create_publication_stmt(node, output)
 
-   Pretty print a `node` of type `CreatePublicationStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3739>`__ to the `output` stream.
+   Pretty print a `node` of type `CreatePublicationStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3739>`__ to the `output` stream.
 
 .. index:: CreateRangeStmt
 
 .. function:: create_range_stmt(node, output)
 
-   Pretty print a `node` of type `CreateRangeStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3295>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateRangeStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3295>`__ to the `output` stream.
 
 .. index:: CreateRoleStmt
 
 .. function:: create_role_stmt(node, output)
 
-   Pretty print a `node` of type `CreateRoleStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2682>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateRoleStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2682>`__ to the `output` stream.
 
 .. index::
    pair: AlterRoleStmt;DefElem
 
 .. index::
    pair: CreateRoleStmt;DefElem
 
 .. function:: create_or_alter_role_option(node, output)
 
-   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `AlterRoleStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2690>`__ or a `CreateRoleStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2682>`__, to the `output` stream.
+   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `AlterRoleStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2690>`__ or a `CreateRoleStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2682>`__, to the `output` stream.
 
 .. index:: CreateSchemaStmt
 
 .. function:: create_schema_stmt(node, output)
 
-   Pretty print a `node` of type `CreateSchemaStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1910>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateSchemaStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1910>`__ to the `output` stream.
 
 .. index:: CreateSeqStmt
 
 .. function:: create_seq_stmt(node, output)
 
-   Pretty print a `node` of type `CreateSeqStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2718>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateSeqStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2718>`__ to the `output` stream.
 
 .. index::
    pair: Constraint;DefElem
 
 .. index::
    pair: CreateSeqStmt;DefElem
 
 .. index::
    pair: AlterSeqStmt;DefElem
 
 .. function:: create_seq_stmt_def_elem(node, output)
 
-   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `Constraint <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2322>`__ or a `CreateSeqStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2718>`__ or a `AlterSeqStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2728>`__, to the `output` stream.
+   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `Constraint <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2322>`__ or a `CreateSeqStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2718>`__ or a `AlterSeqStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2728>`__, to the `output` stream.
 
 .. index:: CreateStatsStmt
 
 .. function:: create_stats_stmt(node, output)
 
-   Pretty print a `node` of type `CreateStatsStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2985>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateStatsStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2985>`__ to the `output` stream.
 
 .. index:: CreateStmt
 
 .. function:: create_stmt(node, output)
 
-   Pretty print a `node` of type `CreateStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2242>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2242>`__ to the `output` stream.
 
 .. index:: CreateTableAsStmt
 
 .. function:: create_table_as_stmt(node, output)
 
-   Pretty print a `node` of type `CreateTableAsStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3476>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateTableAsStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3476>`__ to the `output` stream.
 
 .. index:: CreateTableSpaceStmt
 
 .. function:: create_table_space_stmt(node, output)
 
-   Pretty print a `node` of type `CreateTableSpaceStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2381>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateTableSpaceStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2381>`__ to the `output` stream.
 
 .. index:: CreateTrigStmt
 
 .. function:: create_trig_stmt(node, output)
 
-   Pretty print a `node` of type `CreateTrigStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2602>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateTrigStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2602>`__ to the `output` stream.
 
 .. index::
    pair: AlterSubscriptionStmt;DefElem
 
 .. index::
    pair: CreateSubscriptionStmt;DefElem
 
 .. function:: create_subscription_stmt_stmt_def_elem(node, output)
 
-   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `AlterSubscriptionStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3794>`__ or a `CreateSubscriptionStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3773>`__, to the `output` stream.
+   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `AlterSubscriptionStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3794>`__ or a `CreateSubscriptionStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3773>`__, to the `output` stream.
 
 .. index:: CreateSubscriptionStmt
 
 .. function:: create_subscription_stmt(node, output)
 
-   Pretty print a `node` of type `CreateSubscriptionStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3773>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateSubscriptionStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3773>`__ to the `output` stream.
 
 .. index:: CurrentOfExpr
 
 .. function:: current_of_expr(node, output)
 
-   Pretty print a `node` of type `CurrentOfExpr <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1358>`__ to the `output` stream.
+   Pretty print a `node` of type `CurrentOfExpr <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1358>`__ to the `output` stream.
 
 .. index:: CreateTransformStmt
 
 .. function:: create_transform_stmt(node, output)
 
-   Pretty print a `node` of type `CreateTransformStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3604>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateTransformStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3604>`__ to the `output` stream.
 
 .. index:: ClosePortalStmt
 
 .. function:: close_portal_stmt(node, output)
 
-   Pretty print a `node` of type `ClosePortalStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2906>`__ to the `output` stream.
+   Pretty print a `node` of type `ClosePortalStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2906>`__ to the `output` stream.
 
 .. index:: CreateUserMappingStmt
 
 .. function:: create_user_mapping_stmt(node, output)
 
-   Pretty print a `node` of type `CreateUserMappingStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2508>`__ to the `output` stream.
+   Pretty print a `node` of type `CreateUserMappingStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2508>`__ to the `output` stream.
 
 .. index:: DeallocateStmt
 
 .. function:: deallocate_stmt(node, output)
 
-   Pretty print a `node` of type `DeallocateStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3644>`__ to the `output` stream.
+   Pretty print a `node` of type `DeallocateStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3644>`__ to the `output` stream.
 
 .. index:: DefineStmt
 
 .. function:: define_stmt(node, output)
 
-   Pretty print a `node` of type `DefineStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2741>`__ to the `output` stream.
+   Pretty print a `node` of type `DefineStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2741>`__ to the `output` stream.
 
 .. index:: DefElem
 
 .. function:: def_elem(node, output)
 
-   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L762>`__ to the `output` stream.
+   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L762>`__ to the `output` stream.
 
 .. index::
    pair: DefineStmt;DefElem
 
 .. function:: define_stmt_def_elem(node, output)
 
-   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `DefineStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2741>`__, to the `output` stream.
+   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `DefineStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2741>`__, to the `output` stream.
 
 .. index:: DiscardStmt
 
 .. function:: discard_stmt(node, output)
 
-   Pretty print a `node` of type `DiscardStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3520>`__ to the `output` stream.
+   Pretty print a `node` of type `DiscardStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3520>`__ to the `output` stream.
 
 .. index:: DoStmt
 
 .. function:: do_stmt(node, output)
 
-   Pretty print a `node` of type `DoStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3075>`__ to the `output` stream.
+   Pretty print a `node` of type `DoStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3075>`__ to the `output` stream.
 
 .. index:: DropdbStmt
 
 .. function:: drop_db_stmt(node, output)
 
-   Pretty print a `node` of type `DropdbStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3388>`__ to the `output` stream.
+   Pretty print a `node` of type `DropdbStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3388>`__ to the `output` stream.
 
 .. index:: DropOwnedStmt
 
 .. function:: drop_owned_stmt(node, output)
 
-   Pretty print a `node` of type `DropOwnedStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3654>`__ to the `output` stream.
+   Pretty print a `node` of type `DropOwnedStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3654>`__ to the `output` stream.
 
 .. index:: DropRoleStmt
 
 .. function:: drop_role_stmt(node, output)
 
-   Pretty print a `node` of type `DropRoleStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2706>`__ to the `output` stream.
+   Pretty print a `node` of type `DropRoleStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2706>`__ to the `output` stream.
 
 .. index:: DropStmt
 
 .. function:: drop_stmt(node, output)
 
-   Pretty print a `node` of type `DropStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2827>`__ to the `output` stream.
+   Pretty print a `node` of type `DropStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2827>`__ to the `output` stream.
 
 .. index:: DropSubscriptionStmt
 
 .. function:: drop_subscription_stmt(node, output)
 
-   Pretty print a `node` of type `DropSubscriptionStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3804>`__ to the `output` stream.
+   Pretty print a `node` of type `DropSubscriptionStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3804>`__ to the `output` stream.
 
 .. index:: DropTableSpaceStmt
 
 .. function:: drop_table_space_stmt(node, output)
 
-   Pretty print a `node` of type `DropTableSpaceStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2390>`__ to the `output` stream.
+   Pretty print a `node` of type `DropTableSpaceStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2390>`__ to the `output` stream.
 
 .. index:: DropUserMappingStmt
 
 .. function:: drop_user_mapping_stmt(node, output)
 
-   Pretty print a `node` of type `DropUserMappingStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2525>`__ to the `output` stream.
+   Pretty print a `node` of type `DropUserMappingStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2525>`__ to the `output` stream.
 
 .. index:: FunctionParameter
 
 .. function:: function_parameter(node, output)
 
-   Pretty print a `node` of type `FunctionParameter <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3052>`__ to the `output` stream.
+   Pretty print a `node` of type `FunctionParameter <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3052>`__ to the `output` stream.
 
 .. index:: GrantStmt
 
 .. function:: grant_stmt(node, output)
 
-   Pretty print a `node` of type `GrantStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2085>`__ to the `output` stream.
+   Pretty print a `node` of type `GrantStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2085>`__ to the `output` stream.
 
 .. index:: GrantRoleStmt
 
 .. function:: grant_role_stmt(node, output)
 
-   Pretty print a `node` of type `GrantRoleStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2150>`__ to the `output` stream.
+   Pretty print a `node` of type `GrantRoleStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2150>`__ to the `output` stream.
 
 .. index:: ImportForeignSchemaStmt
 
 .. function:: import_foreign_schema_stmt(node, output)
 
-   Pretty print a `node` of type `ImportForeignSchemaStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2545>`__ to the `output` stream.
+   Pretty print a `node` of type `ImportForeignSchemaStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2545>`__ to the `output` stream.
 
 .. index:: IndexStmt
 
 .. function:: index_stmt(node, output)
 
-   Pretty print a `node` of type `IndexStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2949>`__ to the `output` stream.
+   Pretty print a `node` of type `IndexStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2949>`__ to the `output` stream.
 
 .. index:: LoadStmt
 
 .. function:: load_stmt(node, output)
 
-   Pretty print a `node` of type `LoadStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3343>`__ to the `output` stream.
+   Pretty print a `node` of type `LoadStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3343>`__ to the `output` stream.
 
 .. index:: LockStmt
 
 .. function:: lock_stmt(node, output)
 
-   Pretty print a `node` of type `LockStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3530>`__ to the `output` stream.
+   Pretty print a `node` of type `LockStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3530>`__ to the `output` stream.
 
 .. index:: NotifyStmt
 
 .. function:: notify_stmt(node, output)
 
-   Pretty print a `node` of type `NotifyStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3214>`__ to the `output` stream.
+   Pretty print a `node` of type `NotifyStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3214>`__ to the `output` stream.
 
 .. index:: ObjectWithArgs
 
 .. function:: object_with_args(node, output)
 
-   Pretty print a `node` of type `ObjectWithArgs <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2118>`__ to the `output` stream.
+   Pretty print a `node` of type `ObjectWithArgs <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2118>`__ to the `output` stream.
 
 .. index::
    pair: AlterObjectSchemaStmt;ObjectWithArgs
 
 .. function:: alter_object_schema_stmt_object_with_args(node, output)
 
-   Pretty print a `node` of type `ObjectWithArgs <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2118>`__, when it is inside a `AlterObjectSchemaStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3149>`__, to the `output` stream.
+   Pretty print a `node` of type `ObjectWithArgs <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2118>`__, when it is inside a `AlterObjectSchemaStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3149>`__, to the `output` stream.
 
 .. index::
    pair: AlterOperatorStmt;ObjectWithArgs
 
 .. function:: alter_operator_stmt_object_with_args(node, output)
 
-   Pretty print a `node` of type `ObjectWithArgs <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2118>`__, when it is inside a `AlterOperatorStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3176>`__, to the `output` stream.
+   Pretty print a `node` of type `ObjectWithArgs <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2118>`__, when it is inside a `AlterOperatorStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3176>`__, to the `output` stream.
 
 .. index::
    pair: AlterOwnerStmt;ObjectWithArgs
 
 .. function:: alter_owner_stmt_object_with_args(node, output)
 
-   Pretty print a `node` of type `ObjectWithArgs <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2118>`__, when it is inside a `AlterOwnerStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3163>`__, to the `output` stream.
+   Pretty print a `node` of type `ObjectWithArgs <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2118>`__, when it is inside a `AlterOwnerStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3163>`__, to the `output` stream.
 
 .. index::
    pair: CommentStmt;ObjectWithArgs
 
 .. function:: comment_stmt_object_with_args(node, output)
 
-   Pretty print a `node` of type `ObjectWithArgs <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2118>`__, when it is inside a `CommentStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2853>`__, to the `output` stream.
+   Pretty print a `node` of type `ObjectWithArgs <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2118>`__, when it is inside a `CommentStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2853>`__, to the `output` stream.
 
 .. index::
    pair: DropStmt;ObjectWithArgs
 
 .. function:: drop_stmt_object_with_args(node, output)
 
-   Pretty print a `node` of type `ObjectWithArgs <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2118>`__, when it is inside a `DropStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2827>`__, to the `output` stream.
+   Pretty print a `node` of type `ObjectWithArgs <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2118>`__, when it is inside a `DropStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2827>`__, to the `output` stream.
 
 .. index:: PartitionBoundSpec
 
 .. function:: partition_bound_spec(node, output)
 
-   Pretty print a `node` of type `PartitionBoundSpec <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L845>`__ to the `output` stream.
+   Pretty print a `node` of type `PartitionBoundSpec <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L845>`__ to the `output` stream.
 
 .. index:: PartitionCmd
 
 .. function:: partition_cmd(node, output)
 
-   Pretty print a `node` of type `PartitionCmd <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L892>`__ to the `output` stream.
+   Pretty print a `node` of type `PartitionCmd <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L892>`__ to the `output` stream.
 
 .. index:: PartitionElem
 
 .. function:: partition_elem(node, output)
 
-   Pretty print a `node` of type `PartitionElem <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L810>`__ to the `output` stream.
+   Pretty print a `node` of type `PartitionElem <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L810>`__ to the `output` stream.
 
 .. index:: PartitionRangeDatum
 
 .. function:: partition_range_datum(node, output)
 
-   Pretty print a `node` of type `PartitionRangeDatum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L878>`__ to the `output` stream.
+   Pretty print a `node` of type `PartitionRangeDatum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L878>`__ to the `output` stream.
 
 .. index:: PartitionSpec
 
 .. function:: partition_spec(node, output)
 
-   Pretty print a `node` of type `PartitionSpec <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L825>`__ to the `output` stream.
+   Pretty print a `node` of type `PartitionSpec <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L825>`__ to the `output` stream.
 
 .. index:: PublicationObjSpec
 
 .. function:: publication_obj_spec(node, output)
 
-   Pretty print a `node` of type `PublicationObjSpec <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3730>`__ to the `output` stream.
+   Pretty print a `node` of type `PublicationObjSpec <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3730>`__ to the `output` stream.
 
 .. index:: PublicationTable
 
 .. function:: publication_table(node, output)
 
-   Pretty print a `node` of type `PublicationTable <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3710>`__ to the `output` stream.
+   Pretty print a `node` of type `PublicationTable <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3710>`__ to the `output` stream.
 
 .. index:: ReindexStmt
 
 .. function:: reindex_stmt(node, output)
 
-   Pretty print a `node` of type `ReindexStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3562>`__ to the `output` stream.
+   Pretty print a `node` of type `ReindexStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3562>`__ to the `output` stream.
 
 .. index::
    pair: ReindexStmt;DefElem
 
 .. function:: reindex_stmt_def_elem(node, output)
 
-   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `ReindexStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3562>`__, to the `output` stream.
+   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `ReindexStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3562>`__, to the `output` stream.
 
 .. index:: RenameStmt
 
 .. function:: rename_stmt(node, output)
 
-   Pretty print a `node` of type `RenameStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3117>`__ to the `output` stream.
+   Pretty print a `node` of type `RenameStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3117>`__ to the `output` stream.
 
 .. index::
    pair: RenameStmt;RangeVar
 
 .. function:: rename_stmt_range_var(node, output)
 
-   Pretty print a `node` of type `RangeVar <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L63>`__, when it is inside a `RenameStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3117>`__, to the `output` stream.
+   Pretty print a `node` of type `RangeVar <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L63>`__, when it is inside a `RenameStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3117>`__, to the `output` stream.
 
 .. index:: ReplicaIdentityStmt
 
 .. function:: replica_identity_stmt(node, output)
 
-   Pretty print a `node` of type `ReplicaIdentityStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2013>`__ to the `output` stream.
+   Pretty print a `node` of type `ReplicaIdentityStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2013>`__ to the `output` stream.
 
 .. index:: RoleSpec
 
 .. function:: role_spec(node, output)
 
-   Pretty print a `node` of type `RoleSpec <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L356>`__ to the `output` stream.
+   Pretty print a `node` of type `RoleSpec <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L356>`__ to the `output` stream.
 
 .. index:: RuleStmt
 
 .. function:: rule_stmt_printer(node, output)
 
-   Pretty print a `node` of type `RuleStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3198>`__ to the `output` stream.
+   Pretty print a `node` of type `RuleStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3198>`__ to the `output` stream.
 
 .. index:: RefreshMatViewStmt
 
 .. function:: refresh_mat_view_stmt(node, output)
 
-   Pretty print a `node` of type `RefreshMatViewStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3490>`__ to the `output` stream.
+   Pretty print a `node` of type `RefreshMatViewStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3490>`__ to the `output` stream.
 
 .. index:: ReassignOwnedStmt
 
 .. function:: reassign_owned_stmt(node, output)
 
-   Pretty print a `node` of type `ReassignOwnedStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3664>`__ to the `output` stream.
+   Pretty print a `node` of type `ReassignOwnedStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3664>`__ to the `output` stream.
 
 .. index:: ReturnStmt
 
 .. function:: return_stmt(node, output)
 
-   Pretty print a `node` of type `ReturnStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1800>`__ to the `output` stream.
+   Pretty print a `node` of type `ReturnStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1800>`__ to the `output` stream.
 
 .. index:: SecLabelStmt
 
 .. function:: sec_label_stmt(node, output)
 
-   Pretty print a `node` of type `SecLabelStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2865>`__ to the `output` stream.
+   Pretty print a `node` of type `SecLabelStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2865>`__ to the `output` stream.
 
 .. index:: StatsElem
 
 .. function:: stats_elem(node, output)
 
-   Pretty print a `node` of type `StatsElem <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3004>`__ to the `output` stream.
+   Pretty print a `node` of type `StatsElem <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3004>`__ to the `output` stream.
 
 .. index:: TableLikeClause
 
 .. function:: table_like_clause(node, output)
 
-   Pretty print a `node` of type `TableLikeClause <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L702>`__ to the `output` stream.
+   Pretty print a `node` of type `TableLikeClause <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L702>`__ to the `output` stream.
 
 .. index:: TriggerTransition
 
 .. function:: trigger_transition(node, output)
 
-   Pretty print a `node` of type `TriggerTransition <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1590>`__ to the `output` stream.
+   Pretty print a `node` of type `TriggerTransition <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1590>`__ to the `output` stream.
 
 .. index:: VacuumStmt
 
 .. function:: vacuum_stmt(node, output)
 
-   Pretty print a `node` of type `VacuumStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3425>`__ to the `output` stream.
+   Pretty print a `node` of type `VacuumStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3425>`__ to the `output` stream.
 
 .. index::
    pair: VacuumStmt;DefElem
 
 .. function:: vacuum_stmt_def_elem(node, output)
 
-   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `VacuumStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3425>`__, to the `output` stream.
+   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `VacuumStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3425>`__, to the `output` stream.
 
 .. index:: VacuumRelation
 
 .. function:: vacuum_relation(node, output)
 
-   Pretty print a `node` of type `VacuumRelation <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3440>`__ to the `output` stream.
+   Pretty print a `node` of type `VacuumRelation <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3440>`__ to the `output` stream.
 
 .. index:: VariableSetStmt
 
 .. function:: variable_set_stmt(node, output)
 
-   Pretty print a `node` of type `VariableSetStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2212>`__ to the `output` stream.
+   Pretty print a `node` of type `VariableSetStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2212>`__ to the `output` stream.
 
 .. index:: VariableShowStmt
 
 .. function:: variable_show_statement(node, output)
 
-   Pretty print a `node` of type `VariableShowStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2225>`__ to the `output` stream.
+   Pretty print a `node` of type `VariableShowStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2225>`__ to the `output` stream.
 
 .. index:: ViewStmt
 
 .. function:: view_stmt(node, output)
 
-   Pretty print a `node` of type `ViewStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3328>`__ to the `output` stream.
+   Pretty print a `node` of type `ViewStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3328>`__ to the `output` stream.
 
 .. index::
    pair: ViewStmt;DefElem
 
 .. function:: view_stmt_def_elem(node, output)
 
-   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `ViewStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3328>`__, to the `output` stream.
+   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `ViewStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3328>`__, to the `output` stream.
```

### Comparing `pglast-5.2/docs/development.rst` & `pglast-5.3/docs/development.rst`

 * *Files identical despite different names*

### Comparing `pglast-5.2/docs/dml.rst` & `pglast-5.3/docs/dml.rst`

 * *Files 8% similar despite different names*

```diff
@@ -12,530 +12,530 @@
 .. module:: pglast.printers.dml
    :synopsis: DML printer functions
 
 .. index:: A_ArrayExpr
 
 .. function:: a_array_expr(node, output)
 
-   Pretty print a `node` of type `A_ArrayExpr <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L444>`__ to the `output` stream.
+   Pretty print a `node` of type `A_ArrayExpr <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L444>`__ to the `output` stream.
 
 .. index:: A_Const
 
 .. function:: a_const(node, output)
 
-   Pretty print a `node` of type `A_Const <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L301>`__ to the `output` stream.
+   Pretty print a `node` of type `A_Const <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L301>`__ to the `output` stream.
 
 .. index:: A_Expr
 
 .. function:: a_expr(node, output)
 
-   Pretty print a `node` of type `A_Expr <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L288>`__ to the `output` stream.
+   Pretty print a `node` of type `A_Expr <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L288>`__ to the `output` stream.
 
 .. index:: A_Indices
 
 .. function:: a_indices(node, output)
 
-   Pretty print a `node` of type `A_Indices <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L411>`__ to the `output` stream.
+   Pretty print a `node` of type `A_Indices <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L411>`__ to the `output` stream.
 
 .. index:: A_Indirection
 
 .. function:: a_indirection(node, output)
 
-   Pretty print a `node` of type `A_Indirection <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L434>`__ to the `output` stream.
+   Pretty print a `node` of type `A_Indirection <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L434>`__ to the `output` stream.
 
 .. index::
    pair: A_Indirection;A_Star
 
 .. function:: a_indirection_a_star(node, output)
 
-   Pretty print a `node` of type `A_Star <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L400>`__, when it is inside a `A_Indirection <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L434>`__, to the `output` stream.
+   Pretty print a `node` of type `A_Star <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L400>`__, when it is inside a `A_Indirection <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L434>`__, to the `output` stream.
 
 .. index::
    pair: A_Indirection;ColumnRef
 
 .. function:: a_indirection_column_ref(node, output)
 
-   Pretty print a `node` of type `ColumnRef <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L250>`__, when it is inside a `A_Indirection <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L434>`__, to the `output` stream.
+   Pretty print a `node` of type `ColumnRef <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L250>`__, when it is inside a `A_Indirection <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L434>`__, to the `output` stream.
 
 .. index::
    pair: A_Indirection;FuncCall
 
 .. function:: a_indirection_func_call(node, output)
 
-   Pretty print a `node` of type `FuncCall <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L378>`__, when it is inside a `A_Indirection <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L434>`__, to the `output` stream.
+   Pretty print a `node` of type `FuncCall <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L378>`__, when it is inside a `A_Indirection <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L434>`__, to the `output` stream.
 
 .. index::
    pair: A_Indirection;String
 
 .. function:: a_indirection_field(node, output)
 
-   Pretty print a `node` of type `String <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/value.h#L57>`__, when it is inside a `A_Indirection <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L434>`__, to the `output` stream.
+   Pretty print a `node` of type `String <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/value.h#L57>`__, when it is inside a `A_Indirection <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L434>`__, to the `output` stream.
 
 .. index:: A_Star
 
 .. function:: a_star(node, output)
 
-   Pretty print a `node` of type `A_Star <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L400>`__ to the `output` stream.
+   Pretty print a `node` of type `A_Star <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L400>`__ to the `output` stream.
 
 .. index:: Alias
 
 .. function:: alias(node, output)
 
-   Pretty print a `node` of type `Alias <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L39>`__ to the `output` stream.
+   Pretty print a `node` of type `Alias <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L39>`__ to the `output` stream.
 
 .. index:: BitString
 
 .. function:: bitstring(node, output)
 
-   Pretty print a `node` of type `BitString <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/value.h#L63>`__ to the `output` stream.
+   Pretty print a `node` of type `BitString <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/value.h#L63>`__ to the `output` stream.
 
 .. index:: Boolean
 
 .. function:: boolean(node, output)
 
-   Pretty print a `node` of type `Boolean <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/value.h#L51>`__ to the `output` stream.
+   Pretty print a `node` of type `Boolean <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/value.h#L51>`__ to the `output` stream.
 
 .. index:: BoolExpr
 
 .. function:: bool_expr(node, output)
 
-   Pretty print a `node` of type `BoolExpr <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L622>`__ to the `output` stream.
+   Pretty print a `node` of type `BoolExpr <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L622>`__ to the `output` stream.
 
 .. index:: BooleanTest
 
 .. function:: boolean_test(node, output)
 
-   Pretty print a `node` of type `BooleanTest <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1283>`__ to the `output` stream.
+   Pretty print a `node` of type `BooleanTest <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1283>`__ to the `output` stream.
 
 .. index:: CallStmt
 
 .. function:: call_stmt(node, output)
 
-   Pretty print a `node` of type `CallStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3099>`__ to the `output` stream.
+   Pretty print a `node` of type `CallStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3099>`__ to the `output` stream.
 
 .. index:: CaseExpr
 
 .. function:: case_expr(node, output)
 
-   Pretty print a `node` of type `CaseExpr <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L973>`__ to the `output` stream.
+   Pretty print a `node` of type `CaseExpr <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L973>`__ to the `output` stream.
 
 .. index:: CaseWhen
 
 .. function:: case_when(node, output)
 
-   Pretty print a `node` of type `CaseWhen <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L987>`__ to the `output` stream.
+   Pretty print a `node` of type `CaseWhen <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L987>`__ to the `output` stream.
 
 .. index:: CoalesceExpr
 
 .. function:: coalesce_expr(node, output)
 
-   Pretty print a `node` of type `CoalesceExpr <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1125>`__ to the `output` stream.
+   Pretty print a `node` of type `CoalesceExpr <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1125>`__ to the `output` stream.
 
 .. index:: CollateClause
 
 .. function:: collate_clause(node, output)
 
-   Pretty print a `node` of type `CollateClause <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L336>`__ to the `output` stream.
+   Pretty print a `node` of type `CollateClause <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L336>`__ to the `output` stream.
 
 .. index:: ColumnRef
 
 .. function:: column_ref(node, output)
 
-   Pretty print a `node` of type `ColumnRef <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L250>`__ to the `output` stream.
+   Pretty print a `node` of type `ColumnRef <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L250>`__ to the `output` stream.
 
 .. index:: CTECycleClause
 
 .. function:: cte_cycle_clause(node, output)
 
-   Pretty print a `node` of type `CTECycleClause <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1505>`__ to the `output` stream.
+   Pretty print a `node` of type `CTECycleClause <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1505>`__ to the `output` stream.
 
 .. index::
    pair: CTECycleClause;TypeCast
 
 .. function:: cte_cycle_clause_type_cast(node, output)
 
-   Pretty print a `node` of type `TypeCast <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L325>`__, when it is inside a `CTECycleClause <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1505>`__, to the `output` stream.
+   Pretty print a `node` of type `TypeCast <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L325>`__, when it is inside a `CTECycleClause <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1505>`__, to the `output` stream.
 
 .. index:: CTESearchClause
 
 .. function:: cte_search_clause(node, output)
 
-   Pretty print a `node` of type `CTESearchClause <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1496>`__ to the `output` stream.
+   Pretty print a `node` of type `CTESearchClause <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1496>`__ to the `output` stream.
 
 .. index:: CommonTableExpr
 
 .. function:: common_table_expr(node, output)
 
-   Pretty print a `node` of type `CommonTableExpr <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1521>`__ to the `output` stream.
+   Pretty print a `node` of type `CommonTableExpr <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1521>`__ to the `output` stream.
 
 .. index:: ConstraintsSetStmt
 
 .. function:: constraints_set_stmt(node, output)
 
-   Pretty print a `node` of type `ConstraintsSetStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3542>`__ to the `output` stream.
+   Pretty print a `node` of type `ConstraintsSetStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3542>`__ to the `output` stream.
 
 .. index:: CopyStmt
 
 .. function:: copy_stmt(node, output)
 
-   Pretty print a `node` of type `CopyStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2180>`__ to the `output` stream.
+   Pretty print a `node` of type `CopyStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2180>`__ to the `output` stream.
 
 .. index::
    pair: CopyStmt;DefElem
 
 .. function:: copy_stmt_def_elem(node, output)
 
-   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `CopyStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2180>`__, to the `output` stream.
+   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `CopyStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2180>`__, to the `output` stream.
 
 .. index:: DeclareCursorStmt
 
 .. function:: declare_cursor_stmt(node, output)
 
-   Pretty print a `node` of type `DeclareCursorStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2894>`__ to the `output` stream.
+   Pretty print a `node` of type `DeclareCursorStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2894>`__ to the `output` stream.
 
 .. index:: DeleteStmt
 
 .. function:: delete_stmt(node, output)
 
-   Pretty print a `node` of type `DeleteStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1650>`__ to the `output` stream.
+   Pretty print a `node` of type `DeleteStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1650>`__ to the `output` stream.
 
 .. index:: ExecuteStmt
 
 .. function:: execute_stmt(node, output)
 
-   Pretty print a `node` of type `ExecuteStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3632>`__ to the `output` stream.
+   Pretty print a `node` of type `ExecuteStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3632>`__ to the `output` stream.
 
 .. index:: ExplainStmt
 
 .. function:: explain_stmt(node, output)
 
-   Pretty print a `node` of type `ExplainStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3456>`__ to the `output` stream.
+   Pretty print a `node` of type `ExplainStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3456>`__ to the `output` stream.
 
 .. index::
    pair: ExplainStmt;DefElem
 
 .. function:: explain_stmt_def_elem(node, output)
 
-   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `ExplainStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3456>`__, to the `output` stream.
+   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `ExplainStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3456>`__, to the `output` stream.
 
 .. index:: FetchStmt
 
 .. function:: fetch_stmt(node, output)
 
-   Pretty print a `node` of type `FetchStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2929>`__ to the `output` stream.
+   Pretty print a `node` of type `FetchStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2929>`__ to the `output` stream.
 
 .. index:: Float
 
 .. function:: float(node, output)
 
-   Pretty print a `node` of type `Float <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/value.h#L45>`__ to the `output` stream.
+   Pretty print a `node` of type `Float <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/value.h#L45>`__ to the `output` stream.
 
 .. index:: FuncCall
 
 .. function:: func_call(node, output)
 
-   Pretty print a `node` of type `FuncCall <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L378>`__ to the `output` stream.
+   Pretty print a `node` of type `FuncCall <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L378>`__ to the `output` stream.
 
 .. index::
    pair: FuncCall;WindowDef
 
 .. function:: func_call_window_def(node, output)
 
-   Pretty print a `node` of type `WindowDef <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L516>`__, when it is inside a `FuncCall <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L378>`__, to the `output` stream.
+   Pretty print a `node` of type `WindowDef <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L516>`__, when it is inside a `FuncCall <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L378>`__, to the `output` stream.
 
 .. index:: GroupingSet
 
 .. function:: grouping_set(node, output)
 
-   Pretty print a `node` of type `GroupingSet <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1372>`__ to the `output` stream.
+   Pretty print a `node` of type `GroupingSet <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1372>`__ to the `output` stream.
 
 .. index:: GroupingFunc
 
 .. function:: grouping_func(node, output)
 
-   Pretty print a `node` of type `GroupingFunc <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L369>`__ to the `output` stream.
+   Pretty print a `node` of type `GroupingFunc <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L369>`__ to the `output` stream.
 
 .. index:: IndexElem
 
 .. function:: index_elem(node, output)
 
-   Pretty print a `node` of type `IndexElem <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L731>`__ to the `output` stream.
+   Pretty print a `node` of type `IndexElem <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L731>`__ to the `output` stream.
 
 .. index:: InferClause
 
 .. function:: infer_clause(node, output)
 
-   Pretty print a `node` of type `InferClause <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1459>`__ to the `output` stream.
+   Pretty print a `node` of type `InferClause <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1459>`__ to the `output` stream.
 
 .. index:: Integer
 
 .. function:: integer(node, output)
 
-   Pretty print a `node` of type `Integer <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/value.h#L28>`__ to the `output` stream.
+   Pretty print a `node` of type `Integer <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/value.h#L28>`__ to the `output` stream.
 
 .. index:: InsertStmt
 
 .. function:: insert_stmt(node, output)
 
-   Pretty print a `node` of type `InsertStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1634>`__ to the `output` stream.
+   Pretty print a `node` of type `InsertStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1634>`__ to the `output` stream.
 
 .. index:: IntoClause
 
 .. function:: into_clause(node, output)
 
-   Pretty print a `node` of type `IntoClause <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L108>`__ to the `output` stream.
+   Pretty print a `node` of type `IntoClause <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L108>`__ to the `output` stream.
 
 .. index:: JoinExpr
 
 .. function:: join_expr(node, output)
 
-   Pretty print a `node` of type `JoinExpr <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1536>`__ to the `output` stream.
+   Pretty print a `node` of type `JoinExpr <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1536>`__ to the `output` stream.
 
 .. index:: LockingClause
 
 .. function:: locking_clause(node, output)
 
-   Pretty print a `node` of type `LockingClause <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L782>`__ to the `output` stream.
+   Pretty print a `node` of type `LockingClause <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L782>`__ to the `output` stream.
 
 .. index:: ListenStmt
 
 .. function:: listen_stmt(node, output)
 
-   Pretty print a `node` of type `ListenStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3225>`__ to the `output` stream.
+   Pretty print a `node` of type `ListenStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3225>`__ to the `output` stream.
 
 .. index:: MergeStmt
 
 .. function:: merge_stmt(node, output)
 
-   Pretty print a `node` of type `MergeStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1679>`__ to the `output` stream.
+   Pretty print a `node` of type `MergeStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1679>`__ to the `output` stream.
 
 .. index:: MergeWhenClause
 
 .. function:: merge_when_clause(node, output)
 
-   Pretty print a `node` of type `MergeWhenClause <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1555>`__ to the `output` stream.
+   Pretty print a `node` of type `MergeWhenClause <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1555>`__ to the `output` stream.
 
 .. index:: MinMaxExpr
 
 .. function:: min_max_expr(node, output)
 
-   Pretty print a `node` of type `MinMaxExpr <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1143>`__ to the `output` stream.
+   Pretty print a `node` of type `MinMaxExpr <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1143>`__ to the `output` stream.
 
 .. index:: MultiAssignRef
 
 .. function:: multi_assign_ref(node, output)
 
-   Pretty print a `node` of type `MultiAssignRef <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L487>`__ to the `output` stream.
+   Pretty print a `node` of type `MultiAssignRef <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L487>`__ to the `output` stream.
 
 .. index:: NamedArgExpr
 
 .. function:: named_arg_expr(node, output)
 
-   Pretty print a `node` of type `NamedArgExpr <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L521>`__ to the `output` stream.
+   Pretty print a `node` of type `NamedArgExpr <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L521>`__ to the `output` stream.
 
 .. index:: NullTest
 
 .. function:: null_test(node, output)
 
-   Pretty print a `node` of type `NullTest <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1260>`__ to the `output` stream.
+   Pretty print a `node` of type `NullTest <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1260>`__ to the `output` stream.
 
 .. index:: ParamRef
 
 .. function:: param_ref(node, output)
 
-   Pretty print a `node` of type `ParamRef <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L260>`__ to the `output` stream.
+   Pretty print a `node` of type `ParamRef <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L260>`__ to the `output` stream.
 
 .. index:: PrepareStmt
 
 .. function:: prepare_stmt(node, output)
 
-   Pretty print a `node` of type `PrepareStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3618>`__ to the `output` stream.
+   Pretty print a `node` of type `PrepareStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3618>`__ to the `output` stream.
 
 .. index:: OnConflictClause
 
 .. function:: on_conflict_clause(node, output)
 
-   Pretty print a `node` of type `OnConflictClause <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1474>`__ to the `output` stream.
+   Pretty print a `node` of type `OnConflictClause <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1474>`__ to the `output` stream.
 
 .. index:: RangeFunction
 
 .. function:: range_function(node, output)
 
-   Pretty print a `node` of type `RangeFunction <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L592>`__ to the `output` stream.
+   Pretty print a `node` of type `RangeFunction <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L592>`__ to the `output` stream.
 
 .. index:: RangeSubselect
 
 .. function:: range_subselect(node, output)
 
-   Pretty print a `node` of type `RangeSubselect <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L570>`__ to the `output` stream.
+   Pretty print a `node` of type `RangeSubselect <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L570>`__ to the `output` stream.
 
 .. index:: RangeTableFunc
 
 .. function:: range_table_func(node, output)
 
-   Pretty print a `node` of type `RangeTableFunc <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L607>`__ to the `output` stream.
+   Pretty print a `node` of type `RangeTableFunc <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L607>`__ to the `output` stream.
 
 .. index::
    pair: RangeTableFunc;ResTarget
 
 .. function:: range_table_func_res_target(node, output)
 
-   Pretty print a `node` of type `ResTarget <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L469>`__, when it is inside a `RangeTableFunc <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L607>`__, to the `output` stream.
+   Pretty print a `node` of type `ResTarget <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L469>`__, when it is inside a `RangeTableFunc <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L607>`__, to the `output` stream.
 
 .. index:: RangeTableFuncCol
 
 .. function:: range_table_func_col(node, output)
 
-   Pretty print a `node` of type `RangeTableFuncCol <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L625>`__ to the `output` stream.
+   Pretty print a `node` of type `RangeTableFuncCol <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L625>`__ to the `output` stream.
 
 .. index:: RangeVar
 
 .. function:: range_var(node, output)
 
-   Pretty print a `node` of type `RangeVar <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L63>`__ to the `output` stream.
+   Pretty print a `node` of type `RangeVar <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L63>`__ to the `output` stream.
 
 .. index:: RangeTableSample
 
 .. function:: range_table_sample(node, output)
 
-   Pretty print a `node` of type `RangeTableSample <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L647>`__ to the `output` stream.
+   Pretty print a `node` of type `RangeTableSample <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L647>`__ to the `output` stream.
 
 .. index:: RawStmt
 
 .. function:: raw_stmt(node, output)
 
-   Pretty print a `node` of type `RawStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1614>`__ to the `output` stream.
+   Pretty print a `node` of type `RawStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1614>`__ to the `output` stream.
 
 .. index:: ResTarget
 
 .. function:: res_target(node, output)
 
-   Pretty print a `node` of type `ResTarget <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L469>`__ to the `output` stream.
+   Pretty print a `node` of type `ResTarget <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L469>`__ to the `output` stream.
 
 .. index:: RowExpr
 
 .. function:: row_expr(node, output)
 
-   Pretty print a `node` of type `RowExpr <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1063>`__ to the `output` stream.
+   Pretty print a `node` of type `RowExpr <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1063>`__ to the `output` stream.
 
 .. index:: SelectStmt
 
 .. function:: select_stmt(node, output)
 
-   Pretty print a `node` of type `SelectStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1710>`__ to the `output` stream.
+   Pretty print a `node` of type `SelectStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1710>`__ to the `output` stream.
 
 .. index:: SetToDefault
 
 .. function:: set_to_default(node, output)
 
-   Pretty print a `node` of type `SetToDefault <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1336>`__ to the `output` stream.
+   Pretty print a `node` of type `SetToDefault <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1336>`__ to the `output` stream.
 
 .. index:: SortBy
 
 .. function:: sort_by(node, output)
 
-   Pretty print a `node` of type `SortBy <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L498>`__ to the `output` stream.
+   Pretty print a `node` of type `SortBy <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L498>`__ to the `output` stream.
 
 .. index:: SQLValueFunction
 
 .. function:: sql_value_function(node, output)
 
-   Pretty print a `node` of type `SQLValueFunction <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1184>`__ to the `output` stream.
+   Pretty print a `node` of type `SQLValueFunction <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1184>`__ to the `output` stream.
 
 .. index:: String
 
 .. function:: string(node, output)
 
-   Pretty print a `node` of type `String <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/value.h#L57>`__ to the `output` stream.
+   Pretty print a `node` of type `String <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/value.h#L57>`__ to the `output` stream.
 
 .. index:: SubLink
 
 .. function:: sub_link(node, output)
 
-   Pretty print a `node` of type `SubLink <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L694>`__ to the `output` stream.
+   Pretty print a `node` of type `SubLink <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L694>`__ to the `output` stream.
 
 .. index:: TransactionStmt
 
 .. function:: transaction_stmt(node, output)
 
-   Pretty print a `node` of type `TransactionStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3259>`__ to the `output` stream.
+   Pretty print a `node` of type `TransactionStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3259>`__ to the `output` stream.
 
 .. index::
    pair: TransactionStmt;DefElem
 
 .. function:: transaction_stmt_def_elem(node, output)
 
-   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `TransactionStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3259>`__, to the `output` stream.
+   Pretty print a `node` of type `DefElem <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L762>`__, when it is inside a `TransactionStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3259>`__, to the `output` stream.
 
 .. index:: TruncateStmt
 
 .. function:: truncate_stmt(node, output)
 
-   Pretty print a `node` of type `TruncateStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2841>`__ to the `output` stream.
+   Pretty print a `node` of type `TruncateStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2841>`__ to the `output` stream.
 
 .. index:: TypeCast
 
 .. function:: type_cast(node, output)
 
-   Pretty print a `node` of type `TypeCast <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L325>`__ to the `output` stream.
+   Pretty print a `node` of type `TypeCast <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L325>`__ to the `output` stream.
 
 .. index:: TypeName
 
 .. function:: type_name(node, output)
 
-   Pretty print a `node` of type `TypeName <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L224>`__ to the `output` stream.
+   Pretty print a `node` of type `TypeName <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L224>`__ to the `output` stream.
 
 .. index::
    pair: VariableSetStmt;TypeCast
 
 .. function:: variable_set_stmt_type_cast(node, output)
 
-   Pretty print a `node` of type `TypeCast <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L325>`__, when it is inside a `VariableSetStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2212>`__, to the `output` stream.
+   Pretty print a `node` of type `TypeCast <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L325>`__, when it is inside a `VariableSetStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2212>`__, to the `output` stream.
 
 .. index:: UpdateStmt
 
 .. function:: update_stmt(node, output)
 
-   Pretty print a `node` of type `UpdateStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1664>`__ to the `output` stream.
+   Pretty print a `node` of type `UpdateStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1664>`__ to the `output` stream.
 
 .. index:: UnlistenStmt
 
 .. function:: unlisten_stmt(node, output)
 
-   Pretty print a `node` of type `UnlistenStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3235>`__ to the `output` stream.
+   Pretty print a `node` of type `UnlistenStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3235>`__ to the `output` stream.
 
 .. index:: WithClause
 
 .. function:: with_clause(node, output)
 
-   Pretty print a `node` of type `WithClause <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1445>`__ to the `output` stream.
+   Pretty print a `node` of type `WithClause <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1445>`__ to the `output` stream.
 
 .. index:: WindowDef
 
 .. function:: window_def(node, output)
 
-   Pretty print a `node` of type `WindowDef <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L516>`__ to the `output` stream.
+   Pretty print a `node` of type `WindowDef <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L516>`__ to the `output` stream.
 
 .. index::
    pair: MergeWhenClause;ResTarget
 
 .. index::
    pair: OnConflictClause;ResTarget
 
 .. index::
    pair: UpdateStmt;ResTarget
 
 .. function:: update_stmt_res_target(node, output)
 
-   Pretty print a `node` of type `ResTarget <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L469>`__, when it is inside a `MergeWhenClause <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1555>`__ or a `OnConflictClause <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1474>`__ or a `UpdateStmt <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1664>`__, to the `output` stream.
+   Pretty print a `node` of type `ResTarget <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L469>`__, when it is inside a `MergeWhenClause <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1555>`__ or a `OnConflictClause <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1474>`__ or a `UpdateStmt <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1664>`__, to the `output` stream.
 
 .. index:: XmlExpr
 
 .. function:: xml_expr(node, output)
 
-   Pretty print a `node` of type `XmlExpr <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1222>`__ to the `output` stream.
+   Pretty print a `node` of type `XmlExpr <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1222>`__ to the `output` stream.
 
 .. index:: XmlSerialize
 
 .. function:: xml_serialize(node, output)
 
-   Pretty print a `node` of type `XmlSerialize <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L793>`__ to the `output` stream.
+   Pretty print a `node` of type `XmlSerialize <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L793>`__ to the `output` stream.
```

### Comparing `pglast-5.2/docs/enums.rst` & `pglast-5.3/docs/enums.rst`

 * *Files identical despite different names*

### Comparing `pglast-5.2/docs/index.rst` & `pglast-5.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pglast-5.2/docs/installation.rst` & `pglast-5.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pglast-5.2/docs/introduction.rst` & `pglast-5.3/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `pglast-5.2/docs/keywords.rst` & `pglast-5.3/docs/keywords.rst`

 * *Files identical despite different names*

### Comparing `pglast-5.2/docs/lockdefs.rst` & `pglast-5.3/docs/lockdefs.rst`

 * *Files 12% similar despite different names*

```diff
@@ -5,52 +5,52 @@
 .. :Copyright: © 2017-2023 Lele Gaifax
 ..
 
 ==========================================================================
  :mod:`pglast.enums.lockdefs` --- Constants extracted from `lockdefs.h`__
 ==========================================================================
 
-__ https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/storage/lockdefs.h
+__ https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/storage/lockdefs.h
 
 .. module:: pglast.enums.lockdefs
    :synopsis: Constants extracted from lockdefs.h
 
 
 .. data:: NoLock
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/storage/lockdefs.h#L34>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/storage/lockdefs.h#L34>`__.
 
 .. data:: AccessShareLock
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/storage/lockdefs.h#L36>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/storage/lockdefs.h#L36>`__.
 
 .. data:: RowShareLock
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/storage/lockdefs.h#L37>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/storage/lockdefs.h#L37>`__.
 
 .. data:: RowExclusiveLock
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/storage/lockdefs.h#L38>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/storage/lockdefs.h#L38>`__.
 
 .. data:: ShareUpdateExclusiveLock
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/storage/lockdefs.h#L39>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/storage/lockdefs.h#L39>`__.
 
 .. data:: ShareLock
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/storage/lockdefs.h#L41>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/storage/lockdefs.h#L41>`__.
 
 .. data:: ShareRowExclusiveLock
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/storage/lockdefs.h#L42>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/storage/lockdefs.h#L42>`__.
 
 .. data:: ExclusiveLock
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/storage/lockdefs.h#L44>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/storage/lockdefs.h#L44>`__.
 
 .. data:: AccessExclusiveLock
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/storage/lockdefs.h#L45>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/storage/lockdefs.h#L45>`__.
 
 .. data:: MaxLockMode
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/storage/lockdefs.h#L48>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/storage/lockdefs.h#L48>`__.
```

### Comparing `pglast-5.2/docs/lockoptions.rst` & `pglast-5.3/docs/lockoptions.rst`

 * *Files 16% similar despite different names*

```diff
@@ -5,50 +5,50 @@
 .. :Copyright: © 2017-2023 Lele Gaifax
 ..
 
 ================================================================================
  :mod:`pglast.enums.lockoptions` --- Constants extracted from `lockoptions.h`__
 ================================================================================
 
-__ https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/lockoptions.h
+__ https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/lockoptions.h
 
 .. module:: pglast.enums.lockoptions
    :synopsis: Constants extracted from lockoptions.h
 
 
 .. class:: pglast.enums.lockoptions.LockClauseStrength
 
-   Corresponds to the `LockClauseStrength enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/lockoptions.h#L21>`__.
+   Corresponds to the `LockClauseStrength enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/lockoptions.h#L21>`__.
 
    .. data:: LCS_NONE
 
    .. data:: LCS_FORKEYSHARE
 
    .. data:: LCS_FORSHARE
 
    .. data:: LCS_FORNOKEYUPDATE
 
    .. data:: LCS_FORUPDATE
 
 
 .. class:: pglast.enums.lockoptions.LockTupleMode
 
-   Corresponds to the `LockTupleMode enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/lockoptions.h#L49>`__.
+   Corresponds to the `LockTupleMode enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/lockoptions.h#L49>`__.
 
    .. data:: LockTupleKeyShare
 
    .. data:: LockTupleShare
 
    .. data:: LockTupleNoKeyExclusive
 
    .. data:: LockTupleExclusive
 
 
 .. class:: pglast.enums.lockoptions.LockWaitPolicy
 
-   Corresponds to the `LockWaitPolicy enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/lockoptions.h#L36>`__.
+   Corresponds to the `LockWaitPolicy enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/lockoptions.h#L36>`__.
 
    .. data:: LockWaitBlock
 
    .. data:: LockWaitSkip
 
    .. data:: LockWaitError
```

### Comparing `pglast-5.2/docs/nodes.rst` & `pglast-5.3/docs/nodes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -5,47 +5,47 @@
 .. :Copyright: © 2017-2023 Lele Gaifax
 ..
 
 ====================================================================
  :mod:`pglast.enums.nodes` --- Constants extracted from `nodes.h`__
 ====================================================================
 
-__ https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/nodes.h
+__ https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/nodes.h
 
 .. module:: pglast.enums.nodes
    :synopsis: Constants extracted from nodes.h
 
 
 .. class:: pglast.enums.nodes.AggSplit
 
-   Corresponds to the `AggSplit enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/nodes.h#L799>`__.
+   Corresponds to the `AggSplit enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/nodes.h#L799>`__.
 
    .. data:: AGGSPLIT_SIMPLE
 
    .. data:: AGGSPLIT_INITIAL_SERIAL
 
    .. data:: AGGSPLIT_FINAL_DESERIAL
 
 
 .. class:: pglast.enums.nodes.AggStrategy
 
-   Corresponds to the `AggStrategy enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/nodes.h#L777>`__.
+   Corresponds to the `AggStrategy enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/nodes.h#L777>`__.
 
    .. data:: AGG_PLAIN
 
    .. data:: AGG_SORTED
 
    .. data:: AGG_HASHED
 
    .. data:: AGG_MIXED
 
 
 .. class:: pglast.enums.nodes.CmdType
 
-   Corresponds to the `CmdType enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/nodes.h#L690>`__.
+   Corresponds to the `CmdType enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/nodes.h#L690>`__.
 
    .. data:: CMD_UNKNOWN
 
    .. data:: CMD_SELECT
 
    .. data:: CMD_UPDATE
 
@@ -58,15 +58,15 @@
    .. data:: CMD_UTILITY
 
    .. data:: CMD_NOTHING
 
 
 .. class:: pglast.enums.nodes.JoinType
 
-   Corresponds to the `JoinType enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/nodes.h#L715>`__.
+   Corresponds to the `JoinType enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/nodes.h#L715>`__.
 
    .. data:: JOIN_INNER
 
    .. data:: JOIN_LEFT
 
    .. data:: JOIN_FULL
 
@@ -79,26 +79,26 @@
    .. data:: JOIN_UNIQUE_OUTER
 
    .. data:: JOIN_UNIQUE_INNER
 
 
 .. class:: pglast.enums.nodes.LimitOption
 
-   Corresponds to the `LimitOption enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/nodes.h#L854>`__.
+   Corresponds to the `LimitOption enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/nodes.h#L854>`__.
 
    .. data:: LIMIT_OPTION_DEFAULT
 
    .. data:: LIMIT_OPTION_COUNT
 
    .. data:: LIMIT_OPTION_WITH_TIES
 
 
 .. class:: pglast.enums.nodes.NodeTag
 
-   Corresponds to the `NodeTag enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/nodes.h#L26>`__.
+   Corresponds to the `NodeTag enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/nodes.h#L26>`__.
 
    .. data:: T_Invalid
 
    .. data:: T_IndexInfo
 
    .. data:: T_ExprContext
 
@@ -971,53 +971,53 @@
    .. data:: T_SupportRequestIndexCondition
 
    .. data:: T_SupportRequestWFuncMonotonic
 
 
 .. class:: pglast.enums.nodes.OnConflictAction
 
-   Corresponds to the `OnConflictAction enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/nodes.h#L841>`__.
+   Corresponds to the `OnConflictAction enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/nodes.h#L841>`__.
 
    .. data:: ONCONFLICT_NONE
 
    .. data:: ONCONFLICT_NOTHING
 
    .. data:: ONCONFLICT_UPDATE
 
 
 .. class:: pglast.enums.nodes.SetOpCmd
 
-   Corresponds to the `SetOpCmd enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/nodes.h#L821>`__.
+   Corresponds to the `SetOpCmd enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/nodes.h#L821>`__.
 
    .. data:: SETOPCMD_INTERSECT
 
    .. data:: SETOPCMD_INTERSECT_ALL
 
    .. data:: SETOPCMD_EXCEPT
 
    .. data:: SETOPCMD_EXCEPT_ALL
 
 
 .. class:: pglast.enums.nodes.SetOpStrategy
 
-   Corresponds to the `SetOpStrategy enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/nodes.h#L829>`__.
+   Corresponds to the `SetOpStrategy enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/nodes.h#L829>`__.
 
    .. data:: SETOP_SORTED
 
    .. data:: SETOP_HASHED
 
 
 .. data:: AGGSPLITOP_COMBINE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/nodes.h#L793>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/nodes.h#L793>`__.
 
 .. data:: AGGSPLITOP_SKIPFINAL
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/nodes.h#L794>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/nodes.h#L794>`__.
 
 .. data:: AGGSPLITOP_SERIALIZE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/nodes.h#L795>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/nodes.h#L795>`__.
 
 .. data:: AGGSPLITOP_DESERIALIZE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/nodes.h#L796>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/nodes.h#L796>`__.
```

### Comparing `pglast-5.2/docs/parsenodes.rst` & `pglast-5.3/docs/parsenodes.rst`

 * *Files 6% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 .. :Copyright: © 2017-2023 Lele Gaifax
 ..
 
 ==============================================================================
  :mod:`pglast.enums.parsenodes` --- Constants extracted from `parsenodes.h`__
 ==============================================================================
 
-__ https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h
+__ https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h
 
 .. module:: pglast.enums.parsenodes
    :synopsis: Constants extracted from parsenodes.h
 
 
 .. class:: pglast.enums.parsenodes.A_Expr_Kind
 
-   Corresponds to the `A_Expr_Kind enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L270>`__.
+   Corresponds to the `A_Expr_Kind enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L270>`__.
 
    .. data:: AEXPR_OP
 
    .. data:: AEXPR_OP_ANY
 
    .. data:: AEXPR_OP_ALL
 
@@ -46,26 +46,26 @@
    .. data:: AEXPR_BETWEEN_SYM
 
    .. data:: AEXPR_NOT_BETWEEN_SYM
 
 
 .. class:: pglast.enums.parsenodes.AlterPublicationAction
 
-   Corresponds to the `AlterPublicationAction enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3748>`__.
+   Corresponds to the `AlterPublicationAction enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3748>`__.
 
    .. data:: AP_AddObjects
 
    .. data:: AP_DropObjects
 
    .. data:: AP_SetObjects
 
 
 .. class:: pglast.enums.parsenodes.AlterSubscriptionType
 
-   Corresponds to the `AlterSubscriptionType enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3782>`__.
+   Corresponds to the `AlterSubscriptionType enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3782>`__.
 
    .. data:: ALTER_SUBSCRIPTION_OPTIONS
 
    .. data:: ALTER_SUBSCRIPTION_CONNECTION
 
    .. data:: ALTER_SUBSCRIPTION_SET_PUBLICATION
 
@@ -78,30 +78,30 @@
    .. data:: ALTER_SUBSCRIPTION_ENABLED
 
    .. data:: ALTER_SUBSCRIPTION_SKIP
 
 
 .. class:: pglast.enums.parsenodes.AlterTSConfigType
 
-   Corresponds to the `AlterTSConfigType enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3684>`__.
+   Corresponds to the `AlterTSConfigType enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3684>`__.
 
    .. data:: ALTER_TSCONFIG_ADD_MAPPING
 
    .. data:: ALTER_TSCONFIG_ALTER_MAPPING_FOR_TOKEN
 
    .. data:: ALTER_TSCONFIG_REPLACE_DICT
 
    .. data:: ALTER_TSCONFIG_REPLACE_DICT_FOR_TOKEN
 
    .. data:: ALTER_TSCONFIG_DROP_MAPPING
 
 
 .. class:: pglast.enums.parsenodes.AlterTableType
 
-   Corresponds to the `AlterTableType enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1938>`__.
+   Corresponds to the `AlterTableType enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1938>`__.
 
    .. data:: AT_AddColumn
 
    .. data:: AT_AddColumnRecurse
 
    .. data:: AT_AddColumnToView
 
@@ -240,26 +240,26 @@
    .. data:: AT_DropIdentity
 
    .. data:: AT_ReAddStatistics
 
 
 .. class:: pglast.enums.parsenodes.CTEMaterialize
 
-   Corresponds to the `CTEMaterialize enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1489>`__.
+   Corresponds to the `CTEMaterialize enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1489>`__.
 
    .. data:: CTEMaterializeDefault
 
    .. data:: CTEMaterializeAlways
 
    .. data:: CTEMaterializeNever
 
 
 .. class:: pglast.enums.parsenodes.ConstrType
 
-   Corresponds to the `ConstrType enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2291>`__.
+   Corresponds to the `ConstrType enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2291>`__.
 
    .. data:: CONSTR_NULL
 
    .. data:: CONSTR_NOTNULL
 
    .. data:: CONSTR_DEFAULT
 
@@ -284,63 +284,63 @@
    .. data:: CONSTR_ATTR_DEFERRED
 
    .. data:: CONSTR_ATTR_IMMEDIATE
 
 
 .. class:: pglast.enums.parsenodes.DefElemAction
 
-   Corresponds to the `DefElemAction enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L754>`__.
+   Corresponds to the `DefElemAction enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L754>`__.
 
    .. data:: DEFELEM_UNSPEC
 
    .. data:: DEFELEM_SET
 
    .. data:: DEFELEM_ADD
 
    .. data:: DEFELEM_DROP
 
 
 .. class:: pglast.enums.parsenodes.DiscardMode
 
-   Corresponds to the `DiscardMode enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3512>`__.
+   Corresponds to the `DiscardMode enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3512>`__.
 
    .. data:: DISCARD_ALL
 
    .. data:: DISCARD_PLANS
 
    .. data:: DISCARD_SEQUENCES
 
    .. data:: DISCARD_TEMP
 
 
 .. class:: pglast.enums.parsenodes.DropBehavior
 
-   Corresponds to the `DropBehavior enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1919>`__.
+   Corresponds to the `DropBehavior enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1919>`__.
 
    .. data:: DROP_RESTRICT
 
    .. data:: DROP_CASCADE
 
 
 .. class:: pglast.enums.parsenodes.FetchDirection
 
-   Corresponds to the `FetchDirection enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2917>`__.
+   Corresponds to the `FetchDirection enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2917>`__.
 
    .. data:: FETCH_FORWARD
 
    .. data:: FETCH_BACKWARD
 
    .. data:: FETCH_ABSOLUTE
 
    .. data:: FETCH_RELATIVE
 
 
 .. class:: pglast.enums.parsenodes.FunctionParameterMode
 
-   Corresponds to the `FunctionParameterMode enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3040>`__.
+   Corresponds to the `FunctionParameterMode enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3040>`__.
 
    .. data:: FUNC_PARAM_IN
 
    .. data:: FUNC_PARAM_OUT
 
    .. data:: FUNC_PARAM_INOUT
 
@@ -349,52 +349,52 @@
    .. data:: FUNC_PARAM_TABLE
 
    .. data:: FUNC_PARAM_DEFAULT
 
 
 .. class:: pglast.enums.parsenodes.GrantTargetType
 
-   Corresponds to the `GrantTargetType enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2078>`__.
+   Corresponds to the `GrantTargetType enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2078>`__.
 
    .. data:: ACL_TARGET_OBJECT
 
    .. data:: ACL_TARGET_ALL_IN_SCHEMA
 
    .. data:: ACL_TARGET_DEFAULTS
 
 
 .. class:: pglast.enums.parsenodes.GroupingSetKind
 
-   Corresponds to the `GroupingSetKind enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1363>`__.
+   Corresponds to the `GroupingSetKind enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1363>`__.
 
    .. data:: GROUPING_SET_EMPTY
 
    .. data:: GROUPING_SET_SIMPLE
 
    .. data:: GROUPING_SET_ROLLUP
 
    .. data:: GROUPING_SET_CUBE
 
    .. data:: GROUPING_SET_SETS
 
 
 .. class:: pglast.enums.parsenodes.ImportForeignSchemaType
 
-   Corresponds to the `ImportForeignSchemaType enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2538>`__.
+   Corresponds to the `ImportForeignSchemaType enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2538>`__.
 
    .. data:: FDW_IMPORT_SCHEMA_ALL
 
    .. data:: FDW_IMPORT_SCHEMA_LIMIT_TO
 
    .. data:: FDW_IMPORT_SCHEMA_EXCEPT
 
 
 .. class:: pglast.enums.parsenodes.ObjectType
 
-   Corresponds to the `ObjectType enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1846>`__.
+   Corresponds to the `ObjectType enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1846>`__.
 
    .. data:: OBJECT_ACCESS_METHOD
 
    .. data:: OBJECT_AGGREGATE
 
    .. data:: OBJECT_AMOP
 
@@ -495,65 +495,65 @@
    .. data:: OBJECT_USER_MAPPING
 
    .. data:: OBJECT_VIEW
 
 
 .. class:: pglast.enums.parsenodes.OverridingKind
 
-   Corresponds to the `OverridingKind enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L32>`__.
+   Corresponds to the `OverridingKind enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L32>`__.
 
    .. data:: OVERRIDING_NOT_SET
 
    .. data:: OVERRIDING_USER_VALUE
 
    .. data:: OVERRIDING_SYSTEM_VALUE
 
 
 .. class:: pglast.enums.parsenodes.PartitionRangeDatumKind
 
-   Corresponds to the `PartitionRangeDatumKind enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L871>`__.
+   Corresponds to the `PartitionRangeDatumKind enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L871>`__.
 
    .. data:: PARTITION_RANGE_DATUM_MINVALUE
 
    .. data:: PARTITION_RANGE_DATUM_VALUE
 
    .. data:: PARTITION_RANGE_DATUM_MAXVALUE
 
 
 .. class:: pglast.enums.parsenodes.PublicationObjSpecType
 
-   Corresponds to the `PublicationObjSpecType enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3721>`__.
+   Corresponds to the `PublicationObjSpecType enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3721>`__.
 
    .. data:: PUBLICATIONOBJ_TABLE
 
    .. data:: PUBLICATIONOBJ_TABLES_IN_SCHEMA
 
    .. data:: PUBLICATIONOBJ_TABLES_IN_CUR_SCHEMA
 
    .. data:: PUBLICATIONOBJ_CONTINUATION
 
 
 .. class:: pglast.enums.parsenodes.QuerySource
 
-   Corresponds to the `QuerySource enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L40>`__.
+   Corresponds to the `QuerySource enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L40>`__.
 
    .. data:: QSRC_ORIGINAL
 
    .. data:: QSRC_PARSER
 
    .. data:: QSRC_INSTEAD_RULE
 
    .. data:: QSRC_QUAL_INSTEAD_RULE
 
    .. data:: QSRC_NON_INSTEAD_RULE
 
 
 .. class:: pglast.enums.parsenodes.RTEKind
 
-   Corresponds to the `RTEKind enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L997>`__.
+   Corresponds to the `RTEKind enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L997>`__.
 
    .. data:: RTE_RELATION
 
    .. data:: RTE_SUBQUERY
 
    .. data:: RTE_JOIN
 
@@ -568,104 +568,104 @@
    .. data:: RTE_NAMEDTUPLESTORE
 
    .. data:: RTE_RESULT
 
 
 .. class:: pglast.enums.parsenodes.ReindexObjectType
 
-   Corresponds to the `ReindexObjectType enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3553>`__.
+   Corresponds to the `ReindexObjectType enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3553>`__.
 
    .. data:: REINDEX_OBJECT_INDEX
 
    .. data:: REINDEX_OBJECT_TABLE
 
    .. data:: REINDEX_OBJECT_SCHEMA
 
    .. data:: REINDEX_OBJECT_SYSTEM
 
    .. data:: REINDEX_OBJECT_DATABASE
 
 
 .. class:: pglast.enums.parsenodes.RoleSpecType
 
-   Corresponds to the `RoleSpecType enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L347>`__.
+   Corresponds to the `RoleSpecType enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L347>`__.
 
    .. data:: ROLESPEC_CSTRING
 
    .. data:: ROLESPEC_CURRENT_ROLE
 
    .. data:: ROLESPEC_CURRENT_USER
 
    .. data:: ROLESPEC_SESSION_USER
 
    .. data:: ROLESPEC_PUBLIC
 
 
 .. class:: pglast.enums.parsenodes.RoleStmtType
 
-   Corresponds to the `RoleStmtType enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2675>`__.
+   Corresponds to the `RoleStmtType enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2675>`__.
 
    .. data:: ROLESTMT_ROLE
 
    .. data:: ROLESTMT_USER
 
    .. data:: ROLESTMT_GROUP
 
 
 .. class:: pglast.enums.parsenodes.SetOperation
 
-   Corresponds to the `SetOperation enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1702>`__.
+   Corresponds to the `SetOperation enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1702>`__.
 
    .. data:: SETOP_NONE
 
    .. data:: SETOP_UNION
 
    .. data:: SETOP_INTERSECT
 
    .. data:: SETOP_EXCEPT
 
 
 .. class:: pglast.enums.parsenodes.SetQuantifier
 
-   Corresponds to the `SetQuantifier enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L66>`__.
+   Corresponds to the `SetQuantifier enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L66>`__.
 
    .. data:: SET_QUANTIFIER_DEFAULT
 
    .. data:: SET_QUANTIFIER_ALL
 
    .. data:: SET_QUANTIFIER_DISTINCT
 
 
 .. class:: pglast.enums.parsenodes.SortByDir
 
-   Corresponds to the `SortByDir enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L50>`__.
+   Corresponds to the `SortByDir enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L50>`__.
 
    .. data:: SORTBY_DEFAULT
 
    .. data:: SORTBY_ASC
 
    .. data:: SORTBY_DESC
 
    .. data:: SORTBY_USING
 
 
 .. class:: pglast.enums.parsenodes.SortByNulls
 
-   Corresponds to the `SortByNulls enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L58>`__.
+   Corresponds to the `SortByNulls enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L58>`__.
 
    .. data:: SORTBY_NULLS_DEFAULT
 
    .. data:: SORTBY_NULLS_FIRST
 
    .. data:: SORTBY_NULLS_LAST
 
 
 .. class:: pglast.enums.parsenodes.TableLikeOption
 
-   Corresponds to the `TableLikeOption enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L710>`__.
+   Corresponds to the `TableLikeOption enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L710>`__.
 
    .. data:: CREATE_TABLE_LIKE_COMMENTS
 
    .. data:: CREATE_TABLE_LIKE_COMPRESSION
 
    .. data:: CREATE_TABLE_LIKE_CONSTRAINTS
 
@@ -682,15 +682,15 @@
    .. data:: CREATE_TABLE_LIKE_STORAGE
 
    .. data:: CREATE_TABLE_LIKE_ALL
 
 
 .. class:: pglast.enums.parsenodes.TransactionStmtKind
 
-   Corresponds to the `TransactionStmtKind enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3245>`__.
+   Corresponds to the `TransactionStmtKind enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3245>`__.
 
    .. data:: TRANS_STMT_BEGIN
 
    .. data:: TRANS_STMT_START
 
    .. data:: TRANS_STMT_COMMIT
 
@@ -707,15 +707,15 @@
    .. data:: TRANS_STMT_COMMIT_PREPARED
 
    .. data:: TRANS_STMT_ROLLBACK_PREPARED
 
 
 .. class:: pglast.enums.parsenodes.VariableSetKind
 
-   Corresponds to the `VariableSetKind enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2202>`__.
+   Corresponds to the `VariableSetKind enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2202>`__.
 
    .. data:: VAR_SET_VALUE
 
    .. data:: VAR_SET_DEFAULT
 
    .. data:: VAR_SET_CURRENT
 
@@ -724,26 +724,26 @@
    .. data:: VAR_RESET
 
    .. data:: VAR_RESET_ALL
 
 
 .. class:: pglast.enums.parsenodes.ViewCheckOption
 
-   Corresponds to the `ViewCheckOption enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L3321>`__.
+   Corresponds to the `ViewCheckOption enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L3321>`__.
 
    .. data:: NO_CHECK_OPTION
 
    .. data:: LOCAL_CHECK_OPTION
 
    .. data:: CASCADED_CHECK_OPTION
 
 
 .. class:: pglast.enums.parsenodes.WCOKind
 
-   Corresponds to the `WCOKind enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L1225>`__.
+   Corresponds to the `WCOKind enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L1225>`__.
 
    .. data:: WCO_VIEW_CHECK
 
    .. data:: WCO_RLS_INSERT_CHECK
 
    .. data:: WCO_RLS_UPDATE_CHECK
 
@@ -752,240 +752,240 @@
    .. data:: WCO_RLS_MERGE_UPDATE_CHECK
 
    .. data:: WCO_RLS_MERGE_DELETE_CHECK
 
 
 .. data:: ACL_INSERT
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L82>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L82>`__.
 
 .. data:: ACL_SELECT
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L83>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L83>`__.
 
 .. data:: ACL_UPDATE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L84>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L84>`__.
 
 .. data:: ACL_DELETE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L85>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L85>`__.
 
 .. data:: ACL_TRUNCATE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L86>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L86>`__.
 
 .. data:: ACL_REFERENCES
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L87>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L87>`__.
 
 .. data:: ACL_TRIGGER
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L88>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L88>`__.
 
 .. data:: ACL_EXECUTE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L89>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L89>`__.
 
 .. data:: ACL_USAGE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L90>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L90>`__.
 
 .. data:: ACL_CREATE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L92>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L92>`__.
 
 .. data:: ACL_CREATE_TEMP
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L93>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L93>`__.
 
 .. data:: ACL_CONNECT
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L94>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L94>`__.
 
 .. data:: ACL_SET
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L95>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L95>`__.
 
 .. data:: ACL_ALTER_SYSTEM
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L96>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L96>`__.
 
 .. data:: N_ACL_RIGHTS
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L97>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L97>`__.
 
 .. data:: ACL_NO_RIGHTS
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L98>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L98>`__.
 
 .. data:: FRAMEOPTION_NONDEFAULT
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L536>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L536>`__.
 
 .. data:: FRAMEOPTION_RANGE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L537>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L537>`__.
 
 .. data:: FRAMEOPTION_ROWS
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L538>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L538>`__.
 
 .. data:: FRAMEOPTION_GROUPS
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L539>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L539>`__.
 
 .. data:: FRAMEOPTION_BETWEEN
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L540>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L540>`__.
 
 .. data:: FRAMEOPTION_START_UNBOUNDED_PRECEDING
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L541>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L541>`__.
 
 .. data:: FRAMEOPTION_END_UNBOUNDED_PRECEDING
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L542>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L542>`__.
 
 .. data:: FRAMEOPTION_START_UNBOUNDED_FOLLOWING
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L543>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L543>`__.
 
 .. data:: FRAMEOPTION_END_UNBOUNDED_FOLLOWING
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L544>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L544>`__.
 
 .. data:: FRAMEOPTION_START_CURRENT_ROW
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L545>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L545>`__.
 
 .. data:: FRAMEOPTION_END_CURRENT_ROW
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L546>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L546>`__.
 
 .. data:: FRAMEOPTION_START_OFFSET_PRECEDING
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L547>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L547>`__.
 
 .. data:: FRAMEOPTION_END_OFFSET_PRECEDING
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L548>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L548>`__.
 
 .. data:: FRAMEOPTION_START_OFFSET_FOLLOWING
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L549>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L549>`__.
 
 .. data:: FRAMEOPTION_END_OFFSET_FOLLOWING
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L550>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L550>`__.
 
 .. data:: FRAMEOPTION_EXCLUDE_CURRENT_ROW
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L551>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L551>`__.
 
 .. data:: FRAMEOPTION_EXCLUDE_GROUP
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L552>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L552>`__.
 
 .. data:: FRAMEOPTION_EXCLUDE_TIES
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L553>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L553>`__.
 
 .. data:: PARTITION_STRATEGY_HASH
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L835>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L835>`__.
 
 .. data:: PARTITION_STRATEGY_LIST
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L836>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L836>`__.
 
 .. data:: PARTITION_STRATEGY_RANGE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L837>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L837>`__.
 
 .. data:: FKCONSTR_ACTION_NOACTION
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2311>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2311>`__.
 
 .. data:: FKCONSTR_ACTION_RESTRICT
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2312>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2312>`__.
 
 .. data:: FKCONSTR_ACTION_CASCADE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2313>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2313>`__.
 
 .. data:: FKCONSTR_ACTION_SETNULL
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2314>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2314>`__.
 
 .. data:: FKCONSTR_ACTION_SETDEFAULT
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2315>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2315>`__.
 
 .. data:: FKCONSTR_MATCH_FULL
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2318>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2318>`__.
 
 .. data:: FKCONSTR_MATCH_PARTIAL
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2319>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2319>`__.
 
 .. data:: FKCONSTR_MATCH_SIMPLE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2320>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2320>`__.
 
 .. data:: OPCLASS_ITEM_OPERATOR
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2781>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2781>`__.
 
 .. data:: OPCLASS_ITEM_FUNCTION
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2782>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2782>`__.
 
 .. data:: OPCLASS_ITEM_STORAGETYPE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2783>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2783>`__.
 
 .. data:: CURSOR_OPT_BINARY
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2882>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2882>`__.
 
 .. data:: CURSOR_OPT_SCROLL
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2883>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2883>`__.
 
 .. data:: CURSOR_OPT_NO_SCROLL
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2884>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2884>`__.
 
 .. data:: CURSOR_OPT_INSENSITIVE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2885>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2885>`__.
 
 .. data:: CURSOR_OPT_ASENSITIVE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2886>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2886>`__.
 
 .. data:: CURSOR_OPT_HOLD
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2887>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2887>`__.
 
 .. data:: CURSOR_OPT_FAST_PLAN
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2889>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2889>`__.
 
 .. data:: CURSOR_OPT_GENERIC_PLAN
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2890>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2890>`__.
 
 .. data:: CURSOR_OPT_CUSTOM_PLAN
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2891>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2891>`__.
 
 .. data:: CURSOR_OPT_PARALLEL_OK
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2892>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2892>`__.
 
 .. data:: FETCH_ALL
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/parsenodes.h#L2927>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/parsenodes.h#L2927>`__.
```

### Comparing `pglast-5.2/docs/parser.rst` & `pglast-5.3/docs/parser.rst`

 * *Files identical despite different names*

### Comparing `pglast-5.2/docs/pg_am.rst` & `pglast-5.3/docs/pg_am.rst`

 * *Files 19% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 .. :Copyright: © 2017-2023 Lele Gaifax
 ..
 
 ====================================================================
  :mod:`pglast.enums.pg_am` --- Constants extracted from `pg_am.h`__
 ====================================================================
 
-__ https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_am.h
+__ https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_am.h
 
 .. module:: pglast.enums.pg_am
    :synopsis: Constants extracted from pg_am.h
 
 
 .. data:: AMTYPE_INDEX
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_am.h#L58>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_am.h#L58>`__.
 
 .. data:: AMTYPE_TABLE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_am.h#L59>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_am.h#L59>`__.
```

### Comparing `pglast-5.2/docs/pg_attribute.rst` & `pglast-5.3/docs/pg_attribute.rst`

 * *Files 13% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 .. :Copyright: © 2017-2023 Lele Gaifax
 ..
 
 ==================================================================================
  :mod:`pglast.enums.pg_attribute` --- Constants extracted from `pg_attribute.h`__
 ==================================================================================
 
-__ https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_attribute.h
+__ https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_attribute.h
 
 .. module:: pglast.enums.pg_attribute
    :synopsis: Constants extracted from pg_attribute.h
 
 
 .. data:: ATTRIBUTE_IDENTITY_ALWAYS
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_attribute.h#L214>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_attribute.h#L214>`__.
 
 .. data:: ATTRIBUTE_IDENTITY_BY_DEFAULT
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_attribute.h#L215>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_attribute.h#L215>`__.
 
 .. data:: ATTRIBUTE_GENERATED_STORED
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_attribute.h#L217>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_attribute.h#L217>`__.
```

### Comparing `pglast-5.2/docs/pg_class.rst` & `pglast-5.3/docs/pg_class.rst`

 * *Files 24% similar despite different names*

```diff
@@ -5,80 +5,80 @@
 .. :Copyright: © 2017-2023 Lele Gaifax
 ..
 
 ==========================================================================
  :mod:`pglast.enums.pg_class` --- Constants extracted from `pg_class.h`__
 ==========================================================================
 
-__ https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_class.h
+__ https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_class.h
 
 .. module:: pglast.enums.pg_class
    :synopsis: Constants extracted from pg_class.h
 
 
 .. data:: RELKIND_RELATION
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_class.h#L161>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_class.h#L161>`__.
 
 .. data:: RELKIND_INDEX
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_class.h#L162>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_class.h#L162>`__.
 
 .. data:: RELKIND_SEQUENCE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_class.h#L163>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_class.h#L163>`__.
 
 .. data:: RELKIND_TOASTVALUE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_class.h#L164>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_class.h#L164>`__.
 
 .. data:: RELKIND_VIEW
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_class.h#L165>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_class.h#L165>`__.
 
 .. data:: RELKIND_MATVIEW
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_class.h#L166>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_class.h#L166>`__.
 
 .. data:: RELKIND_COMPOSITE_TYPE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_class.h#L167>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_class.h#L167>`__.
 
 .. data:: RELKIND_FOREIGN_TABLE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_class.h#L168>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_class.h#L168>`__.
 
 .. data:: RELKIND_PARTITIONED_TABLE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_class.h#L169>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_class.h#L169>`__.
 
 .. data:: RELKIND_PARTITIONED_INDEX
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_class.h#L170>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_class.h#L170>`__.
 
 .. data:: RELPERSISTENCE_PERMANENT
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_class.h#L172>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_class.h#L172>`__.
 
 .. data:: RELPERSISTENCE_UNLOGGED
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_class.h#L173>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_class.h#L173>`__.
 
 .. data:: RELPERSISTENCE_TEMP
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_class.h#L174>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_class.h#L174>`__.
 
 .. data:: REPLICA_IDENTITY_DEFAULT
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_class.h#L177>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_class.h#L177>`__.
 
 .. data:: REPLICA_IDENTITY_NOTHING
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_class.h#L179>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_class.h#L179>`__.
 
 .. data:: REPLICA_IDENTITY_FULL
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_class.h#L181>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_class.h#L181>`__.
 
 .. data:: REPLICA_IDENTITY_INDEX
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_class.h#L187>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_class.h#L187>`__.
```

### Comparing `pglast-5.2/docs/pg_trigger.rst` & `pglast-5.3/docs/pg_trigger.rst`

 * *Files 6% similar despite different names*

```diff
@@ -5,48 +5,48 @@
 .. :Copyright: © 2017-2023 Lele Gaifax
 ..
 
 ==============================================================================
  :mod:`pglast.enums.pg_trigger` --- Constants extracted from `pg_trigger.h`__
 ==============================================================================
 
-__ https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_trigger.h
+__ https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_trigger.h
 
 .. module:: pglast.enums.pg_trigger
    :synopsis: Constants extracted from pg_trigger.h
 
 
 .. data:: TRIGGER_TYPE_ROW
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_trigger.h#L93>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_trigger.h#L93>`__.
 
 .. data:: TRIGGER_TYPE_BEFORE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_trigger.h#L94>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_trigger.h#L94>`__.
 
 .. data:: TRIGGER_TYPE_INSERT
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_trigger.h#L95>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_trigger.h#L95>`__.
 
 .. data:: TRIGGER_TYPE_DELETE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_trigger.h#L96>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_trigger.h#L96>`__.
 
 .. data:: TRIGGER_TYPE_UPDATE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_trigger.h#L97>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_trigger.h#L97>`__.
 
 .. data:: TRIGGER_TYPE_TRUNCATE
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_trigger.h#L98>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_trigger.h#L98>`__.
 
 .. data:: TRIGGER_TYPE_INSTEAD
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_trigger.h#L99>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_trigger.h#L99>`__.
 
 .. data:: TRIGGER_TYPE_STATEMENT
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_trigger.h#L102>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_trigger.h#L102>`__.
 
 .. data:: TRIGGER_TYPE_AFTER
 
-   See `here for details <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/catalog/pg_trigger.h#L107>`__.
+   See `here for details <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/catalog/pg_trigger.h#L107>`__.
```

### Comparing `pglast-5.2/docs/primnodes.rst` & `pglast-5.3/docs/primnodes.rst`

 * *Files 6% similar despite different names*

```diff
@@ -5,34 +5,34 @@
 .. :Copyright: © 2017-2023 Lele Gaifax
 ..
 
 ============================================================================
  :mod:`pglast.enums.primnodes` --- Constants extracted from `primnodes.h`__
 ============================================================================
 
-__ https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h
+__ https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h
 
 .. module:: pglast.enums.primnodes
    :synopsis: Constants extracted from primnodes.h
 
 
 .. class:: pglast.enums.primnodes.BoolExprType
 
-   Corresponds to the `BoolExprType enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L617>`__.
+   Corresponds to the `BoolExprType enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L617>`__.
 
    .. data:: AND_EXPR
 
    .. data:: OR_EXPR
 
    .. data:: NOT_EXPR
 
 
 .. class:: pglast.enums.primnodes.BoolTestType
 
-   Corresponds to the `BoolTestType enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1278>`__.
+   Corresponds to the `BoolTestType enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1278>`__.
 
    .. data:: IS_TRUE
 
    .. data:: IS_NOT_TRUE
 
    .. data:: IS_FALSE
 
@@ -41,85 +41,85 @@
    .. data:: IS_UNKNOWN
 
    .. data:: IS_NOT_UNKNOWN
 
 
 .. class:: pglast.enums.primnodes.CoercionContext
 
-   Corresponds to the `CoercionContext enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L461>`__.
+   Corresponds to the `CoercionContext enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L461>`__.
 
    .. data:: COERCION_IMPLICIT
 
    .. data:: COERCION_ASSIGNMENT
 
    .. data:: COERCION_PLPGSQL
 
    .. data:: COERCION_EXPLICIT
 
 
 .. class:: pglast.enums.primnodes.CoercionForm
 
-   Corresponds to the `CoercionForm enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L481>`__.
+   Corresponds to the `CoercionForm enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L481>`__.
 
    .. data:: COERCE_EXPLICIT_CALL
 
    .. data:: COERCE_EXPLICIT_CAST
 
    .. data:: COERCE_IMPLICIT_CAST
 
    .. data:: COERCE_SQL_SYNTAX
 
 
 .. class:: pglast.enums.primnodes.MinMaxOp
 
-   Corresponds to the `MinMaxOp enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1137>`__.
+   Corresponds to the `MinMaxOp enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1137>`__.
 
    .. data:: IS_GREATEST
 
    .. data:: IS_LEAST
 
 
 .. class:: pglast.enums.primnodes.NullTestType
 
-   Corresponds to the `NullTestType enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1255>`__.
+   Corresponds to the `NullTestType enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1255>`__.
 
    .. data:: IS_NULL
 
    .. data:: IS_NOT_NULL
 
 
 .. class:: pglast.enums.primnodes.OnCommitAction
 
-   Corresponds to the `OnCommitAction enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L47>`__.
+   Corresponds to the `OnCommitAction enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L47>`__.
 
    .. data:: ONCOMMIT_NOOP
 
    .. data:: ONCOMMIT_PRESERVE_ROWS
 
    .. data:: ONCOMMIT_DELETE_ROWS
 
    .. data:: ONCOMMIT_DROP
 
 
 .. class:: pglast.enums.primnodes.ParamKind
 
-   Corresponds to the `ParamKind enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L256>`__.
+   Corresponds to the `ParamKind enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L256>`__.
 
    .. data:: PARAM_EXTERN
 
    .. data:: PARAM_EXEC
 
    .. data:: PARAM_SUBLINK
 
    .. data:: PARAM_MULTIEXPR
 
 
 .. class:: pglast.enums.primnodes.RowCompareType
 
-   Corresponds to the `RowCompareType enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1100>`__.
+   Corresponds to the `RowCompareType enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1100>`__.
 
    .. data:: ROWCOMPARE_LT
 
    .. data:: ROWCOMPARE_LE
 
    .. data:: ROWCOMPARE_EQ
 
@@ -128,15 +128,15 @@
    .. data:: ROWCOMPARE_GT
 
    .. data:: ROWCOMPARE_NE
 
 
 .. class:: pglast.enums.primnodes.SQLValueFunctionOp
 
-   Corresponds to the `SQLValueFunctionOp enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1165>`__.
+   Corresponds to the `SQLValueFunctionOp enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1165>`__.
 
    .. data:: SVFOP_CURRENT_DATE
 
    .. data:: SVFOP_CURRENT_TIME
 
    .. data:: SVFOP_CURRENT_TIME_N
 
@@ -163,15 +163,15 @@
    .. data:: SVFOP_CURRENT_CATALOG
 
    .. data:: SVFOP_CURRENT_SCHEMA
 
 
 .. class:: pglast.enums.primnodes.SubLinkType
 
-   Corresponds to the `SubLinkType enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L681>`__.
+   Corresponds to the `SubLinkType enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L681>`__.
 
    .. data:: EXISTS_SUBLINK
 
    .. data:: ALL_SUBLINK
 
    .. data:: ANY_SUBLINK
 
@@ -184,15 +184,15 @@
    .. data:: ARRAY_SUBLINK
 
    .. data:: CTE_SUBLINK
 
 
 .. class:: pglast.enums.primnodes.XmlExprOp
 
-   Corresponds to the `XmlExprOp enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1204>`__.
+   Corresponds to the `XmlExprOp enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1204>`__.
 
    .. data:: IS_XMLCONCAT
 
    .. data:: IS_XMLELEMENT
 
    .. data:: IS_XMLFOREST
 
@@ -205,12 +205,12 @@
    .. data:: IS_XMLSERIALIZE
 
    .. data:: IS_DOCUMENT
 
 
 .. class:: pglast.enums.primnodes.XmlOptionType
 
-   Corresponds to the `XmlOptionType enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/nodes/primnodes.h#L1216>`__.
+   Corresponds to the `XmlOptionType enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/nodes/primnodes.h#L1216>`__.
 
    .. data:: XMLOPTION_DOCUMENT
 
    .. data:: XMLOPTION_CONTENT
```

### Comparing `pglast-5.2/docs/printers.rst` & `pglast-5.3/docs/printers.rst`

 * *Files identical despite different names*

### Comparing `pglast-5.2/docs/sfuncs.rst` & `pglast-5.3/docs/sfuncs.rst`

 * *Files identical despite different names*

### Comparing `pglast-5.2/docs/stream.rst` & `pglast-5.3/docs/stream.rst`

 * *Files identical despite different names*

### Comparing `pglast-5.2/docs/usage.rst` & `pglast-5.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `pglast-5.2/docs/visitors.rst` & `pglast-5.3/docs/visitors.rst`

 * *Files identical despite different names*

### Comparing `pglast-5.2/docs/xml.rst` & `pglast-5.3/docs/xml.rst`

 * *Files 14% similar despite different names*

```diff
@@ -5,43 +5,43 @@
 .. :Copyright: © 2017-2023 Lele Gaifax
 ..
 
 ================================================================
  :mod:`pglast.enums.xml` --- Constants extracted from `xml.h`__
 ================================================================
 
-__ https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/utils/xml.h
+__ https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/utils/xml.h
 
 .. module:: pglast.enums.xml
    :synopsis: Constants extracted from xml.h
 
 
 .. class:: pglast.enums.xml.PgXmlStrictness
 
-   Corresponds to the `PgXmlStrictness enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/utils/xml.h#L39>`__.
+   Corresponds to the `PgXmlStrictness enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/utils/xml.h#L39>`__.
 
    .. data:: PG_XML_STRICTNESS_LEGACY
 
    .. data:: PG_XML_STRICTNESS_WELLFORMED
 
    .. data:: PG_XML_STRICTNESS_ALL
 
 
 .. class:: pglast.enums.xml.XmlBinaryType
 
-   Corresponds to the `XmlBinaryType enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/utils/xml.h#L33>`__.
+   Corresponds to the `XmlBinaryType enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/utils/xml.h#L33>`__.
 
    .. data:: XMLBINARY_BASE64
 
    .. data:: XMLBINARY_HEX
 
 
 .. class:: pglast.enums.xml.XmlStandaloneType
 
-   Corresponds to the `XmlStandaloneType enum <https://github.com/pganalyze/libpg_query/blob/1f2d166/src/postgres/include/utils/xml.h#L25>`__.
+   Corresponds to the `XmlStandaloneType enum <https://github.com/pganalyze/libpg_query/blob/9b21e32/src/postgres/include/utils/xml.h#L25>`__.
 
    .. data:: XML_STANDALONE_YES
 
    .. data:: XML_STANDALONE_NO
 
    .. data:: XML_STANDALONE_NO_VALUE
```

### Comparing `pglast-5.2/libpg_query/LICENSE` & `pglast-5.3/libpg_query/LICENSE`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/Makefile` & `pglast-5.3/libpg_query/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 PGDIR = $(root_dir)/tmp/postgres
 PGDIRBZ2 = $(root_dir)/tmp/postgres.tar.bz2
 
 PG_VERSION = 15.1
 PG_VERSION_MAJOR = $(call word-dot,$(PG_VERSION),1)
 PROTOC_VERSION = 3.14.0
 
-VERSION = 4.2.1
+VERSION = 4.2.3
 VERSION_MAJOR = $(call word-dot,$(VERSION),1)
 VERSION_MINOR = $(call word-dot,$(VERSION),2)
 VERSION_PATCH = $(call word-dot,$(VERSION),3)
 
 SO_VERSION = $(shell printf '%02d%02d' $(PG_VERSION_MAJOR) $(VERSION_MAJOR)).$(VERSION_MINOR)
 
 ifeq ($(shell uname -s), Darwin)
@@ -144,15 +144,16 @@
 	echo "#undef HAVE_X86_64_POPCNTQ" >> $(PGDIR)/src/include/pg_config.h
 	# Avoid dependency on cpuid.h (only supported on x86 systems)
 	echo "#undef HAVE__GET_CPUID" >> $(PGDIR)/src/include/pg_config.h
 	# Avoid CRC extension usage to ensure we are not architecture-dependent
 	echo "#undef USE_ARMV8_CRC32C" >> $(PGDIR)/src/include/pg_config.h
 	echo "#undef USE_SSE42_CRC32C_WITH_RUNTIME_CHECK" >> $(PGDIR)/src/include/pg_config.h
 	# Ensure we don't fail on systems that have strchrnul support (FreeBSD and NetBSD)
-	echo "#if defined(__FreeBSD__) || defined(__NetBSD__)" >> $(PGDIR)/src/include/pg_config.h
+	echo "#include <stdlib.h>" >>  $(PGDIR)/src/include/pg_config.h
+	echo "#if defined(__FreeBSD__) || defined(__NetBSD__) || (defined(__GLIBC__) && ((__GLIBC__ == 2 && __GLIBC_MINOR__ >= 38) || __GLIBC__ > 2))" >> $(PGDIR)/src/include/pg_config.h
 	echo "#define HAVE_STRCHRNUL" >> $(PGDIR)/src/include/pg_config.h
 	echo "#endif" >> $(PGDIR)/src/include/pg_config.h
 
 extract_source: $(PGDIR)
 	-@ $(RM) -rf ./src/postgres/
 	mkdir ./src/postgres
 	mkdir ./src/postgres/include
```

### Comparing `pglast-5.2/libpg_query/pg_query.h` & `pglast-5.3/libpg_query/pg_query.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/protobuf/pg_query.pb-c.c` & `pglast-5.3/libpg_query/protobuf/pg_query.pb-c.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/protobuf/pg_query.pb-c.h` & `pglast-5.3/libpg_query/protobuf/pg_query.pb-c.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/protobuf/pg_query.proto` & `pglast-5.3/libpg_query/protobuf/pg_query.proto`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/pg_query.c` & `pglast-5.3/libpg_query/src/pg_query.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/pg_query_deparse.c` & `pglast-5.3/libpg_query/src/postgres_deparse.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-#include "pg_query.h"
-#include "pg_query_internal.h"
-#include "pg_query_readfuncs.h"
-
+#include "postgres.h"
 #include "catalog/index.h"
 #include "catalog/pg_am.h"
 #include "catalog/pg_attribute.h"
 #include "catalog/pg_class.h"
 #include "catalog/pg_trigger.h"
 #include "commands/trigger.h"
 #include "common/keywords.h"
@@ -137,15 +134,15 @@
 	return true;
 }
 
 static void deparseSelectStmt(StringInfo str, SelectStmt *stmt);
 static void deparseIntoClause(StringInfo str, IntoClause *into_clause);
 static void deparseRangeVar(StringInfo str, RangeVar *range_var, DeparseNodeContext context);
 static void deparseResTarget(StringInfo str, ResTarget *res_target, DeparseNodeContext context);
-static void deparseRawStmt(StringInfo str, RawStmt *raw_stmt);
+void deparseRawStmt(StringInfo str, RawStmt *raw_stmt);
 static void deparseAlias(StringInfo str, Alias *alias);
 static void deparseWindowDef(StringInfo str, WindowDef* window_def);
 static void deparseColumnRef(StringInfo str, ColumnRef* column_ref);
 static void deparseSubLink(StringInfo str, SubLink* sub_link);
 static void deparseAExpr(StringInfo str, A_Expr* a_expr, DeparseNodeContext context);
 static void deparseBoolExpr(StringInfo str, BoolExpr *bool_expr);
 static void deparseAStar(StringInfo str, A_Star* a_star);
@@ -203,14 +200,15 @@
 
 static void deparsePreparableStmt(StringInfo str, Node *node);
 static void deparseRuleActionStmt(StringInfo str, Node *node);
 static void deparseExplainableStmt(StringInfo str, Node *node);
 static void deparseStmt(StringInfo str, Node *node);
 static void deparseValue(StringInfo str, union ValUnion *value, DeparseNodeContext context);
 
+
 // "any_name" in gram.y
 static void deparseAnyName(StringInfo str, List *parts)
 {
 	ListCell *lc = NULL;
 
 	foreach(lc, parts)
 	{
@@ -784,15 +782,15 @@
 		DefElem *def_elem = castNode(DefElem, lfirst(lc));
 		appendStringInfoString(str, quote_identifier(def_elem->defname));
 		appendStringInfoChar(str, ' ');
 		deparseStringLiteral(str, strVal(def_elem->arg));
 		if (lnext(options, lc))
 			appendStringInfoString(str, ", ");
 	}
-	appendStringInfoString(str, ") ");
+	appendStringInfoString(str, ")");
 }
 
 // "common_func_opt_item" in gram.y
 static void deparseCommonFuncOptItem(StringInfo str, DefElem *def_elem)
 {
 	if (strcmp(def_elem->defname, "strict") == 0 && boolVal(def_elem->arg))
 	{
@@ -2265,17 +2263,19 @@
 		if (stmt->limitOption == LIMIT_OPTION_COUNT)
 			appendStringInfoString(str, "LIMIT ");
 		else if (stmt->limitOption == LIMIT_OPTION_WITH_TIES)
 			appendStringInfoString(str, "FETCH FIRST ");
 
 		if (IsA(stmt->limitCount, A_Const) && castNode(A_Const, stmt->limitCount)->isnull)
 			appendStringInfoString(str, "ALL");
-		else
+		else if (stmt->limitOption == LIMIT_OPTION_WITH_TIES)
 			deparseCExpr(str, stmt->limitCount);
-		
+		else
+			deparseExpr(str, stmt->limitCount);
+
 		appendStringInfoChar(str, ' ');
 
 		if (stmt->limitOption == LIMIT_OPTION_WITH_TIES)
 			appendStringInfoString(str, "ROWS WITH TIES ");
 	}
 
 	if (stmt->limitOffset != NULL)
@@ -2376,19 +2376,19 @@
 		deparseAlias(str, range_var->alias);
 		appendStringInfoChar(str, ' ');
 	}
 
 	removeTrailingSpace(str);
 }
 
-static void deparseRawStmt(StringInfo str, RawStmt *raw_stmt)
+void deparseRawStmt(StringInfo str, RawStmt *raw_stmt)
 {
 	if (raw_stmt->stmt == NULL)
 		elog(ERROR, "deparse error in deparseRawStmt: RawStmt with empty Stmt");
-	
+
 	deparseStmt(str, raw_stmt->stmt);
 }
 
 static void deparseAlias(StringInfo str, Alias *alias)
 {
 	appendStringInfoString(str, quote_identifier(alias->aliasname));
 
@@ -4592,15 +4592,15 @@
 static void deparseConstraint(StringInfo str, Constraint *constraint)
 {
 	ListCell *lc;
 
 	if (constraint->conname != NULL)
 	{
 		appendStringInfoString(str, "CONSTRAINT ");
-		appendStringInfoString(str, constraint->conname);
+		appendStringInfoString(str, quote_identifier(constraint->conname));
 		appendStringInfoChar(str, ' ');
 	}
 
 	switch (constraint->contype) {
 		case CONSTR_NULL:
 			appendStringInfoString(str, "NULL ");
 			break;
@@ -4794,14 +4794,25 @@
 	if (list_length(constraint->including) > 0)
 	{
 		appendStringInfoString(str, "INCLUDE (");
 		deparseColumnList(str, constraint->including);
 		appendStringInfoString(str, ") ");
 	}
 
+	switch (constraint->contype)
+	{
+		case CONSTR_PRIMARY:
+		case CONSTR_UNIQUE:
+		case CONSTR_EXCLUSION:
+			deparseOptWith(str, constraint->options);
+			break;
+		default:
+			break;
+	}
+
 	if (constraint->indexname != NULL)
 		appendStringInfo(str, "USING INDEX %s ", quote_identifier(constraint->indexname));
 
 	if (constraint->indexspace != NULL)
 		appendStringInfo(str, "USING INDEX TABLESPACE %s ", quote_identifier(constraint->indexspace));
 
 	if (constraint->deferrable)
@@ -4886,19 +4897,38 @@
 	}
 
 	if (create_function_stmt->sql_body)
 	{
 		/* RETURN or BEGIN ... END
 		 */
 		if (IsA(create_function_stmt->sql_body, ReturnStmt))
+		{
 			deparseReturnStmt(str, castNode(ReturnStmt, create_function_stmt->sql_body));
+		}
 		else
 		{
 			appendStringInfoString(str, "BEGIN ATOMIC ");
-			deparseExprList(str, castNode(List, create_function_stmt->sql_body));
+			if (IsA(create_function_stmt->sql_body, List), linitial((List *) create_function_stmt->sql_body) != NULL)
+			{
+				List *body_stmt_list = castNode(List, linitial((List *) create_function_stmt->sql_body));
+				foreach(lc, body_stmt_list)
+				{
+					if (IsA(lfirst(lc), ReturnStmt))
+					{
+						deparseReturnStmt(str, lfirst_node(ReturnStmt, lc));
+						appendStringInfoString(str, "; ");
+					}
+					else
+					{
+						deparseStmt(str, lfirst(lc));
+						appendStringInfoString(str, "; ");
+					}
+				}
+			}
+			
 			appendStringInfoString(str, "END ");
 		}
 	}
 
 	removeTrailingSpace(str);
 }
 
@@ -9425,15 +9455,15 @@
 	if (strcmp(variable_show_stmt->name, "timezone") == 0)
 		appendStringInfoString(str, "TIME ZONE");
 	else if (strcmp(variable_show_stmt->name, "transaction_isolation") == 0)
 		appendStringInfoString(str, "TRANSACTION ISOLATION LEVEL");
 	else if (strcmp(variable_show_stmt->name, "session_authorization") == 0)
 		appendStringInfoString(str, "SESSION AUTHORIZATION");
 	else if (strcmp(variable_show_stmt->name, "all") == 0)
-		appendStringInfoString(str, "SESSION ALL");
+		appendStringInfoString(str, "ALL");
 	else
 		appendStringInfoString(str, quote_identifier(variable_show_stmt->name));
 }
 
 static void deparseRangeTableSample(StringInfo str, RangeTableSample *range_table_sample)
 {
 	deparseRangeVar(str, castNode(RangeVar, range_table_sample->relation), DEPARSE_NODE_CONTEXT_NONE);
@@ -10633,66 +10663,7 @@
 		case T_CreateRangeStmt:
 			deparseCreateRangeStmt(str, castNode(CreateRangeStmt, node));
 			break;
 		default:
 			elog(ERROR, "deparse: unsupported top-level node type: %u", nodeTag(node));
 	}
 }
-
-PgQueryDeparseResult pg_query_deparse_protobuf(PgQueryProtobuf parse_tree)
-{
-	PgQueryDeparseResult result = {0};
-	StringInfoData str;
-	MemoryContext ctx;
-	List *stmts;
-	ListCell *lc;
-
-	ctx = pg_query_enter_memory_context();
-
-	PG_TRY();
-	{
-		stmts = pg_query_protobuf_to_nodes(parse_tree);
-
-		initStringInfo(&str);
-
-		foreach(lc, stmts) {
-			deparseRawStmt(&str, castNode(RawStmt, lfirst(lc)));
-			if (lnext(stmts, lc))
-				appendStringInfoString(&str, "; ");
-		}
-		result.query = strdup(str.data);
-	}
-	PG_CATCH();
-	{
-		ErrorData* error_data;
-		PgQueryError* error;
-
-		MemoryContextSwitchTo(ctx);
-		error_data = CopyErrorData();
-
-		// Note: This is intentionally malloc so exiting the memory context doesn't free this
-		error = malloc(sizeof(PgQueryError));
-		error->message   = strdup(error_data->message);
-		error->filename  = strdup(error_data->filename);
-		error->funcname  = strdup(error_data->funcname);
-		error->context   = NULL;
-		error->lineno	= error_data->lineno;
-		error->cursorpos = error_data->cursorpos;
-
-		result.error = error;
-		FlushErrorState();
-	}
-	PG_END_TRY();
-
-	pg_query_exit_memory_context(ctx);
-
-	return result;
-}
-
-void pg_query_free_deparse_result(PgQueryDeparseResult result)
-{
-	if (result.error) {
-		pg_query_free_error(result.error);
-	}
-
-	free(result.query);
-}
```

### Comparing `pglast-5.2/libpg_query/src/pg_query_enum_defs.c` & `pglast-5.3/libpg_query/src/pg_query_enum_defs.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/pg_query_fingerprint.c` & `pglast-5.3/libpg_query/src/pg_query_fingerprint.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/pg_query_fingerprint_conds.c` & `pglast-5.3/libpg_query/src/pg_query_fingerprint_conds.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/pg_query_fingerprint_defs.c` & `pglast-5.3/libpg_query/src/pg_query_fingerprint_defs.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/pg_query_internal.h` & `pglast-5.3/libpg_query/src/pg_query_internal.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/pg_query_json_helper.c` & `pglast-5.3/libpg_query/src/pg_query_json_helper.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/pg_query_json_plpgsql.c` & `pglast-5.3/libpg_query/src/pg_query_json_plpgsql.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/pg_query_normalize.c` & `pglast-5.3/libpg_query/src/pg_query_normalize.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/pg_query_outfuncs_conds.c` & `pglast-5.3/libpg_query/src/pg_query_outfuncs_conds.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/pg_query_outfuncs_defs.c` & `pglast-5.3/libpg_query/src/pg_query_outfuncs_defs.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/pg_query_outfuncs_json.c` & `pglast-5.3/libpg_query/src/pg_query_outfuncs_json.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/pg_query_outfuncs_protobuf.c` & `pglast-5.3/libpg_query/src/pg_query_outfuncs_protobuf.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/pg_query_parse.c` & `pglast-5.3/libpg_query/src/pg_query_parse.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/pg_query_parse_plpgsql.c` & `pglast-5.3/libpg_query/src/pg_query_parse_plpgsql.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/pg_query_readfuncs_conds.c` & `pglast-5.3/libpg_query/src/pg_query_readfuncs_conds.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/pg_query_readfuncs_defs.c` & `pglast-5.3/libpg_query/src/pg_query_readfuncs_defs.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/pg_query_readfuncs_protobuf.c` & `pglast-5.3/libpg_query/src/pg_query_readfuncs_protobuf.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/pg_query_scan.c` & `pglast-5.3/libpg_query/src/pg_query_scan.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/pg_query_split.c` & `pglast-5.3/libpg_query/src/pg_query_split.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/amapi.h` & `pglast-5.3/libpg_query/src/postgres/include/access/amapi.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/attmap.h` & `pglast-5.3/libpg_query/src/postgres/include/access/attmap.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/attnum.h` & `pglast-5.3/libpg_query/src/postgres/include/access/attnum.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/clog.h` & `pglast-5.3/libpg_query/src/postgres/include/access/clog.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/commit_ts.h` & `pglast-5.3/libpg_query/src/postgres/include/access/commit_ts.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/detoast.h` & `pglast-5.3/libpg_query/src/postgres/include/access/detoast.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/genam.h` & `pglast-5.3/libpg_query/src/postgres/include/access/genam.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/gin.h` & `pglast-5.3/libpg_query/src/postgres/include/access/gin.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/htup.h` & `pglast-5.3/libpg_query/src/postgres/include/access/htup.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/htup_details.h` & `pglast-5.3/libpg_query/src/postgres/include/access/htup_details.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/itup.h` & `pglast-5.3/libpg_query/src/postgres/include/access/itup.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/parallel.h` & `pglast-5.3/libpg_query/src/postgres/include/access/parallel.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/printtup.h` & `pglast-5.3/libpg_query/src/postgres/include/access/printtup.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/relation.h` & `pglast-5.3/libpg_query/src/postgres/include/access/relation.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/relscan.h` & `pglast-5.3/libpg_query/src/postgres/include/access/relscan.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/rmgr.h` & `pglast-5.3/libpg_query/src/postgres/include/access/rmgr.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/rmgrlist.h` & `pglast-5.3/libpg_query/src/postgres/include/access/rmgrlist.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/sdir.h` & `pglast-5.3/libpg_query/src/postgres/include/access/sdir.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/skey.h` & `pglast-5.3/libpg_query/src/postgres/include/access/skey.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/stratnum.h` & `pglast-5.3/libpg_query/src/postgres/include/access/stratnum.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/sysattr.h` & `pglast-5.3/libpg_query/src/postgres/include/access/sysattr.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/table.h` & `pglast-5.3/libpg_query/src/postgres/include/access/table.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/tableam.h` & `pglast-5.3/libpg_query/src/postgres/include/access/tableam.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/toast_compression.h` & `pglast-5.3/libpg_query/src/postgres/include/access/toast_compression.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/transam.h` & `pglast-5.3/libpg_query/src/postgres/include/access/transam.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/tupconvert.h` & `pglast-5.3/libpg_query/src/postgres/include/access/tupconvert.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/tupdesc.h` & `pglast-5.3/libpg_query/src/postgres/include/access/tupdesc.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/tupmacs.h` & `pglast-5.3/libpg_query/src/postgres/include/access/tupmacs.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/twophase.h` & `pglast-5.3/libpg_query/src/postgres/include/access/twophase.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/xact.h` & `pglast-5.3/libpg_query/src/postgres/include/access/xact.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/xlog.h` & `pglast-5.3/libpg_query/src/postgres/include/access/xlog.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/xlog_internal.h` & `pglast-5.3/libpg_query/src/postgres/include/access/xlog_internal.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/xlogdefs.h` & `pglast-5.3/libpg_query/src/postgres/include/access/xlogdefs.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/xlogprefetcher.h` & `pglast-5.3/libpg_query/src/postgres/include/access/xlogprefetcher.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/xlogreader.h` & `pglast-5.3/libpg_query/src/postgres/include/access/xlogreader.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/xlogrecord.h` & `pglast-5.3/libpg_query/src/postgres/include/access/xlogrecord.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/access/xlogrecovery.h` & `pglast-5.3/libpg_query/src/postgres/include/access/xlogrecovery.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/c.h` & `pglast-5.3/libpg_query/src/postgres/include/c.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/catalog.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/catalog.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/catversion.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/catversion.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/dependency.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/dependency.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/genbki.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/genbki.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/index.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/index.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/indexing.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/indexing.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/namespace.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/namespace.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/objectaccess.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/objectaccess.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/objectaddress.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/objectaddress.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_aggregate.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_aggregate.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_aggregate_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_aggregate_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_am.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_am.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_am_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_am_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_attribute.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_attribute.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_attribute_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_attribute_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_authid.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_authid.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_authid_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_authid_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_class.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_class.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_class_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_class_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_collation.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_collation.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_collation_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_collation_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_constraint.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_constraint.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_constraint_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_constraint_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_control.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_control.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_conversion.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_conversion.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_conversion_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_conversion_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_depend.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_depend.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_depend_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_depend_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_event_trigger.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_event_trigger.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_event_trigger_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_event_trigger_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_index.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_index.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_index_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_index_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_language.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_language.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_language_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_language_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_namespace.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_namespace.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_namespace_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_namespace_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_opclass.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_opclass.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_opclass_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_opclass_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_operator.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_operator.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_operator_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_operator_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_opfamily.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_opfamily.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_opfamily_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_opfamily_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_parameter_acl.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_parameter_acl.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_parameter_acl_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_parameter_acl_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_partitioned_table.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_partitioned_table.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_partitioned_table_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_partitioned_table_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_proc.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_proc.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_proc_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_proc_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_publication.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_publication.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_publication_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_publication_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_replication_origin.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_replication_origin.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_replication_origin_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_replication_origin_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_statistic.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_statistic.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_statistic_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_statistic_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_statistic_ext.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_statistic_ext.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_statistic_ext_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_statistic_ext_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_transform.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_transform.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_transform_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_transform_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_trigger.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_trigger.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_trigger_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_trigger_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_ts_config.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_ts_config.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_ts_config_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_ts_config_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_ts_dict.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_ts_dict.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_ts_dict_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_ts_dict_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_ts_parser.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_ts_parser.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_ts_parser_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_ts_parser_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_ts_template.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_ts_template.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_ts_template_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_ts_template_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_type.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_type.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/pg_type_d.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/pg_type_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/catalog/storage.h` & `pglast-5.3/libpg_query/src/postgres/include/catalog/storage.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/commands/async.h` & `pglast-5.3/libpg_query/src/postgres/include/commands/async.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/commands/dbcommands.h` & `pglast-5.3/libpg_query/src/postgres/include/commands/dbcommands.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/commands/defrem.h` & `pglast-5.3/libpg_query/src/postgres/include/commands/defrem.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/commands/event_trigger.h` & `pglast-5.3/libpg_query/src/postgres/include/commands/event_trigger.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/commands/explain.h` & `pglast-5.3/libpg_query/src/postgres/include/commands/explain.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/commands/prepare.h` & `pglast-5.3/libpg_query/src/postgres/include/commands/prepare.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/commands/tablespace.h` & `pglast-5.3/libpg_query/src/postgres/include/commands/tablespace.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/commands/trigger.h` & `pglast-5.3/libpg_query/src/postgres/include/commands/trigger.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/commands/user.h` & `pglast-5.3/libpg_query/src/postgres/include/commands/user.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/commands/vacuum.h` & `pglast-5.3/libpg_query/src/postgres/include/commands/vacuum.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/commands/variable.h` & `pglast-5.3/libpg_query/src/postgres/include/commands/variable.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/common/file_perm.h` & `pglast-5.3/libpg_query/src/postgres/include/common/file_perm.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/common/hashfn.h` & `pglast-5.3/libpg_query/src/postgres/include/common/hashfn.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/common/ip.h` & `pglast-5.3/libpg_query/src/postgres/include/common/ip.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/common/keywords.h` & `pglast-5.3/libpg_query/src/postgres/include/common/keywords.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/common/kwlookup.h` & `pglast-5.3/libpg_query/src/postgres/include/common/kwlookup.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/common/pg_prng.h` & `pglast-5.3/libpg_query/src/postgres/include/common/pg_prng.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/common/relpath.h` & `pglast-5.3/libpg_query/src/postgres/include/common/relpath.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/common/string.h` & `pglast-5.3/libpg_query/src/postgres/include/common/string.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/common/unicode_combining_table.h` & `pglast-5.3/libpg_query/src/postgres/include/common/unicode_combining_table.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/common/unicode_east_asian_fw_table.h` & `pglast-5.3/libpg_query/src/postgres/include/common/unicode_east_asian_fw_table.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/datatype/timestamp.h` & `pglast-5.3/libpg_query/src/postgres/include/datatype/timestamp.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/executor/execdesc.h` & `pglast-5.3/libpg_query/src/postgres/include/executor/execdesc.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/executor/executor.h` & `pglast-5.3/libpg_query/src/postgres/include/executor/executor.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/executor/functions.h` & `pglast-5.3/libpg_query/src/postgres/include/executor/functions.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/executor/instrument.h` & `pglast-5.3/libpg_query/src/postgres/include/executor/instrument.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/executor/spi.h` & `pglast-5.3/libpg_query/src/postgres/include/executor/spi.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/executor/tablefunc.h` & `pglast-5.3/libpg_query/src/postgres/include/executor/tablefunc.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/executor/tuptable.h` & `pglast-5.3/libpg_query/src/postgres/include/executor/tuptable.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/fmgr.h` & `pglast-5.3/libpg_query/src/postgres/include/fmgr.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/funcapi.h` & `pglast-5.3/libpg_query/src/postgres/include/funcapi.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/getaddrinfo.h` & `pglast-5.3/libpg_query/src/postgres/include/getaddrinfo.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/jit/jit.h` & `pglast-5.3/libpg_query/src/postgres/include/jit/jit.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/kwlist_d.h` & `pglast-5.3/libpg_query/src/postgres/include/kwlist_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/lib/dshash.h` & `pglast-5.3/libpg_query/src/postgres/include/lib/dshash.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/lib/ilist.h` & `pglast-5.3/libpg_query/src/postgres/include/lib/ilist.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/lib/pairingheap.h` & `pglast-5.3/libpg_query/src/postgres/include/lib/pairingheap.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/lib/simplehash.h` & `pglast-5.3/libpg_query/src/postgres/include/lib/simplehash.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/lib/sort_template.h` & `pglast-5.3/libpg_query/src/postgres/include/lib/sort_template.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/lib/stringinfo.h` & `pglast-5.3/libpg_query/src/postgres/include/lib/stringinfo.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/libpq/auth.h` & `pglast-5.3/libpg_query/src/postgres/include/libpq/auth.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/libpq/crypt.h` & `pglast-5.3/libpg_query/src/postgres/include/libpq/crypt.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/libpq/hba.h` & `pglast-5.3/libpg_query/src/postgres/include/libpq/hba.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/libpq/libpq-be.h` & `pglast-5.3/libpg_query/src/postgres/include/libpq/libpq-be.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/libpq/libpq.h` & `pglast-5.3/libpg_query/src/postgres/include/libpq/libpq.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/libpq/pqcomm.h` & `pglast-5.3/libpg_query/src/postgres/include/libpq/pqcomm.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/libpq/pqformat.h` & `pglast-5.3/libpg_query/src/postgres/include/libpq/pqformat.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/libpq/pqsignal.h` & `pglast-5.3/libpg_query/src/postgres/include/libpq/pqsignal.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/mb/pg_wchar.h` & `pglast-5.3/libpg_query/src/postgres/include/mb/pg_wchar.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/mb/stringinfo_mb.h` & `pglast-5.3/libpg_query/src/postgres/include/mb/stringinfo_mb.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/miscadmin.h` & `pglast-5.3/libpg_query/src/postgres/include/miscadmin.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/nodes/bitmapset.h` & `pglast-5.3/libpg_query/src/postgres/include/nodes/bitmapset.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/nodes/execnodes.h` & `pglast-5.3/libpg_query/src/postgres/include/nodes/execnodes.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/nodes/extensible.h` & `pglast-5.3/libpg_query/src/postgres/include/nodes/extensible.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/nodes/lockoptions.h` & `pglast-5.3/libpg_query/src/postgres/include/nodes/lockoptions.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/nodes/makefuncs.h` & `pglast-5.3/libpg_query/src/postgres/include/nodes/makefuncs.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/nodes/memnodes.h` & `pglast-5.3/libpg_query/src/postgres/include/nodes/memnodes.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/nodes/nodeFuncs.h` & `pglast-5.3/libpg_query/src/postgres/include/nodes/nodeFuncs.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/nodes/nodes.h` & `pglast-5.3/libpg_query/src/postgres/include/nodes/nodes.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/nodes/params.h` & `pglast-5.3/libpg_query/src/postgres/include/nodes/params.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/nodes/parsenodes.h` & `pglast-5.3/libpg_query/src/postgres/include/nodes/parsenodes.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/nodes/pathnodes.h` & `pglast-5.3/libpg_query/src/postgres/include/nodes/pathnodes.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/nodes/pg_list.h` & `pglast-5.3/libpg_query/src/postgres/include/nodes/pg_list.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/nodes/plannodes.h` & `pglast-5.3/libpg_query/src/postgres/include/nodes/plannodes.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/nodes/primnodes.h` & `pglast-5.3/libpg_query/src/postgres/include/nodes/primnodes.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/nodes/print.h` & `pglast-5.3/libpg_query/src/postgres/include/nodes/print.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/nodes/tidbitmap.h` & `pglast-5.3/libpg_query/src/postgres/include/nodes/tidbitmap.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/nodes/value.h` & `pglast-5.3/libpg_query/src/postgres/include/nodes/value.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/optimizer/cost.h` & `pglast-5.3/libpg_query/src/postgres/include/optimizer/cost.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/optimizer/geqo.h` & `pglast-5.3/libpg_query/src/postgres/include/optimizer/geqo.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/optimizer/geqo_gene.h` & `pglast-5.3/libpg_query/src/postgres/include/optimizer/geqo_gene.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/optimizer/optimizer.h` & `pglast-5.3/libpg_query/src/postgres/include/optimizer/optimizer.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/optimizer/paths.h` & `pglast-5.3/libpg_query/src/postgres/include/optimizer/paths.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/optimizer/planmain.h` & `pglast-5.3/libpg_query/src/postgres/include/optimizer/planmain.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/parser/analyze.h` & `pglast-5.3/libpg_query/src/postgres/include/parser/analyze.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/parser/gram.h` & `pglast-5.3/libpg_query/src/postgres/include/parser/gram.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/parser/gramparse.h` & `pglast-5.3/libpg_query/src/postgres/include/parser/gramparse.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/parser/kwlist.h` & `pglast-5.3/libpg_query/src/postgres/include/parser/kwlist.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/parser/parse_agg.h` & `pglast-5.3/libpg_query/src/postgres/include/parser/parse_agg.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/parser/parse_coerce.h` & `pglast-5.3/libpg_query/src/postgres/include/parser/parse_coerce.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/parser/parse_expr.h` & `pglast-5.3/libpg_query/src/postgres/include/parser/parse_expr.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/parser/parse_func.h` & `pglast-5.3/libpg_query/src/postgres/include/parser/parse_func.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/parser/parse_node.h` & `pglast-5.3/libpg_query/src/postgres/include/parser/parse_node.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/parser/parse_oper.h` & `pglast-5.3/libpg_query/src/postgres/include/parser/parse_oper.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/parser/parse_relation.h` & `pglast-5.3/libpg_query/src/postgres/include/parser/parse_relation.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/parser/parse_type.h` & `pglast-5.3/libpg_query/src/postgres/include/parser/parse_type.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/parser/parser.h` & `pglast-5.3/libpg_query/src/postgres/include/parser/parser.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/parser/parsetree.h` & `pglast-5.3/libpg_query/src/postgres/include/parser/parsetree.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/parser/scanner.h` & `pglast-5.3/libpg_query/src/postgres/include/parser/scanner.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/parser/scansup.h` & `pglast-5.3/libpg_query/src/postgres/include/parser/scansup.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/partitioning/partdefs.h` & `pglast-5.3/libpg_query/src/postgres/include/partitioning/partdefs.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/pg_config.h` & `pglast-5.3/libpg_query/src/postgres/include/pg_config.h`

 * *Files 0% similar despite different names*

```diff
@@ -1028,10 +1028,11 @@
 #undef HAVE__STATIC_ASSERT
 #undef HAVE_EXECINFO_H
 #undef HAVE_BACKTRACE_SYMBOLS
 #undef HAVE_X86_64_POPCNTQ
 #undef HAVE__GET_CPUID
 #undef USE_ARMV8_CRC32C
 #undef USE_SSE42_CRC32C_WITH_RUNTIME_CHECK
-#if defined(__FreeBSD__) || defined(__NetBSD__)
+#include <stdlib.h>
+#if defined(__FreeBSD__) || defined(__NetBSD__) || (defined(__GLIBC__) && ((__GLIBC__ == 2 && __GLIBC_MINOR__ >= 38) || __GLIBC__ > 2))
 #define HAVE_STRCHRNUL
 #endif
```

### Comparing `pglast-5.2/libpg_query/src/postgres/include/pg_config_manual.h` & `pglast-5.3/libpg_query/src/postgres/include/pg_config_manual.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/pg_getopt.h` & `pglast-5.3/libpg_query/src/postgres/include/pg_getopt.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/pgstat.h` & `pglast-5.3/libpg_query/src/postgres/include/pgstat.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/pgtime.h` & `pglast-5.3/libpg_query/src/postgres/include/pgtime.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/pl_gram.h` & `pglast-5.3/libpg_query/src/postgres/include/pl_gram.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/pl_reserved_kwlist.h` & `pglast-5.3/libpg_query/src/postgres/include/pl_reserved_kwlist.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/pl_reserved_kwlist_d.h` & `pglast-5.3/libpg_query/src/postgres/include/pl_reserved_kwlist_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/pl_unreserved_kwlist.h` & `pglast-5.3/libpg_query/src/postgres/include/pl_unreserved_kwlist.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/pl_unreserved_kwlist_d.h` & `pglast-5.3/libpg_query/src/postgres/include/pl_unreserved_kwlist_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/plerrcodes.h` & `pglast-5.3/libpg_query/src/postgres/include/plerrcodes.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/plpgsql.h` & `pglast-5.3/libpg_query/src/postgres/include/plpgsql.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/port/atomics/arch-arm.h` & `pglast-5.3/libpg_query/src/postgres/include/port/atomics/arch-arm.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/port/atomics/arch-ppc.h` & `pglast-5.3/libpg_query/src/postgres/include/port/atomics/arch-ppc.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/port/atomics/arch-x86.h` & `pglast-5.3/libpg_query/src/postgres/include/port/atomics/arch-x86.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/port/atomics/fallback.h` & `pglast-5.3/libpg_query/src/postgres/include/port/atomics/fallback.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/port/atomics/generic-gcc.h` & `pglast-5.3/libpg_query/src/postgres/include/port/atomics/generic-gcc.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/port/atomics/generic.h` & `pglast-5.3/libpg_query/src/postgres/include/port/atomics/generic.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/port/atomics.h` & `pglast-5.3/libpg_query/src/postgres/include/port/atomics.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/port/pg_bitutils.h` & `pglast-5.3/libpg_query/src/postgres/include/port/pg_bitutils.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/port/pg_bswap.h` & `pglast-5.3/libpg_query/src/postgres/include/port/pg_bswap.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/port/pg_crc32c.h` & `pglast-5.3/libpg_query/src/postgres/include/port/pg_crc32c.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/port.h` & `pglast-5.3/libpg_query/src/postgres/include/port.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/portability/instr_time.h` & `pglast-5.3/libpg_query/src/postgres/include/portability/instr_time.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/postgres.h` & `pglast-5.3/libpg_query/src/postgres/include/postgres.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/postgres_ext.h` & `pglast-5.3/libpg_query/src/postgres/include/postgres_ext.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/postmaster/autovacuum.h` & `pglast-5.3/libpg_query/src/postgres/include/postmaster/autovacuum.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/postmaster/auxprocess.h` & `pglast-5.3/libpg_query/src/postgres/include/postmaster/auxprocess.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/postmaster/bgworker.h` & `pglast-5.3/libpg_query/src/postgres/include/postmaster/bgworker.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/postmaster/bgworker_internals.h` & `pglast-5.3/libpg_query/src/postgres/include/postmaster/bgworker_internals.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/postmaster/bgwriter.h` & `pglast-5.3/libpg_query/src/postgres/include/postmaster/bgwriter.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/postmaster/interrupt.h` & `pglast-5.3/libpg_query/src/postgres/include/postmaster/interrupt.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/postmaster/pgarch.h` & `pglast-5.3/libpg_query/src/postgres/include/postmaster/pgarch.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/postmaster/postmaster.h` & `pglast-5.3/libpg_query/src/postgres/include/postmaster/postmaster.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/postmaster/startup.h` & `pglast-5.3/libpg_query/src/postgres/include/postmaster/startup.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/postmaster/syslogger.h` & `pglast-5.3/libpg_query/src/postgres/include/postmaster/syslogger.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/postmaster/walwriter.h` & `pglast-5.3/libpg_query/src/postgres/include/postmaster/walwriter.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/regex/regex.h` & `pglast-5.3/libpg_query/src/postgres/include/regex/regex.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/replication/logicallauncher.h` & `pglast-5.3/libpg_query/src/postgres/include/replication/logicallauncher.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/replication/logicalproto.h` & `pglast-5.3/libpg_query/src/postgres/include/replication/logicalproto.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/replication/logicalworker.h` & `pglast-5.3/libpg_query/src/postgres/include/replication/logicalworker.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/replication/origin.h` & `pglast-5.3/libpg_query/src/postgres/include/replication/origin.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/replication/reorderbuffer.h` & `pglast-5.3/libpg_query/src/postgres/include/replication/reorderbuffer.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/replication/slot.h` & `pglast-5.3/libpg_query/src/postgres/include/replication/slot.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/replication/syncrep.h` & `pglast-5.3/libpg_query/src/postgres/include/replication/syncrep.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/replication/walreceiver.h` & `pglast-5.3/libpg_query/src/postgres/include/replication/walreceiver.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/replication/walsender.h` & `pglast-5.3/libpg_query/src/postgres/include/replication/walsender.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/rewrite/prs2lock.h` & `pglast-5.3/libpg_query/src/postgres/include/rewrite/prs2lock.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/rewrite/rewriteHandler.h` & `pglast-5.3/libpg_query/src/postgres/include/rewrite/rewriteHandler.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/rewrite/rewriteManip.h` & `pglast-5.3/libpg_query/src/postgres/include/rewrite/rewriteManip.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/rewrite/rewriteSupport.h` & `pglast-5.3/libpg_query/src/postgres/include/rewrite/rewriteSupport.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/backendid.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/backendid.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/block.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/block.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/buf.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/buf.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/bufmgr.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/bufmgr.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/bufpage.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/bufpage.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/condition_variable.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/condition_variable.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/dsm.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/dsm.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/dsm_impl.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/dsm_impl.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/fd.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/fd.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/fileset.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/fileset.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/ipc.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/ipc.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/itemid.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/itemid.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/itemptr.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/itemptr.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/large_object.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/large_object.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/latch.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/latch.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/lmgr.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/lmgr.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/lock.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/lock.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/lockdefs.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/lockdefs.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/lwlock.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/lwlock.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/lwlocknames.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/lwlocknames.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/off.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/off.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/pg_sema.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/pg_sema.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/pg_shmem.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/pg_shmem.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/pmsignal.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/pmsignal.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/predicate.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/predicate.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/proc.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/proc.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/procarray.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/procarray.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/proclist_types.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/proclist_types.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/procsignal.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/procsignal.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/relfilenode.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/relfilenode.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/s_lock.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/s_lock.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/sharedfileset.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/sharedfileset.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/shm_mq.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/shm_mq.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/shm_toc.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/shm_toc.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/shmem.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/shmem.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/sinval.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/sinval.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/sinvaladt.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/sinvaladt.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/smgr.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/smgr.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/spin.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/spin.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/standby.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/standby.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/standbydefs.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/standbydefs.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/storage/sync.h` & `pglast-5.3/libpg_query/src/postgres/include/storage/sync.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/tcop/cmdtag.h` & `pglast-5.3/libpg_query/src/postgres/include/tcop/cmdtag.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/tcop/cmdtaglist.h` & `pglast-5.3/libpg_query/src/postgres/include/tcop/cmdtaglist.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/tcop/deparse_utility.h` & `pglast-5.3/libpg_query/src/postgres/include/tcop/deparse_utility.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/tcop/dest.h` & `pglast-5.3/libpg_query/src/postgres/include/tcop/dest.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/tcop/fastpath.h` & `pglast-5.3/libpg_query/src/postgres/include/tcop/fastpath.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/tcop/pquery.h` & `pglast-5.3/libpg_query/src/postgres/include/tcop/pquery.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/tcop/tcopprot.h` & `pglast-5.3/libpg_query/src/postgres/include/tcop/tcopprot.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/tcop/utility.h` & `pglast-5.3/libpg_query/src/postgres/include/tcop/utility.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/tsearch/ts_cache.h` & `pglast-5.3/libpg_query/src/postgres/include/tsearch/ts_cache.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/acl.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/acl.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/aclchk_internal.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/aclchk_internal.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/array.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/array.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/backend_progress.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/backend_progress.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/backend_status.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/backend_status.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/builtins.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/builtins.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/bytea.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/bytea.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/catcache.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/catcache.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/date.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/date.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/datetime.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/datetime.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/datum.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/datum.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/dsa.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/dsa.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/dynahash.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/dynahash.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/elog.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/elog.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/errcodes.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/errcodes.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/expandeddatum.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/expandeddatum.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/expandedrecord.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/expandedrecord.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/float.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/float.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/fmgroids.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/fmgroids.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/fmgrprotos.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/fmgrprotos.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/fmgrtab.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/fmgrtab.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/guc.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/guc.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/guc_tables.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/guc_tables.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/hsearch.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/hsearch.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/inval.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/inval.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/lsyscache.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/lsyscache.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/memdebug.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/memdebug.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/memutils.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/memutils.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/numeric.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/numeric.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/palloc.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/palloc.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/partcache.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/partcache.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/pg_locale.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/pg_locale.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/pg_lsn.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/pg_lsn.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/pgstat_internal.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/pgstat_internal.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/pidfile.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/pidfile.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/plancache.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/plancache.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/portal.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/portal.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/probes.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/probes.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/ps_status.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/ps_status.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/queryenvironment.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/queryenvironment.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/queryjumble.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/queryjumble.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/regproc.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/regproc.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/rel.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/rel.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/relcache.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/relcache.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/reltrigger.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/reltrigger.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/resowner.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/resowner.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/rls.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/rls.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/ruleutils.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/ruleutils.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/sharedtuplestore.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/sharedtuplestore.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/snapmgr.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/snapmgr.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/snapshot.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/snapshot.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/sortsupport.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/sortsupport.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/syscache.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/syscache.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/timeout.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/timeout.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/timestamp.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/timestamp.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/tuplesort.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/tuplesort.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/tuplestore.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/tuplestore.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/typcache.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/typcache.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/tzparser.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/tzparser.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/varlena.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/varlena.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/wait_event.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/wait_event.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/include/utils/xml.h` & `pglast-5.3/libpg_query/src/postgres/include/utils/xml.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_catalog_namespace.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_catalog_namespace.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_catalog_pg_proc.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_catalog_pg_proc.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_commands_define.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_commands_define.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_nodes_bitmapset.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_nodes_bitmapset.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_nodes_copyfuncs.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_nodes_copyfuncs.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_nodes_equalfuncs.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_nodes_equalfuncs.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_nodes_extensible.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_nodes_extensible.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_nodes_list.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_nodes_list.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_nodes_makefuncs.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_nodes_makefuncs.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_nodes_nodeFuncs.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_nodes_nodeFuncs.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_nodes_value.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_nodes_value.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_parser_gram.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_parser_gram.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_parser_parser.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_parser_parser.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_parser_scan.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_parser_scan.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_parser_scansup.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_parser_scansup.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_postmaster_postmaster.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_postmaster_postmaster.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_storage_ipc_ipc.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_storage_ipc_ipc.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_storage_lmgr_s_lock.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_storage_lmgr_s_lock.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_tcop_postgres.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_tcop_postgres.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_utils_activity_pgstat_database.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_utils_activity_pgstat_database.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_utils_adt_datum.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_utils_adt_datum.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_utils_adt_expandeddatum.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_utils_adt_expandeddatum.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_utils_adt_format_type.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_utils_adt_format_type.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_utils_adt_ruleutils.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_utils_adt_ruleutils.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_utils_error_assert.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_utils_error_assert.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_utils_error_elog.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_utils_error_elog.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_utils_fmgr_fmgr.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_utils_fmgr_fmgr.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_utils_hash_dynahash.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_utils_hash_dynahash.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_utils_init_globals.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_utils_init_globals.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_utils_mb_mbutils.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_utils_mb_mbutils.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_utils_misc_guc.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_utils_misc_guc.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_utils_mmgr_aset.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_utils_mmgr_aset.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_backend_utils_mmgr_mcxt.c` & `pglast-5.3/libpg_query/src/postgres/src_backend_utils_mmgr_mcxt.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_common_encnames.c` & `pglast-5.3/libpg_query/src/postgres/src_common_encnames.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_common_hashfn.c` & `pglast-5.3/libpg_query/src/postgres/src_common_hashfn.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_common_keywords.c` & `pglast-5.3/libpg_query/src/postgres/src_common_keywords.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_common_kwlist_d.h` & `pglast-5.3/libpg_query/src/postgres/src_common_kwlist_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_common_kwlookup.c` & `pglast-5.3/libpg_query/src/postgres/src_common_kwlookup.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_common_pg_prng.c` & `pglast-5.3/libpg_query/src/postgres/src_common_pg_prng.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_common_psprintf.c` & `pglast-5.3/libpg_query/src/postgres/src_common_psprintf.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_common_string.c` & `pglast-5.3/libpg_query/src/postgres/src_common_string.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_common_stringinfo.c` & `pglast-5.3/libpg_query/src/postgres/src_common_stringinfo.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_common_wchar.c` & `pglast-5.3/libpg_query/src/postgres/src_common_wchar.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_pl_plpgsql_src_pl_comp.c` & `pglast-5.3/libpg_query/src/postgres/src_pl_plpgsql_src_pl_comp.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_pl_plpgsql_src_pl_funcs.c` & `pglast-5.3/libpg_query/src/postgres/src_pl_plpgsql_src_pl_funcs.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_pl_plpgsql_src_pl_gram.c` & `pglast-5.3/libpg_query/src/postgres/src_pl_plpgsql_src_pl_gram.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_pl_plpgsql_src_pl_handler.c` & `pglast-5.3/libpg_query/src/postgres/src_pl_plpgsql_src_pl_handler.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_pl_plpgsql_src_pl_reserved_kwlist_d.h` & `pglast-5.3/libpg_query/src/postgres/src_pl_plpgsql_src_pl_reserved_kwlist_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_pl_plpgsql_src_pl_scanner.c` & `pglast-5.3/libpg_query/src/postgres/src_pl_plpgsql_src_pl_scanner.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_pl_plpgsql_src_pl_unreserved_kwlist_d.h` & `pglast-5.3/libpg_query/src/postgres/src_pl_plpgsql_src_pl_unreserved_kwlist_d.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_port_pg_bitutils.c` & `pglast-5.3/libpg_query/src/postgres/src_port_pg_bitutils.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_port_pgsleep.c` & `pglast-5.3/libpg_query/src/postgres/src_port_pgsleep.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_port_pgstrcasecmp.c` & `pglast-5.3/libpg_query/src/postgres/src_port_pgstrcasecmp.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_port_qsort.c` & `pglast-5.3/libpg_query/src/postgres/src_port_qsort.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_port_snprintf.c` & `pglast-5.3/libpg_query/src/postgres/src_port_snprintf.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_port_strerror.c` & `pglast-5.3/libpg_query/src/postgres/src_port_strerror.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/src/postgres/src_port_strnlen.c` & `pglast-5.3/libpg_query/src/postgres/src_port_strnlen.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/srcdata/all_known_enums.json` & `pglast-5.3/libpg_query/srcdata/all_known_enums.json`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/srcdata/enum_defs.json` & `pglast-5.3/libpg_query/srcdata/enum_defs.json`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/srcdata/nodetypes.json` & `pglast-5.3/libpg_query/srcdata/nodetypes.json`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/srcdata/struct_defs.json` & `pglast-5.3/libpg_query/srcdata/struct_defs.json`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/srcdata/typedefs.json` & `pglast-5.3/libpg_query/srcdata/typedefs.json`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/advisory_lock.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/advisory_lock.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/aggregates.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/aggregates.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/alter_generic.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/alter_generic.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/alter_operator.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/alter_operator.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/alter_table.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/alter_table.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/amutils.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/amutils.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/arrays.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/arrays.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/async.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/async.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/bit.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/bit.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/bitmapops.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/bitmapops.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/boolean.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/boolean.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/box.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/box.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/brin.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/brin.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/brin_bloom.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/brin_bloom.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/brin_multi.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/brin_multi.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/btree_index.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/btree_index.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/case.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/case.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/char.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/char.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/circle.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/circle.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/cluster.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/cluster.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/collate.icu.utf8.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/collate.icu.utf8.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/collate.linux.utf8.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/collate.linux.utf8.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/collate.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/collate.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/combocid.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/combocid.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/comments.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/comments.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/compression.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/compression.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/constraints.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/constraints.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/conversion.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/conversion.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/copy.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/copy.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/copy2.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/copy2.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/copydml.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/copydml.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/copyselect.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/copyselect.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/create_aggregate.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/create_aggregate.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/create_am.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/create_am.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/create_cast.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/create_cast.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/create_function_c.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/create_function_c.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/create_function_sql.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/create_function_sql.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/create_index.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/create_index.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/create_index_spgist.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/create_index_spgist.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/create_misc.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/create_misc.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/create_operator.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/create_operator.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/create_procedure.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/create_procedure.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/create_role.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/create_role.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/create_table.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/create_table.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/create_table_like.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/create_table_like.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/create_type.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/create_type.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/create_view.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/create_view.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/date.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/date.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/dbsize.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/dbsize.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/delete.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/delete.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/dependency.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/dependency.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/domain.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/domain.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/drop_if_exists.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/drop_if_exists.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/drop_operator.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/drop_operator.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/enum.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/enum.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/equivclass.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/equivclass.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/errors.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/errors.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/event_trigger.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/event_trigger.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/explain.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/explain.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/expressions.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/expressions.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/fast_default.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/fast_default.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/float4.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/float4.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/float8.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/float8.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/foreign_data.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/foreign_data.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/foreign_key.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/foreign_key.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/functional_deps.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/functional_deps.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/generated.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/generated.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/geometry.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/geometry.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/gin.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/gin.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/gist.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/gist.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/groupingsets.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/groupingsets.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/guc.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/guc.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/hash_func.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/hash_func.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/hash_index.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/hash_index.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/hash_part.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/hash_part.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/horology.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/horology.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/identity.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/identity.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/incremental_sort.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/incremental_sort.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/index_including.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/index_including.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/index_including_gist.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/index_including_gist.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/indexing.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/indexing.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/indirect_toast.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/indirect_toast.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/inet.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/inet.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/infinite_recurse.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/infinite_recurse.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/inherit.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/inherit.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/insert.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/insert.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/insert_conflict.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/insert_conflict.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/int2.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/int2.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/int4.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/int4.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/int8.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/int8.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/interval.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/interval.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/join.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/join.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/join_hash.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/join_hash.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/json.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/json.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/json_encoding.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/json_encoding.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/jsonb.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/jsonb.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/jsonb_jsonpath.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/jsonb_jsonpath.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/jsonpath.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/jsonpath.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/jsonpath_encoding.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/jsonpath_encoding.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/largeobject.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/largeobject.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/limit.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/limit.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/line.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/line.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/lock.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/lock.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/lseg.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/lseg.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/macaddr.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/macaddr.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/macaddr8.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/macaddr8.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/matview.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/matview.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/memoize.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/memoize.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/merge.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/merge.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/misc.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/misc.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/misc_functions.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/misc_functions.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/misc_sanity.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/misc_sanity.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/money.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/money.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/multirangetypes.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/multirangetypes.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/mvcc.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/mvcc.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/name.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/name.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/namespace.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/namespace.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/numeric.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/numeric.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/numeric_big.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/numeric_big.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/numerology.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/numerology.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/object_address.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/object_address.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/oid.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/oid.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/oidjoins.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/oidjoins.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/opr_sanity.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/opr_sanity.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/partition_aggregate.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/partition_aggregate.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/partition_info.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/partition_info.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/partition_join.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/partition_join.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/partition_prune.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/partition_prune.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/password.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/password.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/path.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/path.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/pg_lsn.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/pg_lsn.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/plancache.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/plancache.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/plpgsql.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/plpgsql.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/point.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/point.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/polygon.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/polygon.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/polymorphism.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/polymorphism.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/portals.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/portals.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/portals_p2.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/portals_p2.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/prepare.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/prepare.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/prepared_xacts.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/prepared_xacts.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/privileges.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/privileges.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/psql.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/psql.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/psql_crosstab.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/psql_crosstab.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/publication.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/publication.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/random.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/random.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/rangefuncs.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/rangefuncs.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/rangetypes.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/rangetypes.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/regex.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/regex.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/regproc.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/regproc.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/reindex_catalog.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/reindex_catalog.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/reloptions.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/reloptions.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/replica_identity.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/replica_identity.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/returning.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/returning.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/roleattributes.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/roleattributes.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/rowsecurity.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/rowsecurity.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/rowtypes.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/rowtypes.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/rules.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/rules.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/sanity_check.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/sanity_check.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/security_label.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/security_label.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/select.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/select.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/select_distinct.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/select_distinct.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/select_distinct_on.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/select_distinct_on.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/select_having.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/select_having.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/select_implicit.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/select_implicit.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/select_into.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/select_into.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/select_parallel.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/select_parallel.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/select_views.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/select_views.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/sequence.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/sequence.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/spgist.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/spgist.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/stats.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/stats.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/stats_ext.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/stats_ext.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/strings.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/strings.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/subscription.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/subscription.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/subselect.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/subselect.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/sysviews.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/sysviews.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/tablesample.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/tablesample.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/tablespace.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/tablespace.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/temp.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/temp.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/test_setup.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/test_setup.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/text.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/text.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/tid.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/tid.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/tidrangescan.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/tidrangescan.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/tidscan.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/tidscan.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/time.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/time.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/timestamp.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/timestamp.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/timestamptz.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/timestamptz.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/timetz.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/timetz.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/transactions.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/transactions.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/triggers.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/triggers.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/truncate.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/truncate.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/tsdicts.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/tsdicts.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/tsearch.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/tsearch.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/tsrf.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/tsrf.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/tstypes.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/tstypes.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/tuplesort.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/tuplesort.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/txid.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/txid.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/type_sanity.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/type_sanity.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/typed_table.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/typed_table.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/unicode.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/unicode.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/union.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/union.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/updatable_views.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/updatable_views.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/update.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/update.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/uuid.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/uuid.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/vacuum.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/vacuum.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/vacuum_parallel.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/vacuum_parallel.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/varchar.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/varchar.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/window.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/window.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/with.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/with.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/write_parallel.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/write_parallel.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/xid.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/xid.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/xml.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/xml.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/test/sql/postgres_regress/xmlmap.sql` & `pglast-5.3/libpg_query/test/sql/postgres_regress/xmlmap.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/vendor/protobuf-c/protobuf-c.c` & `pglast-5.3/libpg_query/vendor/protobuf-c/protobuf-c.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/vendor/protobuf-c/protobuf-c.h` & `pglast-5.3/libpg_query/vendor/protobuf-c/protobuf-c.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/vendor/xxhash/xxhash.c` & `pglast-5.3/libpg_query/vendor/xxhash/xxhash.c`

 * *Files identical despite different names*

### Comparing `pglast-5.2/libpg_query/vendor/xxhash/xxhash.h` & `pglast-5.3/libpg_query/vendor/xxhash/xxhash.h`

 * *Files identical despite different names*

### Comparing `pglast-5.2/pglast/__init__.py` & `pglast-5.3/pglast/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     from .parser import fingerprint, get_postgresql_version, parse_sql, scan, split
 except ModuleNotFoundError:  # pragma: no cover
     # bootstrap
     pass
 
 
 # This is injected automatically at release time
-__version__ = 'v5.2'
+__version__ = 'v5.3'
 "Package's version."
 
 __author__ = 'Lele Gaifax <lele@metapensiero.it>'
 "Package's author."
 
 
 def parse_plpgsql(statement):
```

### Comparing `pglast-5.2/pglast/__main__.py` & `pglast-5.3/pglast/__main__.py`

 * *Files identical despite different names*

### Comparing `pglast-5.2/pglast/ast.py` & `pglast-5.3/pglast/ast.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# :Project:   pglast -- DO NOT EDIT: automatically extracted from struct_defs.json @ 15-4.2.1-0-g1f2d166
+# :Project:   pglast -- DO NOT EDIT: automatically extracted from struct_defs.json @ 15-4.2.3-0-g9b21e32
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
 # :Copyright: © 2021-2023 Lele Gaifax
 #
 
 from collections import namedtuple
 from decimal import Decimal
```

### Comparing `pglast-5.2/pglast/ast.pyx` & `pglast-5.3/pglast/ast.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# :Project:   pglast -- DO NOT EDIT: automatically extracted from struct_defs.json @ 15-4.2.1-0-g1f2d166
+# :Project:   pglast -- DO NOT EDIT: automatically extracted from struct_defs.json @ 15-4.2.3-0-g9b21e32
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
 # :Copyright: © 2021-2023 Lele Gaifax
 #
 
 #cython: language_level=3
```

### Comparing `pglast-5.2/pglast/enums/__init__.py` & `pglast-5.3/pglast/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `pglast-5.2/pglast/enums/lockdefs.py` & `pglast-5.3/pglast/enums/lockdefs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# :Project:   pglast -- DO NOT EDIT: automatically extracted from lockdefs.h @ 15-4.2.1-0-g1f2d166
+# :Project:   pglast -- DO NOT EDIT: automatically extracted from lockdefs.h @ 15-4.2.3-0-g9b21e32
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
 # :Copyright: © 2017-2023 Lele Gaifax
 #
 
 from enum import Enum, IntEnum, IntFlag, auto
```

### Comparing `pglast-5.2/pglast/enums/lockoptions.py` & `pglast-5.3/pglast/enums/lockoptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# :Project:   pglast -- DO NOT EDIT: automatically extracted from lockoptions.h @ 15-4.2.1-0-g1f2d166
+# :Project:   pglast -- DO NOT EDIT: automatically extracted from lockoptions.h @ 15-4.2.3-0-g9b21e32
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
 # :Copyright: © 2017-2023 Lele Gaifax
 #
 
 from enum import Enum, IntEnum, IntFlag, auto
```

### Comparing `pglast-5.2/pglast/enums/nodes.py` & `pglast-5.3/pglast/enums/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# :Project:   pglast -- DO NOT EDIT: automatically extracted from nodes.h @ 15-4.2.1-0-g1f2d166
+# :Project:   pglast -- DO NOT EDIT: automatically extracted from nodes.h @ 15-4.2.3-0-g9b21e32
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
 # :Copyright: © 2017-2023 Lele Gaifax
 #
 
 from enum import Enum, IntEnum, IntFlag, auto
```

### Comparing `pglast-5.2/pglast/enums/parsenodes.py` & `pglast-5.3/pglast/enums/parsenodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# :Project:   pglast -- DO NOT EDIT: automatically extracted from parsenodes.h @ 15-4.2.1-0-g1f2d166
+# :Project:   pglast -- DO NOT EDIT: automatically extracted from parsenodes.h @ 15-4.2.3-0-g9b21e32
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
 # :Copyright: © 2017-2023 Lele Gaifax
 #
 
 from enum import Enum, IntEnum, IntFlag, auto
```

### Comparing `pglast-5.2/pglast/enums/pg_am.py` & `pglast-5.3/pglast/enums/pg_am.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# :Project:   pglast -- DO NOT EDIT: automatically extracted from pg_am.h @ 15-4.2.1-0-g1f2d166
+# :Project:   pglast -- DO NOT EDIT: automatically extracted from pg_am.h @ 15-4.2.3-0-g9b21e32
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
 # :Copyright: © 2017-2023 Lele Gaifax
 #
 
 from enum import Enum, IntEnum, IntFlag, auto
```

### Comparing `pglast-5.2/pglast/enums/pg_attribute.py` & `pglast-5.3/pglast/enums/pg_attribute.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# :Project:   pglast -- DO NOT EDIT: automatically extracted from pg_attribute.h @ 15-4.2.1-0-g1f2d166
+# :Project:   pglast -- DO NOT EDIT: automatically extracted from pg_attribute.h @ 15-4.2.3-0-g9b21e32
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
 # :Copyright: © 2017-2023 Lele Gaifax
 #
 
 from enum import Enum, IntEnum, IntFlag, auto
```

### Comparing `pglast-5.2/pglast/enums/pg_class.py` & `pglast-5.3/pglast/enums/pg_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# :Project:   pglast -- DO NOT EDIT: automatically extracted from pg_class.h @ 15-4.2.1-0-g1f2d166
+# :Project:   pglast -- DO NOT EDIT: automatically extracted from pg_class.h @ 15-4.2.3-0-g9b21e32
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
 # :Copyright: © 2017-2023 Lele Gaifax
 #
 
 from enum import Enum, IntEnum, IntFlag, auto
```

### Comparing `pglast-5.2/pglast/enums/pg_trigger.py` & `pglast-5.3/pglast/enums/pg_trigger.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# :Project:   pglast -- DO NOT EDIT: automatically extracted from pg_trigger.h @ 15-4.2.1-0-g1f2d166
+# :Project:   pglast -- DO NOT EDIT: automatically extracted from pg_trigger.h @ 15-4.2.3-0-g9b21e32
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
 # :Copyright: © 2017-2023 Lele Gaifax
 #
 
 from enum import Enum, IntEnum, IntFlag, auto
```

### Comparing `pglast-5.2/pglast/enums/primnodes.py` & `pglast-5.3/pglast/enums/primnodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# :Project:   pglast -- DO NOT EDIT: automatically extracted from primnodes.h @ 15-4.2.1-0-g1f2d166
+# :Project:   pglast -- DO NOT EDIT: automatically extracted from primnodes.h @ 15-4.2.3-0-g9b21e32
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
 # :Copyright: © 2017-2023 Lele Gaifax
 #
 
 from enum import Enum, IntEnum, IntFlag, auto
```

### Comparing `pglast-5.2/pglast/enums/xml.py` & `pglast-5.3/pglast/enums/xml.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# :Project:   pglast -- DO NOT EDIT: automatically extracted from xml.h @ 15-4.2.1-0-g1f2d166
+# :Project:   pglast -- DO NOT EDIT: automatically extracted from xml.h @ 15-4.2.3-0-g9b21e32
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
 # :Copyright: © 2017-2023 Lele Gaifax
 #
 
 from enum import Enum, IntEnum, IntFlag, auto
```

### Comparing `pglast-5.2/pglast/keywords.py` & `pglast-5.3/pglast/keywords.py`

 * *Files identical despite different names*

### Comparing `pglast-5.2/pglast/parser.c` & `pglast-5.3/pglast/parser.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.0b2 */
+/* Generated by Cython 3.0.0 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "libpg_query/pg_query.h",
             "libpg_query/protobuf/pg_query.pb-c.h",
@@ -44,18 +44,18 @@
 
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "3_0_0b2"
+#define CYTHON_ABI "3_0_0"
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030000B2
+#define CYTHON_HEX_VERSION 0x030000F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -181,20 +181,24 @@
   #undef CYTHON_METH_FASTCALL
   #define CYTHON_METH_FASTCALL 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
   #ifndef CYTHON_PEP487_INIT_SUBCLASS
     #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
   #endif
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_MODULE_STATE
   #define CYTHON_USE_MODULE_STATE 0
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -346,15 +350,15 @@
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_GIL
-    #define CYTHON_FAST_GIL (PY_MAJOR_VERSION < 3 || PY_VERSION_HEX >= 0x03060000)
+    #define CYTHON_FAST_GIL (PY_MAJOR_VERSION < 3 || PY_VERSION_HEX >= 0x03060000 && PY_VERSION_HEX < 0x030C00A6)
   #endif
   #ifndef CYTHON_METH_FASTCALL
     #define CYTHON_METH_FASTCALL (PY_VERSION_HEX >= 0x030700A1)
   #endif
   #ifndef CYTHON_FAST_PYCALL
     #define CYTHON_FAST_PYCALL 1
   #endif
@@ -525,14 +529,26 @@
   #if defined(__clang__) && defined(__apple_build_version__)
     #if __apple_build_version__ < 7000000
       #undef  CYTHON_FALLTHROUGH
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
 #endif
+#ifdef __cplusplus
+  template <typename T>
+  struct __PYX_IS_UNSIGNED_IMPL {static const bool value = T(0) < T(-1);};
+  #define __PYX_IS_UNSIGNED(type) (__PYX_IS_UNSIGNED_IMPL<type>::value)
+#else
+  #define __PYX_IS_UNSIGNED(type) (((type)-1) > 0)
+#endif
+#if CYTHON_COMPILING_IN_PYPY == 1
+  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x030A0000)
+#else
+  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000)
+#endif
 #define __PYX_REINTERPRET_FUNCION(func_pointer, other_pointer) ((func_pointer)(void(*)(void))(other_pointer))
 
 #ifndef CYTHON_INLINE
   #if defined(__clang__)
     #define CYTHON_INLINE __inline__ __attribute__ ((__unused__))
   #elif defined(__GNUC__)
     #define CYTHON_INLINE __inline__
@@ -541,17 +557,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_DefaultClassType PyClass_Type
   #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
@@ -560,18 +573,18 @@
   #define __Pyx_DefaultClassType PyType_Type
 #if PY_VERSION_HEX >= 0x030B00A1
     static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
-        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *empty=NULL;
         const char *fn_cstr=NULL;
         const char *name_cstr=NULL;
-        PyCodeObject* co=NULL;
+        PyCodeObject *co=NULL, *result=NULL;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         if (!(kwds=PyDict_New())) goto end;
         if (!(argcount=PyLong_FromLong(a))) goto end;
         if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
         if (!(posonlyargcount=PyLong_FromLong(p))) goto end;
         if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
@@ -589,39 +602,31 @@
         if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
         if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
         if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
         if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
         if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
         if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
         if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
-        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
-        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
-        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
-        Py_XDECREF((PyObject*)co);
-        co = (PyCodeObject*)call_result;
-        call_result = NULL;
-        if (0) {
-            cleanup_code_too:
-            Py_XDECREF((PyObject*)co);
-            co = NULL;
-        }
-        end:
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto end;
+        if (!(empty = PyTuple_New(0))) goto end;
+        result = (PyCodeObject*) PyObject_Call(replace, empty, kwds);
+    end:
+        Py_XDECREF((PyObject*) co);
         Py_XDECREF(kwds);
         Py_XDECREF(argcount);
         Py_XDECREF(posonlyargcount);
         Py_XDECREF(kwonlyargcount);
         Py_XDECREF(nlocals);
         Py_XDECREF(stacksize);
         Py_XDECREF(replace);
-        Py_XDECREF(call_result);
         Py_XDECREF(empty);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
-        return co;
+        return result;
     }
 #elif PY_VERSION_HEX >= 0x030800B2 && !CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_NewWithPosOnlyArgs(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
   #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
@@ -649,14 +654,19 @@
 #endif
 #if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsFalse)
   #define __Pyx_Py_IsFalse(ob) Py_IsFalse(ob)
 #else
   #define __Pyx_Py_IsFalse(ob) __Pyx_Py_Is((ob), Py_False)
 #endif
 #define __Pyx_NoneAsNull(obj)  (__Pyx_Py_IsNone(obj) ? NULL : (obj))
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef CO_COROUTINE
   #define CO_COROUTINE 0x80
 #endif
 #ifndef CO_ASYNC_GENERATOR
   #define CO_ASYNC_GENERATOR 0x200
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -874,15 +884,15 @@
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
 #endif
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define CYTHON_PEP393_ENABLED 1
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GetLength(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_ReadChar(u, i)
-  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((void)u, 1114111)
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((void)u, 1114111U)
   #define __Pyx_PyUnicode_KIND(u)         ((void)u, (0))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)u)
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)k, PyUnicode_ReadChar((PyObject*)(d), i))
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GetLength(u))
 #elif PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
   #if PY_VERSION_HEX >= 0x030C0000
@@ -893,15 +903,15 @@
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         ((int)PyUnicode_KIND(u))
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, (Py_UCS4) ch)
   #if PY_VERSION_HEX >= 0x030C0000
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
     #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
     #else
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
@@ -911,19 +921,19 @@
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) ((Py_UCS4)(PyUnicode_AS_UNICODE(u)[i]))
-  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535 : 1114111)
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535U : 1114111U)
   #define __Pyx_PyUnicode_KIND(u)         ((int)sizeof(Py_UNICODE))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)PyUnicode_AS_UNICODE(u))
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)(k), (Py_UCS4)(((Py_UNICODE*)d)[i]))
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = (Py_UNICODE) ch)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_SIZE(u))
 #endif
 #if CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyUnicode_Concat(a, b)      PyNumber_Add(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  PyNumber_Add(a, b)
 #else
   #define __Pyx_PyUnicode_Concat(a, b)      PyUnicode_Concat(a, b)
@@ -1071,15 +1081,24 @@
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
     { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
-#ifndef __PYX_EXTERN_C
+#ifdef CYTHON_EXTERN_C
+    #undef __PYX_EXTERN_C
+    #define __PYX_EXTERN_C CYTHON_EXTERN_C
+#elif defined(__PYX_EXTERN_C)
+    #ifdef _MSC_VER
+    #pragma message ("Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.")
+    #else
+    #warning Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.
+    #endif
+#else
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
@@ -1189,14 +1208,15 @@
 static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
 {
     const Py_UNICODE *u_end = u;
     while (*u_end++) ;
     return (size_t)(u_end - u - 1);
 }
 #endif
+#define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
 #define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
 #define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
@@ -1215,14 +1235,53 @@
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
 #define __Pyx_PyNumber_Int(x) (PyLong_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Long(x))
 #else
 #define __Pyx_PyNumber_Int(x) (PyInt_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Int(x))
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
+  #if PY_VERSION_HEX >= 0x030C00A7
+  #ifndef _PyLong_SIGN_MASK
+    #define _PyLong_SIGN_MASK 3
+  #endif
+  #ifndef _PyLong_NON_SIZE_BITS
+    #define _PyLong_NON_SIZE_BITS 3
+  #endif
+  #define __Pyx_PyLong_Sign(x)  (((PyLongObject*)x)->long_value.lv_tag & _PyLong_SIGN_MASK)
+  #define __Pyx_PyLong_IsNeg(x)  ((__Pyx_PyLong_Sign(x) & 2) != 0)
+  #define __Pyx_PyLong_IsNonNeg(x)  (!__Pyx_PyLong_IsNeg(x))
+  #define __Pyx_PyLong_IsZero(x)  (__Pyx_PyLong_Sign(x) & 1)
+  #define __Pyx_PyLong_IsPos(x)  (__Pyx_PyLong_Sign(x) == 0)
+  #define __Pyx_PyLong_CompactValueUnsigned(x)  (__Pyx_PyLong_Digits(x)[0])
+  #define __Pyx_PyLong_DigitCount(x)  ((Py_ssize_t) (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS))
+  #define __Pyx_PyLong_SignedDigitCount(x)\
+        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * __Pyx_PyLong_DigitCount(x))
+  #if defined(PyUnstable_Long_IsCompact) && defined(PyUnstable_Long_CompactValue)
+    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact((PyLongObject*) x)
+    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
+  #else
+    #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
+    #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
+  #endif
+  typedef Py_ssize_t  __Pyx_compact_pylong;
+  typedef size_t  __Pyx_compact_upylong;
+  #else  // Py < 3.12
+  #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
+  #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
+  #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
+  #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
+  #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
+  #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
+  #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
+  #define __Pyx_PyLong_IsCompact(x)  (Py_SIZE(x) == 0 || Py_SIZE(x) == 1 || Py_SIZE(x) == -1)
+  #define __Pyx_PyLong_CompactValue(x)\
+        ((Py_SIZE(x) == 0) ? (sdigit) 0 : ((Py_SIZE(x) < 0) ? -(sdigit)__Pyx_PyLong_Digits(x)[0] : (sdigit)__Pyx_PyLong_Digits(x)[0]))
+  typedef sdigit  __Pyx_compact_pylong;
+  typedef digit  __Pyx_compact_upylong;
+  #endif
   #if PY_VERSION_HEX >= 0x030C00A5
   #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->long_value.ob_digit)
   #else
   #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->ob_digit)
   #endif
 #endif
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
@@ -1242,15 +1301,15 @@
     if (!default_encoding_c) goto bad;
     if (strcmp(default_encoding_c, "ascii") == 0) {
         __Pyx_sys_getdefaultencoding_not_ascii = 0;
     } else {
         char ascii_chars[128];
         int c;
         for (c = 0; c < 128; c++) {
-            ascii_chars[c] = c;
+            ascii_chars[c] = (char) c;
         }
         __Pyx_sys_getdefaultencoding_not_ascii = 1;
         ascii_chars_u = PyUnicode_DecodeASCII(ascii_chars, 128, NULL);
         if (!ascii_chars_u) goto bad;
         ascii_chars_b = PyUnicode_AsEncodedString(ascii_chars_u, default_encoding_c, NULL);
         if (!ascii_chars_b || !PyBytes_Check(ascii_chars_b) || memcmp(ascii_chars, PyBytes_AS_STRING(ascii_chars_b), 128) != 0) {
             PyErr_Format(
@@ -1468,31 +1527,38 @@
 #define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
 #endif
 
 /* PyThreadStateGet.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
 #define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
-#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
+#if PY_VERSION_HEX >= 0x030C00A6
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->current_exception != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->current_exception ? (PyObject*) Py_TYPE(__pyx_tstate->current_exception) : (PyObject*) NULL)
+#else
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->curexc_type != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->curexc_type)
+#endif
 #else
 #define __Pyx_PyThreadState_declare
 #define __Pyx_PyThreadState_assign
-#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
+#define __Pyx_PyErr_Occurred()  (PyErr_Occurred() != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  PyErr_Occurred()
 #endif
 
 /* PyErrFetchRestore.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
 #define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
 #define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
 #define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
 static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A6
 #define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
 #else
 #define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
 #endif
 #else
 #define __Pyx_PyErr_Clear() PyErr_Clear()
 #define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
@@ -1804,15 +1870,15 @@
 #define __Pyx_ExceptionSwap(type, value, tb)  __Pyx__ExceptionSwap(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
 static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb);
 #endif
 
 /* GetTopmostException.proto */
-#if CYTHON_USE_EXC_INFO_STACK
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
 /* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
@@ -1910,30 +1976,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-#if __STDC_VERSION__ >= 201112L
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0
+#define __PYX_HAVE_RT_ImportType_proto_3_0_0
+#if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
-#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_3_0_0 {
+   __Pyx_ImportType_CheckSize_Error_3_0_0 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_0 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_0 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size);
 #endif
 
 /* Py3UpdateBases.proto */
 static PyObject* __Pyx_PEP560_update_bases(PyObject *bases);
 
 /* CalculateMetaclass.proto */
 static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases);
@@ -2335,15 +2401,15 @@
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *type1, PyObject *type2);
 #else
 #define __Pyx_TypeCheck(obj, type) PyObject_TypeCheck(obj, (PyTypeObject *)type)
 #define __Pyx_TypeCheck2(obj, type1, type2) (PyObject_TypeCheck(obj, (PyTypeObject *)type1) || PyObject_TypeCheck(obj, (PyTypeObject *)type2))
 #define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
-#define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_Occurred(), err1, err2)
+#define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_CurrentExceptionType(), err1, err2)
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
@@ -53634,15 +53700,15 @@
     /* "pglast/parser.pyx":213
  *         disps = []
  *         for c in s:
  *             c_len_in_utf8 = len(c.encode('utf-8'))             # <<<<<<<<<<<<<<
  *             if c_len_in_utf8 > 1:
  *                 while c_len_in_utf8 > 0:
  */
-    __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 213, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyUnicode_FromOrdinal(__pyx_v_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 213, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_9 = PyUnicode_AsUTF8String(((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 213, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_10 = PyBytes_GET_SIZE(__pyx_t_9); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1))) __PYX_ERR(1, 213, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __pyx_v_c_len_in_utf8 = __pyx_t_10;
@@ -59338,15 +59404,15 @@
   p->displacements = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_6pglast_6parser_Displacements(PyObject *o) {
   struct __pyx_obj_6pglast_6parser_Displacements *p = (struct __pyx_obj_6pglast_6parser_Displacements *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !_PyGC_FINALIZED(o)) {
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_6pglast_6parser_Displacements) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->displacements);
@@ -59463,21 +59529,21 @@
   #else
   NULL, /*tp_finalize*/
   #endif
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+  #if __PYX_NEED_TP_PRINT_SLOT == 1
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030C0000
   0, /*tp_watched*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
@@ -60212,24 +60278,23 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -60936,15 +61001,15 @@
   return;
   #endif
 }
 /* #### Code section: cleanup_globals ### */
 /* #### Code section: cleanup_module ### */
 /* #### Code section: main_method ### */
 /* #### Code section: utility_code_pragmas ### */
-#if _MSC_VER
+#ifdef _MSC_VER
 #pragma warning( push )
 /* Warning 4127: conditional expression is constant
  * Cython uses constant conditional expressions to allow in inline functions to be optimized at
  * compile-time, so this warning is not useful
  */
 #pragma warning( disable : 4127 )
 #endif
@@ -60983,44 +61048,95 @@
 #endif
     for (i=0; i<n; i++) {
         if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
     }
     return 0;
 }
 static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
-    PyObject *exc_type = tstate->curexc_type;
+    int result;
+    PyObject *exc_type;
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *current_exception = tstate->current_exception;
+    if (unlikely(!current_exception)) return 0;
+    exc_type = (PyObject*) Py_TYPE(current_exception);
+    if (exc_type == err) return 1;
+#else
+    exc_type = tstate->curexc_type;
     if (exc_type == err) return 1;
     if (unlikely(!exc_type)) return 0;
-    if (unlikely(PyTuple_Check(err)))
-        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
-    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+#endif
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_INCREF(exc_type);
+    #endif
+    if (unlikely(PyTuple_Check(err))) {
+        result = __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
+    } else {
+        result = __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+    }
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_DECREF(exc_type);
+    #endif
+    return result;
 }
 #endif
 
 /* PyErrFetchRestore */
 #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *tmp_value;
+    assert(type == NULL || (value != NULL && type == (PyObject*) Py_TYPE(value)));
+    if (value) {
+        #if CYTHON_COMPILING_IN_CPYTHON
+        if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
+        #endif
+            PyException_SetTraceback(value, tb);
+    }
+    tmp_value = tstate->current_exception;
+    tstate->current_exception = value;
+    Py_XDECREF(tmp_value);
+#else
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     tmp_type = tstate->curexc_type;
     tmp_value = tstate->curexc_value;
     tmp_tb = tstate->curexc_traceback;
     tstate->curexc_type = type;
     tstate->curexc_value = value;
     tstate->curexc_traceback = tb;
     Py_XDECREF(tmp_type);
     Py_XDECREF(tmp_value);
     Py_XDECREF(tmp_tb);
+#endif
 }
 static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject* exc_value;
+    exc_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    *value = exc_value;
+    *type = NULL;
+    *tb = NULL;
+    if (exc_value) {
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        #if CYTHON_COMPILING_IN_CPYTHON
+        *tb = ((PyBaseExceptionObject*) exc_value)->traceback;
+        Py_XINCREF(*tb);
+        #else
+        *tb = PyException_GetTraceback(exc_value);
+        #endif
+    }
+#else
     *type = tstate->curexc_type;
     *value = tstate->curexc_value;
     *tb = tstate->curexc_traceback;
     tstate->curexc_type = 0;
     tstate->curexc_value = 0;
     tstate->curexc_traceback = 0;
+#endif
 }
 #endif
 
 /* PyObjectGetAttrStr */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name) {
     PyTypeObject* tp = Py_TYPE(obj);
@@ -61569,15 +61685,17 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_FAST_THREAD_STATE
+      #if PY_VERSION_HEX >= 0x030C00A6
+        PyException_SetTraceback(value, tb);
+      #elif CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
@@ -62111,45 +62229,24 @@
     PyErr_Format(PyExc_ValueError,
                  "need more than %" CYTHON_FORMAT_SSIZE_T "d value%.1s to unpack",
                  index, (index == 1) ? "" : "s");
 }
 
 /* IterFinish */
 static CYTHON_INLINE int __Pyx_IterFinish(void) {
-#if CYTHON_FAST_THREAD_STATE
-    PyThreadState *tstate = __Pyx_PyThreadState_Current;
-    PyObject* exc_type = tstate->curexc_type;
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    PyObject* exc_type = __Pyx_PyErr_CurrentExceptionType();
     if (unlikely(exc_type)) {
-        if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) {
-            PyObject *exc_value, *exc_tb;
-            exc_value = tstate->curexc_value;
-            exc_tb = tstate->curexc_traceback;
-            tstate->curexc_type = 0;
-            tstate->curexc_value = 0;
-            tstate->curexc_traceback = 0;
-            Py_DECREF(exc_type);
-            Py_XDECREF(exc_value);
-            Py_XDECREF(exc_tb);
-            return 0;
-        } else {
+        if (unlikely(!__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration)))
             return -1;
-        }
-    }
-    return 0;
-#else
-    if (unlikely(PyErr_Occurred())) {
-        if (likely(PyErr_ExceptionMatches(PyExc_StopIteration))) {
-            PyErr_Clear();
-            return 0;
-        } else {
-            return -1;
-        }
+        __Pyx_PyErr_Clear();
+        return 0;
     }
     return 0;
-#endif
 }
 
 /* UnpackItemEndCheck */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
     if (unlikely(retval)) {
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
@@ -62243,28 +62340,40 @@
 /* GetException */
 #if CYTHON_FAST_THREAD_STATE
 static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
 #else
 static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
 #endif
 {
-    PyObject *local_type, *local_value, *local_tb;
+    PyObject *local_type = NULL, *local_value, *local_tb = NULL;
 #if CYTHON_FAST_THREAD_STATE
     PyObject *tmp_type, *tmp_value, *tmp_tb;
+  #if PY_VERSION_HEX >= 0x030C00A6
+    local_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    if (likely(local_value)) {
+        local_type = (PyObject*) Py_TYPE(local_value);
+        Py_INCREF(local_type);
+        local_tb = PyException_GetTraceback(local_value);
+    }
+  #else
     local_type = tstate->curexc_type;
     local_value = tstate->curexc_value;
     local_tb = tstate->curexc_traceback;
     tstate->curexc_type = 0;
     tstate->curexc_value = 0;
     tstate->curexc_traceback = 0;
+  #endif
 #else
     PyErr_Fetch(&local_type, &local_value, &local_tb);
 #endif
     PyErr_NormalizeException(&local_type, &local_value, &local_tb);
-#if CYTHON_FAST_THREAD_STATE
+#if CYTHON_FAST_THREAD_STATE && PY_VERSION_HEX >= 0x030C00A6
+    if (unlikely(tstate->current_exception))
+#elif CYTHON_FAST_THREAD_STATE
     if (unlikely(tstate->curexc_type))
 #else
     if (unlikely(PyErr_Occurred()))
 #endif
         goto bad;
     #if PY_MAJOR_VERSION >= 3
     if (local_tb) {
@@ -62335,15 +62444,20 @@
         Py_XDECREF(tmp_value);
         tmp_value = NULL;
         tmp_type = NULL;
         tmp_tb = NULL;
     } else {
         tmp_type = (PyObject*) Py_TYPE(tmp_value);
         Py_INCREF(tmp_type);
+        #if CYTHON_COMPILING_IN_CPYTHON
+        tmp_tb = ((PyBaseExceptionObject*) tmp_value)->traceback;
+        Py_XINCREF(tmp_tb);
+        #else
         tmp_tb = PyException_GetTraceback(tmp_value);
+        #endif
     }
   #elif CYTHON_USE_EXC_INFO_STACK
     _PyErr_StackItem *exc_info = tstate->exc_info;
     tmp_type = exc_info->exc_type;
     tmp_value = exc_info->exc_value;
     tmp_tb = exc_info->exc_traceback;
     exc_info->exc_type = *type;
@@ -62369,15 +62483,15 @@
     *type = tmp_type;
     *value = tmp_value;
     *tb = tmp_tb;
 }
 #endif
 
 /* GetTopmostException */
-#if CYTHON_USE_EXC_INFO_STACK
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
     while ((exc_info->exc_value == NULL || exc_info->exc_value == Py_None) &&
            exc_info->previous_item != NULL)
     {
@@ -62685,37 +62799,36 @@
     CYTHON_UNUSED_VAR(zerodivision_check);
     #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_CheckExact(op1))) {
         const long b = intval;
         long x;
         long a = PyInt_AS_LONG(op1);
         
-            x = (long)((unsigned long)a + b);
+            x = (long)((unsigned long)a + (unsigned long)b);
             if (likely((x^a) >= 0 || (x^b) >= 0))
                 return PyInt_FromLong(x);
             return PyLong_Type.tp_as_number->nb_add(op1, op2);
     }
     #endif
     #if CYTHON_USE_PYLONG_INTERNALS
     if (likely(PyLong_CheckExact(op1))) {
         const long b = intval;
         long a, x;
 #ifdef HAVE_LONG_LONG
         const PY_LONG_LONG llb = intval;
         PY_LONG_LONG lla, llx;
 #endif
-        const digit* digits = __Pyx_PyLong_Digits(op1);
-        const Py_ssize_t size = Py_SIZE(op1);
-        if (unlikely(size == 0)) {
+        if (unlikely(__Pyx_PyLong_IsZero(op1))) {
             return __Pyx_NewRef(op2);
         }
-        if (likely(__Pyx_sst_abs(size) <= 1)) {
-            a = likely(size) ? digits[0] : 0;
-            if (size == -1) a = -a;
+        if (likely(__Pyx_PyLong_IsCompact(op1))) {
+            a = __Pyx_PyLong_CompactValue(op1);
         } else {
+            const digit* digits = __Pyx_PyLong_Digits(op1);
+            const Py_ssize_t size = __Pyx_PyLong_SignedDigitCount(op1);
             switch (size) {
                 case -2:
                     if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
                         a = -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
                         break;
                     #ifdef HAVE_LONG_LONG
                     } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
@@ -63420,18 +63533,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_0
+#define __PYX_HAVE_RT_ImportType_3_0_0
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -63477,23 +63590,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_0 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_0 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -64593,21 +64706,21 @@
     0,
 #if PY_VERSION_HEX >= 0x030400a1
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+#if __PYX_NEED_TP_PRINT_SLOT
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030C0000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 #endif
 static int __pyx_CyFunction_init(PyObject *module) {
 #if CYTHON_USE_TYPE_SPECS
     __pyx_CyFunctionType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx_CyFunctionType_spec, NULL);
@@ -65236,48 +65349,53 @@
             return (unsigned long) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = __Pyx_PyLong_Digits(x);
-            switch (Py_SIZE(x)) {
-                case  0: return (unsigned long) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(unsigned long, digit, digits[0])
-                case 2:
-                    if ((8 * sizeof(unsigned long) > 1 * PyLong_SHIFT)) {
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(unsigned long, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(unsigned long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned long) >= 2 * PyLong_SHIFT)) {
+                                return (unsigned long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                            }
+                        }
+                        break;
+                    case 3:
                         if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(unsigned long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(unsigned long) >= 2 * PyLong_SHIFT)) {
-                            return (unsigned long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned long) >= 3 * PyLong_SHIFT)) {
+                                return (unsigned long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                        break;
+                    case 4:
                         if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(unsigned long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(unsigned long) >= 3 * PyLong_SHIFT)) {
-                            return (unsigned long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned long) >= 4 * PyLong_SHIFT)) {
+                                return (unsigned long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(unsigned long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(unsigned long) >= 4 * PyLong_SHIFT)) {
-                            return (unsigned long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -65291,108 +65409,180 @@
 #ifdef HAVE_LONG_LONG
             } else if ((sizeof(unsigned long) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(unsigned long, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = __Pyx_PyLong_Digits(x);
-            switch (Py_SIZE(x)) {
-                case  0: return (unsigned long) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(unsigned long, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(unsigned long,  digit, +digits[0])
-                case -2:
-                    if ((8 * sizeof(unsigned long) - 1 > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(unsigned long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(unsigned long) - 1 > 2 * PyLong_SHIFT)) {
-                            return (unsigned long) (((unsigned long)-1)*(((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(unsigned long, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(unsigned long) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (unsigned long) (((unsigned long)-1)*(((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if ((8 * sizeof(unsigned long) > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(unsigned long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(unsigned long) - 1 > 2 * PyLong_SHIFT)) {
-                            return (unsigned long) ((((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(unsigned long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (unsigned long) ((((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if ((8 * sizeof(unsigned long) - 1 > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(unsigned long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(unsigned long) - 1 > 3 * PyLong_SHIFT)) {
-                            return (unsigned long) (((unsigned long)-1)*(((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(unsigned long) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (unsigned long) (((unsigned long)-1)*(((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(unsigned long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(unsigned long) - 1 > 3 * PyLong_SHIFT)) {
-                            return (unsigned long) ((((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (unsigned long) ((((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if ((8 * sizeof(unsigned long) - 1 > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(unsigned long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(unsigned long) - 1 > 4 * PyLong_SHIFT)) {
-                            return (unsigned long) (((unsigned long)-1)*(((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(unsigned long) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (unsigned long) (((unsigned long)-1)*(((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(unsigned long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(unsigned long) - 1 > 4 * PyLong_SHIFT)) {
-                            return (unsigned long) ((((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (unsigned long) ((((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
             if ((sizeof(unsigned long) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(unsigned long, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
             } else if ((sizeof(unsigned long) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(unsigned long, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if (CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available, cannot convert large numbers");
-#else
             unsigned long val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (unsigned long) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (unsigned long) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (unsigned long) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (unsigned long) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (unsigned long) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(unsigned long) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((unsigned long) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(unsigned long) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((unsigned long) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((unsigned long) 1) << (sizeof(unsigned long) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (unsigned long) -1;
         }
     } else {
         unsigned long val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (unsigned long) -1;
         val = __Pyx_PyInt_As_unsigned_long(tmp);
@@ -65470,48 +65660,53 @@
             return (long) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = __Pyx_PyLong_Digits(x);
-            switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(long, digit, digits[0])
-                case 2:
-                    if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) >= 2 * PyLong_SHIFT)) {
-                            return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 2 * PyLong_SHIFT)) {
+                                return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) >= 3 * PyLong_SHIFT)) {
-                            return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 3 * PyLong_SHIFT)) {
+                                return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) >= 4 * PyLong_SHIFT)) {
-                            return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 4 * PyLong_SHIFT)) {
+                                return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -65525,108 +65720,180 @@
 #ifdef HAVE_LONG_LONG
             } else if ((sizeof(long) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = __Pyx_PyLong_Digits(x);
-            switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(long, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(long,  digit, +digits[0])
-                case -2:
-                    if ((8 * sizeof(long) - 1 > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
-                            return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(long) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
-                            return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
-                            return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
-                            return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
-                            return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
-                            return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
             if ((sizeof(long) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
             } else if ((sizeof(long) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if (CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available, cannot convert large numbers");
-#else
             long val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (long) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (long) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (long) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (long) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (long) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(long) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((long) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(long) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((long) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((long) 1) << (sizeof(long) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (long) -1;
         }
     } else {
         long val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (long) -1;
         val = __Pyx_PyInt_As_long(tmp);
@@ -65704,48 +65971,53 @@
             return (int) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = __Pyx_PyLong_Digits(x);
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(int, digit, digits[0])
-                case 2:
-                    if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) >= 2 * PyLong_SHIFT)) {
-                            return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 2 * PyLong_SHIFT)) {
+                                return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) >= 3 * PyLong_SHIFT)) {
-                            return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 3 * PyLong_SHIFT)) {
+                                return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) >= 4 * PyLong_SHIFT)) {
-                            return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 4 * PyLong_SHIFT)) {
+                                return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -65759,108 +66031,180 @@
 #ifdef HAVE_LONG_LONG
             } else if ((sizeof(int) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = __Pyx_PyLong_Digits(x);
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(int, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(int,  digit, +digits[0])
-                case -2:
-                    if ((8 * sizeof(int) - 1 > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
-                            return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(int) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
-                            return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
-                            return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
-                            return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
-                            return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
-                            return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
             if ((sizeof(int) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
             } else if ((sizeof(int) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if (CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available, cannot convert large numbers");
-#else
             int val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (int) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (int) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (int) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (int) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (int) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(int) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((int) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(int) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((int) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((int) 1) << (sizeof(int) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (int) -1;
         }
     } else {
         int val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (int) -1;
         val = __Pyx_PyInt_As_int(tmp);
@@ -68066,48 +68410,53 @@
             return (size_t) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = __Pyx_PyLong_Digits(x);
-            switch (Py_SIZE(x)) {
-                case  0: return (size_t) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(size_t, digit, digits[0])
-                case 2:
-                    if ((8 * sizeof(size_t) > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(size_t) >= 2 * PyLong_SHIFT)) {
-                            return (size_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(size_t, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(size_t) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(size_t) >= 2 * PyLong_SHIFT)) {
+                                return (size_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if ((8 * sizeof(size_t) > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(size_t) >= 3 * PyLong_SHIFT)) {
-                            return (size_t) (((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(size_t) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(size_t) >= 3 * PyLong_SHIFT)) {
+                                return (size_t) (((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if ((8 * sizeof(size_t) > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(size_t) >= 4 * PyLong_SHIFT)) {
-                            return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(size_t) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(size_t) >= 4 * PyLong_SHIFT)) {
+                                return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -68121,108 +68470,180 @@
 #ifdef HAVE_LONG_LONG
             } else if ((sizeof(size_t) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(size_t, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = __Pyx_PyLong_Digits(x);
-            switch (Py_SIZE(x)) {
-                case  0: return (size_t) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(size_t, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(size_t,  digit, +digits[0])
-                case -2:
-                    if ((8 * sizeof(size_t) - 1 > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT)) {
-                            return (size_t) (((size_t)-1)*(((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(size_t, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(size_t) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT)) {
+                                return (size_t) (((size_t)-1)*(((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if ((8 * sizeof(size_t) > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT)) {
-                            return (size_t) ((((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(size_t) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT)) {
+                                return (size_t) ((((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if ((8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT)) {
-                            return (size_t) (((size_t)-1)*(((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT)) {
+                                return (size_t) (((size_t)-1)*(((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if ((8 * sizeof(size_t) > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT)) {
-                            return (size_t) ((((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(size_t) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT)) {
+                                return (size_t) ((((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if ((8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(size_t) - 1 > 4 * PyLong_SHIFT)) {
-                            return (size_t) (((size_t)-1)*(((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(size_t) - 1 > 4 * PyLong_SHIFT)) {
+                                return (size_t) (((size_t)-1)*(((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if ((8 * sizeof(size_t) > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(size_t) - 1 > 4 * PyLong_SHIFT)) {
-                            return (size_t) ((((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(size_t) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(size_t) - 1 > 4 * PyLong_SHIFT)) {
+                                return (size_t) ((((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
             if ((sizeof(size_t) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(size_t, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
             } else if ((sizeof(size_t) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(size_t, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if (CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available, cannot convert large numbers");
-#else
             size_t val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (size_t) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (size_t) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (size_t) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (size_t) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (size_t) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(size_t) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((size_t) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(size_t) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((size_t) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((size_t) 1) << (sizeof(size_t) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (size_t) -1;
         }
     } else {
         size_t val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (size_t) -1;
         val = __Pyx_PyInt_As_size_t(tmp);
@@ -68617,21 +69038,19 @@
         return PyInt_AS_LONG(b);
     else
         return PyInt_AsSsize_t(b);
   }
 #endif
   if (likely(PyLong_CheckExact(b))) {
     #if CYTHON_USE_PYLONG_INTERNALS
-    const digit* digits = __Pyx_PyLong_Digits(b);
-    const Py_ssize_t size = Py_SIZE(b);
-    if (likely(__Pyx_sst_abs(size) <= 1)) {
-        ival = likely(size) ? digits[0] : 0;
-        if (size == -1) ival = -ival;
-        return ival;
+    if (likely(__Pyx_PyLong_IsCompact(b))) {
+        return __Pyx_PyLong_CompactValue(b);
     } else {
+      const digit* digits = __Pyx_PyLong_Digits(b);
+      const Py_ssize_t size = __Pyx_PyLong_SignedDigitCount(b);
       switch (size) {
          case 2:
            if (8 * sizeof(Py_ssize_t) > 2 * PyLong_SHIFT) {
              return (Py_ssize_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
            }
            break;
          case -2:
@@ -68692,15 +69111,15 @@
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
 
 
 /* #### Code section: utility_code_pragmas_end ### */
-#if _MSV_VER
+#ifdef _MSC_VER
 #pragma warning( pop )
 #endif
 
 
 
 /* #### Code section: end ### */
 #endif /* Py_PYTHON_H */
```

### Comparing `pglast-5.2/pglast/parser.pyx` & `pglast-5.3/pglast/parser.pyx`

 * *Files identical despite different names*

### Comparing `pglast-5.2/pglast/printers/__init__.py` & `pglast-5.3/pglast/printers/__init__.py`

 * *Files identical despite different names*

### Comparing `pglast-5.2/pglast/printers/ddl.py` & `pglast-5.3/pglast/printers/ddl.py`

 * *Files identical despite different names*

### Comparing `pglast-5.2/pglast/printers/dml.py` & `pglast-5.3/pglast/printers/dml.py`

 * *Files identical despite different names*

### Comparing `pglast-5.2/pglast/printers/sfuncs.py` & `pglast-5.3/pglast/printers/sfuncs.py`

 * *Files identical despite different names*

### Comparing `pglast-5.2/pglast/stream.py` & `pglast-5.3/pglast/stream.py`

 * *Files identical despite different names*

### Comparing `pglast-5.2/pglast/structs.pxd` & `pglast-5.3/pglast/structs.pxd`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# :Project:   pglast -- DO NOT EDIT: automatically extracted from struct_defs.json @ 15-4.2.1-0-g1f2d166
+# :Project:   pglast -- DO NOT EDIT: automatically extracted from struct_defs.json @ 15-4.2.3-0-g9b21e32
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
 # :Copyright: © 2021-2023 Lele Gaifax
 #
 
 #cython: language_level=3
```

### Comparing `pglast-5.2/pglast/visitors.py` & `pglast-5.3/pglast/visitors.py`

 * *Files identical despite different names*

### Comparing `pglast-5.2/pglast.egg-info/PKG-INFO` & `pglast-5.3/pglast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pglast
-Version: 5.2
+Version: 5.3
 Summary: PostgreSQL Languages AST and statements prettifier
 Home-page: https://github.com/lelit/pglast
 Author: Lele Gaifax
 Author-email: lele@metapensiero.it
 License: GPLv3+
 Keywords: postgresql parser sql prettifier
 Classifier: Development Status :: 5 - Production/Stable
@@ -111,14 +111,22 @@
 
 Changes
 -------
 
 Version 5
 #########
 
+5.3 (2023-08-05)
+~~~~~~~~~~~~~~~~
+
+- Update libpg_query to `15-4.2.3`__
+
+  __ https://github.com/pganalyze/libpg_query/releases/tag/15-4.2.3
+
+
 5.2 (2023-05-20)
 ~~~~~~~~~~~~~~~~
 
 - Update libpg_query to `15-4.2.1`__
 
   __ https://github.com/pganalyze/libpg_query/releases/tag/15-4.2.1
```

### Comparing `pglast-5.2/pglast.egg-info/SOURCES.txt` & `pglast-5.3/pglast.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -65,14 +65,16 @@
 libpg_query/src/pg_query_parse_plpgsql.c
 libpg_query/src/pg_query_readfuncs.h
 libpg_query/src/pg_query_readfuncs_conds.c
 libpg_query/src/pg_query_readfuncs_defs.c
 libpg_query/src/pg_query_readfuncs_protobuf.c
 libpg_query/src/pg_query_scan.c
 libpg_query/src/pg_query_split.c
+libpg_query/src/postgres_deparse.c
+libpg_query/src/postgres_deparse.h
 libpg_query/src/postgres/guc-file.c
 libpg_query/src/postgres/src_backend_catalog_namespace.c
 libpg_query/src/postgres/src_backend_catalog_pg_proc.c
 libpg_query/src/postgres/src_backend_commands_define.c
 libpg_query/src/postgres/src_backend_nodes_bitmapset.c
 libpg_query/src/postgres/src_backend_nodes_copyfuncs.c
 libpg_query/src/postgres/src_backend_nodes_equalfuncs.c
```

### Comparing `pglast-5.2/setup.py` & `pglast-5.3/setup.py`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_ast.py` & `pglast-5.3/tests/test_ast.py`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_cli.py` & `pglast-5.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_parser.py` & `pglast-5.3/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers.py` & `pglast-5.3/tests/test_printers.py`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_prettification/ddl/alter_subscription.sql` & `pglast-5.3/tests/test_printers_prettification/ddl/alter_subscription.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_prettification/ddl/comment.sql` & `pglast-5.3/tests/test_printers_prettification/ddl/comment.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_prettification/ddl/create_aggregate.sql` & `pglast-5.3/tests/test_printers_prettification/ddl/create_aggregate.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_prettification/ddl/create_event_trigger.sql` & `pglast-5.3/tests/test_printers_prettification/ddl/create_event_trigger.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_prettification/ddl/create_foreign_data_wrapper.sql` & `pglast-5.3/tests/test_printers_prettification/ddl/create_foreign_data_wrapper.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_prettification/ddl/create_foreign_table.sql` & `pglast-5.3/tests/test_printers_prettification/ddl/create_foreign_table.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_prettification/ddl/create_function.sql` & `pglast-5.3/tests/test_printers_prettification/ddl/create_function.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_prettification/ddl/create_rule.sql` & `pglast-5.3/tests/test_printers_prettification/ddl/create_rule.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_prettification/ddl/create_table.sql` & `pglast-5.3/tests/test_printers_prettification/ddl/create_table.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_prettification/ddl/create_trigger.sql` & `pglast-5.3/tests/test_printers_prettification/ddl/create_trigger.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_prettification/ddl/issue110.sql` & `pglast-5.3/tests/test_printers_prettification/ddl/issue110.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_prettification/dml/copy.sql` & `pglast-5.3/tests/test_printers_prettification/dml/copy.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_prettification/dml/insert.sql` & `pglast-5.3/tests/test_printers_prettification/dml/insert.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_prettification/dml/select.sql` & `pglast-5.3/tests/test_printers_prettification/dml/select.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_prettification/dml/update.sql` & `pglast-5.3/tests/test_printers_prettification/dml/update.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_prettification.py` & `pglast-5.3/tests/test_printers_prettification.py`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_roundtrip/ddl/alter_table.sql` & `pglast-5.3/tests/test_printers_roundtrip/ddl/alter_table.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_roundtrip/ddl/comment.sql` & `pglast-5.3/tests/test_printers_roundtrip/ddl/comment.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_roundtrip/ddl/create_aggregate.sql` & `pglast-5.3/tests/test_printers_roundtrip/ddl/create_aggregate.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_roundtrip/ddl/create_function.sql` & `pglast-5.3/tests/test_printers_roundtrip/ddl/create_function.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_roundtrip/ddl/create_index.sql` & `pglast-5.3/tests/test_printers_roundtrip/ddl/create_index.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_roundtrip/ddl/create_operator.sql` & `pglast-5.3/tests/test_printers_roundtrip/ddl/create_operator.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_roundtrip/ddl/create_operator_class.sql` & `pglast-5.3/tests/test_printers_roundtrip/ddl/create_operator_class.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_roundtrip/ddl/create_table.sql` & `pglast-5.3/tests/test_printers_roundtrip/ddl/create_table.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_roundtrip/ddl/create_trigger.sql` & `pglast-5.3/tests/test_printers_roundtrip/ddl/create_trigger.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_roundtrip/ddl/drop.sql` & `pglast-5.3/tests/test_printers_roundtrip/ddl/drop.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_roundtrip/dml/delete.sql` & `pglast-5.3/tests/test_printers_roundtrip/dml/delete.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_roundtrip/dml/insert.sql` & `pglast-5.3/tests/test_printers_roundtrip/dml/insert.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_roundtrip/dml/select.sql` & `pglast-5.3/tests/test_printers_roundtrip/dml/select.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_roundtrip/dml/set.sql` & `pglast-5.3/tests/test_printers_roundtrip/dml/set.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_roundtrip/dml/update.sql` & `pglast-5.3/tests/test_printers_roundtrip/dml/update.sql`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_printers_roundtrip.py` & `pglast-5.3/tests/test_printers_roundtrip.py`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_stream.py` & `pglast-5.3/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tests/test_visitors.py` & `pglast-5.3/tests/test_visitors.py`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tools/extract_ast.py` & `pglast-5.3/tools/extract_ast.py`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tools/extract_enums.py` & `pglast-5.3/tools/extract_enums.py`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tools/extract_keywords.py` & `pglast-5.3/tools/extract_keywords.py`

 * *Files identical despite different names*

### Comparing `pglast-5.2/tools/extract_printers_doc.py` & `pglast-5.3/tools/extract_printers_doc.py`

 * *Files identical despite different names*

