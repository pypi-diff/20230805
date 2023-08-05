# Comparing `tmp/snowflake-connector-python-nightly-2023.8.1.tar.gz` & `tmp/snowflake-connector-python-nightly-2023.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflake-connector-python-nightly-2023.8.1.tar", last modified: Tue Aug  1 04:06:35 2023, max compression
+gzip compressed data, was "snowflake-connector-python-nightly-2023.8.5.tar", last modified: Sat Aug  5 04:07:24 2023, max compression
```

## Comparing `snowflake-connector-python-nightly-2023.8.1.tar` & `snowflake-connector-python-nightly-2023.8.5.tar`

### file list

```diff
@@ -1,203 +1,203 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.305805 snowflake-connector-python-nightly-2023.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-08-01 04:06:24.000000 snowflake-connector-python-nightly-2023.8.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    50115 2023-08-01 04:06:24.000000 snowflake-connector-python-nightly-2023.8.1/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-08-01 04:06:24.000000 snowflake-connector-python-nightly-2023.8.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-01 04:06:24.000000 snowflake-connector-python-nightly-2023.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-01 04:06:24.000000 snowflake-connector-python-nightly-2023.8.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-08-01 04:06:35.305805 snowflake-connector-python-nightly-2023.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-08-01 04:06:24.000000 snowflake-connector-python-nightly-2023.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-01 04:06:24.000000 snowflake-connector-python-nightly-2023.8.1/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-01 04:06:24.000000 snowflake-connector-python-nightly-2023.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-08-01 04:06:35.305805 snowflake-connector-python-nightly-2023.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-08-01 04:06:24.000000 snowflake-connector-python-nightly-2023.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.285803 snowflake-connector-python-nightly-2023.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.281803 snowflake-connector-python-nightly-2023.8.1/src/snowflake/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.293804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-08-01 04:06:25.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-08-01 04:06:25.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/_query_context_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-08-01 04:06:25.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/_sql_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-08-01 04:06:25.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/arrow_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-08-01 04:06:25.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/arrow_iterator.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.293804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27245 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/by_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/idtoken.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/okta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/usrpwdmfa.py
--rw-r--r--   0 runner    (1001) docker     (123)    14011 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/webbrowser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-08-01 04:06:25.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/azure_storage_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-08-01 04:06:25.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/bind_upload_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    23454 2023-08-01 04:06:25.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-08-01 04:06:25.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    67498 2023-08-01 04:06:25.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    30347 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/connection_diagnostic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    26078 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/converter_issue23517.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/converter_null.py
--rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/converter_snowsql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.285803 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.297804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    34612 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/DateConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/IColumnConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/IntConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/IntConverter.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.297804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Python/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Python/Common.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/StringConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.297804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Util/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Util/macros.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.297804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/Logging/
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/Logging/logging.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/Logging/logging.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    57036 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/dbapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/description.py
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/encryption_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/errorcode.py
--rw-r--r--   0 runner    (1001) docker     (123)    20184 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/file_compression_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    47198 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/file_transfer_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    16072 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/gcs_storage_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/gzip_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/local_storage_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42002 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    18429 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/ocsp_asn1crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)    68581 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/ocsp_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    20379 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/pandas_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25927 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/result_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/result_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    21830 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/s3_storage_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/secret_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/sf_dirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-01 04:06:27.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/sfbinaryformat.py
--rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/sfdatetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/snow_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/sqlstate.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/ssd_internal_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/ssl_wrap_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)    17583 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/storage_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    18837 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/telemetry_oob.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/time_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.297804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/tool/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/tool/dump_certs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/tool/dump_ocsp_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/tool/dump_ocsp_response_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/tool/probe_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/url_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/util_text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.297804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.301804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/_internal_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19602 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/certs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/help.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    35231 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30180 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/status_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)    33450 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.301804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    20300 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    39128 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/connectionpool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.301804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.301804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/appengine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    34416 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/socks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/filepost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.301804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.305805 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/packages/backports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/packages/backports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py
--rw-r--r--   0 runner    (1001) docker     (123)    34665 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/packages/six.py
--rw-r--r--   0 runner    (1001) docker     (123)    19786 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/poolmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/request.py
--rw-r--r--   0 runner    (1001) docker     (123)    30761 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.305805 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    22003 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/ssl_.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/ssltransport.py
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/wait.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.305805 snowflake-connector-python-nightly-2023.8.1/src/snowflake_connector_python_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-08-01 04:06:35.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake_connector_python_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-08-01 04:06:35.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake_connector_python_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 04:06:35.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake_connector_python_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-01 04:06:35.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake_connector_python_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 04:06:35.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake_connector_python_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-08-01 04:06:35.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake_connector_python_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 04:06:35.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake_connector_python_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:07:23.997558 snowflake-connector-python-nightly-2023.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-08-05 04:06:58.000000 snowflake-connector-python-nightly-2023.8.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    50291 2023-08-05 04:06:58.000000 snowflake-connector-python-nightly-2023.8.5/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-08-05 04:06:58.000000 snowflake-connector-python-nightly-2023.8.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-05 04:06:58.000000 snowflake-connector-python-nightly-2023.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-05 04:06:58.000000 snowflake-connector-python-nightly-2023.8.5/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-08-05 04:07:23.997558 snowflake-connector-python-nightly-2023.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-08-05 04:06:58.000000 snowflake-connector-python-nightly-2023.8.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-05 04:06:58.000000 snowflake-connector-python-nightly-2023.8.5/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-05 04:06:58.000000 snowflake-connector-python-nightly-2023.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-08-05 04:07:24.001558 snowflake-connector-python-nightly-2023.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-08-05 04:06:58.000000 snowflake-connector-python-nightly-2023.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:07:23.981558 snowflake-connector-python-nightly-2023.8.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:07:23.977558 snowflake-connector-python-nightly-2023.8.5/src/snowflake/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:07:23.985558 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-08-05 04:07:02.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-08-05 04:07:02.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/_query_context_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-08-05 04:07:02.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/_sql_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-08-05 04:07:02.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/arrow_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-08-05 04:07:02.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/arrow_iterator.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:07:23.989558 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-05 04:07:05.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27245 2023-08-05 04:07:05.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/auth/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-08-05 04:07:05.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/auth/by_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-05 04:07:05.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/auth/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-08-05 04:07:05.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/auth/idtoken.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-08-05 04:07:05.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/auth/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-08-05 04:07:05.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/auth/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-08-05 04:07:05.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/auth/okta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-05 04:07:05.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/auth/usrpwdmfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14011 2023-08-05 04:07:05.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/auth/webbrowser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-08-05 04:07:02.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/azure_storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-08-05 04:07:02.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/bind_upload_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23454 2023-08-05 04:07:02.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-08-05 04:07:02.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-08-05 04:07:03.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67586 2023-08-05 04:07:03.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30347 2023-08-05 04:07:03.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/connection_diagnostic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-08-05 04:07:03.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26078 2023-08-05 04:07:03.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-08-05 04:07:03.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/converter_issue23517.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-05 04:07:03.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/converter_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-08-05 04:07:03.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/converter_snowsql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:07:23.977558 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:07:23.989558 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-05 04:07:05.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-05 04:07:06.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-05 04:07:06.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-05 04:07:06.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-08-05 04:07:06.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-08-05 04:07:06.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-05 04:07:06.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-08-05 04:07:06.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    34612 2023-08-05 04:07:06.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-08-05 04:07:06.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-08-05 04:07:06.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-08-05 04:07:06.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/DateConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-05 04:07:06.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-08-05 04:07:06.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-05 04:07:06.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-05 04:07:06.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-05 04:07:07.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/IColumnConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-08-05 04:07:07.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/IntConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-05 04:07:07.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/IntConverter.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:07:23.989558 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/Python/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-05 04:07:07.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/Python/Common.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-08-05 04:07:07.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-08-05 04:07:07.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-05 04:07:07.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-05 04:07:07.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-05 04:07:07.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-05 04:07:07.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/StringConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-05 04:07:07.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-05 04:07:07.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-08-05 04:07:07.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-08-05 04:07:07.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-08-05 04:07:07.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:07:23.989558 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/Util/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-05 04:07:07.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/Util/macros.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-08-05 04:07:08.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-08-05 04:07:08.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:07:23.989558 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/Logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-08-05 04:07:08.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/Logging/logging.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-08-05 04:07:08.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/Logging/logging.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    57036 2023-08-05 04:07:03.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-05 04:07:03.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/dbapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-05 04:07:03.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-08-05 04:07:03.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/encryption_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-08-05 04:07:03.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/errorcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20184 2023-08-05 04:07:03.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-08-05 04:07:03.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-08-05 04:07:03.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/file_compression_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47198 2023-08-05 04:07:03.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/file_transfer_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-08-05 04:07:03.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16072 2023-08-05 04:07:03.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/gcs_storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-08-05 04:07:04.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/gzip_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-08-05 04:07:04.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/local_storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42002 2023-08-05 04:07:04.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18429 2023-08-05 04:07:04.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/ocsp_asn1crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68581 2023-08-05 04:07:04.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/ocsp_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-08-05 04:07:04.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20379 2023-08-05 04:07:04.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/pandas_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-05 04:07:04.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 04:07:04.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25927 2023-08-05 04:07:04.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/result_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-08-05 04:07:04.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/result_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21830 2023-08-05 04:07:04.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/s3_storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-08-05 04:07:04.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/secret_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-08-05 04:07:04.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/sf_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-05 04:07:04.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/sfbinaryformat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-08-05 04:07:04.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/sfdatetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-08-05 04:07:04.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/snow_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-05 04:07:04.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/sqlstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-05 04:07:04.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/ssd_internal_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-08-05 04:07:05.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/ssl_wrap_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17583 2023-08-05 04:07:05.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-08-05 04:07:05.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18837 2023-08-05 04:07:05.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/telemetry_oob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-05 04:07:05.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-08-05 04:07:05.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/time_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:07:23.993559 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-05 04:07:08.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-08-05 04:07:08.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/tool/dump_certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-08-05 04:07:08.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/tool/dump_ocsp_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-08-05 04:07:08.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/tool/dump_ocsp_response_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-08-05 04:07:08.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/tool/probe_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-05 04:07:05.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/url_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-08-05 04:07:05.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/util_text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:07:23.993559 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-05 04:07:08.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:07:23.993559 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-08-05 04:07:09.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-08-05 04:07:09.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-05 04:07:09.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-05 04:07:09.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/_internal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19602 2023-08-05 04:07:09.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-08-05 04:07:09.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-08-05 04:07:09.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-05 04:07:09.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-08-05 04:07:09.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-08-05 04:07:09.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-08-05 04:07:09.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-08-05 04:07:09.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-05 04:07:09.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35231 2023-08-05 04:07:09.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30180 2023-08-05 04:07:09.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-08-05 04:07:09.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/status_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-08-05 04:07:09.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33450 2023-08-05 04:07:09.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:07:23.993559 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-08-05 04:07:10.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-08-05 04:07:09.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-08-05 04:07:09.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-05 04:07:10.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20300 2023-08-05 04:07:10.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39128 2023-08-05 04:07:10.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/connectionpool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:07:23.997558 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 04:07:10.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-05 04:07:10.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:07:23.997558 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 04:07:10.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-08-05 04:07:11.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-08-05 04:07:11.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-08-05 04:07:10.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/contrib/appengine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-08-05 04:07:10.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-08-05 04:07:10.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34416 2023-08-05 04:07:10.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-08-05 04:07:10.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/contrib/socks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-08-05 04:07:10.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-08-05 04:07:10.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-08-05 04:07:10.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/filepost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:07:23.997558 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 04:07:11.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:07:23.997558 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/packages/backports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 04:07:11.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-05 04:07:11.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34665 2023-08-05 04:07:11.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/packages/six.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19786 2023-08-05 04:07:10.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/poolmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-08-05 04:07:10.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30761 2023-08-05 04:07:10.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:07:23.997558 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-05 04:07:11.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-08-05 04:07:11.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-05 04:07:11.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-05 04:07:11.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-08-05 04:07:11.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-08-05 04:07:11.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22003 2023-08-05 04:07:12.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-08-05 04:07:12.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/ssl_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-08-05 04:07:12.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-08-05 04:07:12.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/ssltransport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-08-05 04:07:12.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-08-05 04:07:12.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-08-05 04:07:12.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/wait.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-05 04:07:05.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:07:23.997558 snowflake-connector-python-nightly-2023.8.5/src/snowflake_connector_python_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-08-05 04:07:23.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake_connector_python_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-08-05 04:07:23.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake_connector_python_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 04:07:23.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake_connector_python_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-05 04:07:23.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake_connector_python_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 04:07:23.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake_connector_python_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-08-05 04:07:23.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake_connector_python_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-05 04:07:23.000000 snowflake-connector-python-nightly-2023.8.5/src/snowflake_connector_python_nightly.egg-info/top_level.txt
```

### Comparing `snowflake-connector-python-nightly-2023.8.1/CONTRIBUTING.md` & `snowflake-connector-python-nightly-2023.8.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/DESCRIPTION.md` & `snowflake-connector-python-nightly-2023.8.5/DESCRIPTION.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 Snowflake Documentation is available at:
 https://docs.snowflake.com/
 
 Source code is also available at: https://github.com/snowflakedb/snowflake-connector-python
 
 # Release Notes
 
