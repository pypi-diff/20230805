# Comparing `tmp/SomeTools-0.1.41.tar.gz` & `tmp/SomeTools-0.1.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SomeTools-0.1.41.tar", last modified: Sun Jun 11 05:45:43 2023, max compression
+gzip compressed data, was "SomeTools-0.1.43.tar", last modified: Sun Jun 11 09:21:11 2023, max compression
```

## Comparing `SomeTools-0.1.41.tar` & `SomeTools-0.1.43.tar`

### file list

```diff
@@ -1,83 +1,89 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.468463 SomeTools-0.1.41/
--rw-rw-rw-   0        0        0     1091 2023-06-10 10:45:04.000000 SomeTools-0.1.41/LICENSE
--rw-rw-rw-   0        0        0     2244 2023-06-11 05:45:43.452837 SomeTools-0.1.41/PKG-INFO
--rw-rw-rw-   0        0        0     1527 2023-06-10 15:49:43.000000 SomeTools-0.1.41/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.439331 SomeTools-0.1.41/SomeTools.egg-info/
--rw-rw-rw-   0        0        0     2244 2023-06-11 05:45:43.000000 SomeTools-0.1.41/SomeTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2491 2023-06-11 05:45:43.000000 SomeTools-0.1.41/SomeTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 05:45:43.000000 SomeTools-0.1.41/SomeTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      770 2023-06-11 05:45:43.000000 SomeTools-0.1.41/SomeTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-11 05:45:43.000000 SomeTools-0.1.41/SomeTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 05:45:43.468463 SomeTools-0.1.41/setup.cfg
--rw-rw-rw-   0        0        0     3378 2023-06-11 05:40:12.000000 SomeTools-0.1.41/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.439331 SomeTools-0.1.41/sometools/
--rw-rw-rw-   0        0        0     1545 2023-06-10 15:43:30.000000 SomeTools-0.1.41/sometools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.439331 SomeTools-0.1.41/sometools/async_tools/
--rw-rw-rw-   0        0        0      550 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/async_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.439331 SomeTools-0.1.41/sometools/async_tools/base/
--rw-rw-rw-   0        0        0       42 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/async_tools/base/__init__.py
--rw-rw-rw-   0        0        0      181 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/async_tools/base/base.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.439331 SomeTools-0.1.41/sometools/async_tools/bloom_filter/
--rw-rw-rw-   0        0        0       90 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/async_tools/bloom_filter/__init__.py
--rw-rw-rw-   0        0        0     3632 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/async_tools/bloom_filter/async_bloomfilter_tool.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.439331 SomeTools-0.1.41/sometools/async_tools/database_tools/
--rw-rw-rw-   0        0        0        0 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/async_tools/database_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.439331 SomeTools-0.1.41/sometools/async_tools/database_tools/mysql_tools/
--rw-rw-rw-   0        0        0        0 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/async_tools/database_tools/mysql_tools/__init__.py
--rw-rw-rw-   0        0        0    14159 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/async_tools/database_tools/mysql_tools/async_mysql_orm.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.439331 SomeTools-0.1.41/sometools/async_tools/redis_tools/
--rw-rw-rw-   0        0        0       78 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/async_tools/redis_tools/__init__.py
--rw-rw-rw-   0        0        0     1227 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/async_tools/redis_tools/async_io_redis.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.439331 SomeTools-0.1.41/sometools/sync_tools/
--rw-rw-rw-   0        0        0        0 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.439331 SomeTools-0.1.41/sometools/sync_tools/base/
--rw-rw-rw-   0        0        0       42 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/base/__init__.py
--rw-rw-rw-   0        0        0      196 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/base/base.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.439331 SomeTools-0.1.41/sometools/sync_tools/calendar_tools/
--rw-rw-rw-   0        0        0       69 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/calendar_tools/__init__.py
--rw-rw-rw-   0        0        0     2785 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/calendar_tools/calendar_tool.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/char_tools/
--rw-rw-rw-   0        0        0       58 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/char_tools/__init__.py
--rw-rw-rw-   0        0        0      895 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/char_tools/char_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/chinese_to_pinyin_acronym/
--rw-rw-rw-   0        0        0      121 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/chinese_to_pinyin_acronym/__init__.py
--rw-rw-rw-   0        0        0     3448 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/chinese_to_pinyin_acronym/chinese_to_pinyin.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/database_tools/
--rw-rw-rw-   0        0        0        0 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/database_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/database_tools/mysql_tools/
--rw-rw-rw-   0        0        0        0 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/database_tools/mysql_tools/__init__.py
--rw-rw-rw-   0        0        0     2769 2023-06-11 03:50:46.000000 SomeTools-0.1.41/sometools/sync_tools/database_tools/mysql_tools/conn_pool.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/datetime_tools/
--rw-rw-rw-   0        0        0       71 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/datetime_tools/__init__.py
--rw-rw-rw-   0        0        0    12057 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/datetime_tools/date_conversion.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/encryption_and_decryption_tools/
--rw-rw-rw-   0        0        0      276 2023-06-11 04:17:42.000000 SomeTools-0.1.41/sometools/sync_tools/encryption_and_decryption_tools/__init__.py
--rw-rw-rw-   0        0        0     2839 2023-06-11 04:39:20.000000 SomeTools-0.1.41/sometools/sync_tools/encryption_and_decryption_tools/aes_tool.py
--rw-rw-rw-   0        0        0     2093 2023-06-11 05:09:37.000000 SomeTools-0.1.41/sometools/sync_tools/encryption_and_decryption_tools/rsa_tool.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/image_tools/
--rw-rw-rw-   0        0        0       61 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/image_tools/__init__.py
--rw-rw-rw-   0        0        0     2575 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/image_tools/image_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/ip_tools/
--rw-rw-rw-   0        0        0       51 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/ip_tools/__init__.py
--rw-rw-rw-   0        0        0      538 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/ip_tools/ip_tool.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/log_tools/
--rw-rw-rw-   0        0        0       57 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/log_tools/__init__.py
--rw-rw-rw-   0        0        0     3758 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/log_tools/logger_main.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/os_tools/
--rw-rw-rw-   0        0        0       52 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/os_tools/__init__.py
--rw-rw-rw-   0        0        0     3566 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/os_tools/os_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/re_tools/
--rw-rw-rw-   0        0        0       80 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/re_tools/__init__.py
--rw-rw-rw-   0        0        0     2551 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/re_tools/extract_string.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/redis_tools/
--rw-rw-rw-   0        0        0       60 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/redis_tools/__init__.py
--rw-rw-rw-   0        0        0      916 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/redis_tools/redis_main.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/string_tools/
--rw-rw-rw-   0        0        0       67 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/string_tools/__init__.py
--rw-rw-rw-   0        0        0     1761 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/string_tools/string_cleaning.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/traditional_simplified_chinese_conversion/
--rw-rw-rw-   0        0        0      148 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/traditional_simplified_chinese_conversion/__init__.py
--rw-rw-rw-   0        0        0     1955 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/traditional_simplified_chinese_conversion/traditional_simplified_chinese.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/url_tools/
--rw-rw-rw-   0        0        0       87 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/url_tools/__init__.py
--rw-rw-rw-   0        0        0     1875 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/url_tools/url_encode_decode.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.599892 SomeTools-0.1.43/
+-rw-rw-rw-   0        0        0     1091 2023-06-10 10:45:04.000000 SomeTools-0.1.43/LICENSE
+-rw-rw-rw-   0        0        0     2270 2023-06-11 09:21:11.587875 SomeTools-0.1.43/PKG-INFO
+-rw-rw-rw-   0        0        0     1553 2023-06-11 08:33:29.000000 SomeTools-0.1.43/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.571974 SomeTools-0.1.43/SomeTools.egg-info/
+-rw-rw-rw-   0        0        0     2270 2023-06-11 09:21:11.000000 SomeTools-0.1.43/SomeTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2674 2023-06-11 09:21:11.000000 SomeTools-0.1.43/SomeTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 09:21:11.000000 SomeTools-0.1.43/SomeTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      770 2023-06-11 09:21:11.000000 SomeTools-0.1.43/SomeTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-11 09:21:11.000000 SomeTools-0.1.43/SomeTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 09:21:11.599892 SomeTools-0.1.43/setup.cfg
+-rw-rw-rw-   0        0        0     3378 2023-06-11 09:21:08.000000 SomeTools-0.1.43/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.571974 SomeTools-0.1.43/sometools/
+-rw-rw-rw-   0        0        0     1680 2023-06-11 08:24:03.000000 SomeTools-0.1.43/sometools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.571974 SomeTools-0.1.43/sometools/async_tools/
+-rw-rw-rw-   0        0        0      550 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/async_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.571974 SomeTools-0.1.43/sometools/async_tools/base/
+-rw-rw-rw-   0        0        0       42 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/async_tools/base/__init__.py
+-rw-rw-rw-   0        0        0      181 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/async_tools/base/base.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.571974 SomeTools-0.1.43/sometools/async_tools/bloom_filter/
+-rw-rw-rw-   0        0        0       90 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/async_tools/bloom_filter/__init__.py
+-rw-rw-rw-   0        0        0     3632 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/async_tools/bloom_filter/async_bloomfilter_tool.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.571974 SomeTools-0.1.43/sometools/async_tools/database_tools/
+-rw-rw-rw-   0        0        0        0 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/async_tools/database_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.571974 SomeTools-0.1.43/sometools/async_tools/database_tools/mysql_tools/
+-rw-rw-rw-   0        0        0        0 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/async_tools/database_tools/mysql_tools/__init__.py
+-rw-rw-rw-   0        0        0    15175 2023-06-11 09:16:42.000000 SomeTools-0.1.43/sometools/async_tools/database_tools/mysql_tools/async_mysql_orm.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.571974 SomeTools-0.1.43/sometools/async_tools/redis_tools/
+-rw-rw-rw-   0        0        0       78 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/async_tools/redis_tools/__init__.py
+-rw-rw-rw-   0        0        0     1227 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/async_tools/redis_tools/async_io_redis.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.571974 SomeTools-0.1.43/sometools/sync_tools/
+-rw-rw-rw-   0        0        0        0 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.581368 SomeTools-0.1.43/sometools/sync_tools/base/
+-rw-rw-rw-   0        0        0       42 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/base/__init__.py
+-rw-rw-rw-   0        0        0      196 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/base/base.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.581872 SomeTools-0.1.43/sometools/sync_tools/base64_tools/
+-rw-rw-rw-   0        0        0       68 2023-06-11 08:25:17.000000 SomeTools-0.1.43/sometools/sync_tools/base64_tools/__init__.py
+-rw-rw-rw-   0        0        0     1507 2023-06-11 08:30:33.000000 SomeTools-0.1.43/sometools/sync_tools/base64_tools/base64_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.581872 SomeTools-0.1.43/sometools/sync_tools/calendar_tools/
+-rw-rw-rw-   0        0        0       69 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/calendar_tools/__init__.py
+-rw-rw-rw-   0        0        0     2785 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/calendar_tools/calendar_tool.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.581872 SomeTools-0.1.43/sometools/sync_tools/char_tools/
+-rw-rw-rw-   0        0        0       58 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/char_tools/__init__.py
+-rw-rw-rw-   0        0        0      895 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/char_tools/char_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.581872 SomeTools-0.1.43/sometools/sync_tools/chinese_to_pinyin_acronym/
+-rw-rw-rw-   0        0        0      121 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/chinese_to_pinyin_acronym/__init__.py
+-rw-rw-rw-   0        0        0     3448 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/chinese_to_pinyin_acronym/chinese_to_pinyin.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.581872 SomeTools-0.1.43/sometools/sync_tools/database_tools/
+-rw-rw-rw-   0        0        0        0 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/database_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.581872 SomeTools-0.1.43/sometools/sync_tools/database_tools/mysql_tools/
+-rw-rw-rw-   0        0        0        0 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/database_tools/mysql_tools/__init__.py
+-rw-rw-rw-   0        0        0     2769 2023-06-11 03:50:46.000000 SomeTools-0.1.43/sometools/sync_tools/database_tools/mysql_tools/conn_pool.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.587875 SomeTools-0.1.43/sometools/sync_tools/datetime_tools/
+-rw-rw-rw-   0        0        0       71 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/datetime_tools/__init__.py
+-rw-rw-rw-   0        0        0    12057 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/datetime_tools/date_conversion.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.587875 SomeTools-0.1.43/sometools/sync_tools/encryption_and_decryption_tools/
+-rw-rw-rw-   0        0        0      276 2023-06-11 04:17:42.000000 SomeTools-0.1.43/sometools/sync_tools/encryption_and_decryption_tools/__init__.py
+-rw-rw-rw-   0        0        0     2917 2023-06-11 07:57:46.000000 SomeTools-0.1.43/sometools/sync_tools/encryption_and_decryption_tools/aes_tool.py
+-rw-rw-rw-   0        0        0     2179 2023-06-11 08:26:35.000000 SomeTools-0.1.43/sometools/sync_tools/encryption_and_decryption_tools/rsa_tool.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.587875 SomeTools-0.1.43/sometools/sync_tools/image_tools/
+-rw-rw-rw-   0        0        0       61 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/image_tools/__init__.py
+-rw-rw-rw-   0        0        0     2575 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/image_tools/image_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.587875 SomeTools-0.1.43/sometools/sync_tools/ip_tools/
+-rw-rw-rw-   0        0        0       51 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/ip_tools/__init__.py
+-rw-rw-rw-   0        0        0      538 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/ip_tools/ip_tool.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.587875 SomeTools-0.1.43/sometools/sync_tools/log_tools/
+-rw-rw-rw-   0        0        0       57 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/log_tools/__init__.py
+-rw-rw-rw-   0        0        0     3758 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/log_tools/logger_main.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.587875 SomeTools-0.1.43/sometools/sync_tools/md5_tools/
+-rw-rw-rw-   0        0        0       59 2023-06-11 08:25:13.000000 SomeTools-0.1.43/sometools/sync_tools/md5_tools/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-06-11 08:02:02.000000 SomeTools-0.1.43/sometools/sync_tools/md5_tools/md5_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.587875 SomeTools-0.1.43/sometools/sync_tools/os_tools/
+-rw-rw-rw-   0        0        0       52 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/os_tools/__init__.py
+-rw-rw-rw-   0        0        0     3566 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/os_tools/os_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.587875 SomeTools-0.1.43/sometools/sync_tools/re_tools/
+-rw-rw-rw-   0        0        0       80 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/re_tools/__init__.py
+-rw-rw-rw-   0        0        0     2551 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/re_tools/extract_string.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.587875 SomeTools-0.1.43/sometools/sync_tools/redis_tools/
+-rw-rw-rw-   0        0        0       60 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/redis_tools/__init__.py
+-rw-rw-rw-   0        0        0      916 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/redis_tools/redis_main.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.587875 SomeTools-0.1.43/sometools/sync_tools/string_tools/
+-rw-rw-rw-   0        0        0       67 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/string_tools/__init__.py
+-rw-rw-rw-   0        0        0     1761 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/string_tools/string_cleaning.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.587875 SomeTools-0.1.43/sometools/sync_tools/traditional_simplified_chinese_conversion/
+-rw-rw-rw-   0        0        0      148 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/traditional_simplified_chinese_conversion/__init__.py
+-rw-rw-rw-   0        0        0     1955 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/traditional_simplified_chinese_conversion/traditional_simplified_chinese.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:21:11.587875 SomeTools-0.1.43/sometools/sync_tools/url_tools/
+-rw-rw-rw-   0        0        0       87 2023-06-10 10:45:04.000000 SomeTools-0.1.43/sometools/sync_tools/url_tools/__init__.py
+-rw-rw-rw-   0        0        0     1873 2023-06-11 08:36:12.000000 SomeTools-0.1.43/sometools/sync_tools/url_tools/url_encode_decode.py
```

### Comparing `SomeTools-0.1.41/LICENSE` & `SomeTools-0.1.43/LICENSE`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.41/PKG-INFO` & `SomeTools-0.1.43/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SomeTools
-Version: 0.1.41
+Version: 0.1.43
 Summary: Some python tools
 Home-page: https://pypi.org/project/SomeTools/
 Author: zhangkun
 Author-email: zk.kyle@foxmail.com
 Project-URL: Documentation, https://github.com/584807419/SomeTools
 Project-URL: Funding, https://github.com/584807419/SomeTools
 Project-URL: Source, https://github.com/584807419/SomeTools
@@ -43,16 +43,16 @@
 
 * redis创建连接同步、异步工具
 * 异步布隆过滤工具
 * 异步 mysql orm
 * 图片处理
 * 查看操作系统信息
 * 获取本机ip地址
-* AES加密解密
-
+* AES、RSA加密解密
+* base64、md5封装
 
 ## 安装
 
 ``` bash
 $ python -m pip install --upgrade pip
 $ pip install SomeTools -i https://pypi.python.org/simple
 ```
```

