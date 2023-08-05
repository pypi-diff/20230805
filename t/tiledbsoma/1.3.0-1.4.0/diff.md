# Comparing `tmp/tiledbsoma-1.3.0.tar.gz` & `tmp/tiledbsoma-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiledbsoma-1.3.0.tar", last modified: Tue Jul 18 21:21:53 2023, max compression
+gzip compressed data, was "tiledbsoma-1.4.0.tar", last modified: Sat Aug  5 00:12:54 2023, max compression
```

## Comparing `tiledbsoma-1.3.0.tar` & `tiledbsoma-1.4.0.tar`

### file list

```diff
@@ -1,137 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.822553 tiledbsoma-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-18 21:21:50.000000 tiledbsoma-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5262 2023-07-18 21:21:53.822553 tiledbsoma-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3262 2023-07-18 21:21:50.000000 tiledbsoma-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/RELEASE-VERSION
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.810552 tiledbsoma-1.3.0/dist_links/
--rw-r--r--   0 runner    (1001) docker     (122)      508 2023-07-18 21:21:50.000000 tiledbsoma-1.3.0/dist_links/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.810552 tiledbsoma-1.3.0/dist_links/libtiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (122)     8992 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4035 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.810552 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.814553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/
--rw-r--r--   0 runner    (1001) docker     (122)     2893 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     5006 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     3643 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     5158 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Superbuild.cmake
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.814553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/inputs/
--rw-r--r--   0 runner    (1001) docker     (122)      724 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/inputs/tiledbsoma.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.814553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/patches/
--rw-r--r--   0 runner    (1001) docker     (122)      736 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/patches/spdlog.patch
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.814553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/doc/
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/doc/README.md
--rw-r--r--   0 runner    (1001) docker     (122)    36556 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/doc/reader.svg
--rw-r--r--   0 runner    (1001) docker     (122)     2198 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/doc/reader.uml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.814553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/
--rw-r--r--   0 runner    (1001) docker     (122)    11138 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.814553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/cli/
--rw-r--r--   0 runner    (1001) docker     (122)     4146 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/cli/cli.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.814553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/
--rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.802552 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/include/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.814553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/include/span/
--rw-r--r--   0 runner    (1001) docker     (122)    17276 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/include/span/span.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.814553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/include/thread_pool/
--rw-r--r--   0 runner    (1001) docker     (122)     7142 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h
--rw-r--r--   0 runner    (1001) docker     (122)    17772 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h
--rw-r--r--   0 runner    (1001) docker     (122)     5561 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.802552 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.814553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/src/thread_pool/
--rw-r--r--   0 runner    (1001) docker     (122)     3092 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc
--rw-r--r--   0 runner    (1001) docker     (122)     6694 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.814553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/
--rw-r--r--   0 runner    (1001) docker     (122)     3720 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/array_buffers.h
--rw-r--r--   0 runner    (1001) docker     (122)     7897 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/column_buffer.cc
--rw-r--r--   0 runner    (1001) docker     (122)     8821 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/column_buffer.h
--rw-r--r--   0 runner    (1001) docker     (122)     2886 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/logger_public.h
--rw-r--r--   0 runner    (1001) docker     (122)     7172 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/managed_query.cc
--rw-r--r--   0 runner    (1001) docker     (122)    14575 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/managed_query.h
--rw-r--r--   0 runner    (1001) docker     (122)    16193 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/soma_array.cc
--rw-r--r--   0 runner    (1001) docker     (122)    18139 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/soma_array.h
--rw-r--r--   0 runner    (1001) docker     (122)     4413 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/soma_dataframe.cc
--rw-r--r--   0 runner    (1001) docker     (122)     6905 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/soma_dataframe.h
--rw-r--r--   0 runner    (1001) docker     (122)     5451 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/soma_group.cc
--rw-r--r--   0 runner    (1001) docker     (122)     9491 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/soma_group.h
--rw-r--r--   0 runner    (1001) docker     (122)     2373 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/soma_object.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.814553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/tiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (122)     1979 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.818553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     7271 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/arrow_adapter.h
--rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/carrow.h
--rw-r--r--   0 runner    (1001) docker     (122)     2029 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/common.h
--rw-r--r--   0 runner    (1001) docker     (122)     6904 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/logger.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7858 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/logger.h
--rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/stats.cc
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/stats.h
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/util.cc
--rw-r--r--   0 runner    (1001) docker     (122)     2211 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/util.h
--rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/version.cc
--rw-r--r--   0 runner    (1001) docker     (122)     1650 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/version.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.818553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/
--rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     6489 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/test_query_condition.py
--rw-r--r--   0 runner    (1001) docker     (122)     4038 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (122)     7705 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/test_soma_array.py
--rw-r--r--   0 runner    (1001) docker     (122)     3080 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/unit_column_buffer.cc
--rw-r--r--   0 runner    (1001) docker     (122)     5659 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/unit_managed_query.cc
--rw-r--r--   0 runner    (1001) docker     (122)    13593 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/unit_soma_array.cc
--rw-r--r--   0 runner    (1001) docker     (122)     4222 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/unit_soma_dataframe.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7529 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/unit_soma_group.cc
--rw-r--r--   0 runner    (1001) docker     (122)    15705 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/unit_thread_pool.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.818553 tiledbsoma-1.3.0/dist_links/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/scripts/README.md
--rwxr-xr-x   0 runner    (1001) docker     (122)     2537 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/scripts/bld
--rwxr-xr-x   0 runner    (1001) docker     (122)     1339 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/scripts/run-clang-format.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      821 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/scripts/show-versions.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3483 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/scripts/update-tiledb-version.py
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-18 21:21:53.822553 tiledbsoma-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)    11110 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.806552 tiledbsoma-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.822553 tiledbsoma-1.3.0/src/tiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (122)     5318 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6363 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_arrow_types.py
--rw-r--r--   0 runner    (1001) docker     (122)    27175 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     6830 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_common_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (122)      345 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    33885 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (122)     6920 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_dense_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (122)     1522 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_exception.py
--rw-r--r--   0 runner    (1001) docker     (122)     2592 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_experiment.py
--rw-r--r--   0 runner    (1001) docker     (122)     6792 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_funcs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_general_utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)     3188 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_measurement.py
--rw-r--r--   0 runner    (1001) docker     (122)    16305 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_query_condition.py
--rw-r--r--   0 runner    (1001) docker     (122)     2492 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_read_iters.py
--rw-r--r--   0 runner    (1001) docker     (122)    11655 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_sparse_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (122)    12161 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_tdb_handles.py
--rw-r--r--   0 runner    (1001) docker     (122)     7628 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_tiledb_array.py
--rw-r--r--   0 runner    (1001) docker     (122)     9317 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_tiledb_object.py
--rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     9107 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_util.py
--rw-r--r--   0 runner    (1001) docker     (122)     3079 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/eta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/experiment_query.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.822553 tiledbsoma-1.3.0/src/tiledbsoma/io/
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/io/conversions.py
--rw-r--r--   0 runner    (1001) docker     (122)    62737 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/io/ingest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.822553 tiledbsoma-1.3.0/src/tiledbsoma/options/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4896 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/options/_soma_tiledb_context.py
--rw-r--r--   0 runner    (1001) docker     (122)    11206 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/options/_tiledb_create_options.py
--rw-r--r--   0 runner    (1001) docker     (122)    26382 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/pytiledbsoma.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7767 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/query_condition.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.822553 tiledbsoma-1.3.0/src/tiledbsoma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5262 2023-07-18 21:21:53.000000 tiledbsoma-1.3.0/src/tiledbsoma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4493 2023-07-18 21:21:53.000000 tiledbsoma-1.3.0/src/tiledbsoma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 21:21:53.000000 tiledbsoma-1.3.0/src/tiledbsoma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 21:21:53.000000 tiledbsoma-1.3.0/src/tiledbsoma.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-07-18 21:21:53.000000 tiledbsoma-1.3.0/src/tiledbsoma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-18 21:21:53.000000 tiledbsoma-1.3.0/src/tiledbsoma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4659 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.514388 tiledbsoma-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5262 2023-08-05 00:12:54.514388 tiledbsoma-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3262 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/RELEASE-VERSION
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.474388 tiledbsoma-1.4.0/dist_links/
+-rw-r--r--   0 runner    (1001) docker     (122)      508 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/dist_links/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.474388 tiledbsoma-1.4.0/dist_links/libtiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (122)     8992 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4035 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.474388 tiledbsoma-1.4.0/dist_links/libtiledbsoma/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.478388 tiledbsoma-1.4.0/dist_links/libtiledbsoma/cmake/Modules/
+-rw-r--r--   0 runner    (1001) docker     (122)     2893 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     5006 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     3643 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     5158 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/cmake/Superbuild.cmake
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.478388 tiledbsoma-1.4.0/dist_links/libtiledbsoma/cmake/inputs/
+-rw-r--r--   0 runner    (1001) docker     (122)      724 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/cmake/inputs/tiledbsoma.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.478388 tiledbsoma-1.4.0/dist_links/libtiledbsoma/cmake/patches/
+-rw-r--r--   0 runner    (1001) docker     (122)      736 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/cmake/patches/spdlog.patch
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.478388 tiledbsoma-1.4.0/dist_links/libtiledbsoma/doc/
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/doc/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)    36556 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/doc/reader.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     2198 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/doc/reader.uml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.478388 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/
+-rw-r--r--   0 runner    (1001) docker     (122)    11736 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.478388 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     4182 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/cli/cli.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.482388 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/external/
+-rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/external/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.470388 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/external/include/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.482388 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/external/include/span/
+-rw-r--r--   0 runner    (1001) docker     (122)    17276 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/external/include/span/span.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.482388 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/external/include/thread_pool/
+-rw-r--r--   0 runner    (1001) docker     (122)     7142 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h
+-rw-r--r--   0 runner    (1001) docker     (122)    17772 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5561 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.470388 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/external/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.482388 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/external/src/thread_pool/
+-rw-r--r--   0 runner    (1001) docker     (122)     3092 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     6694 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.490388 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/
+-rw-r--r--   0 runner    (1001) docker     (122)     3720 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/array_buffers.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7897 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/column_buffer.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     8821 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/column_buffer.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1724 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/enums.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2886 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/logger_public.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7172 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/managed_query.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    14575 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/managed_query.h
+-rw-r--r--   0 runner    (1001) docker     (122)    16878 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/soma_array.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    19432 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/soma_array.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7820 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/soma_collection.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     9131 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/soma_collection.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4648 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/soma_dataframe.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7941 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/soma_dataframe.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4762 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/soma_dense_ndarray.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     8049 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/soma_dense_ndarray.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/soma_experiment.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/soma_experiment.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6021 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/soma_group.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     9954 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/soma_group.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2992 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/soma_measurement.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     4188 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/soma_measurement.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2570 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/soma_object.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4820 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/soma_sparse_ndarray.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     8240 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/soma_sparse_ndarray.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.490388 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/tiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.494388 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     7271 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/utils/arrow_adapter.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/utils/carrow.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2029 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/utils/common.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6904 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/utils/logger.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7858 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/utils/logger.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/utils/stats.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/utils/stats.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/utils/util.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     2211 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/utils/util.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/utils/version.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     1650 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/utils/version.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.498388 tiledbsoma-1.4.0/dist_links/libtiledbsoma/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     6489 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/test/test_query_condition.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4038 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/test/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7705 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/test/test_soma_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3080 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/test/unit_column_buffer.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     5659 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/test/unit_managed_query.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    13856 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/test/unit_soma_array.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     9752 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/test/unit_soma_collection.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     4287 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/test/unit_soma_dataframe.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     4210 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/test/unit_soma_dense_ndarray.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7599 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/test/unit_soma_group.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     4180 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/test/unit_soma_sparse_ndarray.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    15705 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/libtiledbsoma/test/unit_thread_pool.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.502388 tiledbsoma-1.4.0/dist_links/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/scripts/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2537 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/scripts/bld
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1339 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/scripts/run-clang-format.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      821 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/scripts/show-versions.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3483 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/dist_links/scripts/update-tiledb-version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-05 00:12:54.514388 tiledbsoma-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)    11110 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.470388 tiledbsoma-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.510388 tiledbsoma-1.4.0/src/tiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (122)     5318 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7438 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/_arrow_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27175 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6830 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/_common_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33885 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6920 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/_dense_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1522 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/_exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2592 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6792 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/_general_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3188 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16301 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/_query_condition.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2492 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/_read_iters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11655 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/_sparse_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12161 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/_tdb_handles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7862 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/_tiledb_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9317 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/_tiledb_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9107 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3079 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/eta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/experiment_query.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.514388 tiledbsoma-1.4.0/src/tiledbsoma/io/
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3610 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/io/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    62442 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/io/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.514388 tiledbsoma-1.4.0/src/tiledbsoma/options/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4896 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/options/_soma_tiledb_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11206 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/options/_tiledb_create_options.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26727 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/pytiledbsoma.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7767 2023-08-05 00:12:50.000000 tiledbsoma-1.4.0/src/tiledbsoma/query_condition.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 00:12:54.514388 tiledbsoma-1.4.0/src/tiledbsoma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5262 2023-08-05 00:12:54.000000 tiledbsoma-1.4.0/src/tiledbsoma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5245 2023-08-05 00:12:54.000000 tiledbsoma-1.4.0/src/tiledbsoma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-05 00:12:54.000000 tiledbsoma-1.4.0/src/tiledbsoma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-05 00:12:54.000000 tiledbsoma-1.4.0/src/tiledbsoma.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-08-05 00:12:54.000000 tiledbsoma-1.4.0/src/tiledbsoma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-08-05 00:12:54.000000 tiledbsoma-1.4.0/src/tiledbsoma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4659 2023-08-05 00:12:51.000000 tiledbsoma-1.4.0/version.py
```

### Comparing `tiledbsoma-1.3.0/PKG-INFO` & `tiledbsoma-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledbsoma
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python API for efficient storage and retrieval of single-cell data using TileDB
 Home-page: https://github.com/single-cell-data/TileDB-SOMA/tree/main/apis/python
 Author: TileDB, Inc.
 Author-email: help@tiledb.io
 Maintainer: TileDB, Inc.
 Maintainer-email: help@tiledb.io
 License: MIT
