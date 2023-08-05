# Comparing `tmp/aa-miningtaxes-1.2.8.tar.gz` & `tmp/aa-miningtaxes-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-miningtaxes-1.2.8.tar", last modified: Mon Jun 26 15:49:26 2023, max compression
+gzip compressed data, was "aa-miningtaxes-1.2.9.tar", last modified: Tue Jul 11 22:34:59 2023, max compression
```

## Comparing `aa-miningtaxes-1.2.8.tar` & `aa-miningtaxes-1.2.9.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:49:26.482810 aa-miningtaxes-1.2.8/
--rw-r--r--   0 root         (0) root         (0)     1070 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      183 2022-11-06 18:50:28.000000 aa-miningtaxes-1.2.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7451 2023-06-26 15:49:26.483810 aa-miningtaxes-1.2.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5740 2023-06-24 15:56:29.000000 aa-miningtaxes-1.2.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:49:26.474810 aa-miningtaxes-1.2.8/aa_miningtaxes.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7451 2023-06-26 15:49:26.000000 aa-miningtaxes-1.2.8/aa_miningtaxes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2941 2023-06-26 15:49:26.000000 aa-miningtaxes-1.2.8/aa_miningtaxes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 15:49:26.000000 aa-miningtaxes-1.2.8/aa_miningtaxes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       75 2023-06-26 15:49:26.000000 aa-miningtaxes-1.2.8/aa_miningtaxes.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-26 15:49:26.000000 aa-miningtaxes-1.2.8/aa_miningtaxes.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:49:26.476810 aa-miningtaxes-1.2.8/miningtaxes/
--rw-r--r--   0 root         (0) root         (0)      108 2023-06-26 15:49:08.000000 aa-miningtaxes-1.2.8/miningtaxes/__init__.py
--rw-r--r--   0 root         (0) root         (0)       84 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.8/miningtaxes/admin.py
--rw-r--r--   0 root         (0) root         (0)     1460 2023-06-24 15:56:21.000000 aa-miningtaxes-1.2.8/miningtaxes/app_settings.py
--rw-r--r--   0 root         (0) root         (0)      200 2022-10-27 10:33:48.000000 aa-miningtaxes-1.2.8/miningtaxes/apps.py
--rw-r--r--   0 root         (0) root         (0)      912 2022-10-24 21:25:29.000000 aa-miningtaxes-1.2.8/miningtaxes/auth_hooks.py
--rw-r--r--   0 root         (0) root         (0)     3304 2022-11-07 04:47:52.000000 aa-miningtaxes-1.2.8/miningtaxes/decorators.py
--rw-r--r--   0 root         (0) root         (0)      264 2022-11-05 16:57:46.000000 aa-miningtaxes-1.2.8/miningtaxes/forms.py
--rw-r--r--   0 root         (0) root         (0)     2295 2023-06-25 02:35:02.000000 aa-miningtaxes-1.2.8/miningtaxes/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:49:26.471810 aa-miningtaxes-1.2.8/miningtaxes/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:49:26.477810 aa-miningtaxes-1.2.8/miningtaxes/management/commands/
--rw-r--r--   0 root         (0) root         (0)      102 2022-10-29 09:17:21.000000 aa-miningtaxes-1.2.8/miningtaxes/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      233 2023-01-08 17:44:15.000000 aa-miningtaxes-1.2.8/miningtaxes/management/commands/miningtaxes_preload_prices.py
--rw-r--r--   0 root         (0) root         (0)      221 2023-04-04 18:04:31.000000 aa-miningtaxes-1.2.8/miningtaxes/management/commands/miningtaxes_update_manual.py
--rw-r--r--   0 root         (0) root         (0)      434 2022-11-22 12:21:22.000000 aa-miningtaxes-1.2.8/miningtaxes/management/commands/miningtaxes_zero_all.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:49:26.478810 aa-miningtaxes-1.2.8/miningtaxes/migrations/
--rw-r--r--   0 root         (0) root         (0)      902 2022-11-06 17:28:27.000000 aa-miningtaxes-1.2.8/miningtaxes/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)    15700 2022-11-06 17:28:28.000000 aa-miningtaxes-1.2.8/miningtaxes/migrations/0002_all_models.py
--rw-r--r--   0 root         (0) root         (0)      779 2022-11-08 09:05:56.000000 aa-miningtaxes-1.2.8/miningtaxes/migrations/0003_alter_general_options.py
--rw-r--r--   0 root         (0) root         (0)      939 2022-11-12 04:17:36.000000 aa-miningtaxes-1.2.8/miningtaxes/migrations/0004_settings_interest_rate_alter_settings_phrase.py
--rw-r--r--   0 root         (0) root         (0)      737 2022-11-14 03:13:49.000000 aa-miningtaxes-1.2.8/miningtaxes/migrations/0005_oreprices_raw_price_oreprices_refined_price_and_more.py
--rw-r--r--   0 root         (0) root         (0)      452 2022-11-22 12:29:33.000000 aa-miningtaxes-1.2.8/miningtaxes/migrations/0006_charactertaxcredits_credit_type.py
--rw-r--r--   0 root         (0) root         (0)      566 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.8/miningtaxes/migrations/0007_character_life_credits_character_life_taxes.py
--rw-r--r--   0 root         (0) root         (0)      793 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.8/miningtaxes/migrations/0008_character_monthly_credits_json_and_more.py
--rw-r--r--   0 root         (0) root         (0)     1461 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.8/miningtaxes/migrations/0009_stats.py
--rw-r--r--   0 root         (0) root         (0)      405 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.8/miningtaxes/migrations/0010_stats_admin_get_all_activity_json.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 16:52:52.000000 aa-miningtaxes-1.2.8/miningtaxes/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:49:26.479810 aa-miningtaxes-1.2.8/miningtaxes/models/
--rw-r--r--   0 root         (0) root         (0)      438 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.8/miningtaxes/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7153 2023-06-19 19:07:48.000000 aa-miningtaxes-1.2.8/miningtaxes/models/admin.py
--rw-r--r--   0 root         (0) root         (0)    18238 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.8/miningtaxes/models/character.py
--rw-r--r--   0 root         (0) root         (0)      712 2022-11-08 03:08:01.000000 aa-miningtaxes-1.2.8/miningtaxes/models/general.py
--rw-r--r--   0 root         (0) root         (0)     3504 2023-06-25 02:35:02.000000 aa-miningtaxes-1.2.8/miningtaxes/models/orePrices.py
--rw-r--r--   0 root         (0) root         (0)     2089 2022-11-12 04:17:36.000000 aa-miningtaxes-1.2.8/miningtaxes/models/settings.py
--rw-r--r--   0 root         (0) root         (0)    24599 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.8/miningtaxes/models/stats.py
--rw-r--r--   0 root         (0) root         (0)      246 2022-10-27 10:44:31.000000 aa-miningtaxes-1.2.8/miningtaxes/providers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:49:26.472810 aa-miningtaxes-1.2.8/miningtaxes/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:49:26.472810 aa-miningtaxes-1.2.8/miningtaxes/static/miningtaxes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:49:26.479810 aa-miningtaxes-1.2.8/miningtaxes/static/miningtaxes/css/
--rw-r--r--   0 root         (0) root         (0)     4582 2022-11-05 13:42:07.000000 aa-miningtaxes-1.2.8/miningtaxes/static/miningtaxes/css/billboards_dark.css
--rw-r--r--   0 root         (0) root         (0)     4558 2022-11-05 13:42:07.000000 aa-miningtaxes-1.2.8/miningtaxes/static/miningtaxes/css/billboards_light.css
--rw-r--r--   0 root         (0) root         (0)     1538 2022-10-27 12:54:28.000000 aa-miningtaxes-1.2.8/miningtaxes/static/miningtaxes/css/global.css
--rw-r--r--   0 root         (0) root         (0)     4331 2022-10-27 12:54:28.000000 aa-miningtaxes-1.2.8/miningtaxes/static/miningtaxes/css/launcher.css
--rw-r--r--   0 root         (0) root         (0)     1555 2023-01-20 16:20:09.000000 aa-miningtaxes-1.2.8/miningtaxes/static/miningtaxes/css/miningtaxes.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:49:26.480810 aa-miningtaxes-1.2.8/miningtaxes/static/miningtaxes/images/
--rw-r--r--   0 root         (0) root         (0)    34837 2022-11-19 22:22:28.000000 aa-miningtaxes-1.2.8/miningtaxes/static/miningtaxes/images/faq1.png
--rw-r--r--   0 root         (0) root         (0)   132605 2022-11-19 22:22:28.000000 aa-miningtaxes-1.2.8/miningtaxes/static/miningtaxes/images/faq2.png
--rw-r--r--   0 root         (0) root         (0)   342376 2022-11-19 22:22:28.000000 aa-miningtaxes-1.2.8/miningtaxes/static/miningtaxes/images/faq3.png
--rw-r--r--   0 root         (0) root         (0)   881821 2022-10-27 12:49:53.000000 aa-miningtaxes-1.2.8/miningtaxes/swagger.json
--rw-r--r--   0 root         (0) root         (0)    13897 2023-06-26 15:49:01.000000 aa-miningtaxes-1.2.8/miningtaxes/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:49:26.472810 aa-miningtaxes-1.2.8/miningtaxes/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:49:26.481810 aa-miningtaxes-1.2.8/miningtaxes/templates/miningtaxes/
--rw-r--r--   0 root         (0) root         (0)     6817 2023-04-06 01:58:02.000000 aa-miningtaxes-1.2.8/miningtaxes/templates/miningtaxes/admin_launcher.html
--rw-r--r--   0 root         (0) root         (0)    20648 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.8/miningtaxes/templates/miningtaxes/admin_tables.html
--rw-r--r--   0 root         (0) root         (0)     2396 2022-11-28 15:03:03.000000 aa-miningtaxes-1.2.8/miningtaxes/templates/miningtaxes/base.html
--rw-r--r--   0 root         (0) root         (0)     2755 2023-01-08 18:57:41.000000 aa-miningtaxes-1.2.8/miningtaxes/templates/miningtaxes/character_viewer.html
--rw-r--r--   0 root         (0) root         (0)     1740 2023-06-25 02:32:57.000000 aa-miningtaxes-1.2.8/miningtaxes/templates/miningtaxes/faq.html
--rw-r--r--   0 root         (0) root         (0)      480 2022-10-24 21:28:14.000000 aa-miningtaxes-1.2.8/miningtaxes/templates/miningtaxes/index.html
--rw-r--r--   0 root         (0) root         (0)     6466 2022-11-01 15:07:04.000000 aa-miningtaxes-1.2.8/miningtaxes/templates/miningtaxes/launcher.html
--rw-r--r--   0 root         (0) root         (0)     2488 2022-11-22 12:28:46.000000 aa-miningtaxes-1.2.8/miningtaxes/templates/miningtaxes/ore_prices.html
--rw-r--r--   0 root         (0) root         (0)    11159 2023-02-21 19:12:52.000000 aa-miningtaxes-1.2.8/miningtaxes/templates/miningtaxes/user_summary.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:49:26.481810 aa-miningtaxes-1.2.8/miningtaxes/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-19 22:43:55.000000 aa-miningtaxes-1.2.8/miningtaxes/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:49:26.482810 aa-miningtaxes-1.2.8/miningtaxes/tests/models/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-19 23:50:12.000000 aa-miningtaxes-1.2.8/miningtaxes/tests/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2747 2022-11-21 22:33:02.000000 aa-miningtaxes-1.2.8/miningtaxes/tests/models/test_admin_character.py
--rw-r--r--   0 root         (0) root         (0)     7665 2022-11-22 12:24:37.000000 aa-miningtaxes-1.2.8/miningtaxes/tests/models/test_character.py
--rw-r--r--   0 root         (0) root         (0)     4321 2022-11-20 04:46:58.000000 aa-miningtaxes-1.2.8/miningtaxes/tests/models/test_orePrice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:49:26.482810 aa-miningtaxes-1.2.8/miningtaxes/tests/testdata/
--rw-r--r--   0 root         (0) root         (0)     1361 2022-11-21 20:39:23.000000 aa-miningtaxes-1.2.8/miningtaxes/tests/testdata/esi_client_stub.py
--rw-r--r--   0 root         (0) root         (0)     3671 2022-11-20 16:09:12.000000 aa-miningtaxes-1.2.8/miningtaxes/tests/testdata/load_entities.py
--rw-r--r--   0 root         (0) root         (0)      434 2022-11-20 04:51:22.000000 aa-miningtaxes-1.2.8/miningtaxes/tests/testdata/load_eveuniverse.py
--rw-r--r--   0 root         (0) root         (0)     3204 2022-11-21 22:30:35.000000 aa-miningtaxes-1.2.8/miningtaxes/tests/utils.py
--rw-r--r--   0 root         (0) root         (0)     2900 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.8/miningtaxes/urls.py
--rw-r--r--   0 root         (0) root         (0)    20987 2023-06-25 02:31:46.000000 aa-miningtaxes-1.2.8/miningtaxes/views.py
--rw-r--r--   0 root         (0) root         (0)      252 2023-06-26 15:49:26.483810 aa-miningtaxes-1.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1586 2022-11-23 22:55:27.000000 aa-miningtaxes-1.2.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:49:26.482810 aa-miningtaxes-1.2.8/testauth/
--rw-r--r--   0 root         (0) root         (0)       46 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.8/testauth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      612 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.8/testauth/celery.py
--rwxr-xr-x   0 root         (0) root         (0)     9919 2022-11-03 12:24:46.000000 aa-miningtaxes-1.2.8/testauth/settingsAA2.py
--rwxr-xr-x   0 root         (0) root         (0)     9932 2022-11-03 12:24:55.000000 aa-miningtaxes-1.2.8/testauth/settingsAA3.py
--rw-r--r--   0 root         (0) root         (0)      174 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.8/testauth/urls.py
--rw-r--r--   0 root         (0) root         (0)      397 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.8/testauth/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:34:59.988644 aa-miningtaxes-1.2.9/
+-rw-r--r--   0 root         (0) root         (0)     1070 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      183 2022-11-06 18:50:28.000000 aa-miningtaxes-1.2.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7451 2023-07-11 22:34:59.988644 aa-miningtaxes-1.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5740 2023-07-11 15:04:06.000000 aa-miningtaxes-1.2.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:34:59.979644 aa-miningtaxes-1.2.9/aa_miningtaxes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7451 2023-07-11 22:34:59.000000 aa-miningtaxes-1.2.9/aa_miningtaxes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2941 2023-07-11 22:34:59.000000 aa-miningtaxes-1.2.9/aa_miningtaxes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 22:34:59.000000 aa-miningtaxes-1.2.9/aa_miningtaxes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       75 2023-07-11 22:34:59.000000 aa-miningtaxes-1.2.9/aa_miningtaxes.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-11 22:34:59.000000 aa-miningtaxes-1.2.9/aa_miningtaxes.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:34:59.981644 aa-miningtaxes-1.2.9/miningtaxes/
+-rw-r--r--   0 root         (0) root         (0)      108 2023-07-11 22:34:38.000000 aa-miningtaxes-1.2.9/miningtaxes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       84 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.9/miningtaxes/admin.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2023-07-11 22:32:45.000000 aa-miningtaxes-1.2.9/miningtaxes/app_settings.py
+-rw-r--r--   0 root         (0) root         (0)      200 2022-10-27 10:33:48.000000 aa-miningtaxes-1.2.9/miningtaxes/apps.py
+-rw-r--r--   0 root         (0) root         (0)      912 2022-10-24 21:25:29.000000 aa-miningtaxes-1.2.9/miningtaxes/auth_hooks.py
+-rw-r--r--   0 root         (0) root         (0)     3304 2022-11-07 04:47:52.000000 aa-miningtaxes-1.2.9/miningtaxes/decorators.py
+-rw-r--r--   0 root         (0) root         (0)      264 2022-11-05 16:57:46.000000 aa-miningtaxes-1.2.9/miningtaxes/forms.py
+-rw-r--r--   0 root         (0) root         (0)     2295 2023-07-11 15:04:06.000000 aa-miningtaxes-1.2.9/miningtaxes/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:34:59.975644 aa-miningtaxes-1.2.9/miningtaxes/management/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:34:59.981644 aa-miningtaxes-1.2.9/miningtaxes/management/commands/
+-rw-r--r--   0 root         (0) root         (0)      102 2022-10-29 09:17:21.000000 aa-miningtaxes-1.2.9/miningtaxes/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      233 2023-01-08 17:44:15.000000 aa-miningtaxes-1.2.9/miningtaxes/management/commands/miningtaxes_preload_prices.py
+-rw-r--r--   0 root         (0) root         (0)      221 2023-04-04 18:04:31.000000 aa-miningtaxes-1.2.9/miningtaxes/management/commands/miningtaxes_update_manual.py
+-rw-r--r--   0 root         (0) root         (0)      434 2022-11-22 12:21:22.000000 aa-miningtaxes-1.2.9/miningtaxes/management/commands/miningtaxes_zero_all.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:34:59.982644 aa-miningtaxes-1.2.9/miningtaxes/migrations/
+-rw-r--r--   0 root         (0) root         (0)      902 2022-11-06 17:28:27.000000 aa-miningtaxes-1.2.9/miningtaxes/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)    15700 2022-11-06 17:28:28.000000 aa-miningtaxes-1.2.9/miningtaxes/migrations/0002_all_models.py
+-rw-r--r--   0 root         (0) root         (0)      779 2022-11-08 09:05:56.000000 aa-miningtaxes-1.2.9/miningtaxes/migrations/0003_alter_general_options.py
+-rw-r--r--   0 root         (0) root         (0)      939 2022-11-12 04:17:36.000000 aa-miningtaxes-1.2.9/miningtaxes/migrations/0004_settings_interest_rate_alter_settings_phrase.py
+-rw-r--r--   0 root         (0) root         (0)      737 2022-11-14 03:13:49.000000 aa-miningtaxes-1.2.9/miningtaxes/migrations/0005_oreprices_raw_price_oreprices_refined_price_and_more.py
+-rw-r--r--   0 root         (0) root         (0)      452 2022-11-22 12:29:33.000000 aa-miningtaxes-1.2.9/miningtaxes/migrations/0006_charactertaxcredits_credit_type.py
+-rw-r--r--   0 root         (0) root         (0)      566 2023-07-11 15:04:06.000000 aa-miningtaxes-1.2.9/miningtaxes/migrations/0007_character_life_credits_character_life_taxes.py
+-rw-r--r--   0 root         (0) root         (0)      793 2023-07-11 15:04:06.000000 aa-miningtaxes-1.2.9/miningtaxes/migrations/0008_character_monthly_credits_json_and_more.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-07-11 15:04:06.000000 aa-miningtaxes-1.2.9/miningtaxes/migrations/0009_stats.py
+-rw-r--r--   0 root         (0) root         (0)      405 2023-07-11 15:04:06.000000 aa-miningtaxes-1.2.9/miningtaxes/migrations/0010_stats_admin_get_all_activity_json.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 16:52:52.000000 aa-miningtaxes-1.2.9/miningtaxes/migrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:34:59.983644 aa-miningtaxes-1.2.9/miningtaxes/models/
+-rw-r--r--   0 root         (0) root         (0)      438 2023-07-11 15:04:06.000000 aa-miningtaxes-1.2.9/miningtaxes/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7153 2023-07-11 15:04:06.000000 aa-miningtaxes-1.2.9/miningtaxes/models/admin.py
+-rw-r--r--   0 root         (0) root         (0)    18238 2023-07-11 15:04:06.000000 aa-miningtaxes-1.2.9/miningtaxes/models/character.py
+-rw-r--r--   0 root         (0) root         (0)      712 2022-11-08 03:08:01.000000 aa-miningtaxes-1.2.9/miningtaxes/models/general.py
+-rw-r--r--   0 root         (0) root         (0)     3508 2023-07-11 22:22:40.000000 aa-miningtaxes-1.2.9/miningtaxes/models/orePrices.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2022-11-12 04:17:36.000000 aa-miningtaxes-1.2.9/miningtaxes/models/settings.py
+-rw-r--r--   0 root         (0) root         (0)    24599 2023-07-11 15:04:06.000000 aa-miningtaxes-1.2.9/miningtaxes/models/stats.py
+-rw-r--r--   0 root         (0) root         (0)      246 2022-10-27 10:44:31.000000 aa-miningtaxes-1.2.9/miningtaxes/providers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:34:59.976644 aa-miningtaxes-1.2.9/miningtaxes/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:34:59.976644 aa-miningtaxes-1.2.9/miningtaxes/static/miningtaxes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:34:59.983644 aa-miningtaxes-1.2.9/miningtaxes/static/miningtaxes/css/
+-rw-r--r--   0 root         (0) root         (0)     4582 2022-11-05 13:42:07.000000 aa-miningtaxes-1.2.9/miningtaxes/static/miningtaxes/css/billboards_dark.css
+-rw-r--r--   0 root         (0) root         (0)     4558 2022-11-05 13:42:07.000000 aa-miningtaxes-1.2.9/miningtaxes/static/miningtaxes/css/billboards_light.css
+-rw-r--r--   0 root         (0) root         (0)     1538 2022-10-27 12:54:28.000000 aa-miningtaxes-1.2.9/miningtaxes/static/miningtaxes/css/global.css
+-rw-r--r--   0 root         (0) root         (0)     4331 2022-10-27 12:54:28.000000 aa-miningtaxes-1.2.9/miningtaxes/static/miningtaxes/css/launcher.css
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-01-20 16:20:09.000000 aa-miningtaxes-1.2.9/miningtaxes/static/miningtaxes/css/miningtaxes.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:34:59.984644 aa-miningtaxes-1.2.9/miningtaxes/static/miningtaxes/images/
+-rw-r--r--   0 root         (0) root         (0)    34837 2022-11-19 22:22:28.000000 aa-miningtaxes-1.2.9/miningtaxes/static/miningtaxes/images/faq1.png
+-rw-r--r--   0 root         (0) root         (0)   132605 2022-11-19 22:22:28.000000 aa-miningtaxes-1.2.9/miningtaxes/static/miningtaxes/images/faq2.png
+-rw-r--r--   0 root         (0) root         (0)   342376 2022-11-19 22:22:28.000000 aa-miningtaxes-1.2.9/miningtaxes/static/miningtaxes/images/faq3.png
+-rw-r--r--   0 root         (0) root         (0)   881821 2022-10-27 12:49:53.000000 aa-miningtaxes-1.2.9/miningtaxes/swagger.json
+-rw-r--r--   0 root         (0) root         (0)    13988 2023-07-11 21:49:28.000000 aa-miningtaxes-1.2.9/miningtaxes/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:34:59.976644 aa-miningtaxes-1.2.9/miningtaxes/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:34:59.985644 aa-miningtaxes-1.2.9/miningtaxes/templates/miningtaxes/
+-rw-r--r--   0 root         (0) root         (0)     6817 2023-04-06 01:58:02.000000 aa-miningtaxes-1.2.9/miningtaxes/templates/miningtaxes/admin_launcher.html
+-rw-r--r--   0 root         (0) root         (0)    20648 2023-07-11 15:04:06.000000 aa-miningtaxes-1.2.9/miningtaxes/templates/miningtaxes/admin_tables.html
+-rw-r--r--   0 root         (0) root         (0)     2396 2022-11-28 15:03:03.000000 aa-miningtaxes-1.2.9/miningtaxes/templates/miningtaxes/base.html
+-rw-r--r--   0 root         (0) root         (0)     2755 2023-01-08 18:57:41.000000 aa-miningtaxes-1.2.9/miningtaxes/templates/miningtaxes/character_viewer.html
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-07-11 15:04:06.000000 aa-miningtaxes-1.2.9/miningtaxes/templates/miningtaxes/faq.html
+-rw-r--r--   0 root         (0) root         (0)      480 2022-10-24 21:28:14.000000 aa-miningtaxes-1.2.9/miningtaxes/templates/miningtaxes/index.html
+-rw-r--r--   0 root         (0) root         (0)     6466 2022-11-01 15:07:04.000000 aa-miningtaxes-1.2.9/miningtaxes/templates/miningtaxes/launcher.html
+-rw-r--r--   0 root         (0) root         (0)     2488 2022-11-22 12:28:46.000000 aa-miningtaxes-1.2.9/miningtaxes/templates/miningtaxes/ore_prices.html
+-rw-r--r--   0 root         (0) root         (0)    11159 2023-02-21 19:12:52.000000 aa-miningtaxes-1.2.9/miningtaxes/templates/miningtaxes/user_summary.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:34:59.985644 aa-miningtaxes-1.2.9/miningtaxes/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-19 22:43:55.000000 aa-miningtaxes-1.2.9/miningtaxes/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:34:59.986644 aa-miningtaxes-1.2.9/miningtaxes/tests/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-19 23:50:12.000000 aa-miningtaxes-1.2.9/miningtaxes/tests/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2747 2022-11-21 22:33:02.000000 aa-miningtaxes-1.2.9/miningtaxes/tests/models/test_admin_character.py
+-rw-r--r--   0 root         (0) root         (0)     7665 2022-11-22 12:24:37.000000 aa-miningtaxes-1.2.9/miningtaxes/tests/models/test_character.py
+-rw-r--r--   0 root         (0) root         (0)     4321 2022-11-20 04:46:58.000000 aa-miningtaxes-1.2.9/miningtaxes/tests/models/test_orePrice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:34:59.986644 aa-miningtaxes-1.2.9/miningtaxes/tests/testdata/
+-rw-r--r--   0 root         (0) root         (0)     1361 2022-11-21 20:39:23.000000 aa-miningtaxes-1.2.9/miningtaxes/tests/testdata/esi_client_stub.py
+-rw-r--r--   0 root         (0) root         (0)     3671 2022-11-20 16:09:12.000000 aa-miningtaxes-1.2.9/miningtaxes/tests/testdata/load_entities.py
+-rw-r--r--   0 root         (0) root         (0)      434 2022-11-20 04:51:22.000000 aa-miningtaxes-1.2.9/miningtaxes/tests/testdata/load_eveuniverse.py
+-rw-r--r--   0 root         (0) root         (0)     3204 2022-11-21 22:30:35.000000 aa-miningtaxes-1.2.9/miningtaxes/tests/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2900 2023-07-11 15:04:06.000000 aa-miningtaxes-1.2.9/miningtaxes/urls.py
+-rw-r--r--   0 root         (0) root         (0)    20987 2023-07-11 15:04:06.000000 aa-miningtaxes-1.2.9/miningtaxes/views.py
+-rw-r--r--   0 root         (0) root         (0)      252 2023-07-11 22:34:59.989644 aa-miningtaxes-1.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1586 2022-11-23 22:55:27.000000 aa-miningtaxes-1.2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:34:59.988644 aa-miningtaxes-1.2.9/testauth/
+-rw-r--r--   0 root         (0) root         (0)       46 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.9/testauth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      612 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.9/testauth/celery.py
+-rwxr-xr-x   0 root         (0) root         (0)     9919 2022-11-03 12:24:46.000000 aa-miningtaxes-1.2.9/testauth/settingsAA2.py
+-rwxr-xr-x   0 root         (0) root         (0)     9932 2022-11-03 12:24:55.000000 aa-miningtaxes-1.2.9/testauth/settingsAA3.py
+-rw-r--r--   0 root         (0) root         (0)      174 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.9/testauth/urls.py
+-rw-r--r--   0 root         (0) root         (0)      397 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.9/testauth/wsgi.py
```

### Comparing `aa-miningtaxes-1.2.8/LICENSE` & `aa-miningtaxes-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/PKG-INFO` & `aa-miningtaxes-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-miningtaxes
-Version: 1.2.8
+Version: 1.2.9
 Summary: An Alliance Auth app that tracks and applies taxes for mining
 Home-page: https://gitlab.com/arctiru/aa-miningtaxes
 Author: Arc Tiru
 Author-email: arcturusstl@gmail.com
 License: MIT
 Description: # Mining Taxes