### Comparing `SomeTools-0.1.41/README.md` & `SomeTools-0.1.43/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 
 * redis创建连接同步、异步工具
 * 异步布隆过滤工具
 * 异步 mysql orm
 * 图片处理
 * 查看操作系统信息
 * 获取本机ip地址
-* AES加密解密
-
+* AES、RSA加密解密
+* base64、md5封装
 
 ## 安装
 
 ``` bash
 $ python -m pip install --upgrade pip
 $ pip install SomeTools -i https://pypi.python.org/simple
 ```
```

### Comparing `SomeTools-0.1.41/SomeTools.egg-info/PKG-INFO` & `SomeTools-0.1.43/SomeTools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SomeTools
-Version: 0.1.41
+Version: 0.1.43
 Summary: Some python tools
 Home-page: https://pypi.org/project/SomeTools/
 Author: zhangkun
 Author-email: zk.kyle@foxmail.com
 Project-URL: Documentation, https://github.com/584807419/SomeTools
 Project-URL: Funding, https://github.com/584807419/SomeTools
 Project-URL: Source, https://github.com/584807419/SomeTools
@@ -43,16 +43,16 @@
 
 * redis创建连接同步、异步工具
 * 异步布隆过滤工具
 * 异步 mysql orm
 * 图片处理
 * 查看操作系统信息
 * 获取本机ip地址
