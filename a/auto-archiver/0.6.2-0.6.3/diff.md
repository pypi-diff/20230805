# Comparing `tmp/auto_archiver-0.6.2.tar.gz` & `tmp/auto_archiver-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_archiver-0.6.2.tar", last modified: Fri Jul 28 12:13:39 2023, max compression
+gzip compressed data, was "auto_archiver-0.6.3.tar", last modified: Sat Aug  5 13:02:14 2023, max compression
```

## Comparing `auto_archiver-0.6.2.tar` & `auto_archiver-0.6.3.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.364216 auto_archiver-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-07-28 12:13:39.364216 auto_archiver-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-28 12:13:39.364216 auto_archiver-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.356216 auto_archiver-0.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.356216 auto_archiver-0.6.2/src/auto_archiver/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.360216 auto_archiver-0.6.2/src/auto_archiver/archivers/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/archivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/archivers/archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/archivers/instagram_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/archivers/instagram_tbot_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/archivers/telegram_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/archivers/telethon_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/archivers/tiktok_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/archivers/twitter_api_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/archivers/twitter_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/archivers/vk_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/archivers/youtubedl_archiver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.360216 auto_archiver-0.6.2/src/auto_archiver/core/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/core/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/core/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/core/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/core/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/core/step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.360216 auto_archiver-0.6.2/src/auto_archiver/databases/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/databases/api_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/databases/console_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/databases/csv_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/databases/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/databases/gsheet_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.360216 auto_archiver-0.6.2/src/auto_archiver/enrichers/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/enrichers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/enrichers/enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/enrichers/hash_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/enrichers/metadata_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/enrichers/pdq_hash_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/enrichers/screenshot_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/enrichers/thumbnail_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/enrichers/wacz_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/enrichers/wayback_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/enrichers/whisper_enricher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.364216 auto_archiver-0.6.2/src/auto_archiver/feeders/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/feeders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/feeders/cli_feeder.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/feeders/feeder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/feeders/gsheet_feeder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.364216 auto_archiver-0.6.2/src/auto_archiver/formatters/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/formatters/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/formatters/html_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/formatters/mute_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.364216 auto_archiver-0.6.2/src/auto_archiver/formatters/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/formatters/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/formatters/templates/html_template.html
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/formatters/templates/macros.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.364216 auto_archiver-0.6.2/src/auto_archiver/storages/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/storages/gd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/storages/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/storages/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/storages/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.364216 auto_archiver-0.6.2/src/auto_archiver/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/utils/gsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/utils/gworksheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/utils/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/utils/webdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.356216 auto_archiver-0.6.2/src/auto_archiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-07-28 12:13:39.000000 auto_archiver-0.6.2/src/auto_archiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-28 12:13:39.000000 auto_archiver-0.6.2/src/auto_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 12:13:39.000000 auto_archiver-0.6.2/src/auto_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-28 12:13:39.000000 auto_archiver-0.6.2/src/auto_archiver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 12:13:39.000000 auto_archiver-0.6.2/src/auto_archiver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-28 12:13:39.000000 auto_archiver-0.6.2/src/auto_archiver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 12:13:39.000000 auto_archiver-0.6.2/src/auto_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:02:14.342625 auto_archiver-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-08-05 13:02:14.342625 auto_archiver-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-05 13:02:14.342625 auto_archiver-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:02:14.330624 auto_archiver-0.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:02:14.334624 auto_archiver-0.6.3/src/auto_archiver/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:02:14.334624 auto_archiver-0.6.3/src/auto_archiver/archivers/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/archivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/archivers/archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/archivers/instagram_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/archivers/instagram_tbot_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/archivers/telegram_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/archivers/telethon_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/archivers/tiktok_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/archivers/twitter_api_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/archivers/twitter_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/archivers/vk_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/archivers/youtubedl_archiver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:02:14.338624 auto_archiver-0.6.3/src/auto_archiver/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/core/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/core/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/core/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/core/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:02:14.338624 auto_archiver-0.6.3/src/auto_archiver/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/databases/api_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/databases/console_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/databases/csv_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/databases/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/databases/gsheet_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:02:14.338624 auto_archiver-0.6.3/src/auto_archiver/enrichers/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/enrichers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/enrichers/enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/enrichers/hash_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/enrichers/metadata_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/enrichers/pdq_hash_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/enrichers/screenshot_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/enrichers/thumbnail_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/enrichers/wacz_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/enrichers/wayback_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/enrichers/whisper_enricher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:02:14.338624 auto_archiver-0.6.3/src/auto_archiver/feeders/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/feeders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/feeders/cli_feeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/feeders/feeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/feeders/gsheet_feeder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:02:14.342625 auto_archiver-0.6.3/src/auto_archiver/formatters/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/formatters/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/formatters/html_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/formatters/mute_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:02:14.342625 auto_archiver-0.6.3/src/auto_archiver/formatters/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/formatters/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/formatters/templates/html_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/formatters/templates/macros.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:02:14.342625 auto_archiver-0.6.3/src/auto_archiver/storages/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/storages/gd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/storages/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/storages/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/storages/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:02:14.342625 auto_archiver-0.6.3/src/auto_archiver/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/utils/gsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/utils/gworksheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/utils/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/utils/webdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-05 12:59:13.000000 auto_archiver-0.6.3/src/auto_archiver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:02:14.334624 auto_archiver-0.6.3/src/auto_archiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-08-05 13:02:14.000000 auto_archiver-0.6.3/src/auto_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-08-05 13:02:14.000000 auto_archiver-0.6.3/src/auto_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 13:02:14.000000 auto_archiver-0.6.3/src/auto_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-05 13:02:14.000000 auto_archiver-0.6.3/src/auto_archiver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 13:02:14.000000 auto_archiver-0.6.3/src/auto_archiver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-05 13:02:14.000000 auto_archiver-0.6.3/src/auto_archiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-05 13:02:14.000000 auto_archiver-0.6.3/src/auto_archiver.egg-info/top_level.txt
```

### Comparing `auto_archiver-0.6.2/LICENSE` & `auto_archiver-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/PKG-INFO` & `auto_archiver-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_archiver
-Version: 0.6.2
+Version: 0.6.3
 Summary: Easily archive online media content
 Author: Bellingcat
 Author-email: tech@bellingcat.com
 License: MIT
 Project-URL: Source Code, https://github.com/bellingcat/auto-archiver
 Project-URL: Bug Tracker, https://github.com/bellingcat/auto-archiver/issues
 Project-URL: Bellingcat, https://www.bellingcat.com