```

### Comparing `aa-miningtaxes-1.2.8/README.md` & `aa-miningtaxes-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/aa_miningtaxes.egg-info/PKG-INFO` & `aa-miningtaxes-1.2.9/aa_miningtaxes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-miningtaxes
-Version: 1.2.8
+Version: 1.2.9
 Summary: An Alliance Auth app that tracks and applies taxes for mining
 Home-page: https://gitlab.com/arctiru/aa-miningtaxes
 Author: Arc Tiru
 Author-email: arcturusstl@gmail.com
 License: MIT
 Description: # Mining Taxes
```

### Comparing `aa-miningtaxes-1.2.8/aa_miningtaxes.egg-info/SOURCES.txt` & `aa-miningtaxes-1.2.9/aa_miningtaxes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/app_settings.py` & `aa-miningtaxes-1.2.9/miningtaxes/app_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 """Global timeout for tasks in seconds to reduce task accumulation during outages."""
 
 MININGTAXES_REFINED_RATE = clean_setting("MININGTAXES_REFINED_RATE", 0.9063)
 """Refining rate for ores."""
 
 MININGTAXES_UNKNOWN_TAX_RATE = 0.10
 
-MININGTAXES_ALWAYS_TAX_REFINED = False
+MININGTAXES_ALWAYS_TAX_REFINED = clean_setting("MININGTAXES_ALWAYS_TAX_REFINED", False)
 
 MININGTAXES_PRICE_SOURCE_ID = clean_setting("MININGTAXES_PRICE_SOURCE_ID", 60003760)
 
 MININGTAXES_PRICE_SOURCE_NAME = clean_setting("MININGTAXES_PRICE_SOURCE_NAME", "Jita")
 
 MININGTAXES_PRICE_METHOD = clean_setting("MININGTAXES_PRICE_METHOD", "Fuzzwork")