```

### Comparing `tiledbsoma-1.3.0/README.md` & `tiledbsoma-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/CMakeLists.txt` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/README.md` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/README.md`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake`

 * *Files 8% similar despite different names*

```diff
@@ -54,16 +54,16 @@
     # loaded by the Python and R tiledbsoma packages. Those packages -also- use TileDB-Py and
     # TileDB-R, each of which links their own 'copy' of TileDB Embedded, whose version we don't
     # control here. Ideally the TileDB Embedded versions should match! The show_package_versions()
     # helper function in each package can help to diagnose any mismatch.
     # NB When updating the pinned URLs here, please also update in file apis/r/tools/get_tarball.R
     if(DOWNLOAD_TILEDB_PREBUILT)
         if (WIN32) # Windows
-          SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.16.0/tiledb-windows-x86_64-2.16.0-d682dd0.zip")
-          SET(DOWNLOAD_SHA1 "82a79fda3daecc46ae24c86a328e52184460dabe")
+          SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.16.2/tiledb-windows-x86_64-2.16.2-07b65de.zip")
+          SET(DOWNLOAD_SHA1 "1cda23235ceeff70cb2b30e0c0e22fcd9fd83b51")
         elseif(APPLE) # OSX
 
           # Status quo as of 2023-05-18:
           # * GitHub Actions does not have MacOS arm64 hardware available -- tracked at
           #   https://github.com/github/roadmap/issues/528
           # * The best we can do is cross-compile for arm64 while actually running on x86_64
           # * When we're invoked from python setup.py:
@@ -72,30 +72,30 @@
           #   o We must download the tiledb artifacts for the cross-compile architecture (x86_64 or arm64)
           #   o Therefore we must respect CMAKE_OSX_ARCHITECTURES not CMAKE_SYSTEM_PROCESSOR
           # * When we're invoked from R configure and src/Makevars.in:
           #   o CMAKE_OSX_ARCHITECTURES is unset
           #   o CMAKE_SYSTEM_PROCESSOR is x86_64
 
           if (CMAKE_OSX_ARCHITECTURES STREQUAL x86_64)
-            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.16.0/tiledb-macos-x86_64-2.16.0-d682dd0.tar.gz")
-            SET(DOWNLOAD_SHA1 "d7b22fa3cb9cbe131734d9f18beb3362908aeccf")
+            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.16.2/tiledb-macos-x86_64-2.16.2-07b65de.tar.gz")
+            SET(DOWNLOAD_SHA1 "355233cee1515857c91b2f12fe4f7bbc1ac02465")
           elseif (CMAKE_OSX_ARCHITECTURES STREQUAL arm64)
-            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.16.0/tiledb-macos-arm64-2.16.0-d682dd0.tar.gz")
-            SET(DOWNLOAD_SHA1 "09c62e3211e5277263c1545d74d698d450ebcb77")
+            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.16.2/tiledb-macos-arm64-2.16.2-07b65de.tar.gz")
+            SET(DOWNLOAD_SHA1 "5aad92b76e6fe3f7129f514ed926ef1c8af4bfa3")
           elseif (CMAKE_SYSTEM_PROCESSOR MATCHES "(x86_64)|(AMD64|amd64)|(^i.86$)")
-            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.16.0/tiledb-macos-x86_64-2.16.0-d682dd0.tar.gz")
-            SET(DOWNLOAD_SHA1 "d7b22fa3cb9cbe131734d9f18beb3362908aeccf")
+            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.16.2/tiledb-macos-x86_64-2.16.2-07b65de.tar.gz")
+            SET(DOWNLOAD_SHA1 "355233cee1515857c91b2f12fe4f7bbc1ac02465")
           elseif (CMAKE_SYSTEM_PROCESSOR MATCHES "^aarch64" OR CMAKE_SYSTEM_PROCESSOR MATCHES "^arm")
-            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.16.0/tiledb-macos-arm64-2.16.0-d682dd0.tar.gz")
-            SET(DOWNLOAD_SHA1 "09c62e3211e5277263c1545d74d698d450ebcb77")
+            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.16.2/tiledb-macos-arm64-2.16.2-07b65de.tar.gz")
+            SET(DOWNLOAD_SHA1 "5aad92b76e6fe3f7129f514ed926ef1c8af4bfa3")
           endif()
 
         else() # Linux
-          SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.16.0/tiledb-linux-x86_64-2.16.0-d682dd0.tar.gz")
-          SET(DOWNLOAD_SHA1 "be0bfd5512c159b960988a4bd41366e9f020115f")
+          SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.16.2/tiledb-linux-x86_64-2.16.2-07b65de.tar.gz")
+          SET(DOWNLOAD_SHA1 "b9fc44a104f31a9348a399e55ef9e32903b99590")
         endif()
 
         ExternalProject_Add(ep_tiledb
                 PREFIX "externals"
                 URL ${DOWNLOAD_URL}
                 URL_HASH SHA1=${DOWNLOAD_SHA1}
                 CONFIGURE_COMMAND ""
@@ -109,16 +109,16 @@
                 LOG_CONFIGURE FALSE
                 LOG_BUILD FALSE
                 LOG_INSTALL FALSE
                 )
     else() # Build from source
         ExternalProject_Add(ep_tiledb
           PREFIX "externals"
-          URL "https://github.com/TileDB-Inc/TileDB/archive/2.16.0.zip"
-          URL_HASH SHA1=c2779f931c84d931e5fca6dc3a858e66fc542276
+          URL "https://github.com/TileDB-Inc/TileDB/archive/2.16.2.zip"
+          URL_HASH SHA1=d54ff7fc4c3a1c5afb1027bab1ba011ae47c3d79
           DOWNLOAD_NAME "tiledb.zip"
           CMAKE_ARGS
             -DCMAKE_INSTALL_PREFIX=${EP_INSTALL_PREFIX}
             -DCMAKE_PREFIX_PATH=${EP_INSTALL_PREFIX}
             -DTILEDB_S3=${TILEDB_S3}
             -DTILEDB_AZURE=${TILEDB_AZURE}
             -DTILEDB_GCS=${TILEDB_GCS}
```

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Superbuild.cmake` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/cmake/Superbuild.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/patches/spdlog.patch` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/cmake/patches/spdlog.patch`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/doc/reader.svg` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/doc/reader.svg`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/doc/reader.uml` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/doc/reader.uml`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/CMakeLists.txt` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,20 @@
 # ###########################################################
 # Common object library
 # ###########################################################
 add_library(TILEDB_SOMA_OBJECTS OBJECT
   ${CMAKE_CURRENT_SOURCE_DIR}/soma/managed_query.cc
   ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_array.cc
   ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_group.cc
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_collection.cc
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_experiment.cc
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_measurement.cc
   ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_dataframe.cc
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_dense_ndarray.cc
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_sparse_ndarray.cc
   ${CMAKE_CURRENT_SOURCE_DIR}/soma/column_buffer.cc
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/logger.cc
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/stats.cc
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/util.cc
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/version.cc
 
   # TODO: uncomment when thread_pool is enabled
@@ -166,22 +171,28 @@
 #   ${CMAKE_CURRENT_SOURCE_DIR}/cpp_api/soma_measurement.h
 #   ${CMAKE_CURRENT_SOURCE_DIR}/cpp_api/soma_object.h
 #   ${CMAKE_CURRENT_SOURCE_DIR}/cpp_api/soma_sparse_ndarray.h
 #   ${CMAKE_CURRENT_SOURCE_DIR}/cpp_api/logger_public.h
 # )
 
 install(FILES 
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/enums.h
   ${CMAKE_CURRENT_SOURCE_DIR}/soma/logger_public.h
   ${CMAKE_CURRENT_SOURCE_DIR}/soma/managed_query.h
   ${CMAKE_CURRENT_SOURCE_DIR}/soma/array_buffers.h  
   ${CMAKE_CURRENT_SOURCE_DIR}/soma/column_buffer.h  
   ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_array.h 
   ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_group.h
-  ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_object.h 
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_collection.h 
   ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_dataframe.h 
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_dense_ndarray.h
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_sparse_ndarray.h 
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_experiment.h 
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_measurement.h 
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_object.h 
   DESTINATION "include/tiledbsoma/soma"
 )
 
 install(FILES 
   ${CMAKE_CURRENT_SOURCE_DIR}/tiledbsoma/tiledbsoma
   DESTINATION "include/tiledbsoma"
 )
```

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/cli/cli.cc` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/cli/cli.cc`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,15 @@
  * THE SOFTWARE.
  *
  * @section DESCRIPTION
  *
  * This file is currently a sandbox for C++ API experiments
  */
 
+#include "soma/enums.h"
 #include "soma/soma_array.h"
 #include "utils/arrow_adapter.h"
 
 using namespace tiledbsoma;
 
 // [[Rcpp::export]]
 void test_sdf(const std::string& uri) {
@@ -41,31 +42,31 @@
     // Control buffer sizes, similar to tiledb-py
     // config["soma.init_buffer_bytes"] = "4294967296";
 
     // Control core memory usage
     // config["sm.mem.total_budget"] = "1118388608";
 
     // Read all values from the obs array
-    auto obs = SOMAArray::open(TILEDB_READ, uri + "/obs", "obs");
+    auto obs = SOMAArray::open(OpenMode::read, uri + "/obs", "obs");
     obs->submit();
     auto obs_data = obs->read_next();
 
     // Read all values from the var array
-    auto var = SOMAArray::open(TILEDB_READ, uri + "/ms/RNA/var", "var");
+    auto var = SOMAArray::open(OpenMode::read, uri + "/ms/RNA/var", "var");
     var->submit();
     auto var_data = var->read_next();
 
     // Check if obs and var reads are complete
     if (obs->results_complete() && var->results_complete()) {
         LOG_INFO("var and obs queries are complete");
     }
 
     // Read all values from the X/data array
     auto x_data = SOMAArray::open(
-        TILEDB_READ, uri + "/ms/RNA/X/data", "X/data", config);
+        OpenMode::read, uri + "/ms/RNA/X/data", "X/data", config);
     x_data->submit();
 
     int batches = 0;
     int total_num_rows = 0;
 
     // Handle incomplete queries
     while (auto batch = x_data->read_next()) {
@@ -76,15 +77,15 @@
     LOG_INFO(fmt::format("X/data rows = {}", total_num_rows));
     LOG_INFO(fmt::format("  batches = {}", batches));
 }
 
 namespace tdbs = tiledbsoma;
 void test_arrow(const std::string& uri) {
     const std::vector<std::string>& colnames{"n_counts", "n_genes", "louvain"};
-    auto obs = tdbs::SOMAArray::open(TILEDB_READ, uri, "", {}, colnames);
+    auto obs = tdbs::SOMAArray::open(OpenMode::read, uri, "", {}, colnames);
     obs->submit();
     // Getting next batch:  std::optional<std::shared_ptr<ArrayBuffers>>
     auto obs_data = obs->read_next();
     if (!obs->results_complete()) {
         tdbs::LOG_WARN(fmt::format("Read of '{}' incomplete", uri));
         exit(-1);
     }
```

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/.clang-format` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/external/.clang-format`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/include/span/span.hpp` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/external/include/span/span.hpp`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/array_buffers.h` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/array_buffers.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/column_buffer.cc` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/column_buffer.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/column_buffer.h` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/column_buffer.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/logger_public.h` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/logger_public.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/managed_query.cc` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/managed_query.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/managed_query.h` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/managed_query.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/soma_array.cc` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/soma_array.cc`

 * *Files 6% similar despite different names*

```diff
@@ -41,30 +41,30 @@
 //= public static
 //===================================================================
 
 void SOMAArray::create(
     std::shared_ptr<Context> ctx,
     std::string_view uri,
     ArraySchema schema,
-    std::string soma_object_type) {
+    std::string soma_type) {
     Array::create(std::string(uri), schema);
     auto array = Array(*ctx, std::string(uri), TILEDB_WRITE);
     array.put_metadata(
-        "soma_object_type", TILEDB_STRING_UTF8, 1, soma_object_type.c_str());
+        "soma_object_type", TILEDB_STRING_UTF8, 1, soma_type.c_str());
     array.close();
 }
 
 std::unique_ptr<SOMAArray> SOMAArray::open(
-    tiledb_query_type_t mode,
+    OpenMode mode,
     std::string_view uri,
     std::string_view name,
     std::map<std::string, std::string> platform_config,
     std::vector<std::string> column_names,
     std::string_view batch_size,
-    std::string_view result_order,
+    ResultOrder result_order,
     std::optional<std::pair<uint64_t, uint64_t>> timestamp) {
     LOG_DEBUG(
         fmt::format("[SOMAArray] static method 'cfg' opening array '{}'", uri));
     return std::make_unique<SOMAArray>(
         mode,
         uri,
         name,
@@ -72,21 +72,21 @@
         column_names,
         batch_size,
         result_order,
         timestamp);
 }
 
 std::unique_ptr<SOMAArray> SOMAArray::open(
-    tiledb_query_type_t mode,
+    OpenMode mode,
     std::shared_ptr<Context> ctx,
     std::string_view uri,
     std::string_view name,
     std::vector<std::string> column_names,
     std::string_view batch_size,
-    std::string_view result_order,
+    ResultOrder result_order,
     std::optional<std::pair<uint64_t, uint64_t>> timestamp) {
     LOG_DEBUG(
         fmt::format("[SOMAArray] static method 'ctx' opening array '{}'", uri));
     return std::make_unique<SOMAArray>(
         mode,
         uri,
         name,
@@ -98,103 +98,91 @@
 }
 
 //===================================================================
 //= public non-static
 //===================================================================
 
 SOMAArray::SOMAArray(
-    tiledb_query_type_t mode,
+    OpenMode mode,
+    std::string_view uri,
+    std::string_view name,
+    std::map<std::string, std::string> platform_config,
+    std::vector<std::string> column_names,
+    std::string_view batch_size,
+    ResultOrder result_order,
+    std::optional<std::pair<uint64_t, uint64_t>> timestamp)
+    : uri_(util::rstrip_uri(uri))
+    , timestamp_(timestamp) {
+    ctx_ = std::make_shared<Context>(Config(platform_config));
+    validate(mode, name, timestamp);
+    reset(column_names, batch_size, result_order);
+}
+
+SOMAArray::SOMAArray(
+    OpenMode mode,
     std::string_view uri,
     std::string_view name,
     std::shared_ptr<Context> ctx,
     std::vector<std::string> column_names,
     std::string_view batch_size,
-    std::string_view result_order,
+    ResultOrder result_order,
     std::optional<std::pair<uint64_t, uint64_t>> timestamp)
     : ctx_(ctx)
     , uri_(util::rstrip_uri(uri))
     , timestamp_(timestamp) {
-    // Validate parameters
-    try {
-        LOG_DEBUG(fmt::format("[SOMAArray] opening array '{}'", uri_));
-        arr_ = std::make_shared<Array>(*ctx_, uri_, mode);
-        if (timestamp) {
-            if (timestamp->first > timestamp->second) {
-                throw std::invalid_argument("timestamp start > end");
-            }
-            arr_->set_open_timestamp_start(timestamp->first);
-            arr_->set_open_timestamp_end(timestamp->second);
-            arr_->close();
-            arr_->open(mode);
-            LOG_DEBUG(fmt::format(
-                "[SOMAArray] timestamp_start = {}",
-                arr_->open_timestamp_start()));
-            LOG_DEBUG(fmt::format(
-                "[SOMAArray] timestamp_end = {}", arr_->open_timestamp_end()));
-        }
-        mq_ = std::make_unique<ManagedQuery>(arr_, name);
-    } catch (const std::exception& e) {
-        throw TileDBSOMAError(
-            fmt::format("Error opening array: '{}'\n  {}", uri_, e.what()));
-    }
-
+    validate(mode, name, timestamp);
     reset(column_names, batch_size, result_order);
 }
 
 const std::string& SOMAArray::uri() const {
     return uri_;
 };
 
 std::shared_ptr<Context> SOMAArray::ctx() {
     return ctx_;
 };
 
 void SOMAArray::open(
-    tiledb_query_type_t mode,
-    std::optional<std::pair<uint64_t, uint64_t>> timestamp) {
-    arr_->open(mode);
+    OpenMode mode, std::optional<std::pair<uint64_t, uint64_t>> timestamp) {
+    auto tdb_mode = mode == OpenMode::read ? TILEDB_READ : TILEDB_WRITE;
+    arr_->open(tdb_mode);
     if (timestamp) {
         if (timestamp->first > timestamp->second) {
             throw std::invalid_argument("timestamp start > end");
         }
         arr_->set_open_timestamp_start(timestamp->first);
         arr_->set_open_timestamp_end(timestamp->second);
         arr_->close();
-        arr_->open(mode);
+        arr_->open(tdb_mode);
     }
 }
 
 void SOMAArray::close() {
     arr_->close();
 }
 
 void SOMAArray::reset(
     std::vector<std::string> column_names,
     std::string_view batch_size,
-    std::string_view result_order) {
+    ResultOrder result_order) {
     // Reset managed query
     mq_->reset();
 
     if (!column_names.empty()) {
         mq_->select_columns(column_names);
     }
 
     batch_size_ = batch_size;
 
-    result_order_ = "auto";
-    if (result_order != "auto") {  // default "auto" is set in soma_array.h
-        tiledb_layout_t layout;
-        if (result_order == "row-major") {
-            layout = TILEDB_ROW_MAJOR;
-        } else if (result_order == "column-major") {
-            layout = TILEDB_COL_MAJOR;
-        } else {
-            throw TileDBSOMAError(
-                fmt::format("Unknown result_order '{}'", result_order));
-        }
+    if (result_order !=
+        ResultOrder::automatic) {  // default ResultOrder::automatic is set in
+                                   // soma_array.h
+        tiledb_layout_t layout = (result_order == ResultOrder::rowmajor) ?
+                                     TILEDB_ROW_MAJOR :
+                                     TILEDB_COL_MAJOR;
         mq_->set_layout(layout);
         result_order_ = result_order;
     }
 
     first_read_next_ = true;
     submitted_ = false;
 }
@@ -350,15 +338,15 @@
 
 uint64_t SOMAArray::nnz_slow() {
     LOG_DEBUG(
         "[SOMAArray] nnz() found consolidated or overlapping fragments, "
         "counting cells...");
 
     auto sr = SOMAArray::open(
-        TILEDB_READ,
+        OpenMode::read,
         ctx_,
         uri_,
         "count_cells",
         {mq_->schema()->domain().dimension(0).name()},
         batch_size_,
         result_order_,
         timestamp_);
@@ -495,8 +483,38 @@
     return arr_->has_metadata(key, &value_type);
 }
 
 uint64_t SOMAArray::metadata_num() const {
     return arr_->metadata_num();
 }
 
+void SOMAArray::validate(
+    OpenMode mode,
+    std::string_view name,
+    std::optional<std::pair<uint64_t, uint64_t>> timestamp) {
+    // Validate parameters
+    auto tdb_mode = mode == OpenMode::read ? TILEDB_READ : TILEDB_WRITE;
+    try {
+        LOG_DEBUG(fmt::format("[SOMAArray] opening array '{}'", uri_));
+        arr_ = std::make_shared<Array>(*ctx_, uri_, tdb_mode);
+        if (timestamp) {
+            if (timestamp->first > timestamp->second) {
+                throw std::invalid_argument("timestamp start > end");
+            }
+            arr_->set_open_timestamp_start(timestamp->first);
+            arr_->set_open_timestamp_end(timestamp->second);
+            arr_->close();
+            arr_->open(tdb_mode);
+            LOG_DEBUG(fmt::format(
+                "[SOMAArray] timestamp_start = {}",
+                arr_->open_timestamp_start()));
+            LOG_DEBUG(fmt::format(
+                "[SOMAArray] timestamp_end = {}", arr_->open_timestamp_end()));
+        }
+        mq_ = std::make_unique<ManagedQuery>(arr_, name);
+    } catch (const std::exception& e) {
+        throw TileDBSOMAError(
+            fmt::format("Error opening array: '{}'\n  {}", uri_, e.what()));
+    }
+}
+
 }  // namespace tiledbsoma
```

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/soma_array.h` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/soma_array.h`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 #include <stdexcept>  // for windows: error C2039: 'runtime_error': is not a member of 'std'
 
 #include <future>
 
 #include <tiledb/tiledb>
 
+#include "enums.h"
 #include "managed_query.h"
 
 namespace tiledbsoma {
 using namespace tiledb;
 
 class SOMAArray {
    public:
@@ -52,90 +53,117 @@
 
     /**
      * @brief Create a SOMAArray object at the given URI.
      *
      * @param ctx TileDB context
      * @param uri URI to create the SOMAArray
      * @param schema TileDB ArraySchema
+     * @param soma_type SOMADataFrame, SOMADenseNDArray, or SOMASparseNDArray
      */
     static void create(
         std::shared_ptr<Context> ctx,
         std::string_view uri,
         ArraySchema schema,
-        std::string soma_object_type);
+        std::string soma_type);
 
     /**
      * @brief Open an array at the specified URI and return SOMAArray
      * object.
      *
-     * @param mode TILEDB_READ or TILEDB_WRITE
+     * @param mode read or write
      * @param uri URI of the array
      * @param name Name of the array
      * @param platform_config Config parameter dictionary
      * @param column_names Columns to read
      * @param batch_size Read batch size
-     * @param result_order Read result order
+     * @param result_order Read result order: automatic (default), rowmajor, or
+     * colmajor
      * @return std::unique_ptr<SOMAArray> SOMAArray
      */
     static std::unique_ptr<SOMAArray> open(
-        tiledb_query_type_t mode,
+        OpenMode mode,
         std::string_view uri,
         std::string_view name = "unnamed",
         std::map<std::string, std::string> platform_config = {},
         std::vector<std::string> column_names = {},
         std::string_view batch_size = "auto",
-        std::string_view result_order = "auto",
+        ResultOrder result_order = ResultOrder::automatic,
         std::optional<std::pair<uint64_t, uint64_t>> timestamp = std::nullopt);
 
     /**
      * @brief Open an array at the specified URI and return SOMAArray
      * object.
      *
-     * @param mode TILEDB_READ or TILEDB_WRITE
+     * @param mode read or write
      * @param ctx TileDB context
      * @param uri URI of the array
      * @param name Name of the array
      * @param column_names Columns to read
      * @param batch_size Read batch size
-     * @param result_order Read result order
+     * @param result_order Read result order: automatic (default), rowmajor, or
+     * colmajor
      * @return std::unique_ptr<SOMAArray> SOMAArray
      */
     static std::unique_ptr<SOMAArray> open(
-        tiledb_query_type_t mode,
+        OpenMode mode,
         std::shared_ptr<Context> ctx,
         std::string_view uri,
         std::string_view name = "unnamed",
         std::vector<std::string> column_names = {},
         std::string_view batch_size = "auto",
-        std::string_view result_order = "auto",
+        ResultOrder result_order = ResultOrder::automatic,
         std::optional<std::pair<uint64_t, uint64_t>> timestamp = std::nullopt);
 
     //===================================================================
     //= public non-static
     //===================================================================
+
     /**
      * @brief Construct a new SOMAArray object
      *
-     * @param mode TILEDB_READ or TILEDB_WRITE
+     * @param mode read or write
      * @param uri URI of the array
      * @param name name of the array
-     * @param ctx TileDB context
+     * @param platform_config Config parameter dictionary
      * @param column_names Columns to read
      * @param batch_size Batch size
      * @param result_order Result order
      * @param timestamp Timestamp
      */
     SOMAArray(
-        tiledb_query_type_t mode,
+        OpenMode mode,
+        std::string_view uri,
+        std::string_view name,
+        std::map<std::string, std::string> platform_config,
+        std::vector<std::string> column_names,
+        std::string_view batch_size,
+        ResultOrder result_order,
+        std::optional<std::pair<uint64_t, uint64_t>> timestamp = std::nullopt);
+
+    /**
+     * @brief Construct a new SOMAArray object
+     *
+     * @param mode read or write
+     * @param uri URI of the array
+     * @param name name of the array
+     * @param ctx TileDB context
+     * @param column_names Columns to read
+     * @param batch_size Batch size
+     * @param result_order Read result order: automatic (default), rowmajor, or
+     * colmajor
+     * @param timestamp Timestamp
+     */
+    SOMAArray(
+        OpenMode mode,
         std::string_view uri,
         std::string_view name,
         std::shared_ptr<Context> ctx,
         std::vector<std::string> column_names,
         std::string_view batch_size,
-        std::string_view result_order,
+        ResultOrder result_order,
         std::optional<std::pair<uint64_t, uint64_t>> timestamp = std::nullopt);
 
     SOMAArray() = delete;
     SOMAArray(const SOMAArray&) = delete;
     SOMAArray(SOMAArray&&) = default;
     ~SOMAArray() = default;
 
@@ -152,38 +180,47 @@
      * @return std::string URI
      */
     std::shared_ptr<Context> ctx();
 
     /**
      * Open the SOMAArray object.
      *
-     * @param mode TILEDB_READ or TILEDB_WRITE
+     * @param mode read or write
      * @param timestamp Timestamp
      */
     void open(
-        tiledb_query_type_t mode,
+        OpenMode mode,
         std::optional<std::pair<uint64_t, uint64_t>> timestamp = std::nullopt);
 
     /**
      * Close the SOMAArray object.
      */
     void close();
 
     /**
+     * Check if the SOMAArray is open.
+     *
+     * @return bool true if open
+     */
+    bool is_open() const {
+        return arr_->is_open();
+    }
+
+    /**
      * @brief Reset the state of this SOMAArray object to prepare for a
      * new query, while holding the array open.
      *
      * @param column_names
      * @param batch_size
      * @param result_order
      */
     void reset(
         std::vector<std::string> column_names = {},
         std::string_view batch_size = "auto",
-        std::string_view result_order = "auto");
+        ResultOrder result_order = ResultOrder::automatic);
 
     /**
      * @brief Set the dimension slice using one point
      *
      * @note Partitioning is not supported
      *
      * @tparam T
@@ -532,14 +569,22 @@
 
     /**
      * Return then number of metadata items in an open array. The array must
      * be opened in READ mode, otherwise the function will error out.
      */
     uint64_t metadata_num() const;
 
+    /**
+     * Validates input parameters before opening array.
+     */
+    void validate(
+        OpenMode mode,
+        std::string_view name,
+        std::optional<std::pair<uint64_t, uint64_t>> timestamp);
+
    private:
     //===================================================================
     //= private non-static
     //===================================================================
 
     // TileDB context
     std::shared_ptr<Context> ctx_;
@@ -547,15 +592,15 @@
     // SOMAArray URI
     std::string uri_;
 
     // Batch size
     std::string batch_size_;
 
     // Result order
-    std::string result_order_;
+    ResultOrder result_order_;
 
     // Read timestamp range (start, end)
     std::optional<std::pair<uint64_t, uint64_t>> timestamp_;
 
     // Managed query for the array
     std::unique_ptr<ManagedQuery> mq_;
```

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/soma_dataframe.cc` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/soma_dataframe.cc`

 * *Files 17% similar despite different names*

```diff
@@ -39,80 +39,94 @@
 using namespace tiledb;
 
 //===================================================================
 //= public static
 //===================================================================
 
 std::unique_ptr<SOMADataFrame> SOMADataFrame::create(
-    std::shared_ptr<Context> ctx, std::string_view uri, ArraySchema schema) {
-    if (schema.array_type() != TILEDB_DENSE)
-        throw TileDBSOMAError("ArraySchema must be set to dense.");
+    std::string_view uri,
+    ArraySchema schema,
+    std::map<std::string, std::string> platform_config) {
+    return SOMADataFrame::create(
+        uri, schema, std::make_shared<Context>(Config(platform_config)));
+}
 
+std::unique_ptr<SOMADataFrame> SOMADataFrame::create(
+    std::string_view uri, ArraySchema schema, std::shared_ptr<Context> ctx) {
     SOMAArray::create(ctx, uri, schema, "SOMADataFrame");
-    return std::make_unique<SOMADataFrame>(
-        TILEDB_READ, uri, ctx, std::vector<std::string>(), std::nullopt);
+    return SOMADataFrame::open(uri, OpenMode::read, ctx);
 }
 
 std::unique_ptr<SOMADataFrame> SOMADataFrame::open(
-    tiledb_query_type_t mode,
     std::string_view uri,
-    std::vector<std::string> column_names,
+    OpenMode mode,
     std::map<std::string, std::string> platform_config,
+    std::vector<std::string> column_names,
+    ResultOrder result_order,
     std::optional<std::pair<uint64_t, uint64_t>> timestamp) {
-    auto ctx = std::make_shared<Context>(Config(platform_config));
-    return std::make_unique<SOMADataFrame>(
-        mode, uri, ctx, column_names, timestamp);
+    return SOMADataFrame::open(
+        uri,
+        mode,
+        std::make_shared<Context>(Config(platform_config)),
+        column_names,
+        result_order,
+        timestamp);
 }
 
 std::unique_ptr<SOMADataFrame> SOMADataFrame::open(
-    tiledb_query_type_t mode,
-    std::shared_ptr<Context> ctx,
     std::string_view uri,
+    OpenMode mode,
+    std::shared_ptr<Context> ctx,
     std::vector<std::string> column_names,
+    ResultOrder result_order,
     std::optional<std::pair<uint64_t, uint64_t>> timestamp) {
     return std::make_unique<SOMADataFrame>(
-        mode, uri, ctx, column_names, timestamp);
+        mode, uri, ctx, column_names, result_order, timestamp);
 }
 
 //===================================================================
 //= public non-static
 //===================================================================
 
 SOMADataFrame::SOMADataFrame(
-    tiledb_query_type_t mode,
+    OpenMode mode,
     std::string_view uri,
     std::shared_ptr<Context> ctx,
     std::vector<std::string> column_names,
+    ResultOrder result_order,
     std::optional<std::pair<uint64_t, uint64_t>> timestamp) {
     array_ = std::make_shared<SOMAArray>(
         mode,
         uri,
         "unnamed",  // name
         ctx,
         column_names,
         "auto",  // batch_size,
-        "auto",  // result_order,
+        result_order,
         timestamp);
     array_->reset();
     array_->submit();
 }
 
 void SOMADataFrame::open(
-    tiledb_query_type_t mode,
-    std::optional<std::pair<uint64_t, uint64_t>> timestamp) {
+    OpenMode mode, std::optional<std::pair<uint64_t, uint64_t>> timestamp) {
     array_->open(mode, timestamp);
     array_->reset();
     array_->submit();
 }
 
 void SOMADataFrame::close() {
     array_->close();
 }
 