```

### Comparing `auto_archiver-0.6.2/README.md` & `auto_archiver-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/setup.cfg` & `auto_archiver-0.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/archivers/archiver.py` & `auto_archiver-0.6.3/src/auto_archiver/archivers/archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/archivers/instagram_archiver.py` & `auto_archiver-0.6.3/src/auto_archiver/archivers/instagram_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/archivers/instagram_tbot_archiver.py` & `auto_archiver-0.6.3/src/auto_archiver/archivers/instagram_tbot_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/archivers/telegram_archiver.py` & `auto_archiver-0.6.3/src/auto_archiver/archivers/telegram_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/archivers/telethon_archiver.py` & `auto_archiver-0.6.3/src/auto_archiver/archivers/telethon_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/archivers/tiktok_archiver.py` & `auto_archiver-0.6.3/src/auto_archiver/archivers/tiktok_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/archivers/twitter_api_archiver.py` & `auto_archiver-0.6.3/src/auto_archiver/archivers/twitter_api_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/archivers/twitter_archiver.py` & `auto_archiver-0.6.3/src/auto_archiver/archivers/twitter_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/archivers/vk_archiver.py` & `auto_archiver-0.6.3/src/auto_archiver/archivers/vk_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/archivers/youtubedl_archiver.py` & `auto_archiver-0.6.3/src/auto_archiver/archivers/youtubedl_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/core/config.py` & `auto_archiver-0.6.3/src/auto_archiver/core/config.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/core/context.py` & `auto_archiver-0.6.3/src/auto_archiver/core/context.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/core/media.py` & `auto_archiver-0.6.3/src/auto_archiver/core/media.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
     def is_valid_video(self) -> bool:
         # checks for video streams with ffmpeg, or min file size for a video
         # self.is_video() should be used together with this method
         try:
             streams = ffmpeg.probe(self.filename, select_streams='v')['streams']
             logger.warning(f"STREAMS FOR {self.filename} {streams}")