```

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/auth_hooks.py` & `aa-miningtaxes-1.2.9/miningtaxes/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/decorators.py` & `aa-miningtaxes-1.2.9/miningtaxes/decorators.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/helpers.py` & `aa-miningtaxes-1.2.9/miningtaxes/helpers.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/migrations/0001_initial.py` & `aa-miningtaxes-1.2.9/miningtaxes/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/migrations/0002_all_models.py` & `aa-miningtaxes-1.2.9/miningtaxes/migrations/0002_all_models.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/migrations/0003_alter_general_options.py` & `aa-miningtaxes-1.2.9/miningtaxes/migrations/0003_alter_general_options.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/migrations/0004_settings_interest_rate_alter_settings_phrase.py` & `aa-miningtaxes-1.2.9/miningtaxes/migrations/0004_settings_interest_rate_alter_settings_phrase.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/migrations/0005_oreprices_raw_price_oreprices_refined_price_and_more.py` & `aa-miningtaxes-1.2.9/miningtaxes/migrations/0005_oreprices_raw_price_oreprices_refined_price_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/migrations/0007_character_life_credits_character_life_taxes.py` & `aa-miningtaxes-1.2.9/miningtaxes/migrations/0007_character_life_credits_character_life_taxes.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/migrations/0008_character_monthly_credits_json_and_more.py` & `aa-miningtaxes-1.2.9/miningtaxes/migrations/0008_character_monthly_credits_json_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/migrations/0009_stats.py` & `aa-miningtaxes-1.2.9/miningtaxes/migrations/0009_stats.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/models/admin.py` & `aa-miningtaxes-1.2.9/miningtaxes/models/admin.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/models/character.py` & `aa-miningtaxes-1.2.9/miningtaxes/models/character.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/models/general.py` & `aa-miningtaxes-1.2.9/miningtaxes/models/general.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/models/orePrices.py` & `aa-miningtaxes-1.2.9/miningtaxes/models/orePrices.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,10 +96,10 @@
         self.refined_price = 0.0
         for mat in materials:
             q = MININGTAXES_REFINED_RATE * mat.quantity / self.eve_type.portion_size
             self.refined_price += q * get_price(mat.material_eve_type)
         if self.refined_price == 0.0:
             self.refined_price = self.raw_price
         self.taxed_price = self.refined_price
-        if MININGTAXES_ALWAYS_TAX_REFINED and self.raw_price > self.taxed_price:
+        if not MININGTAXES_ALWAYS_TAX_REFINED and self.raw_price > self.taxed_price:
             self.taxed_price = self.raw_price
         self.save()
```

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/models/settings.py` & `aa-miningtaxes-1.2.9/miningtaxes/models/settings.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/models/stats.py` & `aa-miningtaxes-1.2.9/miningtaxes/models/stats.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/static/miningtaxes/css/billboards_dark.css` & `aa-miningtaxes-1.2.9/miningtaxes/static/miningtaxes/css/billboards_dark.css`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/static/miningtaxes/css/billboards_light.css` & `aa-miningtaxes-1.2.9/miningtaxes/static/miningtaxes/css/billboards_light.css`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/static/miningtaxes/css/global.css` & `aa-miningtaxes-1.2.9/miningtaxes/static/miningtaxes/css/global.css`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/static/miningtaxes/css/launcher.css` & `aa-miningtaxes-1.2.9/miningtaxes/static/miningtaxes/css/launcher.css`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/static/miningtaxes/css/miningtaxes.css` & `aa-miningtaxes-1.2.9/miningtaxes/static/miningtaxes/css/miningtaxes.css`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/static/miningtaxes/images/faq1.png` & `aa-miningtaxes-1.2.9/miningtaxes/static/miningtaxes/images/faq1.png`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/static/miningtaxes/images/faq2.png` & `aa-miningtaxes-1.2.9/miningtaxes/static/miningtaxes/images/faq2.png`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/static/miningtaxes/images/faq3.png` & `aa-miningtaxes-1.2.9/miningtaxes/static/miningtaxes/images/faq3.png`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/swagger.json` & `aa-miningtaxes-1.2.9/miningtaxes/swagger.json`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/tasks.py` & `aa-miningtaxes-1.2.9/miningtaxes/tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -184,23 +184,25 @@
             eve_type_id=item.id
         ).prefetch_related("eve_type")
         for mat in materials:
             mat = mat.material_eve_type
             matset.add(mat.id)
 
     if MININGTAXES_PRICE_METHOD == "Fuzzwork":
+        logger.debug("Using Fuzzwork")
         logger.debug(
             "Price setup starting for %s items from Fuzzworks API from station id %s (%s), this may take up to 30 seconds..."
             % (
                 len(prices),
                 MININGTAXES_PRICE_SOURCE_ID,
                 MININGTAXES_PRICE_SOURCE_NAME,
             )
         )
     elif MININGTAXES_PRICE_METHOD == "Janice":
+        logger.debug("Using Janice")
         if valid_janice_api_key():
             logger.debug(
                 "Price setup starting for %s items from Janice API for Jita 4-4, this may take up to 30 seconds..."
                 % (len(prices),)
             )
         else:
             logger.debug(
@@ -252,16 +254,16 @@
                 toupdate.append(found)
             else:
                 tocreate.append(
                     OrePrices(eve_type_id=price.id, buy=buy, sell=sell, updated=now)
                 )
 
         # Handling refined material prices
-        logger.debug("Materials price updating...")
         type_ids = list(matset)
+        logger.debug(f"Materials price updating: {len(type_ids)}")
         market_data = {}
         market_data.update(get_bulk_prices(type_ids))
         for mat in matset:
             if not str(mat) in market_data:
                 logger.debug(f"Missing data on {mat}")
                 continue
             buy = int(float(market_data[str(mat)]["buy"]["max"]))
```

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/templates/miningtaxes/admin_launcher.html` & `aa-miningtaxes-1.2.9/miningtaxes/templates/miningtaxes/admin_launcher.html`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/templates/miningtaxes/admin_tables.html` & `aa-miningtaxes-1.2.9/miningtaxes/templates/miningtaxes/admin_tables.html`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/templates/miningtaxes/base.html` & `aa-miningtaxes-1.2.9/miningtaxes/templates/miningtaxes/base.html`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/templates/miningtaxes/character_viewer.html` & `aa-miningtaxes-1.2.9/miningtaxes/templates/miningtaxes/character_viewer.html`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/templates/miningtaxes/faq.html` & `aa-miningtaxes-1.2.9/miningtaxes/templates/miningtaxes/faq.html`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/templates/miningtaxes/launcher.html` & `aa-miningtaxes-1.2.9/miningtaxes/templates/miningtaxes/launcher.html`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/templates/miningtaxes/ore_prices.html` & `aa-miningtaxes-1.2.9/miningtaxes/templates/miningtaxes/ore_prices.html`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/templates/miningtaxes/user_summary.html` & `aa-miningtaxes-1.2.9/miningtaxes/templates/miningtaxes/user_summary.html`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/tests/models/test_admin_character.py` & `aa-miningtaxes-1.2.9/miningtaxes/tests/models/test_admin_character.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/tests/models/test_character.py` & `aa-miningtaxes-1.2.9/miningtaxes/tests/models/test_character.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/tests/models/test_orePrice.py` & `aa-miningtaxes-1.2.9/miningtaxes/tests/models/test_orePrice.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/tests/testdata/esi_client_stub.py` & `aa-miningtaxes-1.2.9/miningtaxes/tests/testdata/esi_client_stub.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/tests/testdata/load_entities.py` & `aa-miningtaxes-1.2.9/miningtaxes/tests/testdata/load_entities.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/tests/utils.py` & `aa-miningtaxes-1.2.9/miningtaxes/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/urls.py` & `aa-miningtaxes-1.2.9/miningtaxes/urls.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/miningtaxes/views.py` & `aa-miningtaxes-1.2.9/miningtaxes/views.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/setup.py` & `aa-miningtaxes-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/testauth/celery.py` & `aa-miningtaxes-1.2.9/testauth/celery.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/testauth/settingsAA2.py` & `aa-miningtaxes-1.2.9/testauth/settingsAA2.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.2.8/testauth/settingsAA3.py` & `aa-miningtaxes-1.2.9/testauth/settingsAA3.py`

 * *Files identical despite different names*