-* AES加密解密
-
+* AES、RSA加密解密
+* base64、md5封装
 
 ## 安装
 
 ``` bash
 $ python -m pip install --upgrade pip
 $ pip install SomeTools -i https://pypi.python.org/simple
 ```
```

### Comparing `SomeTools-0.1.41/SomeTools.egg-info/SOURCES.txt` & `SomeTools-0.1.43/SomeTools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 sometools/async_tools/database_tools/mysql_tools/__init__.py
 sometools/async_tools/database_tools/mysql_tools/async_mysql_orm.py
 sometools/async_tools/redis_tools/__init__.py
 sometools/async_tools/redis_tools/async_io_redis.py
 sometools/sync_tools/__init__.py
 sometools/sync_tools/base/__init__.py
 sometools/sync_tools/base/base.py
+sometools/sync_tools/base64_tools/__init__.py
+sometools/sync_tools/base64_tools/base64_tools.py
 sometools/sync_tools/calendar_tools/__init__.py
 sometools/sync_tools/calendar_tools/calendar_tool.py
 sometools/sync_tools/char_tools/__init__.py
 sometools/sync_tools/char_tools/char_tools.py
 sometools/sync_tools/chinese_to_pinyin_acronym/__init__.py
 sometools/sync_tools/chinese_to_pinyin_acronym/chinese_to_pinyin.py
 sometools/sync_tools/database_tools/__init__.py