+- v3.1.1(TBD)
+
+  - Fixed a bug in retry logic for okta authentication to refresh token.
+  - Support `RSAPublicKey` when constructing `AuthByKeyPair` in addition to raw bytes.
+
 - v3.1.0(July 31,2023)
 
   - Added a feature that lets you add connection definitions to the `connections.toml` configuration file. A connection definition refers to a collection of connection parameters, for example, if you wanted to define a connection named `prod``:
 
     ```toml
     [prod]
     account = "my_account"
```

### Comparing `snowflake-connector-python-nightly-2023.8.1/LICENSE.txt` & `snowflake-connector-python-nightly-2023.8.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/MANIFEST.in` & `snowflake-connector-python-nightly-2023.8.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/PKG-INFO` & `snowflake-connector-python-nightly-2023.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-connector-python-nightly
-Version: 2023.8.1
+Version: 2023.8.5
 Summary: Nigthly build of Snowflake Connector for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/user-guide/python-connector.html
 Project-URL: Source, https://github.com/keller00/snowflake-connector-python-nightlies/
```

### Comparing `snowflake-connector-python-nightly-2023.8.1/README.md` & `snowflake-connector-python-nightly-2023.8.5/README.md`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/pyproject.toml` & `snowflake-connector-python-nightly-2023.8.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/setup.cfg` & `snowflake-connector-python-nightly-2023.8.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/setup.py` & `snowflake-connector-python-nightly-2023.8.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,11 +204,11 @@
                 ret.append(source)
 
             return ret
 
     cmd_class = {"build_ext": MyBuildExt}
 
 setup(
-    version="2023.08.01",
+    version="2023.08.05",
     ext_modules=extensions,
     cmdclass=cmd_class,
 )
```

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/__init__.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/_query_context_cache.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/_query_context_cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/_sql_util.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/_sql_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/arrow_context.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/arrow_context.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/arrow_iterator.pyx` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/arrow_iterator.pyx`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/__init__.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/_auth.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/auth/_auth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/by_plugin.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/auth/by_plugin.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/default.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/auth/default.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/idtoken.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/auth/idtoken.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/keypair.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/auth/keypair.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,25 +43,26 @@
     ISSUE_TIME = "iat"
     LIFETIME = 60
     DEFAULT_JWT_RETRY_ATTEMPTS = 10
     DEFAULT_JWT_CNXN_WAIT_TIME = 10
 
     def __init__(
         self,
-        private_key: bytes,
+        private_key: bytes | RSAPrivateKey,
         lifetime_in_seconds: int = LIFETIME,
     ) -> None:
         """Inits AuthByKeyPair class with private key.
 
         Args:
-            private_key: a byte array of der formats of private key
+            private_key: a byte array of der formats of private key, or an
+                object that implements the `RSAPrivateKey` interface.
             lifetime_in_seconds: number of seconds the JWT token will be valid
         """
         super().__init__()