-const std::string& SOMADataFrame::uri() const {
+bool SOMADataFrame::is_open() const {
+    return array_->is_open();
+}
+
+const std::string SOMADataFrame::uri() const {
     return array_->uri();
 }
 
 std::shared_ptr<Context> SOMADataFrame::ctx() {
     return array_->ctx();
 }
```

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/soma_dataframe.h` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/soma_dataframe.h`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,15 @@
  *   This file defines the SOMADataFrame class.
  */
 
 #ifndef SOMA_DATAFRAME
 #define SOMA_DATAFRAME
 
 #include <tiledb/tiledb>
+#include "enums.h"
 #include "soma_object.h"
 
 namespace tiledbsoma {
 
 class SOMAArray;
 class ArrayBuffers;
 
@@ -48,119 +49,148 @@
     //===================================================================
     //= public static
     //===================================================================
 
     /**
      * @brief Create a SOMADataFrame object at the given URI.
      *
-     * @param ctx TileDB context
      * @param uri URI to create the SOMADataFrame
      * @param schema TileDB ArraySchema
-     * @return std::unique_ptr<SOMADataFrame> opened in read mode
+     * @param platform_config Optional config parameter dictionary
+     * @return std::shared_ptr<SOMADataFrame> opened in read mode
+     */
+    static std::unique_ptr<SOMADataFrame> create(
+        std::string_view uri,
+        ArraySchema schema,
+        std::map<std::string, std::string> platform_config = {});
+
+    /**
+     * @brief Create a SOMADataFrame object at the given URI.
+     *
+     * @param uri URI to create the SOMADataFrame
+     * @param schema TileDB ArraySchema
+     * @param ctx TileDB context
+     * @return std::shared_ptr<SOMADataFrame> opened in read mode
      */
     static std::unique_ptr<SOMADataFrame> create(
-        std::shared_ptr<Context> ctx, std::string_view uri, ArraySchema schema);
+        std::string_view uri, ArraySchema schema, std::shared_ptr<Context> ctx);
 
     /**
      * @brief Open and return a SOMADataFrame object at the given URI.
      *
-     * @param mode TILEDB_READ or TILEDB_WRITE
+     * @param mode read or write
      * @param uri URI to create the SOMADataFrame
      * @param column_names A list of column names to use as user-defined index
      * columns (e.g., ``['cell_type', 'tissue_type']``). All named columns must
      * exist in the schema, and at least one index column name is required.
      * @param platform_config Platform-specific options used to create this
      * DataFrame
+     * @param result_order Read result order: automatic (default), rowmajor, or
+     * colmajor
      * @param timestamp If specified, overrides the default timestamp used to
      * open this object. If unset, uses the timestamp provided by the context.
-     * @return std::unique_ptr<SOMADataFrame> SOMADataFrame
+     * @return std::shared_ptr<SOMADataFrame> SOMADataFrame
      */
     static std::unique_ptr<SOMADataFrame> open(
-        tiledb_query_type_t mode,
         std::string_view uri,
-        std::vector<std::string> column_names = {},
+        OpenMode mode,
         std::map<std::string, std::string> platform_config = {},
+        std::vector<std::string> column_names = {},
+        ResultOrder result_order = ResultOrder::automatic,
         std::optional<std::pair<uint64_t, uint64_t>> timestamp = std::nullopt);
 
     /**
      * @brief Open and return a SOMADataFrame object at the given URI.
      *
-     * @param mode TILEDB_READ or TILEDB_WRITE
+     * @param mode read or write
      * @param ctx TileDB context
      * @param uri URI to create the SOMADataFrame
      * @param schema TileDB ArraySchema
      * @param column_names A list of column names to use as user-defined index
      * columns (e.g., ``['cell_type', 'tissue_type']``). All named columns must
      * exist in the schema, and at least one index column name is required.
+     * @param result_order Read result order: automatic (default), rowmajor, or
+     * colmajor
      * @param timestamp If specified, overrides the default timestamp used to
      * open this object. If unset, uses the timestamp provided by the context.
-     * @return std::unique_ptr<SOMADataFrame> SOMADataFrame
+     * @return std::shared_ptr<SOMADataFrame> SOMADataFrame
      */
     static std::unique_ptr<SOMADataFrame> open(
-        tiledb_query_type_t mode,
-        std::shared_ptr<Context> ctx,
         std::string_view uri,
+        OpenMode mode,
+        std::shared_ptr<Context> ctx,
         std::vector<std::string> column_names = {},
+        ResultOrder result_order = ResultOrder::automatic,
         std::optional<std::pair<uint64_t, uint64_t>> timestamp = std::nullopt);
 
     //===================================================================
     //= public non-static
     //===================================================================
 
     /**
      * @brief Construct a new SOMADataFrame object.
      *
-     * @param mode TILEDB_READ or TILEDB_WRITE
+     * @param mode read or write
      * @param uri URI of the array
      * @param ctx TileDB context
      * @param column_names Columns to read
+     * @param result_order Read result order: automatic (default), rowmajor, or
+     * colmajor
      * @param timestamp Timestamp
      */
     SOMADataFrame(
-        tiledb_query_type_t mode,
+        OpenMode mode,
         std::string_view uri,
         std::shared_ptr<Context> ctx,
         std::vector<std::string> column_names,
-        std::optional<std::pair<uint64_t, uint64_t>> timestamp);
+        ResultOrder result_order,
+        std::optional<std::pair<uint64_t, uint64_t>> timestamp = std::nullopt);
 
     SOMADataFrame() = delete;
     SOMADataFrame(const SOMADataFrame&) = delete;
     SOMADataFrame(SOMADataFrame&&) = default;
     ~SOMADataFrame() = default;
 
     /**
      * Open the SOMADataFrame object.
      *
-     * @param mode TILEDB_READ or TILEDB_WRITE
+     * @param mode read or write
      * @param timestamp Timestamp
      */
     void open(
-        tiledb_query_type_t mode,
+        OpenMode mode,
         std::optional<std::pair<uint64_t, uint64_t>> timestamp = std::nullopt);
 
     /**
      * Close the SOMADataFrame object.
      */
     void close();
 
     /**
+     * Check if the SOMADataFrame is open.
+     *
+     * @return bool true if open
+     */
+    bool is_open() const;
+
+    /**
      * Return the constant "SOMADataFrame".
      *
      * @return std::string
      */
-    std::string type() const {
+    const std::string type() const {
         return "SOMADataFrame";
     }
 
     /**
      * @brief Get the URI of the SOMADataFrame.
      *
      * @return std::string URI
      */
-    const std::string& uri() const;
+    const std::string uri() const;
 
     /**
      * Get the Context associated with the SOMADataFrame.
      *
      * @return std::shared_ptr<Context>
      */
     std::shared_ptr<Context> ctx();
@@ -190,14 +220,15 @@
      * @brief Read the next chunk of results from the query. If all results have
      * already been read, std::nullopt is returned.
      */
     std::optional<std::shared_ptr<ArrayBuffers>> read_next();
 
     /**
      * @brief Write data to the dataframe.
+     * @param buffers The ArrayBuffers to write
      */
     void write(std::shared_ptr<ArrayBuffers> buffers);
 
    private:
     //===================================================================
     //= private non-static
     //===================================================================
```

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/soma_group.cc` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/soma_group.cc`

 * *Files 9% similar despite different names*

```diff
@@ -37,72 +37,84 @@
 namespace tiledbsoma {
 using namespace tiledb;
 
 //===================================================================
 //= public static
 //===================================================================
 
+void SOMAGroup::create(
+    std::shared_ptr<Context> ctx, std::string_view uri, std::string soma_type) {
+    Group::create(*ctx, std::string(uri));
+    auto group = Group(*ctx, std::string(uri), TILEDB_WRITE);
+    group.put_metadata(
+        "soma_object_type", TILEDB_STRING_UTF8, 1, soma_type.c_str());
+    group.close();
+}
+
 std::unique_ptr<SOMAGroup> SOMAGroup::open(
-    tiledb_query_type_t mode,
+    OpenMode mode,
     std::string_view uri,
     std::string_view name,
     std::map<std::string, std::string> platform_config,
     std::optional<uint64_t> timestamp) {
     return std::make_unique<SOMAGroup>(
         mode,
         uri,
         name,
         std::make_shared<Context>(Config(platform_config)),
         timestamp);
 }
 
 std::unique_ptr<SOMAGroup> SOMAGroup::open(
-    tiledb_query_type_t mode,
+    OpenMode mode,
     std::shared_ptr<Context> ctx,
     std::string_view uri,
     std::string_view name,
     std::optional<uint64_t> timestamp) {
     return std::make_unique<SOMAGroup>(mode, uri, name, ctx, timestamp);
 }
 
 //===================================================================
 //= public non-static
 //===================================================================
 
 SOMAGroup::SOMAGroup(
-    tiledb_query_type_t mode,
+    OpenMode mode,
     std::string_view uri,
     std::string_view name,
     std::shared_ptr<Context> ctx,
     std::optional<uint64_t> timestamp)
     : ctx_(ctx)
     , uri_(util::rstrip_uri(uri))
     , name_(name) {
     auto cfg = ctx_->config();
     if (timestamp) {
         cfg["sm.group.timestamp_end"] = timestamp.value();
     }
-    group_ = std::make_unique<Group>(*ctx_, std::string(uri), mode, cfg);
+    group_ = std::make_unique<Group>(
+        *ctx_,
+        std::string(uri),
+        mode == OpenMode::read ? TILEDB_READ : TILEDB_WRITE,
+        cfg);
 }
 
-void SOMAGroup::open(
-    tiledb_query_type_t query_type, std::optional<uint64_t> timestamp) {
+void SOMAGroup::open(OpenMode query_type, std::optional<uint64_t> timestamp) {
     if (timestamp) {
         auto cfg = ctx_->config();
         cfg["sm.group.timestamp_end"] = timestamp.value();
         group_->set_config(cfg);
     }
-    group_->open(query_type);
+    group_->open(query_type == OpenMode::read ? TILEDB_READ : TILEDB_WRITE);
 }
 
 void SOMAGroup::close() {
     group_->close();
 }
 
-std::string SOMAGroup::uri() const {
+const std::string SOMAGroup::uri() const {
     return group_->uri();
 }
 
 std::shared_ptr<Context> SOMAGroup::ctx() {
     return ctx_;
 }
 
@@ -120,15 +132,19 @@
     } catch (const TileDBError& e) {
         return false;
     }
     return true;
 }
 
 void SOMAGroup::add_member(
-    const std::string& uri, bool relative, const std::string& name) {
+    const std::string& uri, URIType uri_type, const std::string& name) {
+    bool relative = uri_type == URIType::relative;
+    if (uri_type == URIType::automatic) {
+        relative = uri.find("://") != std::string::npos;
+    }
     group_->add_member(uri, relative, name);
 }
 
 uint64_t SOMAGroup::get_length() const {
     return group_->member_count();
 }
```

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/soma_group.h` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/soma_group.h`

 * *Files 5% similar despite different names*

```diff
@@ -35,104 +35,124 @@
 
 #include <future>
 #include <stdexcept>
 #include <tiledb/tiledb>
 #include <tiledb/tiledb_experimental>
 
 #include "../utils/common.h"
+#include "enums.h"
 
 namespace tiledbsoma {
 using namespace tiledb;
 
 class SOMAGroup {
    public:
     //===================================================================
     //= public static
     //===================================================================
 
     /**
+     * @brief Create a SOMAGroup object at the given URI.
+     *
+     * @param ctx TileDB context
+     * @param uri URI to create the SOMAGroup
+     * @param soma_type SOMACollection, SOMAMeasurement, or SOMAExperiment
+     */
+    static void create(
+        std::shared_ptr<Context> ctx,
+        std::string_view uri,
+        std::string soma_type);
+
+    /**
      * @brief Open a group at the specified URI and return SOMAGroup
      * object.
      *
-     * @param mode TILEDB_READ or TILEDB_WRITE
+     * @param mode read or write
      * @param uri URI of the group
      * @param name Name of the group
      * @param platform_config Config parameter dictionary
      * @param timestamp Timestamp
      * @return std::unique_ptr<SOMAGroup> SOMAGroup
      */
     static std::unique_ptr<SOMAGroup> open(
-        tiledb_query_type_t mode,
+        OpenMode mode,
         std::string_view uri,
         std::string_view name = "unnamed",
         std::map<std::string, std::string> platform_config = {},
         std::optional<uint64_t> timestamp = std::nullopt);
 
     /**
      * @brief Open a group at the specified URI and return SOMAGroup
      * object.
      *
-     * @param mode TILEDB_READ or TILEDB_WRITE
+     * @param mode read or write
      * @param ctx TileDB context
      * @param uri URI of the group
      * @param name Name of the group
      * @param timestamp Timestamp
      * @return std::unique_ptr<SOMAGroup> SOMAGroup
      */
     static std::unique_ptr<SOMAGroup> open(
-        tiledb_query_type_t mode,
+        OpenMode mode,
         std::shared_ptr<Context> ctx,
         std::string_view uri,
         std::string_view name = "unnamed",
         std::optional<uint64_t> timestamp = std::nullopt);
 
     //===================================================================
     //= public non-static
     //===================================================================
 
     /**
      * @brief Construct a new SOMAGroup object.
      *
-     * @param mode TILEDB_READ or TILEDB_WRITE
+     * @param mode read or write
      * @param uri URI of the group
      * @param name Name of the group
      * @param ctx TileDB context
      * @param timestamp Timestamp
      */
     SOMAGroup(
-        tiledb_query_type_t mode,
+        OpenMode mode,
         std::string_view uri,
         std::string_view name,
         std::shared_ptr<Context> ctx,
         std::optional<uint64_t> timestamp = std::nullopt);
 
     SOMAGroup() = delete;
     SOMAGroup(const SOMAGroup&) = delete;
     SOMAGroup(SOMAGroup&&) = default;
     ~SOMAGroup() = default;
 
     /**
      * Open the SOMAGroup object.
      *
-     * @param mode TILEDB_READ or TILEDB_WRITE
+     * @param mode read or write
      * @param timestamp Timestamp
      */
-    void open(
-        tiledb_query_type_t mode,
-        std::optional<uint64_t> timestamp = std::nullopt);
+    void open(OpenMode mode, std::optional<uint64_t> timestamp = std::nullopt);
 
     /**
      * Close the SOMAGroup object.
      */
     void close();
 
     /**
+     * Check if the SOMAGroup is open.
+     *
+     * @return bool true if open
+     */
+    bool is_open() const {
+        return group_->is_open();
+    }
+
+    /**
      * Get the SOMAGroup URI.
      */
-    std::string uri() const;
+    const std::string uri() const;
 
     /**
      * Get the Context associated with the SOMAGroup.
      *
      * @return std::shared_ptr<Context>
      */
     std::shared_ptr<Context> ctx();
@@ -158,19 +178,20 @@
      */
     bool has_member(const std::string& name);
 
     /**
      * Add a named member to a SOMAGroup.
      *
      * @param uri of member to add
-     * @param relative is the URI relative to the SOMAGroup location
+     * @param uri_type whether the given URI is automatic (default), absolute,
+     * or relative
      * @param name of member
      */
     void add_member(
-        const std::string& uri, bool relative, const std::string& name);
+        const std::string& uri, URIType uri_type, const std::string& name);
 
     /**
      * Get the number of members in the SOMAGroup.
      */
     uint64_t get_length() const;
 
     /**
```

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/soma_object.h` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/soma/soma_object.h`

 * *Files 11% similar despite different names*

```diff
@@ -50,26 +50,36 @@
     virtual ~SOMAObject() = default;
 
     /**
      * @brief Return a constant string describing the type of the object.
      *
      * @return std::string SOMA type
      */
-    virtual std::string type() const = 0;
+    virtual const std::string type() const = 0;
 
     /**
      * @brief Get URI of the SOMAObject.
      *
      * @return std::string URI
      */
-    virtual const std::string& uri() const = 0;
+    virtual const std::string uri() const = 0;
 
     /**
-     * Get the context associated with the SOMAObject.
+     * @brief Get the context associated with the SOMAObject.
      *
      * @return std::shared_ptr<Context>
      */
     virtual std::shared_ptr<Context> ctx() = 0;
+
+    /**
+     * @brief Close the SOMAObject.
+     */
+    virtual void close() = 0;
+
+    /**
+     * @brief Check if the SOMAObject is open.
+     */
+    virtual bool is_open() const = 0;
 };
 }  // namespace tiledbsoma
 
 #endif  // SOMA_OBJECT
```

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/utils/stats.h`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 /**
- * @file   tiledbsoma
+ * @file   stats.h
  *
  * @section LICENSE
  *
  * The MIT License
  *
- * @copyright Copyright (c) 2022 TileDB, Inc.
+ * @copyright Copyright (c) 2023 TileDB, Inc.
  *
  * Permission is hereby granted, free of charge, to any person obtaining a copy
  * of this software and associated documentation files (the "Software"), to deal
  * in the Software without restriction, including without limitation the rights
  * to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  * copies of the Software, and to permit persons to whom the Software is
  * furnished to do so, subject to the following conditions:
@@ -23,36 +23,27 @@
  * AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
  * LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
  * OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
  * THE SOFTWARE.
  *
  * @section DESCRIPTION
  *
- * This is the main import header for the C++ API
+ *   This declares the common functions in the API
  */
 
-#ifndef __TILEDBSOMA__
-#define __TILEDBSOMA__
+#ifndef TILEDBSOMA_STATS_H
+#define TILEDBSOMA_STATS_H
 
-// TODO Uncomment after finishing Python and R bindings
-// #include "soma_collection.h"
-// #include "soma_dataframe.h"
-// #include "soma_dense_ndarray.h"
-// #include "soma_experiment.h"
-// #include "soma_measurement.h"
-// #include "soma_object.h"
-// #include "soma_sparse_ndarray.h"
-
-#include "utils/arrow_adapter.h"
-#include "utils/common.h"
-#include "utils/stats.h"
-#include "utils/version.h"
-#include "soma/logger_public.h"
-#include "soma/managed_query.h"
-#include "soma/array_buffers.h"
-#include "soma/column_buffer.h"
-#include "soma/soma_array.h"
-#include "soma/soma_group.h"
-#include "soma/soma_object.h"
-#include "soma/soma_dataframe.h"
+#include <stdexcept>  // for windows: error C2039: 'runtime_error': is not a member of 'std'
 
-#endif
+#include <string>
+
+namespace tiledbsoma::stats {
+
+void enable();
+void disable();
+void reset();
+std::string dump();
+
+};  // namespace tiledbsoma::stats
+
+#endif  // TILEDBSOMA_STATS_H
```

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/arrow_adapter.h` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/utils/arrow_adapter.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/carrow.h` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/utils/carrow.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/common.h` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/utils/common.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/logger.cc` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/utils/logger.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/logger.h` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/utils/logger.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/stats.cc` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/utils/stats.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/stats.h` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/utils/version.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * @file   stats.h
+ * @file   version.h
  *
  * @section LICENSE
  *
  * The MIT License
  *
  * @copyright Copyright (c) 2023 TileDB, Inc.
  *
@@ -23,27 +23,25 @@
  * AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
  * LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
  * OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
  * THE SOFTWARE.
  *
  * @section DESCRIPTION
  *
- *   This declares the common functions in the API
+ * This exposes the version of the TileDB Embedded library in use.
  */
 
-#ifndef TILEDBSOMA_STATS_H
-#define TILEDBSOMA_STATS_H
+#ifndef TILEDBSOMA_VERSION_H
+#define TILEDBSOMA_VERSION_H
 
 #include <stdexcept>  // for windows: error C2039: 'runtime_error': is not a member of 'std'
 
 #include <string>
 
-namespace tiledbsoma::stats {
+namespace tiledbsoma::version {
 
-void enable();
-void disable();
-void reset();
-std::string dump();
+std::string as_string();
+std::tuple<int, int, int> embedded_version_triple();
 
-};  // namespace tiledbsoma::stats
+};  // namespace tiledbsoma::version
 
-#endif  // TILEDBSOMA_STATS_H
+#endif  // TILEDBSOMA_VERSION_H
```

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/util.cc` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/utils/util.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/util.h` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/utils/util.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/version.cc` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/src/utils/version.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/CMakeLists.txt` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/test/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 add_executable(unit_soma EXCLUDE_FROM_ALL
     $<TARGET_OBJECTS:TILEDB_SOMA_OBJECTS>
     unit_column_buffer.cc
     unit_managed_query.cc
     unit_soma_array.cc
     unit_soma_group.cc
     unit_soma_dataframe.cc
+    unit_soma_dense_ndarray.cc
+    unit_soma_sparse_ndarray.cc
+    unit_soma_collection.cc
 # TODO: uncomment when thread_pool is enabled
 #    unit_thread_pool.cc
 )
 
 target_link_libraries(unit_soma
   PRIVATE
     Catch2::Catch2WithMain
```

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/test_query_condition.py` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/test/test_query_condition.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/test_simple.py` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/test/test_simple.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/test_soma_array.py` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/test/test_soma_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/unit_column_buffer.cc` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/test/unit_column_buffer.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/unit_managed_query.cc` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/test/unit_managed_query.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/unit_soma_array.cc` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/test/unit_soma_array.cc`

 * *Files 8% similar despite different names*

```diff
@@ -122,21 +122,21 @@
     std::iota(frags.begin(), frags.end(), 0);
     std::shuffle(frags.begin(), frags.end(), std::random_device{});
 
     // Write to SOMAArray
     for (auto i = 0; i < num_fragments; ++i) {
         auto frag_num = frags[i];
         auto soma_array = SOMAArray::open(
-            TILEDB_WRITE,
+            OpenMode::write,
             ctx,
             uri,
             "",
             {},
             "auto",
-            "auto",
+            ResultOrder::automatic,
             std::pair<uint64_t, uint64_t>(timestamp + i, timestamp + i));
 
         if (LOG_DEBUG_ENABLED()) {
             soma_array->schema()->dump();
         }
 
         std::vector<int64_t> d0(num_cells_per_fragment);
@@ -215,21 +215,21 @@
             num_cells_per_fragment,
             num_fragments,
             overlap,
             timestamp);
 
         // Get total cell num
         auto soma_array = SOMAArray::open(
-            TILEDB_READ,
+            OpenMode::read,
             ctx,
             uri,
             "",
             {},
             "auto",
-            "auto",
+            ResultOrder::automatic,
             std::pair<uint64_t, uint64_t>(
                 timestamp, timestamp + num_fragments - 1));
 
         uint64_t nnz = soma_array->nnz();
         REQUIRE(nnz == expected_nnz);
 
         std::vector<int64_t> shape = soma_array->shape();
@@ -287,15 +287,22 @@
         // not be included in the nnz call with a timestamp
         write_array(
             uri, ctx, num_cells_per_fragment, num_fragments, overlap, 40);
 
         // Get total cell num at timestamp (0, 20)
         std::pair<uint64_t, uint64_t> timestamp{0, 20};
         auto soma_array = SOMAArray::open(
-            TILEDB_READ, ctx, uri, "nnz", {}, "auto", "auto", timestamp);
+            OpenMode::read,
+            ctx,
+            uri,
+            "nnz",
+            {},
+            "auto",
+            ResultOrder::automatic,
+            timestamp);
 
         uint64_t nnz = soma_array->nnz();
         REQUIRE(nnz == expected_nnz);
     }
 }
 
 TEST_CASE("SOMAArray: nnz with consolidation") {
@@ -337,15 +344,21 @@
         Array::consolidate(*ctx, uri);
         if (vacuum) {
             Array::vacuum(*ctx, uri);
         }
 
         // Get total cell num
         auto soma_array = SOMAArray::open(
-            TILEDB_READ, ctx, uri, "nnz", {}, "auto", "auto");
+            OpenMode::read,
+            ctx,
+            uri,
+            "nnz",
+            {},
+            "auto",
+            ResultOrder::automatic);
 
         uint64_t nnz = soma_array->nnz();
         if (allow_duplicates) {
             // Since we wrote twice
             REQUIRE(nnz == 2 * expected_nnz);
         } else {
             REQUIRE(nnz == expected_nnz);
@@ -356,27 +369,27 @@
 TEST_CASE("SOMAArray: metadata") {
     auto ctx = std::make_shared<Context>();
 
     std::string base_uri = "mem://unit-test-array";
     const auto& [uri, expected_nnz] = create_array(base_uri, ctx);
 
     auto soma_array = SOMAArray::open(
-        TILEDB_WRITE,
+        OpenMode::write,
         ctx,
         uri,
         "metadata_test",
         {},
         "auto",
-        "auto",
+        ResultOrder::automatic,
         std::pair<uint64_t, uint64_t>(1, 1));
     int32_t val = 100;
     soma_array->set_metadata("md", TILEDB_INT32, 1, &val);
     soma_array->close();
 
-    soma_array->open(TILEDB_READ, std::pair<uint64_t, uint64_t>(1, 1));
+    soma_array->open(OpenMode::read, std::pair<uint64_t, uint64_t>(1, 1));
     REQUIRE(soma_array->has_metadata("md") == true);
     REQUIRE(soma_array->metadata_num() == 1);
 
     auto mdval = soma_array->get_metadata(0);
     REQUIRE(std::get<MetadataInfo::key>(mdval) == "md");
     REQUIRE(std::get<MetadataInfo::dtype>(mdval) == TILEDB_INT32);
     REQUIRE(std::get<MetadataInfo::num>(mdval) == 1);
@@ -385,19 +398,19 @@
     mdval = soma_array->get_metadata("md");
     REQUIRE(std::get<MetadataInfo::key>(mdval) == "md");
     REQUIRE(std::get<MetadataInfo::dtype>(mdval) == TILEDB_INT32);
     REQUIRE(std::get<MetadataInfo::num>(mdval) == 1);
     REQUIRE(*((const int32_t*)std::get<MetadataInfo::value>(mdval)) == 100);
     soma_array->close();
 
-    soma_array->open(TILEDB_WRITE, std::pair<uint64_t, uint64_t>(2, 2));
+    soma_array->open(OpenMode::write, std::pair<uint64_t, uint64_t>(2, 2));
     soma_array->delete_metadata("md");
     soma_array->close();
 
-    soma_array->open(TILEDB_READ, std::pair<uint64_t, uint64_t>(3, 3));
+    soma_array->open(OpenMode::read, std::pair<uint64_t, uint64_t>(3, 3));
     REQUIRE(soma_array->has_metadata("md") == false);
     REQUIRE(soma_array->metadata_num() == 0);
     soma_array->close();
 }
 
 TEST_CASE("SOMAArray: Test buffer size") {
     // Test soma.init_buffer_bytes by making buffer small
@@ -407,15 +420,15 @@
     Config cfg;
     cfg["soma.init_buffer_bytes"] = 8;
     auto ctx = std::make_shared<Context>(cfg);
 
     std::string base_uri = "mem://unit-test-array";
     auto [uri, expected_nnz] = create_array(base_uri, ctx);
     auto [expected_d0, expected_a0] = write_array(uri, ctx);
-    auto soma_array = SOMAArray::open(TILEDB_READ, ctx, uri);
+    auto soma_array = SOMAArray::open(OpenMode::read, ctx, uri);
 
     size_t loops = 0;
     soma_array->submit();
     while (auto batch = soma_array->read_next())
         ++loops;
     REQUIRE(loops == 10);
     soma_array->close();
```

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/unit_soma_dataframe.cc` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/test/unit_soma_dataframe.cc`

 * *Files 3% similar despite different names*

```diff
@@ -76,19 +76,20 @@
 }
 };  // namespace
 
 TEST_CASE("SOMADataFrame: basic") {
     auto ctx = std::make_shared<Context>();
     std::string uri = "mem://unit-test-dataframe-basic";
 
-    SOMADataFrame::create(ctx, uri, create_schema(*ctx));
+    SOMADataFrame::create(uri, create_schema(*ctx), ctx);
 
-    auto soma_dataframe = SOMADataFrame::open(TILEDB_READ, ctx, uri);
+    auto soma_dataframe = SOMADataFrame::open(uri, OpenMode::read, ctx);
     REQUIRE(soma_dataframe->uri() == uri);
     REQUIRE(soma_dataframe->ctx() == ctx);
+    REQUIRE(soma_dataframe->type() == "SOMADataFrame");
     auto schema = soma_dataframe->schema();
     REQUIRE(schema->has_attribute("a0"));
     REQUIRE(schema->domain().has_dimension("d0"));
     std::vector<std::string> expected_index_column_names = {"d0"};
     REQUIRE(
         soma_dataframe->index_column_names() == expected_index_column_names);
     REQUIRE(soma_dataframe->count() == 1);
@@ -97,19 +98,19 @@
     std::vector<int64_t> d0{1, 10};
     std::vector<int> a0(10, 1);
 
     auto array_buffer = std::make_shared<ArrayBuffers>();
     array_buffer->emplace("a0", ColumnBuffer::create(*schema, "a0", a0));
     array_buffer->emplace("d0", ColumnBuffer::create(*schema, "d0", d0));
 
-    soma_dataframe->open(TILEDB_WRITE);
+    soma_dataframe->open(OpenMode::write);
     soma_dataframe->write(array_buffer);
     soma_dataframe->close();
 
-    soma_dataframe->open(TILEDB_READ);
+    soma_dataframe->open(OpenMode::read);
     while (auto batch = soma_dataframe->read_next()) {
         auto arrbuf = batch.value();
         auto d0span = arrbuf->at("d0")->data<int64_t>();
         auto a0span = arrbuf->at("a0")->data<int>();
         REQUIRE(
             std::vector<int64_t>{1, 2, 3, 4, 5, 6, 7, 8, 9, 10} ==
             std::vector<int64_t>(d0span.begin(), d0span.end()));
```

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/unit_soma_group.cc` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/test/unit_soma_group.cc`

 * *Files 5% similar despite different names*

```diff
@@ -150,60 +150,60 @@
 
 };  // namespace
 
 TEST_CASE("SOMAGroup: basic") {
     auto ctx = std::make_shared<Context>();
 
     std::string uri_main_group = "mem://main-group";
-    Group::create(*ctx, uri_main_group);
+    SOMAGroup::create(ctx, uri_main_group, "NONE");
 
     std::string uri_sub_group = "mem://sub-group";
-    Group::create(*ctx, uri_sub_group);
+    SOMAGroup::create(ctx, uri_sub_group, "NONE");
 
     auto [uri_sub_array, expected_nnz] = create_array("mem://sub-array", *ctx);
 
     auto soma_group = SOMAGroup::open(
-        TILEDB_WRITE, ctx, uri_main_group, "metadata", 1);
-    soma_group->add_member(uri_sub_group, false, "subgroup");
-    soma_group->add_member(uri_sub_array, false, "subarray");
+        OpenMode::write, ctx, uri_main_group, "metadata", 1);
+    soma_group->add_member(uri_sub_group, URIType::absolute, "subgroup");
+    soma_group->add_member(uri_sub_array, URIType::absolute, "subarray");
     soma_group->close();
 
-    soma_group->open(TILEDB_READ, 1);
+    soma_group->open(OpenMode::read, 1);
     REQUIRE(soma_group->ctx() == ctx);
     REQUIRE(soma_group->uri() == uri_main_group);
     REQUIRE(soma_group->get_length() == 2);
     std::map<std::string, std::string> expected_map{
         {"subgroup", uri_sub_group}, {"subarray", uri_sub_array}};
     REQUIRE(expected_map == soma_group->member_to_uri_mapping());
     REQUIRE(soma_group->get_member("subgroup").type() == Object::Type::Group);
     REQUIRE(soma_group->get_member("subarray").type() == Object::Type::Array);
     soma_group->close();
 
-    soma_group->open(TILEDB_WRITE, 3);
+    soma_group->open(OpenMode::write, 3);
     soma_group->remove_member("subgroup");
     soma_group->close();
 
-    soma_group->open(TILEDB_READ, 4);
+    soma_group->open(OpenMode::read, 4);
     REQUIRE(soma_group->get_length() == 1);
     REQUIRE(soma_group->has_member("subgroup") == false);
     REQUIRE(soma_group->has_member("subarray") == true);
     soma_group->close();
 }
 
 TEST_CASE("SOMAGroup: metadata") {
     auto ctx = std::make_shared<Context>();
 
     std::string uri = "mem://unit-test-group";
     Group::create(*ctx, uri);
-    auto soma_group = SOMAGroup::open(TILEDB_WRITE, ctx, uri, "metadata", 1);
+    auto soma_group = SOMAGroup::open(OpenMode::write, ctx, uri, "metadata", 1);
     int32_t val = 100;
     soma_group->set_metadata("md", TILEDB_INT32, 1, &val);
     soma_group->close();
 
-    soma_group->open(TILEDB_READ, 1);
+    soma_group->open(OpenMode::read, 1);
     REQUIRE(soma_group->has_metadata("md") == true);
     REQUIRE(soma_group->metadata_num() == 1);
 
     auto mdval = soma_group->get_metadata(0);
     REQUIRE(std::get<MetadataInfo::key>(mdval) == "md");
     REQUIRE(std::get<MetadataInfo::dtype>(mdval) == TILEDB_INT32);
     REQUIRE(std::get<MetadataInfo::num>(mdval) == 1);
@@ -212,16 +212,16 @@
     mdval = soma_group->get_metadata("md");
     REQUIRE(std::get<MetadataInfo::key>(mdval) == "md");
     REQUIRE(std::get<MetadataInfo::dtype>(mdval) == TILEDB_INT32);
     REQUIRE(std::get<MetadataInfo::num>(mdval) == 1);
     REQUIRE(*((const int32_t*)std::get<MetadataInfo::value>(mdval)) == 100);
     soma_group->close();
 
-    soma_group->open(TILEDB_WRITE, 2);
+    soma_group->open(OpenMode::write, 2);
     soma_group->delete_metadata("md");
     soma_group->close();
 
-    soma_group->open(TILEDB_READ, 3);
+    soma_group->open(OpenMode::read, 3);
     REQUIRE(soma_group->has_metadata("md") == false);
     REQUIRE(soma_group->metadata_num() == 0);
     soma_group->close();
 }
```

### Comparing `tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/unit_thread_pool.cc` & `tiledbsoma-1.4.0/dist_links/libtiledbsoma/test/unit_thread_pool.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/scripts/bld` & `tiledbsoma-1.4.0/dist_links/scripts/bld`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/scripts/run-clang-format.sh` & `tiledbsoma-1.4.0/dist_links/scripts/run-clang-format.sh`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/scripts/show-versions.py` & `tiledbsoma-1.4.0/dist_links/scripts/show-versions.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/dist_links/scripts/update-tiledb-version.py` & `tiledbsoma-1.4.0/dist_links/scripts/update-tiledb-version.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/setup.py` & `tiledbsoma-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,16 +286,16 @@
         "numba==0.57; python_version=='3.11'",
         "numpy>=1.18,<1.24; python_version<'3.11'",
         "numpy>=1.18,<1.25; python_version=='3.11'",
         "pandas",
         "pyarrow>=9.0.0",
         "scanpy>=1.9.2",
         "scipy",
-        "somacore==1.0.3",
-        "tiledb~=0.22.0",
+        "somacore==1.0.4",
+        "tiledb~=0.22.2",
         "typing-extensions",  # Note "-" even though `import typing_extensions`
     ],
     extras_require={
         "dev": [
             "black",
             "ruff",
             "pytest",
```

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/__init__.py` & `tiledbsoma-1.4.0/src/tiledbsoma/__init__.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/_arrow_types.py` & `tiledbsoma-1.4.0/src/tiledbsoma/_arrow_types.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 fully supported in SOMA DataFrame non-indexed columns.
 """
 
 from typing import Any, Dict, Union
 
 import numpy as np
 import numpy.typing as npt
+import pandas as pd
 import pyarrow as pa
 import tiledb
 
 _ARROW_TO_TDB_ATTR: Dict[Any, Union[str, TypeError]] = {
     pa.string(): "U1",
     pa.large_string(): "U1",
     pa.binary(): "bytes",
@@ -155,7 +156,36 @@
         attr = tdb_schema.attr(i)
         name = attr.name
         if name == "":
             name = "unnamed"
         arrow_schema_dict[name] = arrow_type_from_tiledb_dtype(attr.dtype, attr.isascii)
 
     return pa.schema(arrow_schema_dict)
+
+
+def df_to_arrow(df: pd.DataFrame) -> pa.Table:
+    """
+    Categoricals are not yet well supported, so we must flatten.
+    Also replace Numpy/Pandas-style nulls with Arrow-style nulls.
+    """
+    null_fields = set()
+    # Not for name, col in df.items() since we need df[k] on the left-hand sides
+    for k in df:
+        if df[k].dtype == "category":
+            df[k] = df[k].astype(df[k].cat.categories.dtype)
+        if df[k].isnull().any():
+            if df[k].isnull().all():
+                df[k] = pa.nulls(df.shape[0], pa.infer_type(df[k]))
+            else:
+                df[k].where(
+                    df[k].notnull(),
+                    pd.Series(pa.nulls(df[k].isnull().sum(), pa.infer_type(df[k]))),
+                    inplace=True,
+                )
+            null_fields.add(k)
+    arrow_table = pa.Table.from_pandas(df)
+    if null_fields:
+        md = arrow_table.schema.metadata
+        md.update(dict.fromkeys(null_fields, "nullable"))
+        arrow_table = arrow_table.replace_schema_metadata(md)
+
+    return arrow_table
```

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/_collection.py` & `tiledbsoma-1.4.0/src/tiledbsoma/_collection.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/_common_nd_array.py` & `tiledbsoma-1.4.0/src/tiledbsoma/_common_nd_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/_dataframe.py` & `tiledbsoma-1.4.0/src/tiledbsoma/_dataframe.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/_dense_nd_array.py` & `tiledbsoma-1.4.0/src/tiledbsoma/_dense_nd_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/_exception.py` & `tiledbsoma-1.4.0/src/tiledbsoma/_exception.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/_experiment.py` & `tiledbsoma-1.4.0/src/tiledbsoma/_experiment.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/_factory.py` & `tiledbsoma-1.4.0/src/tiledbsoma/_factory.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/_funcs.py` & `tiledbsoma-1.4.0/src/tiledbsoma/_funcs.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/_general_utilities.py` & `tiledbsoma-1.4.0/src/tiledbsoma/_general_utilities.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/_measurement.py` & `tiledbsoma-1.4.0/src/tiledbsoma/_measurement.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/_query_condition.py` & `tiledbsoma-1.4.0/src/tiledbsoma/_query_condition.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 #
 # Licensed under the MIT License.
 
 """A high level wrapper around the Pybind11 query_condition.cc implementation for
 filtering query results on attribute values.
 """
 import ast
-from dataclasses import dataclass, field
 from typing import Any, Callable, List, Tuple, Union
 
+import attrs
 import numpy as np
 import tiledb
 
 from . import pytiledbsoma as clib
 from ._exception import SOMAError
 
 # In Python 3.7, a boolean literal like `True` is of type `ast.NameConstant`.
 # Above that, it's of type `ast.Constant`.
 QueryConditionNodeElem = Union[
     ast.Name, ast.Constant, ast.NameConstant, ast.Call, ast.Num, ast.Str, ast.Bytes
 ]
 
 
-@dataclass
+@attrs.define
 class QueryCondition:
     """Class representing a TileDB query condition object for attribute filtering
     pushdown.
 
     A query condition is set with a string representing an expression
     as defined by the grammar below. A more straight forward example of usage is
     given beneath.
@@ -106,18 +106,18 @@
             # 1, 2, or 3.
             # Note this is equivalent to:
             # "foo == 1 or foo == 2 or foo == 3"
             foo_123 = dataframe.read(value_filter="foo in [1, 2, 3]")
     """
 
     expression: str
-    tree: ast.Expression = field(init=False, repr=False)
-    c_obj: clib.PyQueryCondition = field(init=False, repr=False)
+    tree: ast.Expression = attrs.field(init=False, repr=False)
+    c_obj: clib.PyQueryCondition = attrs.field(init=False, repr=False)
 
-    def __post_init__(self):
+    def __attrs_post_init__(self):
         try:
             self.tree = ast.parse(self.expression, mode="eval")
         except Exception as pex:
             raise SOMAError(
                 "Could not parse the given QueryCondition statement: "
                 f"{self.expression}"
             ) from pex
@@ -137,15 +137,15 @@
                 "Malformed query condition statement. A query condition must "
                 "be made up of one or more Boolean expressions."
             )
 
         return query_attrs
 
 
-@dataclass
+@attrs.define
 class QueryConditionTree(ast.NodeVisitor):
     schema: tiledb.ArraySchema
     query_attrs: List[str]
 
     def visit_BitOr(self, node):
         return clib.TILEDB_OR
```

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/_read_iters.py` & `tiledbsoma-1.4.0/src/tiledbsoma/_read_iters.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/_sparse_nd_array.py` & `tiledbsoma-1.4.0/src/tiledbsoma/_sparse_nd_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/_tdb_handles.py` & `tiledbsoma-1.4.0/src/tiledbsoma/_tdb_handles.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/_tiledb_array.py` & `tiledbsoma-1.4.0/src/tiledbsoma/_tiledb_array.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,16 +104,21 @@
         if schema:
             kwargs["schema"] = schema
         if column_names:
             kwargs["column_names"] = column_names
         if query_condition:
             kwargs["query_condition"] = query_condition
         if result_order:
-            result_order_str = ResultOrder(result_order).value
-            kwargs["result_order"] = result_order_str
+            result_order_map = {
+                "auto": clib.ResultOrder.automatic,
+                "row-major": clib.ResultOrder.rowmajor,
+                "column-major": clib.ResultOrder.colmajor,
+            }
+            result_order_enum = result_order_map[ResultOrder(result_order).value]
+            kwargs["result_order"] = result_order_enum
         return clib.SOMAArray(
             self.uri,
             name=f"{self} reader",
             platform_config=self._ctx.config().dict(),
             timestamp=(0, self.tiledb_timestamp_ms),
             **kwargs,
         )
```

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/_tiledb_object.py` & `tiledbsoma-1.4.0/src/tiledbsoma/_tiledb_object.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/_types.py` & `tiledbsoma-1.4.0/src/tiledbsoma/_types.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/_util.py` & `tiledbsoma-1.4.0/src/tiledbsoma/_util.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/eta.py` & `tiledbsoma-1.4.0/src/tiledbsoma/eta.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/experiment_query.py` & `tiledbsoma-1.4.0/src/tiledbsoma/experiment_query.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/io/conversions.py` & `tiledbsoma-1.4.0/src/tiledbsoma/io/conversions.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,28 +22,31 @@
 _str_to_type = {"boolean": bool, "string": str, "bytes": bytes}
 
 
 def decategoricalize_obs_or_var(obs_or_var: pd.DataFrame) -> pd.DataFrame:
     """Performs a typecast into types that TileDB can persist."""
     if len(obs_or_var.columns) > 0:
         return pd.DataFrame.from_dict(
-            {k: to_tiledb_supported_array_type(v) for k, v in obs_or_var.items()},
+            {
+                str(k): to_tiledb_supported_array_type(str(k), v)
+                for k, v in obs_or_var.items()
+            },
         )
     else:
         return obs_or_var
 
 
 @typeguard_ignore
 def _to_tiledb_supported_dtype(dtype: _DT) -> _DT:
     """A handful of types are cast into the TileDB type system."""
     # TileDB has no float16 -- cast up to float32
     return cast(_DT, np.dtype("float32")) if dtype == np.dtype("float16") else dtype
 
 
-def to_tiledb_supported_array_type(x: _MT) -> _MT:
+def to_tiledb_supported_array_type(name: str, x: _MT) -> _MT:
     """Converts datatypes unrepresentable by TileDB into datatypes it can represent.
     E.g., categorical strings -> string.
 
     See also `https://docs.scipy.org/doc/numpy-1.10.1/reference/arrays.dtypes.html ,https://docs.scipy.org/doc/numpy-1.10.1/reference/arrays.dtypes.html>`_.
 
     Preferentially converts to the underlying primitive type, as TileDB does not support
     most complex types. NOTE: this does not support ``datetime64`` conversion.
@@ -59,15 +62,15 @@
         return x if target_dtype == x.dtype else x.astype(target_dtype)
 
     categories = x.cat.categories
     cat_dtype = categories.dtype
     if cat_dtype.kind in ("f", "u", "i"):
         if x.hasnans and cat_dtype.kind == "i":
             raise ValueError(
-                "Categorical array contains NaN -- unable to convert to TileDB array."
+                f"Categorical column {name!r} contains NaN -- unable to convert to TileDB array."
             )
         # More mysterious spurious mypy errors.
         target_dtype = _to_tiledb_supported_dtype(cat_dtype)  # type: ignore[arg-type]
     else:
         # Into the weirdness. See if Pandas can help with edge cases.
         inferred = infer_dtype(categories)
         if x.hasnans and inferred in ("boolean", "bytes"):
```

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/io/ingest.py` & `tiledbsoma-1.4.0/src/tiledbsoma/io/ingest.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     Measurement,
     SparseNDArray,
     _factory,
     _util,
     eta,
     logging,
 )
+from .._arrow_types import df_to_arrow
 from .._collection import AnyTileDBCollection
 from .._common_nd_array import NDArray
 from .._constants import SOMA_JOINID
 from .._exception import DoesNotExistError, SOMAError
 from .._funcs import typeguard_ignore
 from .._tdb_handles import RawHandle
 from .._tiledb_array import TileDBArray
@@ -395,15 +396,15 @@
                             with _create_from_matrix(
                                 # TODO (https://github.com/single-cell-data/TileDB-SOMA/issues/1245):
                                 # consider a use-dense flag at the tiledbsoma.io API
                                 # DenseNDArray,
                                 SparseNDArray,
                                 _util.uri_joinpath(obsm.uri, key),
                                 conversions.to_tiledb_supported_array_type(
-                                    anndata.obsm[key]
+                                    key, anndata.obsm[key]
                                 ),
                                 ingestion_params=ingestion_params,
                                 platform_config=platform_config,
                                 context=context,
                             ) as arr:
                                 _maybe_set(
                                     obsm, key, arr, use_relative_uri=use_relative_uri
@@ -426,15 +427,15 @@
                             with _create_from_matrix(
                                 # TODO (https://github.com/single-cell-data/TileDB-SOMA/issues/1245):
                                 # consider a use-dense flag at the tiledbsoma.io API
                                 # DenseNDArray,
                                 SparseNDArray,
                                 _util.uri_joinpath(varm.uri, key),
                                 conversions.to_tiledb_supported_array_type(
-                                    anndata.varm[key]
+                                    key, anndata.varm[key]
                                 ),
                                 ingestion_params=ingestion_params,
                                 platform_config=platform_config,
                                 context=context,
                             ) as darr:
                                 _maybe_set(
                                     varm,
@@ -455,15 +456,15 @@
                             measurement, "obsp", obsp, use_relative_uri=use_relative_uri
                         )
                         for key in anndata.obsp.keys():
                             with _create_from_matrix(
                                 SparseNDArray,
                                 _util.uri_joinpath(obsp.uri, key),
                                 conversions.to_tiledb_supported_array_type(
-                                    anndata.obsp[key]
+                                    key, anndata.obsp[key]
                                 ),
                                 ingestion_params=ingestion_params,
                                 platform_config=platform_config,
                                 context=context,
                             ) as sarr:
                                 _maybe_set(
                                     obsp,
@@ -484,15 +485,15 @@
                             measurement, "varp", varp, use_relative_uri=use_relative_uri
                         )
                         for key in anndata.varp.keys():
                             with _create_from_matrix(
                                 SparseNDArray,
                                 _util.uri_joinpath(varp.uri, key),
                                 conversions.to_tiledb_supported_array_type(
-                                    anndata.varp[key]
+                                    key, anndata.varp[key]
                                 ),
                                 ingestion_params=ingestion_params,
                                 platform_config=platform_config,
                                 context=context,
                             ) as sarr:
                                 _maybe_set(
                                     varp,
@@ -637,42 +638,14 @@
         if ingestion_params.error_if_already_exists:
             raise SOMAError(f"{uri} already exists")
         return thing
 
     return cls.create(uri, context=context)
 
 
-def _df_to_arrow(df: pd.DataFrame) -> pa.Table:
-    """
-    Categoricals are not yet well supported, so we must flatten.
-    Also replace Numpy/Pandas-style nulls with Arrow-style nulls.
-    """
-    null_fields = set()
-    for k in df:
-        if df[k].dtype == "category":
-            df[k] = df[k].astype(df[k].cat.categories.dtype)
-        if df[k].isnull().any():
-            if df[k].isnull().all():
-                df[k] = pa.nulls(df.shape[0], pa.infer_type(df[k]))
-            else:
-                df[k].where(
-                    df[k].notnull(),
-                    pd.Series(pa.nulls(df[k].isnull().sum(), pa.infer_type(df[k]))),
-                    inplace=True,
-                )
-            null_fields.add(k)
-    arrow_table = pa.Table.from_pandas(df)
-    if null_fields:
-        md = arrow_table.schema.metadata
-        md.update(dict.fromkeys(null_fields, "nullable"))
-        arrow_table = arrow_table.replace_schema_metadata(md)
-
-    return arrow_table
-
-
 def _write_dataframe(
     df_uri: str,
     df: pd.DataFrame,
     id_column_name: Optional[str],
     *,
     ingestion_params: IngestionParams,
     platform_config: Optional[PlatformConfig] = None,
@@ -701,15 +674,15 @@
     ingestion_params: IngestionParams,
     platform_config: Optional[PlatformConfig] = None,
     context: Optional[SOMATileDBContext] = None,
 ) -> DataFrame:
     s = _util.get_start_stamp()
     logging.log_io(None, f"START  WRITING {df_uri}")
 
-    arrow_table = _df_to_arrow(df)
+    arrow_table = df_to_arrow(df)
 
     try:
         soma_df = _factory.open(df_uri, "w", soma_type=DataFrame, context=context)
     except DoesNotExistError:
         soma_df = DataFrame.create(
             df_uri,
             schema=arrow_table.schema,
@@ -895,31 +868,46 @@
     ``scanpy.pp.log1p``, etc.
 
     Use ``ingest_mode="resume"`` to not error out if the schema already exists.
 
     Lifecycle:
         Experimental.
     """
+
     ingestion_params = IngestionParams(ingest_mode)
+
+    # For local disk and S3, creation and storage URIs are identical.  For
+    # cloud, creation URIs look like tiledb://namespace/s3://bucket/path/to/obj
+    # whereas storage URIs (for the same object) look like
+    # tiledb://namespace/uuid.  When the caller passes a creation URI (which
+    # they must) via exp.uri, we need to follow that.
+    extend_creation_uri = exp.uri.startswith("tiledb://")
+
     with exp.ms[measurement_name] as meas:
+        if extend_creation_uri:
+            coll_uri = f"{exp.uri}/ms/{measurement_name}/{collection_name}"
+        else:
+            coll_uri = f"{meas.uri}/{collection_name}"
+
         if collection_name in meas:
             coll = cast(Collection[RawHandle], meas[collection_name])
         else:
             coll = _create_or_open_coll(
                 Collection,
-                f"{meas.uri}/{collection_name}",
+                coll_uri,
                 ingestion_params=ingestion_params,
                 context=context,
             )
             _maybe_set(meas, collection_name, coll, use_relative_uri=use_relative_uri)
         with coll:
-            uri = f"{coll.uri}/{matrix_name}"
+            matrix_uri = f"{coll_uri}/{matrix_name}"
+
             with _create_from_matrix(
                 SparseNDArray,
-                uri,
+                matrix_uri,
                 matrix_data,
                 ingestion_params=ingestion_params,
                 context=context,
             ) as sparse_nd_array:
                 _maybe_set(
                     coll,
                     matrix_name,
@@ -1494,15 +1482,15 @@
         msg = (
             f"Skipped {arr_uri} (uns ndarray):"
             f" unsupported dtype {value.dtype!r} ({value.dtype})"
         )
         logging.log_io(msg, msg)
         return
     try:
-        soma_arr = _factory.open(arr_uri, "w", soma_type=DenseNDArray)
+        soma_arr = _factory.open(arr_uri, "w", soma_type=DenseNDArray, context=context)
     except DoesNotExistError:
         soma_arr = DenseNDArray.create(
             arr_uri,
             type=pa_dtype,
             shape=value.shape,
             platform_config=platform_config,
             context=context,
@@ -1524,14 +1512,15 @@
         _maybe_set(coll, key, soma_arr, use_relative_uri=use_relative_uri)
         soma_arr.write(
             (),
             pa.Tensor.from_numpy(value),
             platform_config=platform_config,
         )
     msg = f"Wrote   {soma_arr.uri} (uns ndarray)"
+    logging.log_io(msg, msg)
 
 
 # ----------------------------------------------------------------
 def to_h5ad(
     experiment: Experiment,
     h5ad_path: Path,
     measurement_name: str,
```

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/logging.py` & `tiledbsoma-1.4.0/src/tiledbsoma/logging.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/options/_soma_tiledb_context.py` & `tiledbsoma-1.4.0/src/tiledbsoma/options/_soma_tiledb_context.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/options/_tiledb_create_options.py` & `tiledbsoma-1.4.0/src/tiledbsoma/options/_tiledb_create_options.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/pytiledbsoma.cc` & `tiledbsoma-1.4.0/src/tiledbsoma/pytiledbsoma.cc`

 * *Files 3% similar despite different names*

```diff
@@ -86,14 +86,23 @@
 }
 
 /**
  * @brief pybind11 bindings
  *
  */
 PYBIND11_MODULE(pytiledbsoma, m) {
+    py::enum_<OpenMode>(m, "OpenMode")
+        .value("read", OpenMode::read)
+        .value("write", OpenMode::write);
+
+    py::enum_<ResultOrder>(m, "ResultOrder")
+        .value("automatic", ResultOrder::automatic)
+        .value("rowmajor", ResultOrder::rowmajor)
+        .value("colmajor", ResultOrder::colmajor);
+
     tiledbpy::init_query_condition(m);
 
     m.doc() = "SOMA acceleration library";
 
     m.def("version", []() { return tiledbsoma::version::as_string(); });
 
     m.def(
@@ -133,15 +142,15 @@
             py::init(
                 [](std::string_view uri,
                    std::string_view name,
                    std::optional<std::vector<std::string>> column_names_in,
                    py::object py_query_condition,
                    py::object py_schema,
                    std::string_view batch_size,
-                   std::string_view result_order,
+                   ResultOrder result_order,
                    std::map<std::string, std::string> platform_config,
                    std::optional<std::pair<uint64_t, uint64_t>> timestamp) {
                     // Handle optional args
                     std::vector<std::string> column_names;
                     if (column_names_in) {
                         column_names = *column_names_in;
                     }
@@ -177,15 +186,15 @@
                     }
 
                     // Release python GIL after we're done accessing python
                     // objects
                     py::gil_scoped_release release;
 
                     auto reader = SOMAArray::open(
-                        TILEDB_READ,
+                        OpenMode::read,
                         uri,
                         name,
                         platform_config,
                         column_names,
                         batch_size,
                         result_order,
                         timestamp);
@@ -200,26 +209,26 @@
             "uri"_a,
             py::kw_only(),
             "name"_a = "unnamed",
             "column_names"_a = py::none(),
             "query_condition"_a = py::none(),
             "schema"_a = py::none(),
             "batch_size"_a = "auto",
-            "result_order"_a = "auto",
+            "result_order"_a = ResultOrder::automatic,
             "platform_config"_a = py::dict(),
             "timestamp"_a = py::none())
 
         .def(
             "reset",
             [](SOMAArray& reader,
                std::optional<std::vector<std::string>> column_names_in,
                py::object py_query_condition,
                py::object py_schema,
                std::string_view batch_size,
-               std::string_view result_order) {
+               ResultOrder result_order) {
                 // Handle optional args
                 std::vector<std::string> column_names;
                 if (column_names_in) {
                     column_names = *column_names_in;
                 }
 
                 // Handle query condition based on
@@ -264,15 +273,15 @@
                 }
             },
             py::kw_only(),
             "column_names"_a = py::none(),
             "query_condition"_a = py::none(),
             "schema"_a = py::none(),
             "batch_size"_a = "auto",
-            "result_order"_a = "auto")
+            "result_order"_a = ResultOrder::automatic)
 
         // After this are short functions expected to be invoked when the coords
         // are Python list/tuple, or NumPy arrays.  Arrow arrays are in this
         // long if-else-if function.
         .def(
             "set_dim_points_arrow",
             [](SOMAArray& reader,
```

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma/query_condition.cc` & `tiledbsoma-1.4.0/src/tiledbsoma/query_condition.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma.egg-info/PKG-INFO` & `tiledbsoma-1.4.0/src/tiledbsoma.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledbsoma
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python API for efficient storage and retrieval of single-cell data using TileDB
 Home-page: https://github.com/single-cell-data/TileDB-SOMA/tree/main/apis/python
 Author: TileDB, Inc.
 Author-email: help@tiledb.io
 Maintainer: TileDB, Inc.
 Maintainer-email: help@tiledb.io
 License: MIT
```

### Comparing `tiledbsoma-1.3.0/src/tiledbsoma.egg-info/SOURCES.txt` & `tiledbsoma-1.4.0/src/tiledbsoma.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -28,24 +28,35 @@
 dist_links/libtiledbsoma/src/external/include/thread_pool/status.h
 dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h
 dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc
 dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc
 dist_links/libtiledbsoma/src/soma/array_buffers.h
 dist_links/libtiledbsoma/src/soma/column_buffer.cc
 dist_links/libtiledbsoma/src/soma/column_buffer.h
+dist_links/libtiledbsoma/src/soma/enums.h
 dist_links/libtiledbsoma/src/soma/logger_public.h
 dist_links/libtiledbsoma/src/soma/managed_query.cc
 dist_links/libtiledbsoma/src/soma/managed_query.h
 dist_links/libtiledbsoma/src/soma/soma_array.cc
 dist_links/libtiledbsoma/src/soma/soma_array.h
+dist_links/libtiledbsoma/src/soma/soma_collection.cc
+dist_links/libtiledbsoma/src/soma/soma_collection.h
 dist_links/libtiledbsoma/src/soma/soma_dataframe.cc
 dist_links/libtiledbsoma/src/soma/soma_dataframe.h
+dist_links/libtiledbsoma/src/soma/soma_dense_ndarray.cc
+dist_links/libtiledbsoma/src/soma/soma_dense_ndarray.h
+dist_links/libtiledbsoma/src/soma/soma_experiment.cc
+dist_links/libtiledbsoma/src/soma/soma_experiment.h
 dist_links/libtiledbsoma/src/soma/soma_group.cc
 dist_links/libtiledbsoma/src/soma/soma_group.h
+dist_links/libtiledbsoma/src/soma/soma_measurement.cc
+dist_links/libtiledbsoma/src/soma/soma_measurement.h
 dist_links/libtiledbsoma/src/soma/soma_object.h
+dist_links/libtiledbsoma/src/soma/soma_sparse_ndarray.cc
+dist_links/libtiledbsoma/src/soma/soma_sparse_ndarray.h
 dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma
 dist_links/libtiledbsoma/src/utils/arrow_adapter.h
 dist_links/libtiledbsoma/src/utils/carrow.h
 dist_links/libtiledbsoma/src/utils/common.h
 dist_links/libtiledbsoma/src/utils/logger.cc
 dist_links/libtiledbsoma/src/utils/logger.h
 dist_links/libtiledbsoma/src/utils/stats.cc
@@ -57,16 +68,19 @@
 dist_links/libtiledbsoma/test/CMakeLists.txt
 dist_links/libtiledbsoma/test/test_query_condition.py
 dist_links/libtiledbsoma/test/test_simple.py
 dist_links/libtiledbsoma/test/test_soma_array.py
 dist_links/libtiledbsoma/test/unit_column_buffer.cc
 dist_links/libtiledbsoma/test/unit_managed_query.cc
 dist_links/libtiledbsoma/test/unit_soma_array.cc
+dist_links/libtiledbsoma/test/unit_soma_collection.cc
 dist_links/libtiledbsoma/test/unit_soma_dataframe.cc
+dist_links/libtiledbsoma/test/unit_soma_dense_ndarray.cc
 dist_links/libtiledbsoma/test/unit_soma_group.cc
+dist_links/libtiledbsoma/test/unit_soma_sparse_ndarray.cc
 dist_links/libtiledbsoma/test/unit_thread_pool.cc
 dist_links/scripts/README.md
 dist_links/scripts/bld
 dist_links/scripts/run-clang-format.sh
 dist_links/scripts/show-versions.py
 dist_links/scripts/update-tiledb-version.py
 src/tiledbsoma/__init__.py
```

### Comparing `tiledbsoma-1.3.0/version.py` & `tiledbsoma-1.4.0/version.py`

 * *Files identical despite different names*