@@ -36,14 +38,16 @@
 sometools/sync_tools/encryption_and_decryption_tools/rsa_tool.py
 sometools/sync_tools/image_tools/__init__.py
 sometools/sync_tools/image_tools/image_tools.py
 sometools/sync_tools/ip_tools/__init__.py
 sometools/sync_tools/ip_tools/ip_tool.py
 sometools/sync_tools/log_tools/__init__.py
 sometools/sync_tools/log_tools/logger_main.py
+sometools/sync_tools/md5_tools/__init__.py
+sometools/sync_tools/md5_tools/md5_tools.py
 sometools/sync_tools/os_tools/__init__.py
 sometools/sync_tools/os_tools/os_tools.py
 sometools/sync_tools/re_tools/__init__.py
 sometools/sync_tools/re_tools/extract_string.py
 sometools/sync_tools/redis_tools/__init__.py
 sometools/sync_tools/redis_tools/redis_main.py
 sometools/sync_tools/string_tools/__init__.py
```

### Comparing `SomeTools-0.1.41/SomeTools.egg-info/requires.txt` & `SomeTools-0.1.43/SomeTools.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.41/setup.py` & `SomeTools-0.1.43/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from setuptools import find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(name='SomeTools',
-      version='0.1.41',
+      version='0.1.43',
       description="Some python tools",
       author="zhangkun",
       author_email="zk.kyle@foxmail.com",
       project_urls={
           'Documentation': 'https://github.com/584807419/SomeTools',
           'Funding': 'https://github.com/584807419/SomeTools',
           'Source': 'https://github.com/584807419/SomeTools',
```

### Comparing `SomeTools-0.1.41/sometools/__init__.py` & `SomeTools-0.1.43/sometools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from sometools.sync_tools.re_tools import ExtractStringMixIn
 from sometools.sync_tools.image_tools import ImageMixin
 from sometools.sync_tools.char_tools import CharMixin
 from sometools.sync_tools.os_tools import OsMixin
 from sometools.sync_tools.ip_tools import IpMixIn
 from sometools.sync_tools.calendar_tools import CalendarMixIn
 from sometools.sync_tools.encryption_and_decryption_tools import EncryptionDecryptionMixIn
+from sometools.sync_tools.md5_tools import Md5Mixin
+from sometools.sync_tools.base64_tools import Base64Mixin
 
 
 class Common_tools(ChineseToPinyinMixIn, TraditionalSimplifiedChineseMixIn, UrlEncodeDecodeMixIn, DatetimeMixIn,
                    StringMixIn, IpMixIn, CalendarMixIn, ImageMixin, CharMixin, ExtractStringMixIn, OsMixin, LogMixIn,
-                   RedisMixIn, MysqlPoolMixIn, EncryptionDecryptionMixIn):
+                   RedisMixIn, MysqlPoolMixIn, EncryptionDecryptionMixIn, Md5Mixin, Base64Mixin):
     def __init__(self, *args, **kwargs):
         super(Common_tools, self).__init__(*args, **kwargs)
```

### Comparing `SomeTools-0.1.41/sometools/async_tools/__init__.py` & `SomeTools-0.1.43/sometools/async_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.41/sometools/async_tools/bloom_filter/async_bloomfilter_tool.py` & `SomeTools-0.1.43/sometools/async_tools/bloom_filter/async_bloomfilter_tool.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.41/sometools/async_tools/database_tools/mysql_tools/async_mysql_orm.py` & `SomeTools-0.1.43/sometools/async_tools/database_tools/mysql_tools/async_mysql_orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,32 +91,44 @@
 
 
 class StringField(Field):
 
     def __init__(self, name=None, primary_key=False, default=None, ddl='varchar(100)'):
         super().__init__(name, ddl, primary_key, default)
 
+class DecimalField(Field):
+
+    def __init__(self, name=None, primary_key=False, default=None, ddl='decimal(20,6)'):
+        super().__init__(name, ddl, primary_key, default)
 
 class BooleanField(Field):
 
     def __init__(self, name=None, default=False):
         super().__init__(name, 'boolean', False, default)
 
 
 class IntegerField(Field):
 
     def __init__(self, name=None, primary_key=False, default=0):
         super().__init__(name, 'bigint', primary_key, default)
 
+# class IntegerFieldWithNull(Field):
+#
+#     def __init__(self, name=None, primary_key=False, default=None):
+#         super().__init__(name, 'bigint', primary_key, default)
 
 class FloatField(Field):
 
     def __init__(self, name=None, primary_key=False, default=0.0):
         super().__init__(name, 'real', primary_key, default)
 
+class FloatFieldWithNull(Field):
+
+    def __init__(self, name=None, primary_key=False, default=None):
+        super().__init__(name, 'real', primary_key, default)
 
 class TextField(Field):
 
     def __init__(self, name=None, default=None):
         super().__init__(name, 'text', False, default)
 
 
@@ -227,14 +239,28 @@
             async with conn.cursor(aiomysql.DictCursor) as cur:
                 await cur.execute(sql_statement)
                 rs = await cur.fetchall()
                 await cur.close()
                 return rs
 
     @classmethod
+    async def select_by_pk(cls, db_pool, table_name, pk: int):
+        """
+        根据主键查找数据
+        :param db_pool:
+        :param pk: int
+        :return: cls
+        """
+        ' find object by primary key. '
+        rs = await _exec_select_sql(db_pool, '%s where `%s`=?' % (cls.__select__.replace("__Placeholder_identifier__", table_name), cls.__primary_key__), [pk], 1)
+        if len(rs) == 0:
+            return None
+        return cls(**rs[0])
+
+    @classmethod
     async def select_by_where(cls, db_pool=None, table_name=None, **kwargs) -> list:
         """
         where条件查询,适用于固定相等的筛选条件
         """
         if not table_name:
             table_name = cls.__table__
         if not db_pool:
@@ -279,15 +305,15 @@
                 temp_list.append(None)
             else:
                 temp_list.append(i)
         data_pk, rows = await _execute(self.__db_conn_pool__,
                                        self.__insert__.replace("__Placeholder_identifier__", table_name),
                                        temp_list)
         if rows != 1:
-            raise BaseException('failed to insert record: affected rows: %s' % rows)
+            raise Exception('failed to insert record: affected rows: %s' % rows)
         return data_pk
 
     async def update_db_date(self, table_name=None):
         if not table_name:
             table_name = self.__table__
         args = list(map(self.getValue, self.__fields__))
         args.append(self.getValue(self.__primary_key__))
@@ -300,15 +326,15 @@
 
     async def remove_db_date(self, table_name=None):
         if not table_name:
             table_name = self.__table__
         args = [self.getValue(self.__primary_key__)]
         data_pk, rows = await _execute(self.__db_conn_pool__, self.__delete__.replace("__Placeholder_identifier__", table_name), args)
         if rows != 1:
-            raise BaseException('failed to remove by primary key: affected rows: %s' % rows)
+            raise Exception('failed to remove by primary key: affected rows: %s' % rows)
         return rows
 
     @classmethod
     async def create_db_table(cls, db_pool, sql, autocommit=True):
         async with cls.__db_conn_pool__.acquire() as conn:
             if not autocommit:
                 await conn.begin()
```

### Comparing `SomeTools-0.1.41/sometools/async_tools/redis_tools/async_io_redis.py` & `SomeTools-0.1.43/sometools/async_tools/redis_tools/async_io_redis.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.41/sometools/sync_tools/calendar_tools/calendar_tool.py` & `SomeTools-0.1.43/sometools/sync_tools/calendar_tools/calendar_tool.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.41/sometools/sync_tools/char_tools/char_tools.py` & `SomeTools-0.1.43/sometools/sync_tools/char_tools/char_tools.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.41/sometools/sync_tools/chinese_to_pinyin_acronym/chinese_to_pinyin.py` & `SomeTools-0.1.43/sometools/sync_tools/chinese_to_pinyin_acronym/chinese_to_pinyin.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.41/sometools/sync_tools/database_tools/mysql_tools/conn_pool.py` & `SomeTools-0.1.43/sometools/sync_tools/database_tools/mysql_tools/conn_pool.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.41/sometools/sync_tools/datetime_tools/date_conversion.py` & `SomeTools-0.1.43/sometools/sync_tools/datetime_tools/date_conversion.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.41/sometools/sync_tools/encryption_and_decryption_tools/aes_tool.py` & `SomeTools-0.1.43/sometools/sync_tools/encryption_and_decryption_tools/aes_tool.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,67 +4,73 @@
 
 
 class AesMixIn(Base):
 
     def __init__(self, *args, **kwargs):
         super(AesMixIn, self).__init__(*args, **kwargs)
 
-    def aes_ecb_encryption(self, content, password: bytes) -> bytes:
+    @staticmethod
+    def aes_ecb_encryption(content, password: bytes) -> bytes:
         """
         ECB模式加密
         :param content:明文必须为16字节或者16字节的倍数的字节型数据，如果不够16字节需要进行补全
         :param password:秘钥必须为16字节或者16字节的倍数的字节型数据。
         :return: bytes
         """
         aes = AES.new(password, AES.MODE_ECB)  # 创建一个aes对象,aes 加密常用的有 ECB 和 CBC 模式,AES.MODE_ECB 表示模式是ECB模式
         en_text = aes.encrypt(content)  # 加密明文
         return en_text
 
-    def aes_ecb_decryption(self, en_text, password: bytes) -> bytes:
+    @staticmethod
+    def aes_ecb_decryption(en_text, password: bytes) -> bytes:
         """
         ECB模式解密
         :param en_text 加密后的密文
         :param password:秘钥必须为16字节或者16字节的倍数的字节型数据。
         :return: bytes
         """
         aes = AES.new(password, AES.MODE_ECB)
         content = aes.decrypt(en_text)
         return content
 
-    def aes_cbc_encryption(self, content, password, iv: bytes) -> bytes:
+    @staticmethod
+    def aes_cbc_encryption(content, password, iv: bytes) -> bytes:
         """
         CBC模式的加密
         :param content:明文必须为16字节或者16字节的倍数的字节型数据，如果不够16字节需要进行补全
         :param password:秘钥必须为16字节或者16字节的倍数的字节型数据
         :param iv 偏移量，bytes类型
         :return: bytes
         """
         aes = AES.new(password, AES.MODE_CBC, iv)  # 创建一个aes对象  AES.MODE_CBC 表示模式是CBC模式
         en_text = aes.encrypt(content)  # 加密明文
         return en_text
 
-    def aes_cbc_decryption(self, en_text, password, iv: bytes) -> bytes:
+    @staticmethod
+    def aes_cbc_decryption(en_text, password, iv: bytes) -> bytes:
         """
         CBC模式解密
         :param en_text 加密后的密文
         :param password:秘钥必须为16字节或者16字节的倍数的字节型数据。
         :param iv 偏移量，bytes类型
         :return: bytes
         """
         aes = AES.new(password, AES.MODE_CBC,
                       iv)  # CBC模式与ECB模式的区别：AES.new() 解密和加密重新生成了aes对象，加密和解密不能调用同一个aes对象，否则会报错TypeError: decrypt() cannot be called after encrypt()
         content = aes.decrypt(en_text)
         return content
 
-    def aes_pad(self, content) -> bytes:
+    @staticmethod
+    def aes_pad(content) -> bytes:
         """
         填充
         """
         text = pad(content, AES.block_size)
         return text
 
-    def aes_unpad(self, en_text) -> bytes:
+    @staticmethod
+    def aes_unpad(en_text) -> bytes:
         """
         去填充
         """
         text = unpad(en_text, AES.block_size)
         return text
```

### Comparing `SomeTools-0.1.41/sometools/sync_tools/encryption_and_decryption_tools/rsa_tool.py` & `SomeTools-0.1.43/sometools/sync_tools/encryption_and_decryption_tools/rsa_tool.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,48 +4,54 @@
 
 
 class RsaMixIn(Base):
 
     def __init__(self, *args, **kwargs):
         super(RsaMixIn, self).__init__(*args, **kwargs)
 
-    def rsa_get_key_pair(self) -> (PublicKey, PrivateKey):
+    @staticmethod
+    def rsa_get_key_pair() -> (PublicKey, PrivateKey):
         """生成密钥对"""
         pubkey, prikey = rsa.newkeys(1024)
         return pubkey, prikey
 
+    @staticmethod
     def rsa_create_pub_key(self) -> (PublicKey, PrivateKey):
         """创建公钥"""
         # 公钥有两个值  n,e
         public_n = "e0b509f62a8fc9" * 4
         public_e = '010001'
         # n、e必须为整数
         # 将16进制的字符串转为整数
         rsa_n = int(public_n, 16)
         rsa_e = int(public_e, 16)
         print('n：{}\ne：{}'.format(rsa_n, rsa_e))
         # 创建公钥 rsa.PublicKey(n,e)
         pubkey = rsa.PublicKey(rsa_n, rsa_e)
         return pubkey
 
-    def rsa_sign(self, content: bytes, pri_key: PrivateKey, sign_type: str = 'MD5') -> bytes:
+    @staticmethod
+    def rsa_sign(content: bytes, pri_key: PrivateKey, sign_type: str = 'MD5') -> bytes:
         """加签    rsa.sign(原信息，私钥，加密方式)  生成加签过后的信息"""
         sign_message = rsa.sign(content, pri_key, sign_type)
         return sign_message
 
-    def rsa_verify(self, content: bytes, pub_key: PublicKey, sign_message: bytes) -> (PublicKey, PrivateKey):
+    @staticmethod
+    def rsa_verify(content: bytes, pub_key: PublicKey, sign_message: bytes) -> (PublicKey, PrivateKey):
         """验签    rsa.verify(需要验证的信息，加签过后的信息，公钥),如果需要验证的信息，是原信息，返回加密方式"""
         try:
             veri_res = rsa.verify(content, sign_message, pub_key)
             print(f'校验通过无修改-加密方式{veri_res}')
             return True
         except rsa.pkcs1.VerificationError as e:
             print(f"校验未通过-信息被篡改过-{e}")
             return False
 
-    def rsa_encryption(self, content: bytes, pubkey: PublicKey) -> bytes:
+    @staticmethod
+    def rsa_encryption(content: bytes, pubkey: PublicKey) -> bytes:
         """加密：使用公钥"""
         return rsa.encrypt(content, pubkey)
 
-    def rsa_decryption(self, en_text: bytes, prikey: PrivateKey) -> bytes:
+    @staticmethod
+    def rsa_decryption(en_text: bytes, prikey: PrivateKey) -> bytes:
         """解密：使用私钥"""
         return rsa.decrypt(en_text, prikey)
```

### Comparing `SomeTools-0.1.41/sometools/sync_tools/image_tools/image_tools.py` & `SomeTools-0.1.43/sometools/sync_tools/image_tools/image_tools.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.41/sometools/sync_tools/ip_tools/ip_tool.py` & `SomeTools-0.1.43/sometools/sync_tools/ip_tools/ip_tool.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.41/sometools/sync_tools/log_tools/logger_main.py` & `SomeTools-0.1.43/sometools/sync_tools/log_tools/logger_main.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.41/sometools/sync_tools/os_tools/os_tools.py` & `SomeTools-0.1.43/sometools/sync_tools/os_tools/os_tools.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.41/sometools/sync_tools/re_tools/extract_string.py` & `SomeTools-0.1.43/sometools/sync_tools/re_tools/extract_string.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.41/sometools/sync_tools/redis_tools/redis_main.py` & `SomeTools-0.1.43/sometools/sync_tools/redis_tools/redis_main.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.41/sometools/sync_tools/string_tools/string_cleaning.py` & `SomeTools-0.1.43/sometools/sync_tools/string_tools/string_cleaning.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.41/sometools/sync_tools/traditional_simplified_chinese_conversion/traditional_simplified_chinese.py` & `SomeTools-0.1.43/sometools/sync_tools/traditional_simplified_chinese_conversion/traditional_simplified_chinese.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.41/sometools/sync_tools/url_tools/url_encode_decode.py` & `SomeTools-0.1.43/sometools/sync_tools/url_tools/url_encode_decode.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #     通常如果一样东西需要编码，说明这样东西并不适合传输。原因多种多样，如Size过大，包含隐私数据。对于Url来说，之所以要进行编码，是因为Url中有些字符会引起歧义。
 #
 #     例如，Url参数字符串中使用key=value键值对这样的形式来传参，键值对之间以&符号分隔，如/s?q=abc&ie=utf-8。如果你的value字符串中包含了=或者&，那么势必会造成接收Url的服务器解析错误，因此必须将引起歧义的&和=符号进行转义，也就是对其进行编码。
 #
 #     又如，Url的编码格式采用的是ASCII码，而不是Unicode，这也就是说你不能在Url中包含任何非ASCII字符，例如中文。否则如果客户端浏览器和服务端浏览器支持的字符集不同的情况下，中文可能会造成问题。
 # -*- coding: utf-8 -*-
 
-from urllib.request import quote, unquote
+from urllib.parse import quote, unquote
 
 from sometools.sync_tools.base import Base
 
 
 class UrlEncodeDecodeMixIn(Base):
     def __init__(self, *args, **kwargs):
         super(UrlEncodeDecodeMixIn, self).__init__(*args, **kwargs)
```