-            return any(s.get("duration_ts") > 0 for s in streams)
+            return any(s.get("duration_ts", 0) > 0 for s in streams)
         except Error: return False # ffmpeg errors when reading bad files
         except Exception as e:
             logger.error(e)
             logger.error(traceback.format_exc())
             try:
                 fsize = os.path.getsize(self.filename)
                 return fsize > 20_000
```

### Comparing `auto_archiver-0.6.2/src/auto_archiver/core/metadata.py` & `auto_archiver-0.6.3/src/auto_archiver/core/metadata.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/core/orchestrator.py` & `auto_archiver-0.6.3/src/auto_archiver/core/orchestrator.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/core/step.py` & `auto_archiver-0.6.3/src/auto_archiver/core/step.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/databases/api_db.py` & `auto_archiver-0.6.3/src/auto_archiver/databases/api_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/databases/console_db.py` & `auto_archiver-0.6.3/src/auto_archiver/databases/console_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/databases/csv_db.py` & `auto_archiver-0.6.3/src/auto_archiver/databases/csv_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/databases/database.py` & `auto_archiver-0.6.3/src/auto_archiver/databases/database.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/databases/gsheet_db.py` & `auto_archiver-0.6.3/src/auto_archiver/databases/gsheet_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/enrichers/enricher.py` & `auto_archiver-0.6.3/src/auto_archiver/enrichers/enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/enrichers/hash_enricher.py` & `auto_archiver-0.6.3/src/auto_archiver/enrichers/hash_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/enrichers/metadata_enricher.py` & `auto_archiver-0.6.3/src/auto_archiver/enrichers/metadata_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/enrichers/pdq_hash_enricher.py` & `auto_archiver-0.6.3/src/auto_archiver/enrichers/pdq_hash_enricher.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,19 +22,24 @@
     @staticmethod
     def configs() -> dict:
         return {}
 
     def enrich(self, to_enrich: Metadata) -> None:
         url = to_enrich.get_url()
         logger.debug(f"calculating perceptual hashes for {url=}")
+        media_with_hashes = []
 
         for m in to_enrich.media:
             for media in m.all_inner_media(True):
-                if media.is_image() and "screenshot" not in media.get("id") and "warc-file-" not in media.get("id") and len(hd := self.calculate_pdq_hash(media.filename)):
+                media_id = media.get("id", "")
+                if media.is_image() and "screenshot" not in media_id and "warc-file-" not in media_id and len(hd := self.calculate_pdq_hash(media.filename)):
                     media.set("pdq_hash", hd)
+                    media_with_hashes.append(media.filename)
+
+        logger.debug(f"calculated '{len(media_with_hashes)}' perceptual hashes for {url=}: {media_with_hashes}")
 
     def calculate_pdq_hash(self, filename):
         # returns a hexadecimal string with the perceptual hash for the given filename
         try:
             with Image.open(filename) as img:
                 # convert the image to RGB
                 image_rgb = np.array(img.convert("RGB"))