-        self._private_key: bytes | None = private_key
+        self._private_key: bytes | RSAPrivateKey | None = private_key
         self._jwt_token = ""
         self._jwt_token_exp = 0
         self._lifetime = timedelta(
             seconds=int(os.getenv("JWT_LIFETIME_IN_SECONDS", lifetime_in_seconds))
         )
         self._jwt_retry_attempts = int(
             os.getenv(
@@ -98,33 +99,40 @@
         else:
             account = account.partition(".")[0]
         account = account.upper()
         user = user.upper()
 
         now = datetime.utcnow()
 
-        try:
-            private_key = load_der_private_key(
-                data=self._private_key,
-                password=None,
-                backend=default_backend(),
-            )
-        except Exception as e:
-            raise ProgrammingError(
-                msg=f"Failed to load private key: {e}\nPlease provide a valid "
-                "unencrypted rsa private key in DER format as bytes object",
-                errno=ER_INVALID_PRIVATE_KEY,
-            )
+        if isinstance(self._private_key, bytes):
+            try:
+                private_key = load_der_private_key(
+                    data=self._private_key,
+                    password=None,
+                    backend=default_backend(),
+                )
+            except Exception as e:
+                raise ProgrammingError(
+                    msg=f"Failed to load private key: {e}\nPlease provide a valid "
+                    "unencrypted rsa private key in DER format as bytes object",
+                    errno=ER_INVALID_PRIVATE_KEY,
+                )
 
-        if not isinstance(private_key, RSAPrivateKey):
-            raise ProgrammingError(
-                msg=f"Private key type ({private_key.__class__.__name__}) not supported."
-                "\nPlease provide a valid rsa private key in DER format as bytes "
-                "object",
-                errno=ER_INVALID_PRIVATE_KEY,
+            if not isinstance(private_key, RSAPrivateKey):
+                raise ProgrammingError(
+                    msg=f"Private key type ({private_key.__class__.__name__}) not supported."
+                    "\nPlease provide a valid rsa private key in DER format as bytes "
+                    "object",
+                    errno=ER_INVALID_PRIVATE_KEY,
+                )
+        elif isinstance(self._private_key, RSAPrivateKey):
+            private_key = self._private_key
+        else:
+            raise TypeError(
+                f"Expected bytes or RSAPrivateKey, got {type(self._private_key)}"
             )
 
         public_key_fp = self.calculate_public_key_fingerprint(private_key)
 
         self._jwt_token_exp = now + self._lifetime
         payload = {
             self.ISSUER: f"{account}.{user}.{public_key_fp}",
```

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/oauth.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/okta.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/auth/okta.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,21 +273,22 @@
         conn: SnowflakeConnection,
         generate_one_time_token: Callable,
         sso_url: str,
     ) -> dict[Any, Any]:
         logger.debug("step 4: query IDP URL snowflake app to get SAML " "response")
         timeout_time = time.time() + conn.login_timeout if conn.login_timeout else None
         response_html = {}
+        origin_sso_url = sso_url
         while timeout_time is None or time.time() < timeout_time:
             try:
                 url_parameters = {
                     "RelayState": "/some/deep/link",
                     "onetimetoken": generate_one_time_token(),
                 }
-                sso_url = sso_url + "?" + urlencode(url_parameters)
+                sso_url = origin_sso_url + "?" + urlencode(url_parameters)
                 headers = {
                     HTTP_HEADER_ACCEPT: "*/*",
                 }
                 remaining_timeout = timeout_time - time.time() if timeout_time else None
                 response_html = conn._rest.fetch(
                     "get",
                     sso_url,
```

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/usrpwdmfa.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/auth/usrpwdmfa.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/webbrowser.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/auth/webbrowser.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/azure_storage_client.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/azure_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/bind_upload_agent.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/bind_upload_agent.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cache.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/compat.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/compat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/config_manager.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/config_manager.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/connection.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 from logging import getLogger
 from threading import Lock
 from time import strptime
 from types import TracebackType
 from typing import Any, Callable, Generator, Iterable, NamedTuple, Sequence
 from uuid import UUID
 
+from cryptography.hazmat.primitives.asymmetric.rsa import RSAPrivateKey
+
 from . import errors, proxy
 from ._query_context_cache import QueryContextCache
 from .auth import (
     FIRST_PARTY_AUTHENTICATORS,
     Auth,
     AuthByDefault,
     AuthByKeyPair,
@@ -142,15 +144,15 @@
     "login_timeout": (120, int),  # login timeout
     "network_timeout": (
         None,
         (type(None), int),
     ),  # network timeout (infinite by default)
     "passcode_in_password": (False, bool),  # Snowflake MFA
     "passcode": (None, (type(None), str)),  # Snowflake MFA
-    "private_key": (None, (type(None), str)),
+    "private_key": (None, (type(None), str, RSAPrivateKey)),
     "token": (None, (type(None), str)),  # OAuth or JWT Token
     "authenticator": (DEFAULT_AUTHENTICATOR, (type(None), str)),
     "mfa_callback": (None, (type(None), Callable)),
     "password_callback": (None, (type(None), Callable)),
     "auth_class": (None, (type(None), AuthByPlugin)),
     "application": (CLIENT_NAME, (type(None), str)),
     "internal_application_name": (CLIENT_NAME, (type(None), str)),
```

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/connection_diagnostic.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/connection_diagnostic.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/constants.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/constants.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/converter.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/converter.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/converter_issue23517.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/converter_issue23517.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/converter_snowsql.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/converter_snowsql.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.cpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.cpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.hpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.cpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.hpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.cpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.hpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/DateConverter.hpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/DateConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.cpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.hpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/IntConverter.hpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/IntConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/StringConverter.cpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/StringConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.hpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.cpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.hpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/Logging/logging.cpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/Logging/logging.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/Logging/logging.hpp` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cpp/Logging/logging.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cursor.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/cursor.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/dbapi.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/dbapi.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/description.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/description.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/encryption_util.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/encryption_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/errorcode.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/errorcode.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/errors.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/errors.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/file_compression_type.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/file_compression_type.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/file_transfer_agent.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/file_transfer_agent.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/file_util.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/file_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/gcs_storage_client.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/gcs_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/gzip_decoder.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/gzip_decoder.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/local_storage_client.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/local_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/network.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/network.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/ocsp_asn1crypto.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/ocsp_asn1crypto.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/ocsp_snowflake.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/ocsp_snowflake.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/options.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/options.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/pandas_tools.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/pandas_tools.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/proxy.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/proxy.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/result_batch.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/result_batch.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/result_set.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/result_set.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/s3_storage_client.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/s3_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/secret_detector.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/secret_detector.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/sf_dirs.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/sf_dirs.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/sfbinaryformat.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/sfbinaryformat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/sfdatetime.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/sfdatetime.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/snow_logging.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/snow_logging.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/ssd_internal_keys.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/ssd_internal_keys.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/ssl_wrap_socket.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/ssl_wrap_socket.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/storage_client.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/telemetry.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/telemetry.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/telemetry_oob.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/telemetry_oob.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/test_util.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/test_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/time_util.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/time_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/tool/dump_certs.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/tool/dump_certs.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/tool/dump_ocsp_response.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/tool/dump_ocsp_response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/tool/dump_ocsp_response_cache.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/tool/dump_ocsp_response_cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/tool/probe_connection.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/tool/probe_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/url_util.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/url_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/util_text.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/util_text.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/LICENSE` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/__init__.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/_internal_utils.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/adapters.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/api.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/api.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/auth.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/auth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/compat.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/compat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/cookies.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/exceptions.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/help.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/help.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/hooks.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/models.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/models.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/sessions.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/status_codes.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/structures.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/structures.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/utils.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/requests/utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/LICENSE.txt` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/__init__.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/_collections.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/connection.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/connectionpool.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/appengine.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/socks.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/exceptions.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/fields.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/filepost.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/packages/six.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/poolmanager.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/request.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/response.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/__init__.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/connection.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/proxy.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/request.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/response.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/retry.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/ssl_.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/ssltransport.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/timeout.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/url.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/wait.py` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake/connector/vendored/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake_connector_python_nightly.egg-info/PKG-INFO` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake_connector_python_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-connector-python-nightly
-Version: 2023.8.1
+Version: 2023.8.5
 Summary: Nigthly build of Snowflake Connector for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/user-guide/python-connector.html
 Project-URL: Source, https://github.com/keller00/snowflake-connector-python-nightlies/
```

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake_connector_python_nightly.egg-info/SOURCES.txt` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake_connector_python_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.8.1/src/snowflake_connector_python_nightly.egg-info/requires.txt` & `snowflake-connector-python-nightly-2023.8.5/src/snowflake_connector_python_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