```

### Comparing `auto_archiver-0.6.2/src/auto_archiver/enrichers/screenshot_enricher.py` & `auto_archiver-0.6.3/src/auto_archiver/enrichers/screenshot_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/enrichers/thumbnail_enricher.py` & `auto_archiver-0.6.3/src/auto_archiver/enrichers/thumbnail_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/enrichers/wacz_enricher.py` & `auto_archiver-0.6.3/src/auto_archiver/enrichers/wacz_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/enrichers/wayback_enricher.py` & `auto_archiver-0.6.3/src/auto_archiver/enrichers/wayback_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/enrichers/whisper_enricher.py` & `auto_archiver-0.6.3/src/auto_archiver/enrichers/whisper_enricher.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,25 +14,26 @@
     Only works if an S3 compatible storage is used
     """
     name = "whisper_enricher"
 
     def __init__(self, config: dict) -> None:
         # without this STEP.__init__ is not called
         super().__init__(config)
+        assert type(self.api_endpoint) == str and len(self.api_endpoint) > 0, "please provide a value for the whisper_enricher api_endpoint"
         assert type(self.api_key) == str and len(self.api_key) > 0, "please provide a value for the whisper_enricher api_key"
         self.timeout = int(self.timeout)
 
     @staticmethod
     def configs() -> dict:
         return {
-            "api_endpoint": {"default": "https://whisper.spoettel.dev/api/v1", "help": "WhisperApi api endpoint"},
+            "api_endpoint": {"default": None, "help": "WhisperApi api endpoint, eg: https://whisperbox-api.com/api/v1, a deployment of https://github.com/bellingcat/whisperbox-transcribe."},
             "api_key": {"default": None, "help": "WhisperApi api key for authentication"},
             "include_srt": {"default": False, "help": "Whether to include a subtitle SRT (SubRip Subtitle file) for the video (can be used in video players)."},
             "timeout": {"default": 90, "help": "How many seconds to wait at most for a successful job completion."},
-            "action": {"default": "translation", "help": "which Whisper operation to execute", "choices": ["transcript", "translation", "language_detection"]},
+            "action": {"default": "translate", "help": "which Whisper operation to execute", "choices": ["transcribe", "translate", "language_detection"]},
 
         }
 
     def enrich(self, to_enrich: Metadata) -> None:
         if not self._get_s3_storage():
             logger.error("WhisperEnricher: To use the WhisperEnricher you need to use S3Storage so files are accessible publicly to the whisper service being called.")
             return
@@ -72,14 +73,15 @@
         s3_url = s3.get_cdn_url(media)
         assert s3_url in media.urls, f"Could not find S3 url ({s3_url}) in list of stored media urls "
         payload = {
             "url": s3_url,
             "type": self.action,
             # "language": "string" # may be a config
         }
+        logger.debug(f"calling API with {payload=}")
         response = requests.post(f'{self.api_endpoint}/jobs', json=payload, headers={'Authorization': f'Bearer {self.api_key}'})
         assert response.status_code == 201, f"calling the whisper api {self.api_endpoint} returned a non-success code: {response.status_code}"
         logger.debug(response.json())
         return response.json()['id']
 
     def check_jobs(self, job_results: dict):
         start_time = time.time()
```

### Comparing `auto_archiver-0.6.2/src/auto_archiver/feeders/cli_feeder.py` & `auto_archiver-0.6.3/src/auto_archiver/feeders/cli_feeder.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/feeders/feeder.py` & `auto_archiver-0.6.3/src/auto_archiver/feeders/feeder.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/feeders/gsheet_feeder.py` & `auto_archiver-0.6.3/src/auto_archiver/feeders/gsheet_feeder.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/formatters/formatter.py` & `auto_archiver-0.6.3/src/auto_archiver/formatters/formatter.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/formatters/html_formatter.py` & `auto_archiver-0.6.3/src/auto_archiver/formatters/html_formatter.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/formatters/templates/html_template.html` & `auto_archiver-0.6.3/src/auto_archiver/formatters/templates/html_template.html`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/formatters/templates/macros.html` & `auto_archiver-0.6.3/src/auto_archiver/formatters/templates/macros.html`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     <div>
         Reverse Image Search:&nbsp;
         <a href="https://www.google.com/searchbyimage?sbisrc=4chanx&image_url={{ url | quote }}&safe=off">Google</a>,&nbsp;
         <a href="https://lens.google.com/uploadbyurl?url={{ url | quote }}">Google Lens</a>,&nbsp;
         <a href="https://yandex.ru/images/touch/search?rpt=imageview&url={{ url | quote }}">Yandex</a>,&nbsp;
         <a href="https://www.bing.com/images/search?view=detailv2&iss=sbi&form=SBIVSP&sbisrc=UrlPaste&q=imgurl:{{ url | quote }}">Bing</a>,&nbsp;
-        <a href="https://www.tineye.com/search/?url={{ url | quote }}">Tineye</a>,&nbsp;
+        <a href="https://www.tineye.com/search/?url={{ url | quote }}">Tineye</a>
     </div>
     <p></p>
 </div>
 {% elif 'video' in m.mimetype %}
 <div>
     <video src="{{ url }}" controls style="max-height:400px;max-width:600px;">
         Your browser does not support the video element.
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% macro display_media(m, links, main_url) -%} {% for url in m.urls %} {% if
 url | length == 0 %} No URL available for {{ m.key }}. {% elif 'http' in url %}
 {% if 'image' in m.mimetype %}
 [{{_url_}}]
-Reverse Image Search:  Google,  Google_Lens,  Yandex,  Bing,  Tineye, 
+Reverse Image Search:  Google,  Google_Lens,  Yandex,  Bing,  Tineye
 {% elif 'video' in m.mimetype %}
  Your browser does not support the video element.
 {% elif 'audio' in m.mimetype %}
   Your browser does not support the audio element.
 {% elif m.filename | get_extension == ".wacz" %} replayweb {% else %} No
 preview available for {{ m.key }}. {% endif %} {% else %} {{ m.url | urlize }}
 {% endif %} {% if links %} open or download or {{ copy_urlize(url, "copy") }}
```

### Comparing `auto_archiver-0.6.2/src/auto_archiver/storages/gd.py` & `auto_archiver-0.6.3/src/auto_archiver/storages/gd.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/storages/local.py` & `auto_archiver-0.6.3/src/auto_archiver/storages/local.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/storages/s3.py` & `auto_archiver-0.6.3/src/auto_archiver/storages/s3.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/storages/storage.py` & `auto_archiver-0.6.3/src/auto_archiver/storages/storage.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/utils/gsheet.py` & `auto_archiver-0.6.3/src/auto_archiver/utils/gsheet.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/utils/gworksheet.py` & `auto_archiver-0.6.3/src/auto_archiver/utils/gworksheet.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/utils/misc.py` & `auto_archiver-0.6.3/src/auto_archiver/utils/misc.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver/utils/url.py` & `auto_archiver-0.6.3/src/auto_archiver/utils/url.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,14 +48,19 @@
         if "https://scontent.cdninstagram.com/" in url and "150x150" in url: return False
         # instagram recurring images
         if "https://static.cdninstagram.com/rsrc.php/" in url: return False
 
         # telegram
         if "https://telegram.org/img/emoji/" in url: return False
 
+        # youtube
+        if "https://www.youtube.com/s/gaming/emoji/" in url: return False
+        if "https://yt3.ggpht.com" in url and "default-user=" in url: return False
+        if "https://www.youtube.com/s/search/audio/" in url: return False
+
         return True
 
     @staticmethod
     def twitter_best_quality_url(url: str) -> str:
         """
         some twitter image URLs point to a less-than best quality
         this returns the URL pointing to the highest (original) quality
```

### Comparing `auto_archiver-0.6.2/src/auto_archiver/utils/webdriver.py` & `auto_archiver-0.6.3/src/auto_archiver/utils/webdriver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.2/src/auto_archiver.egg-info/PKG-INFO` & `auto_archiver-0.6.3/src/auto_archiver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-archiver
-Version: 0.6.2
+Version: 0.6.3
 Summary: Easily archive online media content
 Author: Bellingcat
 Author-email: tech@bellingcat.com
 License: MIT
 Project-URL: Source Code, https://github.com/bellingcat/auto-archiver
 Project-URL: Bug Tracker, https://github.com/bellingcat/auto-archiver/issues
 Project-URL: Bellingcat, https://www.bellingcat.com
```

### Comparing `auto_archiver-0.6.2/src/auto_archiver.egg-info/SOURCES.txt` & `auto_archiver-0.6.3/src/auto_archiver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

